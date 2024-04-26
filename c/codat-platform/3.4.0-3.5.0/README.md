# Comparing `tmp/codat-platform-3.4.0.tar.gz` & `tmp/codat-platform-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codat-platform-3.4.0.tar", last modified: Wed Mar  6 11:19:51 2024, max compression
+gzip compressed data, was "codat-platform-3.5.0.tar", last modified: Fri Apr 26 15:57:58 2024, max compression
```

## Comparing `codat-platform-3.4.0.tar` & `codat-platform-3.5.0.tar`

### file list

```diff
@@ -1,184 +1,193 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 11:19:51.731114 codat-platform-3.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)    14880 2024-03-06 11:19:51.731114 codat-platform-3.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11823 2024-03-06 11:19:43.000000 codat-platform-3.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-06 11:19:51.731114 codat-platform-3.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-03-06 11:19:43.000000 codat-platform-3.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 11:19:51.703114 codat-platform-3.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 11:19:51.707114 codat-platform-3.4.0/src/codat_platform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14880 2024-03-06 11:19:51.000000 codat-platform-3.4.0/src/codat_platform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8897 2024-03-06 11:19:51.000000 codat-platform-3.4.0/src/codat_platform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 11:19:51.000000 codat-platform-3.4.0/src/codat_platform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-06 11:19:51.000000 codat-platform-3.4.0/src/codat_platform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-06 11:19:51.000000 codat-platform-3.4.0/src/codat_platform.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 11:19:51.707114 codat-platform-3.4.0/src/codatplatform/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 11:19:51.707114 codat-platform-3.4.0/src/codatplatform/_hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/_hooks/registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/_hooks/sdkhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/_hooks/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    22990 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/companies.py
--rw-r--r--   0 runner    (1001) docker     (127)    25329 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/connections.py
--rw-r--r--   0 runner    (1001) docker     (127)    18702 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/custom_data_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    17205 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    12152 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/integrations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 11:19:51.711114 codat-platform-3.4.0/src/codatplatform/models/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 11:19:51.711114 codat-platform-3.4.0/src/codatplatform/models/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/errors/errormessage.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/errors/sdkerror.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 11:19:51.715114 codat-platform-3.4.0/src/codatplatform/models/operations/
--rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/operations/add_company_to_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/operations/configure_custom_data_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/operations/configure_supplemental_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/operations/create_api_key.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/operations/create_company.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/operations/create_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/operations/create_group.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/operations/create_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/operations/create_webhook_consumer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/operations/delete_api_key.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/operations/delete_company.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/operations/delete_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/operations/delete_webhook_consumer.py
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/operations/get_company.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/operations/get_company_data_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/operations/get_company_push_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/operations/get_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/operations/get_create_update_model_options_by_data_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/operations/get_custom_data_type_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/operations/get_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/operations/get_integrations_branding.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/operations/get_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/operations/get_profile_syncsettings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/operations/get_pull_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/operations/get_push_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/operations/get_supplemental_data_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/operations/get_webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/operations/list_api_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/operations/list_companies.py
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/operations/list_connections.py
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/operations/list_custom_data_type_records.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/operations/list_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/operations/list_integrations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/operations/list_pull_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/operations/list_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/operations/list_webhook_consumers.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/operations/refresh_company_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/operations/refresh_custom_data_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/operations/refresh_data_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/operations/remove_company_from_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/operations/unlink_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/operations/update_company.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/operations/update_connection_authorization.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/operations/update_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/operations/update_profile_syncsettings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 11:19:51.727114 codat-platform-3.4.0/src/codatplatform/models/shared/
--rw-r--r--   0 runner    (1001) docker     (127)     4623 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/apikeydetails.py
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/apikeys.py
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/branding.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/brandingbutton.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/brandingimage.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/brandinglogo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/clientratelimitreachedwebhook.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/clientratelimitreachedwebhookdata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/clientratelimitresetwebhook.py
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/clientratelimitresetwebhookdata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/companies.py
--rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/company.py
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/companygroupassignment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/companyrequestbody.py
--rw-r--r--   0 runner    (1001) docker     (127)     6000 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/connections.py
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/connectionstatuschangedwebhook.py
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/connectionstatuschangedwebhookdata.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/createapikey.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/createrule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/customdatatypeconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/customdatatyperecord.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/customdatatyperecords.py
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/dataconnectionerror.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/dataconnectionstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/datasetdatachangedwebhook.py
--rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/datasetstatuschangederrorwebhook.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/datasetstatuschangederrorwebhookdata.py
--rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/datastatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/datasynccompletedwebhook.py
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/datasynccompletedwebhookdata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/datatype.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/datatypefeature.py
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/errorvalidation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/errorvalidationitem.py
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/featurestate.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/featuretype.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/group.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/groupprototype.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/groupref.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/halref.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/imagereference.py
--rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/integrations.py
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/links.py
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/newcompanysynchronizedwebhook.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/newcompanysynchronizedwebhookdata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/pulloperation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/pulloperations.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/pushchangetype.py
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/pushfieldvalidation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5576 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/pushoperation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/pushoperationchange.py
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/pushoperationref.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/pushoperations.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/pushoperationstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/pushoperationstatuschangedwebhook.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/pushoperationstatuschangedwebhookdata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/pushoperationtimedoutwebhook.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/pushoperationtimedoutwebhookdata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/pushoption.py
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/pushoptionchoice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/pushoptionproperty.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/pushoptiontype.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/pushvalidationinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/schema_datatype.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/security.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/sourcetype.py
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/supplementaldataconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/supportedfeature.py
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/syncsetting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/syncsettings.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/updateconnectionstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/validationitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/webhookconsumer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/webhookconsumerprototype.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/webhookconsumers.py
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/webhooknotifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/shared/webhooks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 11:19:51.727114 codat-platform-3.4.0/src/codatplatform/models/webhooks/
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/webhooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/webhooks/client_rate_limit_reached.py
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/webhooks/client_rate_limit_reset.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/webhooks/company_data_connection_status_changed.py
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/webhooks/data_sync_completed.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/webhooks/dataset_data_changed.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/webhooks/dataset_status_has_changed_to_an_error_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/webhooks/new_company_synchronized.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/webhooks/push_operation_has_timed_out.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/models/webhooks/push_operation_status_has_changed.py
--rw-r--r--   0 runner    (1001) docker     (127)    13545 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/push_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    20385 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/refresh_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/sdkconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)    29978 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     9213 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/supplemental_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 11:19:51.731114 codat-platform-3.4.0/src/codatplatform/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/utils/retries.py
--rw-r--r--   0 runner    (1001) docker     (127)    30091 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    25111 2024-03-06 11:19:43.000000 codat-platform-3.4.0/src/codatplatform/webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:57:58.134720 codat-platform-3.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    18914 2024-04-26 15:57:58.134720 codat-platform-3.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12211 2024-04-26 15:57:48.000000 codat-platform-3.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 15:57:58.134720 codat-platform-3.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-26 15:57:48.000000 codat-platform-3.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:57:58.106720 codat-platform-3.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:57:58.106720 codat-platform-3.5.0/src/codat_platform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18914 2024-04-26 15:57:57.000000 codat-platform-3.5.0/src/codat_platform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9438 2024-04-26 15:57:58.000000 codat-platform-3.5.0/src/codat_platform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 15:57:57.000000 codat-platform-3.5.0/src/codat_platform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-26 15:57:57.000000 codat-platform-3.5.0/src/codat_platform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-26 15:57:57.000000 codat-platform-3.5.0/src/codat_platform.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:57:58.110720 codat-platform-3.5.0/src/codatplatform/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:57:58.110720 codat-platform-3.5.0/src/codatplatform/_hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/_hooks/registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/_hooks/sdkhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/_hooks/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24742 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/companies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/connection_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27352 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10600 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/cors_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20117 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/custom_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18633 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13268 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/integrations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:57:58.110720 codat-platform-3.5.0/src/codatplatform/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:57:58.110720 codat-platform-3.5.0/src/codatplatform/models/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/errors/errormessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/errors/sdkerror.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:57:58.118720 codat-platform-3.5.0/src/codatplatform/models/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/operations/add_company_to_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/operations/configure_custom_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/operations/configure_supplemental_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/operations/create_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/operations/create_company.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/operations/create_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/operations/create_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/operations/create_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/operations/create_webhook_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/operations/delete_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/operations/delete_company.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/operations/delete_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/operations/delete_webhook_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/operations/get_company.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/operations/get_company_data_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/operations/get_company_push_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/operations/get_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/operations/get_connection_management_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/operations/get_connection_management_cors_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/operations/get_create_update_model_options_by_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/operations/get_custom_data_type_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/operations/get_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/operations/get_integrations_branding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/operations/get_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/operations/get_profile_syncsettings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/operations/get_pull_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/operations/get_push_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/operations/get_supplemental_data_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/operations/get_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/operations/list_api_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/operations/list_companies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/operations/list_connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/operations/list_custom_data_type_records.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/operations/list_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/operations/list_integrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/operations/list_pull_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/operations/list_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/operations/list_webhook_consumers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/operations/refresh_company_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/operations/refresh_custom_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/operations/refresh_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/operations/remove_company_from_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/operations/set_connection_management_cors_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/operations/unlink_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/operations/update_company.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/operations/update_connection_authorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/operations/update_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/operations/update_profile_syncsettings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:57:58.130720 codat-platform-3.5.0/src/codatplatform/models/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)     4872 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/apikeydetails.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/apikeys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/branding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/brandingbutton.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/brandingimage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/brandinglogo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/clientratelimitreachedwebhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/clientratelimitreachedwebhookdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/clientratelimitresetwebhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/clientratelimitresetwebhookdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/companies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/company.py
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/companygroupassignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/companyrequestbody.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6000 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/connectionmanagementaccesstoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/connectionmanagementallowedorigins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/connectionstatuschangedwebhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/connectionstatuschangedwebhookdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/createapikey.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/createrule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/customdatatypeconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/customdatatyperecord.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/customdatatyperecords.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/dataconnectionerror.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/dataconnectionstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/datasetdatachangedwebhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/datasetstatuschangederrorwebhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/datasetstatuschangederrorwebhookdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/datastatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12624 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/datastatuses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/datasynccompletedwebhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/datasynccompletedwebhookdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/datatype.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/datatypefeature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/errorvalidation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/errorvalidationitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/featurestate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/featuretype.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/groupprototype.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/groupref.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/halref.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/imagereference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/newcompanysynchronizedwebhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/newcompanysynchronizedwebhookdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/pulloperation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/pulloperations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/pushchangetype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/pushfieldvalidation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5576 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/pushoperation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/pushoperationchange.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/pushoperationref.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/pushoperations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/pushoperationstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/pushoperationstatuschangedwebhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/pushoperationstatuschangedwebhookdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/pushoperationtimedoutwebhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/pushoperationtimedoutwebhookdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/pushoption.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/pushoptionchoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/pushoptionproperty.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/pushoptiontype.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/pushvalidationinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/schema_datatype.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/sourcetype.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/supplementaldataconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/supportedfeature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/syncsetting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/syncsettings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/updateconnectionstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/validationitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/webhookconsumer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/webhookconsumerprototype.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/webhookconsumers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/webhooknotifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/shared/webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:57:58.134720 codat-platform-3.5.0/src/codatplatform/models/webhooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/webhooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/webhooks/client_rate_limit_reached.py
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/webhooks/client_rate_limit_reset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/webhooks/company_data_connection_status_changed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/webhooks/data_sync_completed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/webhooks/dataset_data_changed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/webhooks/dataset_status_has_changed_to_an_error_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/webhooks/new_company_synchronized.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/webhooks/push_operation_has_timed_out.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/models/webhooks/push_operation_status_has_changed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14609 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/push_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21967 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/refresh_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6371 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/sdkconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32630 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9856 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/supplemental_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:57:58.134720 codat-platform-3.5.0/src/codatplatform/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/utils/retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32089 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27294 2024-04-26 15:57:48.000000 codat-platform-3.5.0/src/codatplatform/webhooks.py
```

### Comparing `codat-platform-3.4.0/README.md` & `codat-platform-3.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 )
 
 res = s.settings.create_api_key(req)
 
 if res.api_key_details is not None:
     # handle response
     pass
+
 ```
 <!-- End SDK Example Usage [usage] -->
 
 <!-- Start Available Resources and Operations [operations] -->
 ## Available Resources and Operations
 
 ### [settings](docs/sdks/settings/README.md)
@@ -57,14 +58,23 @@
 
 * [create](docs/sdks/companies/README.md#create) - Create company
 * [delete](docs/sdks/companies/README.md#delete) - Delete a company
 * [get](docs/sdks/companies/README.md#get) - Get company
 * [list](docs/sdks/companies/README.md#list) - List companies
 * [update](docs/sdks/companies/README.md#update) - Update company
 
+### [connection_management](docs/sdks/connectionmanagement/README.md)
+
+* [get_access_token](docs/sdks/connectionmanagement/README.md#get_access_token) - Get access token
+
+### [connection_management.cors_settings](docs/sdks/corssettings/README.md)
+
+* [get](docs/sdks/corssettings/README.md#get) - Get CORS settings
+* [set](docs/sdks/corssettings/README.md#set) - Set CORS settings
+
 ### [connections](docs/sdks/connections/README.md)
 
 * [create](docs/sdks/connections/README.md#create) - Create connection
 * [delete](docs/sdks/connections/README.md#delete) - Delete connection
 * [get](docs/sdks/connections/README.md#get) - Get connection
 * [list](docs/sdks/connections/README.md#list) - List connections
 * [unlink](docs/sdks/connections/README.md#unlink) - Unlink connection
@@ -144,50 +154,52 @@
 
 res = s.settings.create_api_key(req,
     RetryConfig('backoff', BackoffStrategy(1, 50, 1.1, 100), False))
 
 if res.api_key_details is not None:
     # handle response
     pass
+
 ```
 
 If you'd like to override the default retry strategy for all operations that support retries, you can use the `retry_config` optional parameter when initializing the SDK:
 ```python
 import codatplatform
 from codatplatform.models import shared
 from codatplatform.utils import BackoffStrategy, RetryConfig
 
 s = codatplatform.CodatPlatform(
-    retry_config=RetryConfig('backoff', BackoffStrategy(1, 50, 1.1, 100), False)
+    retry_config=RetryConfig('backoff', BackoffStrategy(1, 50, 1.1, 100), False),
     security=shared.Security(
         auth_header="Basic BASE_64_ENCODED(API_KEY)",
     ),
 )
 
 req = shared.CreateAPIKey(
     name='azure-invoice-finance-processor',
 )
 
 res = s.settings.create_api_key(req)
 
 if res.api_key_details is not None:
     # handle response
     pass
+
 ```
 <!-- End Retries [retries] -->
 
 <!-- Start Error Handling [errors] -->
 ## Error Handling
 
 Handling errors in this SDK should largely match your expectations.  All operations return a response object or raise an error.  If Error objects are specified in your OpenAPI Spec, the SDK will raise the appropriate Error type.
 
 | Error Object                    | Status Code                     | Content Type                    |
 | ------------------------------- | ------------------------------- | ------------------------------- |
 | errors.ErrorMessage             | 400,401,402,403,409,429,500,503 | application/json                |
-| errors.SDKError                 | 4x-5xx                          | */*                             |
+| errors.SDKError                 | 4xx-5xx                         | */*                             |
 
 ### Example
 
 ```python
 import codatplatform
 from codatplatform.models import errors, shared
 
@@ -210,14 +222,15 @@
 except errors.SDKError as e:
     # handle exception
     raise(e)
 
 if res.api_key_details is not None:
     # handle response
     pass
+
 ```
 <!-- End Error Handling [errors] -->
 
 <!-- Start Server Selection [server] -->
 ## Server Selection
 
 ### Select Server by Index
@@ -246,14 +259,15 @@
 )
 
 res = s.settings.create_api_key(req)
 
 if res.api_key_details is not None:
     # handle response
     pass
+
 ```
 
 
 ### Override Server URL Per-Client
 
 The default server can also be overridden globally by passing a URL to the `server_url: str` optional parameter when initializing the SDK client instance. For example:
 ```python
@@ -272,14 +286,15 @@
 )
 
 res = s.settings.create_api_key(req)
 
 if res.api_key_details is not None:
     # handle response
     pass
+
 ```
 <!-- End Server Selection [server] -->
 
 <!-- Start Custom HTTP Client [http-client] -->
 ## Custom HTTP Client
 
 The Python SDK makes API calls using the [requests](https://pypi.org/project/requests/) HTTP library.  In order to provide a convenient way to configure timeouts, cookies, proxies, custom headers, and other low-level configuration, you can initialize the SDK client with a custom `requests.Session` object.
@@ -287,15 +302,15 @@
 For example, you could specify a header for every request that this sdk makes as follows:
 ```python
 import codatplatform
 import requests
 
 http_client = requests.Session()
 http_client.headers.update({'x-custom-header': 'someValue'})
-s = codatplatform.CodatPlatform(client: http_client)
+s = codatplatform.CodatPlatform(client=http_client)
 ```
 <!-- End Custom HTTP Client [http-client] -->
 
 <!-- Start Authentication [security] -->
 ## Authentication
 
 ### Per-Client Security Schemes
@@ -322,14 +337,15 @@
 )
 
 res = s.settings.create_api_key(req)
 
 if res.api_key_details is not None:
     # handle response
     pass
+
 ```
 <!-- End Authentication [security] -->
 
 <!-- Placeholder for Future Speakeasy SDK Sections -->
 
 <!-- Start Codat Support Notes -->
 ### Support
```

### Comparing `codat-platform-3.4.0/src/codat_platform.egg-info/SOURCES.txt` & `codat-platform-3.5.0/src/codat_platform.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 src/codat_platform.egg-info/PKG-INFO
 src/codat_platform.egg-info/SOURCES.txt
 src/codat_platform.egg-info/dependency_links.txt
 src/codat_platform.egg-info/requires.txt
 src/codat_platform.egg-info/top_level.txt
 src/codatplatform/__init__.py
 src/codatplatform/companies.py
+src/codatplatform/connection_management.py
 src/codatplatform/connections.py
+src/codatplatform/cors_settings.py
 src/codatplatform/custom_data_type.py
 src/codatplatform/groups.py
 src/codatplatform/integrations.py
 src/codatplatform/push_data.py
 src/codatplatform/refresh_data.py
 src/codatplatform/sdk.py
 src/codatplatform/sdkconfiguration.py
@@ -40,14 +42,16 @@
 src/codatplatform/models/operations/delete_company.py
 src/codatplatform/models/operations/delete_connection.py
 src/codatplatform/models/operations/delete_webhook_consumer.py
 src/codatplatform/models/operations/get_company.py
 src/codatplatform/models/operations/get_company_data_status.py
 src/codatplatform/models/operations/get_company_push_history.py
 src/codatplatform/models/operations/get_connection.py
+src/codatplatform/models/operations/get_connection_management_access_token.py
+src/codatplatform/models/operations/get_connection_management_cors_settings.py
 src/codatplatform/models/operations/get_create_update_model_options_by_data_type.py
 src/codatplatform/models/operations/get_custom_data_type_configuration.py
 src/codatplatform/models/operations/get_integration.py
 src/codatplatform/models/operations/get_integrations_branding.py
 src/codatplatform/models/operations/get_profile.py
 src/codatplatform/models/operations/get_profile_syncsettings.py
 src/codatplatform/models/operations/get_pull_operation.py
@@ -63,14 +67,15 @@
 src/codatplatform/models/operations/list_pull_operations.py
 src/codatplatform/models/operations/list_rules.py
 src/codatplatform/models/operations/list_webhook_consumers.py
 src/codatplatform/models/operations/refresh_company_data.py
 src/codatplatform/models/operations/refresh_custom_data_type.py
 src/codatplatform/models/operations/refresh_data_type.py
 src/codatplatform/models/operations/remove_company_from_group.py
+src/codatplatform/models/operations/set_connection_management_cors_settings.py
 src/codatplatform/models/operations/unlink_connection.py
 src/codatplatform/models/operations/update_company.py
 src/codatplatform/models/operations/update_connection_authorization.py
 src/codatplatform/models/operations/update_profile.py
 src/codatplatform/models/operations/update_profile_syncsettings.py
 src/codatplatform/models/shared/__init__.py
 src/codatplatform/models/shared/apikeydetails.py
@@ -84,28 +89,31 @@
 src/codatplatform/models/shared/clientratelimitresetwebhook.py
 src/codatplatform/models/shared/clientratelimitresetwebhookdata.py
 src/codatplatform/models/shared/companies.py
 src/codatplatform/models/shared/company.py
 src/codatplatform/models/shared/companygroupassignment.py
 src/codatplatform/models/shared/companyrequestbody.py
 src/codatplatform/models/shared/connection.py
+src/codatplatform/models/shared/connectionmanagementaccesstoken.py
+src/codatplatform/models/shared/connectionmanagementallowedorigins.py
 src/codatplatform/models/shared/connections.py
 src/codatplatform/models/shared/connectionstatuschangedwebhook.py
 src/codatplatform/models/shared/connectionstatuschangedwebhookdata.py
 src/codatplatform/models/shared/createapikey.py
 src/codatplatform/models/shared/createrule.py
 src/codatplatform/models/shared/customdatatypeconfiguration.py
 src/codatplatform/models/shared/customdatatyperecord.py
 src/codatplatform/models/shared/customdatatyperecords.py
 src/codatplatform/models/shared/dataconnectionerror.py
 src/codatplatform/models/shared/dataconnectionstatus.py
 src/codatplatform/models/shared/datasetdatachangedwebhook.py
 src/codatplatform/models/shared/datasetstatuschangederrorwebhook.py
 src/codatplatform/models/shared/datasetstatuschangederrorwebhookdata.py
 src/codatplatform/models/shared/datastatus.py
+src/codatplatform/models/shared/datastatuses.py
 src/codatplatform/models/shared/datasynccompletedwebhook.py
 src/codatplatform/models/shared/datasynccompletedwebhookdata.py
 src/codatplatform/models/shared/datatype.py
 src/codatplatform/models/shared/datatypefeature.py
 src/codatplatform/models/shared/errorvalidation.py
 src/codatplatform/models/shared/errorvalidationitem.py
 src/codatplatform/models/shared/featurestate.py
@@ -139,14 +147,15 @@
 src/codatplatform/models/shared/pushoptionchoice.py
 src/codatplatform/models/shared/pushoptionproperty.py
 src/codatplatform/models/shared/pushoptiontype.py
 src/codatplatform/models/shared/pushvalidationinfo.py
 src/codatplatform/models/shared/schema_datatype.py
 src/codatplatform/models/shared/security.py
 src/codatplatform/models/shared/sourcetype.py
+src/codatplatform/models/shared/status.py
 src/codatplatform/models/shared/supplementaldataconfiguration.py
 src/codatplatform/models/shared/supportedfeature.py
 src/codatplatform/models/shared/syncsetting.py
 src/codatplatform/models/shared/syncsettings.py
 src/codatplatform/models/shared/updateconnectionstatus.py
 src/codatplatform/models/shared/validation.py
 src/codatplatform/models/shared/validationitem.py
```

### Comparing `codat-platform-3.4.0/src/codatplatform/_hooks/registration.py` & `codat-platform-3.5.0/src/codatplatform/_hooks/registration.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/_hooks/sdkhooks.py` & `codat-platform-3.5.0/src/codatplatform/_hooks/sdkhooks.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests
 from .types import SDKInitHook, BeforeRequestContext, BeforeRequestHook, AfterSuccessContext, AfterSuccessHook, AfterErrorContext, AfterErrorHook, Hooks
 from .registration import init_hooks
-from typing import List, Optional, Tuple, Union
+from typing import List, Optional, Tuple
 
 
 class SDKHooks(Hooks):
-    sdk_init_hooks: List[SDKInitHook] = []
-    before_request_hooks: List[BeforeRequestHook] = []
-    after_success_hooks: List[AfterSuccessHook] = []
-    after_error_hooks: List[AfterErrorHook] = []
-
     def __init__(self):
+        self.sdk_init_hooks: List[SDKInitHook] = []
+        self.before_request_hooks: List[BeforeRequestHook] = []
+        self.after_success_hooks: List[AfterSuccessHook] = []
+        self.after_error_hooks: List[AfterErrorHook] = []
         init_hooks(self)
 
     def register_sdk_init_hook(self, hook: SDKInitHook) -> None:
         self.sdk_init_hooks.append(hook)
 
     def register_before_request_hook(self, hook: BeforeRequestHook) -> None:
         self.before_request_hooks.append(hook)
@@ -28,27 +27,29 @@
         self.after_error_hooks.append(hook)
 
     def sdk_init(self, base_url: str, client: requests.Session) -> Tuple[str, requests.Session]:
         for hook in self.sdk_init_hooks:
             base_url, client = hook.sdk_init(base_url, client)
         return base_url, client
 
-    def before_request(self, hook_ctx: BeforeRequestContext, request: requests.PreparedRequest) -> Union[requests.PreparedRequest, Exception]:
+    def before_request(self, hook_ctx: BeforeRequestContext, request: requests.PreparedRequest) -> requests.PreparedRequest:
         for hook in self.before_request_hooks:
-            request = hook.before_request(hook_ctx, request)
-            if isinstance(request, Exception):
-                raise request
+            out = hook.before_request(hook_ctx, request)
+            if isinstance(out, Exception):
+                raise out
+            request = out
 
         return request
 
     def after_success(self, hook_ctx: AfterSuccessContext, response: requests.Response) -> requests.Response:
         for hook in self.after_success_hooks:
-            response = hook.after_success(hook_ctx, response)
-            if isinstance(response, Exception):
-                raise response
+            out = hook.after_success(hook_ctx, response)
+            if isinstance(out, Exception):
+                raise out
+            response = out
         return response
 
     def after_error(self, hook_ctx: AfterErrorContext, response: Optional[requests.Response], error: Optional[Exception]) -> Tuple[Optional[requests.Response], Optional[Exception]]:
         for hook in self.after_error_hooks:
             result = hook.after_error(hook_ctx, response, error)
             if isinstance(result, Exception):
                 raise result
```

### Comparing `codat-platform-3.4.0/src/codatplatform/_hooks/types.py` & `codat-platform-3.5.0/src/codatplatform/_hooks/types.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,23 +13,27 @@
     def __init__(self, operation_id: str, oauth2_scopes: Optional[List[str]], security_source: Optional[Union[Any, Callable[[], Any]]]):
         self.operation_id = operation_id
         self.oauth2_scopes = oauth2_scopes
         self.security_source = security_source
 
 
 class BeforeRequestContext(HookContext):
-    pass
+    def __init__(self, hook_ctx: HookContext):
+        super().__init__(hook_ctx.operation_id, hook_ctx.oauth2_scopes, hook_ctx.security_source)
 
 
 class AfterSuccessContext(HookContext):
-    pass
+    def __init__(self, hook_ctx: HookContext):
+        super().__init__(hook_ctx.operation_id, hook_ctx.oauth2_scopes, hook_ctx.security_source)
+    
 
 
 class AfterErrorContext(HookContext):
-    pass
+    def __init__(self, hook_ctx: HookContext):
+        super().__init__(hook_ctx.operation_id, hook_ctx.oauth2_scopes, hook_ctx.security_source)
 
 
 class SDKInitHook(ABC):
     @abstractmethod
     def sdk_init(self, base_url: str, client: requests_http.Session) -> Tuple[str, requests_http.Session]:
         pass
 
@@ -38,21 +42,21 @@
     @abstractmethod
     def before_request(self, hook_ctx: BeforeRequestContext, request: requests_http.PreparedRequest) -> Union[requests_http.PreparedRequest, Exception]:
         pass
 
 
 class AfterSuccessHook(ABC):
     @abstractmethod
-    def after_success(self, hook_ctx: AfterSuccessContext, response: requests_http.Response) -> Union[requests_http.PreparedRequest, Exception]:
+    def after_success(self, hook_ctx: AfterSuccessContext, response: requests_http.Response) -> Union[requests_http.Response, Exception]:
         pass
 
 
 class AfterErrorHook(ABC):
     @abstractmethod
-    def after_error(self, hook_ctx: AfterErrorContext, response: Optional[requests_http.Response], error: Optional[Exception]) -> Union[Tuple[Optional[requests_http.PreparedRequest], Optional[Exception]], Exception]:
+    def after_error(self, hook_ctx: AfterErrorContext, response: Optional[requests_http.Response], error: Optional[Exception]) -> Union[Tuple[Optional[requests_http.Response], Optional[Exception]], Exception]:
         pass
 
 
 class Hooks(ABC):
     @abstractmethod
     def register_sdk_init_hook(self, hook: SDKInitHook):
         pass
```

### Comparing `codat-platform-3.4.0/src/codatplatform/companies.py` & `codat-platform-3.5.0/src/codatplatform/companies.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from codatplatform import utils
-from codatplatform._hooks import HookContext
+from codatplatform._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from codatplatform.models import errors, operations, shared
 from typing import Optional
 
 class Companies:
-    r"""Create and manage your Codat companies."""
+    r"""Create and manage your SMB users' companies."""
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
@@ -25,83 +25,85 @@
 
         If forbidden characters (see `name` pattern) are present in the request, a company will be created with the forbidden characters removed. For example, `Company (Codat[1])` with be created as `Company Codat1`.
         """
         hook_ctx = HookContext(operation_id='create-company', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
         url = base_url + '/companies'
-        headers = {}
+        
+        if callable(self.sdk_configuration.security):
+            headers, query_params = utils.get_security(self.sdk_configuration.security())
+        else:
+            headers, query_params = utils.get_security(self.sdk_configuration.security)
+        
         req_content_type, data, form = utils.serialize_request_body(request, Optional[shared.CompanyRequestBody], "request", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
-        
-        if callable(self.sdk_configuration.security):
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security())
-        else:
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security)
-        
+        client = self.sdk_configuration.client
         
         global_retry_config = self.sdk_configuration.retry_config
         retry_config = retries
         if retry_config is None:
             if global_retry_config:
                 retry_config = global_retry_config
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
+        req = None
         def do_request():
+            nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('POST', url, data=data, files=form, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
             if utils.match_status_codes(['400','401','402','403','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
-        content_type = http_res.headers.get('Content-Type')
         
-        res = operations.CreateCompanyResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.CreateCompanyResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(content_type, 'application/json'):
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.Company])
                 res.company = out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [400, 401, 402, 403, 429, 500, 503]:
-            if utils.match_content_type(content_type, 'application/json'):
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
-                out.raw_response = http_res
                 raise out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+        else:
+            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
     def delete(self, request: operations.DeleteCompanyRequest, retries: Optional[utils.RetryConfig] = None) -> operations.DeleteCompanyResponse:
         r"""Delete a company
@@ -109,77 +111,78 @@
 
         A [company](https://docs.codat.io/platform-api#/schemas/Company) represents a business sharing access to their data.
         Each company can have multiple [connections](https://docs.codat.io/platform-api#/schemas/Connection) to different data sources, such as one connection to Xero for accounting data, two connections to Plaid for two bank accounts, and a connection to Zettle for POS data.
         """
         hook_ctx = HookContext(operation_id='delete-company', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.DeleteCompanyRequest, base_url, '/companies/{companyId}', request)
-        headers = {}
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = self.sdk_configuration.user_agent
+        url = utils.generate_url(base_url, '/companies/{companyId}', request)
         
         if callable(self.sdk_configuration.security):
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security())
+            headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security)
+            headers, query_params = utils.get_security(self.sdk_configuration.security)
         
+        headers['Accept'] = 'application/json'
+        headers['user-agent'] = self.sdk_configuration.user_agent
+        client = self.sdk_configuration.client
         
         global_retry_config = self.sdk_configuration.retry_config
         retry_config = retries
         if retry_config is None:
             if global_retry_config:
                 retry_config = global_retry_config
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
+        req = None
         def do_request():
+            nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('DELETE', url, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('DELETE', url, params=query_params, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
             if utils.match_status_codes(['401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
-        content_type = http_res.headers.get('Content-Type')
         
-        res = operations.DeleteCompanyResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.DeleteCompanyResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 204:
             pass
         elif http_res.status_code in [401, 402, 403, 404, 429, 500, 503]:
-            if utils.match_content_type(content_type, 'application/json'):
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
-                out.raw_response = http_res
                 raise out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+        else:
+            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
     def get(self, request: operations.GetCompanyRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetCompanyResponse:
         r"""Get company
@@ -187,81 +190,83 @@
 
         A [company](https://docs.codat.io/platform-api#/schemas/Company) represents a business sharing access to their data.
         Each company can have multiple [connections](https://docs.codat.io/platform-api#/schemas/Connection) to different data sources, such as one connection to Xero for accounting data, two connections to Plaid for two bank accounts, and a connection to Zettle for POS data.
         """
         hook_ctx = HookContext(operation_id='get-company', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetCompanyRequest, base_url, '/companies/{companyId}', request)
-        headers = {}
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = self.sdk_configuration.user_agent
+        url = utils.generate_url(base_url, '/companies/{companyId}', request)
         
         if callable(self.sdk_configuration.security):
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security())
+            headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security)
+            headers, query_params = utils.get_security(self.sdk_configuration.security)
         
+        headers['Accept'] = 'application/json'
+        headers['user-agent'] = self.sdk_configuration.user_agent
+        client = self.sdk_configuration.client
         
         global_retry_config = self.sdk_configuration.retry_config
         retry_config = retries
         if retry_config is None:
             if global_retry_config:
                 retry_config = global_retry_config
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
+        req = None
         def do_request():
+            nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('GET', url, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
             if utils.match_status_codes(['401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
-        content_type = http_res.headers.get('Content-Type')
         
-        res = operations.GetCompanyResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetCompanyResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(content_type, 'application/json'):
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.Company])
                 res.company = out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [401, 402, 403, 404, 429, 500, 503]:
-            if utils.match_content_type(content_type, 'application/json'):
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
-                out.raw_response = http_res
                 raise out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+        else:
+            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
     def list(self, request: operations.ListCompaniesRequest, retries: Optional[utils.RetryConfig] = None) -> operations.ListCompaniesResponse:
         r"""List companies
@@ -270,81 +275,83 @@
         A [company](https://docs.codat.io/platform-api#/schemas/Company) represents a business sharing access to their data.
         Each company can have multiple [connections](https://docs.codat.io/platform-api#/schemas/Connection) to different data sources, such as one connection to Xero for accounting data, two connections to Plaid for two bank accounts, and a connection to Zettle for POS data.
         """
         hook_ctx = HookContext(operation_id='list-companies', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
         url = base_url + '/companies'
-        headers = {}
-        query_params = utils.get_query_params(operations.ListCompaniesRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = self.sdk_configuration.user_agent
         
         if callable(self.sdk_configuration.security):
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security())
+            headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security)
+            headers, query_params = utils.get_security(self.sdk_configuration.security)
         
+        query_params = { **utils.get_query_params(request), **query_params }
+        headers['Accept'] = 'application/json'
+        headers['user-agent'] = self.sdk_configuration.user_agent
+        client = self.sdk_configuration.client
         
         global_retry_config = self.sdk_configuration.retry_config
         retry_config = retries
         if retry_config is None:
             if global_retry_config:
                 retry_config = global_retry_config
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
+        req = None
         def do_request():
+            nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
             if utils.match_status_codes(['400','401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
-        content_type = http_res.headers.get('Content-Type')
         
-        res = operations.ListCompaniesResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.ListCompaniesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(content_type, 'application/json'):
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.Companies])
                 res.companies = out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [400, 401, 402, 403, 404, 429, 500, 503]:
-            if utils.match_content_type(content_type, 'application/json'):
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
-                out.raw_response = http_res
                 raise out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+        else:
+            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
     def update(self, request: operations.UpdateCompanyRequest, retries: Optional[utils.RetryConfig] = None) -> operations.UpdateCompanyResponse:
         r"""Update company
@@ -353,81 +360,84 @@
 
         A [company](https://docs.codat.io/platform-api#/schemas/Company) represents a business sharing access to their data.
         Each company can have multiple [connections](https://docs.codat.io/platform-api#/schemas/Connection) to different data sources, such as one connection to Xero for accounting data, two connections to Plaid for two bank accounts, and a connection to Zettle for POS data.
         """
         hook_ctx = HookContext(operation_id='update-company', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateCompanyRequest, base_url, '/companies/{companyId}', request)
-        headers = {}
+        url = utils.generate_url(base_url, '/companies/{companyId}', request)
+        
+        if callable(self.sdk_configuration.security):
+            headers, query_params = utils.get_security(self.sdk_configuration.security())
+        else:
+            headers, query_params = utils.get_security(self.sdk_configuration.security)
+        
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateCompanyRequest, "company_request_body", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
-        
-        if callable(self.sdk_configuration.security):
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security())
-        else:
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security)
-        
+        client = self.sdk_configuration.client
         
         global_retry_config = self.sdk_configuration.retry_config
         retry_config = retries
         if retry_config is None:
             if global_retry_config:
                 retry_config = global_retry_config
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
+        req = None
         def do_request():
+            nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('PUT', url, data=data, files=form, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('PUT', url, params=query_params, data=data, files=form, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
             if utils.match_status_codes(['401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
-        content_type = http_res.headers.get('Content-Type')
         
-        res = operations.UpdateCompanyResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.UpdateCompanyResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(content_type, 'application/json'):
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.Company])
                 res.company = out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [401, 402, 403, 404, 429, 500, 503]:
-            if utils.match_content_type(content_type, 'application/json'):
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
-                out.raw_response = http_res
                 raise out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+        else:
+            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
-    
+    
+
```

### Comparing `codat-platform-3.4.0/src/codatplatform/connections.py` & `codat-platform-3.5.0/src/codatplatform/webhooks.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,500 +1,518 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from codatplatform import utils
-from codatplatform._hooks import HookContext
+from codatplatform._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from codatplatform.models import errors, operations, shared
 from typing import Optional
 
-class Connections:
-    r"""Manage your companies' data connections."""
+class Webhooks:
+    r"""Create and manage webhooks that listen to Codat's events."""
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
-    def create(self, request: operations.CreateConnectionRequest, retries: Optional[utils.RetryConfig] = None) -> operations.CreateConnectionResponse:
-        r"""Create connection
-        Creates a connection for the company by providing a valid `platformKey`. 
+    def create(self, request: Optional[shared.CreateRule], retries: Optional[utils.RetryConfig] = None) -> operations.CreateRuleResponse:
+        r"""Create webhook
+        Create a new webhook configuration
 
-        Use the [List Integrations](https://docs.codat.io/platform-api#/operations/list-integrations) endpoint to access valid platform keys.
+        Deprecated method: This will be removed in a future release, please migrate away from it as soon as possible.
         """
-        hook_ctx = HookContext(operation_id='create-connection', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        hook_ctx = HookContext(operation_id='create-rule', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateConnectionRequest, base_url, '/companies/{companyId}/connections', request)
-        headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, operations.CreateConnectionRequest, "request_body", False, True, 'json')
-        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
-            headers['content-type'] = req_content_type
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = self.sdk_configuration.user_agent
+        url = base_url + '/rules'
         
         if callable(self.sdk_configuration.security):
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security())
+            headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security)
+            headers, query_params = utils.get_security(self.sdk_configuration.security)
         
+        req_content_type, data, form = utils.serialize_request_body(request, Optional[shared.CreateRule], "request", False, True, 'json')
+        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
+        headers['Accept'] = 'application/json'
+        headers['user-agent'] = self.sdk_configuration.user_agent
+        client = self.sdk_configuration.client
         
         global_retry_config = self.sdk_configuration.retry_config
         retry_config = retries
         if retry_config is None:
             if global_retry_config:
                 retry_config = global_retry_config
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
+        req = None
         def do_request():
+            nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('POST', url, data=data, files=form, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
-            if utils.match_status_codes(['401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+            if utils.match_status_codes(['401','402','403','429','4XX','500','503','5XX'], http_res.status_code):
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
-        content_type = http_res.headers.get('Content-Type')
         
-        res = operations.CreateConnectionResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.CreateRuleResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[shared.Connection])
-                res.connection = out
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Webhook])
+                res.webhook = out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code in [401, 402, 403, 404, 429, 500, 503]:
-            if utils.match_content_type(content_type, 'application/json'):
+        elif http_res.status_code in [401, 402, 403, 429, 500, 503]:
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
-                out.raw_response = http_res
                 raise out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+        else:
+            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def delete(self, request: operations.DeleteConnectionRequest, retries: Optional[utils.RetryConfig] = None) -> operations.DeleteConnectionResponse:
-        r"""Delete connection
-        Revoke and remove a connection from a company.
-        This operation is not reversible. The end user would need to reauthorize a new data connection if you wish to view new data for this company.
+    def create_consumer(self, request: Optional[shared.WebhookConsumerPrototype], retries: Optional[utils.RetryConfig] = None) -> operations.CreateWebhookConsumerResponse:
+        r"""Create webhook consumer
+        Use the *Create webhook consumer* endpoint to create a new webhook consumer that will listen to messages we send you.
+
+        [Webhook consumer](https://docs.codat.io/platform-api#/schemas/WebhookConsumer) is an HTTP endpoint that you configure to subscribe to specific events. See our documentation for more details on [Codat's webhook service](https://docs.codat.io/using-the-api/webhooks/overview).
         """
-        hook_ctx = HookContext(operation_id='delete-connection', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        hook_ctx = HookContext(operation_id='create-webhook-consumer', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.DeleteConnectionRequest, base_url, '/companies/{companyId}/connections/{connectionId}', request)
-        headers = {}
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = self.sdk_configuration.user_agent
+        url = base_url + '/webhooks'
         
         if callable(self.sdk_configuration.security):
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security())
+            headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security)
+            headers, query_params = utils.get_security(self.sdk_configuration.security)
         
+        req_content_type, data, form = utils.serialize_request_body(request, Optional[shared.WebhookConsumerPrototype], "request", False, True, 'json')
+        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
+        headers['Accept'] = 'application/json'
+        headers['user-agent'] = self.sdk_configuration.user_agent
+        client = self.sdk_configuration.client
         
         global_retry_config = self.sdk_configuration.retry_config
         retry_config = retries
         if retry_config is None:
             if global_retry_config:
                 retry_config = global_retry_config
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
+        req = None
         def do_request():
+            nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('DELETE', url, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
-            if utils.match_status_codes(['401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+            if utils.match_status_codes(['401','402','403','429','4XX','500','503','5XX'], http_res.status_code):
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
-        content_type = http_res.headers.get('Content-Type')
         
-        res = operations.DeleteConnectionResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.CreateWebhookConsumerResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
-        if http_res.status_code == 200:
-            pass
-        elif http_res.status_code in [401, 402, 403, 404, 429, 500, 503]:
-            if utils.match_content_type(content_type, 'application/json'):
+        if http_res.status_code == 201:
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[shared.WebhookConsumer])
+                res.webhook_consumer = out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
+        elif http_res.status_code in [401, 402, 403, 429, 500, 503]:
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
-                out.raw_response = http_res
                 raise out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+        else:
+            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def get(self, request: operations.GetConnectionRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetConnectionResponse:
-        r"""Get connection
-        Returns a specific connection for a company when valid identifiers are provided. If the identifiers are for a deleted company and/or connection, a not found response is returned.
+    def delete_consumer(self, request: operations.DeleteWebhookConsumerRequest, retries: Optional[utils.RetryConfig] = None) -> operations.DeleteWebhookConsumerResponse:
+        r"""Delete webhook consumer
+        Use the *Delete webhook consumer* endpoint to delete an existing webhoook consumer, providing its valid `id` as a parameter.
+
+        [Webhook consumer](https://docs.codat.io/platform-api#/schemas/WebhookConsumer) is an HTTP endpoint that you configure to subscribe to specific events. See our documentation for more details on [Codat's webhook service](https://docs.codat.io/using-the-api/webhooks/overview).
         """
-        hook_ctx = HookContext(operation_id='get-connection', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        hook_ctx = HookContext(operation_id='delete-webhook-consumer', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetConnectionRequest, base_url, '/companies/{companyId}/connections/{connectionId}', request)
-        headers = {}
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = self.sdk_configuration.user_agent
+        url = utils.generate_url(base_url, '/webhooks/{webhookId}', request)
         
         if callable(self.sdk_configuration.security):
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security())
+            headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security)
+            headers, query_params = utils.get_security(self.sdk_configuration.security)
         
+        headers['Accept'] = 'application/json'
+        headers['user-agent'] = self.sdk_configuration.user_agent
+        client = self.sdk_configuration.client
         
         global_retry_config = self.sdk_configuration.retry_config
         retry_config = retries
         if retry_config is None:
             if global_retry_config:
                 retry_config = global_retry_config
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
+        req = None
         def do_request():
+            nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('GET', url, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('DELETE', url, params=query_params, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
             if utils.match_status_codes(['401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
-        content_type = http_res.headers.get('Content-Type')
         
-        res = operations.GetConnectionResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.DeleteWebhookConsumerResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
-        if http_res.status_code == 200:
-            if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[shared.Connection])
-                res.connection = out
-            else:
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
+        if http_res.status_code == 204:
+            pass
         elif http_res.status_code in [401, 402, 403, 404, 429, 500, 503]:
-            if utils.match_content_type(content_type, 'application/json'):
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
-                out.raw_response = http_res
                 raise out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+        else:
+            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def list(self, request: operations.ListConnectionsRequest, retries: Optional[utils.RetryConfig] = None) -> operations.ListConnectionsResponse:
-        r"""List connections
-        List the connections for a company.
+    def get(self, request: operations.GetWebhookRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetWebhookResponse:
+        r"""Get webhook
+        Get a single webhook
+
+        Deprecated method: This will be removed in a future release, please migrate away from it as soon as possible.
         """
-        hook_ctx = HookContext(operation_id='list-connections', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        hook_ctx = HookContext(operation_id='get-webhook', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListConnectionsRequest, base_url, '/companies/{companyId}/connections', request)
-        headers = {}
-        query_params = utils.get_query_params(operations.ListConnectionsRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = self.sdk_configuration.user_agent
+        url = utils.generate_url(base_url, '/rules/{ruleId}', request)
         
         if callable(self.sdk_configuration.security):
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security())
+            headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security)
+            headers, query_params = utils.get_security(self.sdk_configuration.security)
         
+        headers['Accept'] = 'application/json'
+        headers['user-agent'] = self.sdk_configuration.user_agent
+        client = self.sdk_configuration.client
         
         global_retry_config = self.sdk_configuration.retry_config
         retry_config = retries
         if retry_config is None:
             if global_retry_config:
                 retry_config = global_retry_config
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
+        req = None
         def do_request():
+            nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
-            if utils.match_status_codes(['400','401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+            if utils.match_status_codes(['401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
-        content_type = http_res.headers.get('Content-Type')
         
-        res = operations.ListConnectionsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetWebhookResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[shared.Connections])
-                res.connections = out
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Webhook])
+                res.webhook = out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code in [400, 401, 402, 403, 404, 429, 500, 503]:
-            if utils.match_content_type(content_type, 'application/json'):
+        elif http_res.status_code in [401, 402, 403, 404, 429, 500, 503]:
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
-                out.raw_response = http_res
                 raise out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+        else:
+            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def unlink(self, request: operations.UnlinkConnectionRequest, retries: Optional[utils.RetryConfig] = None) -> operations.UnlinkConnectionResponse:
-        r"""Unlink connection
-        This allows you to deauthorize a connection, without deleting it from Codat. This means you can still view any data that has previously been pulled into Codat, and also lets you re-authorize in future if your customer wishes to resume sharing their data.
+    def list(self, request: operations.ListRulesRequest, retries: Optional[utils.RetryConfig] = None) -> operations.ListRulesResponse:
+        r"""List webhooks
+        List webhooks that you are subscribed to.
+
+        Deprecated method: This will be removed in a future release, please migrate away from it as soon as possible.
         """
-        hook_ctx = HookContext(operation_id='unlink-connection', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        hook_ctx = HookContext(operation_id='list-rules', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UnlinkConnectionRequest, base_url, '/companies/{companyId}/connections/{connectionId}', request)
-        headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, operations.UnlinkConnectionRequest, "update_connection_status", False, True, 'json')
-        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
-            headers['content-type'] = req_content_type
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = self.sdk_configuration.user_agent
+        url = base_url + '/rules'
         
         if callable(self.sdk_configuration.security):
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security())
+            headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security)
+            headers, query_params = utils.get_security(self.sdk_configuration.security)
         
+        query_params = { **utils.get_query_params(request), **query_params }
+        headers['Accept'] = 'application/json'
+        headers['user-agent'] = self.sdk_configuration.user_agent
+        client = self.sdk_configuration.client
         
         global_retry_config = self.sdk_configuration.retry_config
         retry_config = retries
         if retry_config is None:
             if global_retry_config:
                 retry_config = global_retry_config
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
+        req = None
         def do_request():
+            nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('PATCH', url, data=data, files=form, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
-            if utils.match_status_codes(['401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+            if utils.match_status_codes(['400','401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
-        content_type = http_res.headers.get('Content-Type')
         
-        res = operations.UnlinkConnectionResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.ListRulesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[shared.Connection])
-                res.connection = out
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Webhooks])
+                res.webhooks = out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code in [401, 402, 403, 404, 429, 500, 503]:
-            if utils.match_content_type(content_type, 'application/json'):
+        elif http_res.status_code in [400, 401, 402, 403, 404, 429, 500, 503]:
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
-                out.raw_response = http_res
                 raise out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+        else:
+            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def update_authorization(self, request: operations.UpdateConnectionAuthorizationRequest, retries: Optional[utils.RetryConfig] = None) -> operations.UpdateConnectionAuthorizationResponse:
-        r"""Update authorization
-        Update data connection's authorization.
+    def list_consumers(self, retries: Optional[utils.RetryConfig] = None) -> operations.ListWebhookConsumersResponse:
+        r"""List webhook consumers
+        Use the *List webhook consumers* endpoint to return a list of all webhook consumers that currently exist for your client.
+
+        [Webhook consumer](https://docs.codat.io/platform-api#/schemas/WebhookConsumer) is an HTTP endpoint that you configure to subscribe to specific events. See our documentation for more details on [Codat's webhook service](https://docs.codat.io/using-the-api/webhooks/overview).
         """
-        hook_ctx = HookContext(operation_id='update-connection-authorization', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        hook_ctx = HookContext(operation_id='list-webhook-consumers', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateConnectionAuthorizationRequest, base_url, '/companies/{companyId}/connections/{connectionId}/authorization', request)
-        headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateConnectionAuthorizationRequest, "request_body", False, True, 'json')
-        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
-            headers['content-type'] = req_content_type
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = self.sdk_configuration.user_agent
+        url = base_url + '/webhooks'
         
         if callable(self.sdk_configuration.security):
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security())
+            headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security)
+            headers, query_params = utils.get_security(self.sdk_configuration.security)
         
+        headers['Accept'] = 'application/json'
+        headers['user-agent'] = self.sdk_configuration.user_agent
+        client = self.sdk_configuration.client
         
         global_retry_config = self.sdk_configuration.retry_config
         retry_config = retries
         if retry_config is None:
             if global_retry_config:
                 retry_config = global_retry_config
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
+        req = None
         def do_request():
+            nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('PUT', url, data=data, files=form, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
-            if utils.match_status_codes(['401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+            if utils.match_status_codes(['400','401','402','403','429','4XX','500','503','5XX'], http_res.status_code):
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
-        content_type = http_res.headers.get('Content-Type')
         
-        res = operations.UpdateConnectionAuthorizationResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.ListWebhookConsumersResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[shared.Connection])
-                res.connection = out
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[shared.WebhookConsumers])
+                res.webhook_consumers = out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code in [401, 402, 403, 404, 429, 500, 503]:
-            if utils.match_content_type(content_type, 'application/json'):
+        elif http_res.status_code in [400, 401, 402, 403, 429, 500, 503]:
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
-                out.raw_response = http_res
                 raise out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+        else:
+            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
-    
+    
+
```

### Comparing `codat-platform-3.4.0/src/codatplatform/custom_data_type.py` & `codat-platform-3.5.0/src/codatplatform/groups.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,351 +1,356 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from codatplatform import utils
-from codatplatform._hooks import HookContext
+from codatplatform._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from codatplatform.models import errors, operations, shared
 from typing import Optional
 
-class CustomDataType:
-    r"""View and configure custom data types for supported integrations."""
+class Groups:
+    r"""Define and manage sets of companies based on a chosen characteristic."""
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
-    def configure(self, request: operations.ConfigureCustomDataTypeRequest, retries: Optional[utils.RetryConfig] = None) -> operations.ConfigureCustomDataTypeResponse:
-        r"""Configure custom data type
-        The *Configure custom data type* endpoint allows you to maintain or change the configuration required to return a custom data type for a specific integration. 
+    def add_company(self, request: operations.AddCompanyToGroupRequest, retries: Optional[utils.RetryConfig] = None) -> operations.AddCompanyToGroupResponse:
+        r"""Add company
+        Use the *Add company* endpoint to assign a company to a group. A company can belong to multiple groups, but can only be added to one group at a time.
 
-        A [custom data type](https://docs.codat.io/using-the-api/custom-data) is an additional data type you can create that is not included in Codat's standardized data model.
-
-        ### Tips and traps
-
-        - You can only configure a single custom data type for a single platform at a time. Use the endpoint multiple times if you need to configure it for multiple platforms. 
-
-        - You can only indicate a single data source for each customer data type. 
-
-        - Make your custom configuration as similar as possible to our standard data types so you can interact with them in exactly the same way.
+        [Groups](https://docs.codat.io/platform-api#/schemas/Group) define a set of companies that are organized based on a chosen characteristic and can be managed in the same way.
         """
-        hook_ctx = HookContext(operation_id='configure-custom-data-type', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        hook_ctx = HookContext(operation_id='add-company-to-group', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ConfigureCustomDataTypeRequest, base_url, '/integrations/{platformKey}/dataTypes/custom/{customDataIdentifier}', request)
-        headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, operations.ConfigureCustomDataTypeRequest, "custom_data_type_configuration", False, True, 'json')
-        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
-            headers['content-type'] = req_content_type
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = self.sdk_configuration.user_agent
+        url = utils.generate_url(base_url, '/companies/{companyId}/groups', request)
         
         if callable(self.sdk_configuration.security):
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security())
+            headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security)
+            headers, query_params = utils.get_security(self.sdk_configuration.security)
         
+        req_content_type, data, form = utils.serialize_request_body(request, operations.AddCompanyToGroupRequest, "company_group_assignment", False, True, 'json')
+        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
+        headers['Accept'] = 'application/json'
+        headers['user-agent'] = self.sdk_configuration.user_agent
+        client = self.sdk_configuration.client
         
         global_retry_config = self.sdk_configuration.retry_config
         retry_config = retries
         if retry_config is None:
             if global_retry_config:
                 retry_config = global_retry_config
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
+        req = None
         def do_request():
+            nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('PUT', url, data=data, files=form, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('PATCH', url, params=query_params, data=data, files=form, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
             if utils.match_status_codes(['401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
-        content_type = http_res.headers.get('Content-Type')
         
-        res = operations.ConfigureCustomDataTypeResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.AddCompanyToGroupResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[shared.CustomDataTypeConfiguration])
-                res.custom_data_type_configuration = out
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Company])
+                res.company = out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [401, 402, 403, 404, 429, 500, 503]:
-            if utils.match_content_type(content_type, 'application/json'):
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
-                out.raw_response = http_res
                 raise out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+        else:
+            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def get_configuration(self, request: operations.GetCustomDataTypeConfigurationRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetCustomDataTypeConfigurationResponse:
-        r"""Get custom data configuration
-        The *Get custom data configuration* endpoint returns existing configuration details for the specified custom data type and integration pair you previously configured.
+    def create(self, request: Optional[shared.GroupPrototype], retries: Optional[utils.RetryConfig] = None) -> operations.CreateGroupResponse:
+        r"""Create group
+        Use the *Create group* endpoint to generate a new group that you can assign your companies to.
+
+        [Groups](https://docs.codat.io/platform-api#/schemas/Group) define a set of companies that are organized based on a chosen characteristic and can be managed in the same way.
+
+        ### Tips and traps
 
-        A [custom data type](https://docs.codat.io/using-the-api/custom-data) is an additional data type you can create that is not included in Codat's standardized data model.
+        * The maximum length for the group name is 50 characters.
+        * It's possible to create up to 20 groups per client.
         """
-        hook_ctx = HookContext(operation_id='get-custom-data-type-configuration', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        hook_ctx = HookContext(operation_id='create-group', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetCustomDataTypeConfigurationRequest, base_url, '/integrations/{platformKey}/dataTypes/custom/{customDataIdentifier}', request)
-        headers = {}
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = self.sdk_configuration.user_agent
+        url = base_url + '/groups'
         
         if callable(self.sdk_configuration.security):
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security())
+            headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security)
+            headers, query_params = utils.get_security(self.sdk_configuration.security)
         
+        req_content_type, data, form = utils.serialize_request_body(request, Optional[shared.GroupPrototype], "request", False, True, 'json')
+        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
+        headers['Accept'] = 'application/json'
+        headers['user-agent'] = self.sdk_configuration.user_agent
+        client = self.sdk_configuration.client
         
         global_retry_config = self.sdk_configuration.retry_config
         retry_config = retries
         if retry_config is None:
             if global_retry_config:
                 retry_config = global_retry_config
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
+        req = None
         def do_request():
+            nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('GET', url, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
-            if utils.match_status_codes(['401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+            if utils.match_status_codes(['401','402','403','409','429','4XX','500','503','5XX'], http_res.status_code):
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
-        content_type = http_res.headers.get('Content-Type')
         
-        res = operations.GetCustomDataTypeConfigurationResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.CreateGroupResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[shared.CustomDataTypeRecords])
-                res.custom_data_type_records = out
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Group])
+                res.group = out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code in [401, 402, 403, 404, 429, 500, 503]:
-            if utils.match_content_type(content_type, 'application/json'):
+        elif http_res.status_code in [401, 402, 403, 409, 429, 500, 503]:
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
-                out.raw_response = http_res
                 raise out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+        else:
+            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def list(self, request: operations.ListCustomDataTypeRecordsRequest, retries: Optional[utils.RetryConfig] = None) -> operations.ListCustomDataTypeRecordsResponse:
-        r"""List custom data type records
-        The *List custom data type records* endpoint returns a paginated list of records pulled for the specified custom data type you previously configured.
+    def list(self, retries: Optional[utils.RetryConfig] = None) -> operations.ListGroupsResponse:
+        r"""List groups
+        Use the *List group* endpoint to return a list of all groups that currently exist for your client.
 
-        A [custom data type](https://docs.codat.io/using-the-api/custom-data) is an additional data type you can create that is not included in Codat's standardized data model.s endpoint returns a paginated list of records whose schema is defined [Configure custom data type](https://docs.codat.io/platform-api#/operations/configure-custom-data-type)
+        [Groups](https://docs.codat.io/platform-api#/schemas/Group) define a set of companies that are organized based on a chosen characteristic and can be managed in the same way.
         """
-        hook_ctx = HookContext(operation_id='list-custom-data-type-records', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        hook_ctx = HookContext(operation_id='list-groups', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListCustomDataTypeRecordsRequest, base_url, '/companies/{companyId}/connections/{connectionId}/data/custom/{customDataIdentifier}', request)
-        headers = {}
-        query_params = utils.get_query_params(operations.ListCustomDataTypeRecordsRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = self.sdk_configuration.user_agent
+        url = base_url + '/groups'
         
         if callable(self.sdk_configuration.security):
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security())
+            headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security)
+            headers, query_params = utils.get_security(self.sdk_configuration.security)
         
+        headers['Accept'] = 'application/json'
+        headers['user-agent'] = self.sdk_configuration.user_agent
+        client = self.sdk_configuration.client
         
         global_retry_config = self.sdk_configuration.retry_config
         retry_config = retries
         if retry_config is None:
             if global_retry_config:
                 retry_config = global_retry_config
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
+        req = None
         def do_request():
+            nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
-            if utils.match_status_codes(['400','401','402','403','404','429','451','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+            if utils.match_status_codes(['401','402','403','429','4XX','500','503','5XX'], http_res.status_code):
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
-        content_type = http_res.headers.get('Content-Type')
         
-        res = operations.ListCustomDataTypeRecordsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.ListGroupsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[shared.CustomDataTypeRecords])
-                res.custom_data_type_records = out
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Groups])
+                res.groups = out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code in [400, 401, 402, 403, 404, 429, 451, 500, 503]:
-            if utils.match_content_type(content_type, 'application/json'):
+        elif http_res.status_code in [401, 402, 403, 429, 500, 503]:
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
-                out.raw_response = http_res
                 raise out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+        else:
+            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def refresh(self, request: operations.RefreshCustomDataTypeRequest, retries: Optional[utils.RetryConfig] = None) -> operations.RefreshCustomDataTypeResponse:
-        r"""Refresh custom data type
-        The *Refresh custom data type* endpoint refreshes the specified custom data type for a given company. This is an asynchronous operation that will sync updated data from the linked integration into Codat for you to view.
+    def remove_company(self, request: operations.RemoveCompanyFromGroupRequest, retries: Optional[utils.RetryConfig] = None) -> operations.RemoveCompanyFromGroupResponse:
+        r"""Remove company
+        Use the *Remove company* endpoint to remove a company from a group.
+
+        [Groups](https://docs.codat.io/platform-api#/schemas/Group) define a set of companies that are organized based on a chosen characteristic and can be managed in the same way.
         """
-        hook_ctx = HookContext(operation_id='refresh-custom-data-type', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        hook_ctx = HookContext(operation_id='remove-company-from-group', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RefreshCustomDataTypeRequest, base_url, '/companies/{companyId}/connections/{connectionId}/data/queue/custom/{customDataIdentifier}', request)
-        headers = {}
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = self.sdk_configuration.user_agent
+        url = utils.generate_url(base_url, '/companies/{companyId}/groups/{groupId}', request)
         
         if callable(self.sdk_configuration.security):
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security())
+            headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security)
+            headers, query_params = utils.get_security(self.sdk_configuration.security)
         
+        headers['Accept'] = 'application/json'
+        headers['user-agent'] = self.sdk_configuration.user_agent
+        client = self.sdk_configuration.client
         
         global_retry_config = self.sdk_configuration.retry_config
         retry_config = retries
         if retry_config is None:
             if global_retry_config:
                 retry_config = global_retry_config
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
+        req = None
         def do_request():
+            nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('POST', url, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('DELETE', url, params=query_params, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
-            if utils.match_status_codes(['401','402','403','404','429','451','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+            if utils.match_status_codes(['401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
-        content_type = http_res.headers.get('Content-Type')
         
-        res = operations.RefreshCustomDataTypeResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.RemoveCompanyFromGroupResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
-        if http_res.status_code == 200:
-            if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[shared.PullOperation])
-                res.pull_operation = out
-            else:
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code in [401, 402, 403, 404, 429, 451, 500, 503]:
-            if utils.match_content_type(content_type, 'application/json'):
+        if http_res.status_code == 204:
+            pass
+        elif http_res.status_code in [401, 402, 403, 404, 429, 500, 503]:
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
-                out.raw_response = http_res
                 raise out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+        else:
+            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
-    
+    
+
```

### Comparing `codat-platform-3.4.0/src/codatplatform/groups.py` & `codat-platform-3.5.0/src/codatplatform/push_data.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,348 +1,271 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from codatplatform import utils
-from codatplatform._hooks import HookContext
+from codatplatform._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from codatplatform.models import errors, operations, shared
 from typing import Optional
 
-class Groups:
-    r"""Create groups and link them to your Codat companies."""
+class PushData:
+    r"""Initiate and monitor Create, Update, and Delete operations."""
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
-    def add_company(self, request: operations.AddCompanyToGroupRequest, retries: Optional[utils.RetryConfig] = None) -> operations.AddCompanyToGroupResponse:
-        r"""Add company
-        Use the *Add company* endpoint to assign a company to a group. A company can belong to multiple groups, but can only be added to one group at a time.
+    def get_model_options(self, request: operations.GetCreateUpdateModelOptionsByDataTypeRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetCreateUpdateModelOptionsByDataTypeResponse:
+        r"""Get push options
+        This is the generic documentation for creation and updating of data. See the equivalent endpoint for a given data type for more specific information. 
 
-        [Groups](https://docs.codat.io/platform-api#/schemas/Group) define a set of companies that are organized based on a chosen characteristic and can be managed in the same way.
+        Before pushing data into accounting software, it is often necessary to collect some details from the user as to how they would like the data to be inserted. This includes names and amounts on transactional entities, but also factors such as categorisation of entities, which is often handled differently between different accounting packages. A good example of this is specifying where on the balance sheet/profit and loss reports the user would like a newly-created nominal account to appear.
+
+        Codat tries not to limit users to pushing to a very limited number of standard categories, so we have implemented \"options\" endpoints, which allow us to expose to our clients the fields which are required to be pushed for a specific linked company, and the options which may be selected for each field.
+
+
+        > **Supported Integrations**
+        > 
+        > Check out our [coverage explorer](https://knowledge.codat.io/) for integrations that support push (POST/PUT methods).
         """
-        hook_ctx = HookContext(operation_id='add-company-to-group', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        hook_ctx = HookContext(operation_id='get-create-update-model-options-by-data-type', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.AddCompanyToGroupRequest, base_url, '/companies/{companyId}/groups', request)
-        headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, operations.AddCompanyToGroupRequest, "company_group_assignment", False, True, 'json')
-        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
-            headers['content-type'] = req_content_type
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = self.sdk_configuration.user_agent
+        url = utils.generate_url(base_url, '/companies/{companyId}/connections/{connectionId}/options/{dataType}', request)
         
         if callable(self.sdk_configuration.security):
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security())
+            headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security)
+            headers, query_params = utils.get_security(self.sdk_configuration.security)
         
+        headers['Accept'] = 'application/json'
+        headers['user-agent'] = self.sdk_configuration.user_agent
+        client = self.sdk_configuration.client
         
         global_retry_config = self.sdk_configuration.retry_config
         retry_config = retries
         if retry_config is None:
             if global_retry_config:
                 retry_config = global_retry_config
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
+        req = None
         def do_request():
+            nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('PATCH', url, data=data, files=form, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
             if utils.match_status_codes(['401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
-        content_type = http_res.headers.get('Content-Type')
         
-        res = operations.AddCompanyToGroupResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetCreateUpdateModelOptionsByDataTypeResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[shared.Company])
-                res.company = out
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[shared.PushOption])
+                res.push_option = out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [401, 402, 403, 404, 429, 500, 503]:
-            if utils.match_content_type(content_type, 'application/json'):
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
-                out.raw_response = http_res
                 raise out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+        else:
+            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def create(self, request: Optional[shared.GroupPrototype], retries: Optional[utils.RetryConfig] = None) -> operations.CreateGroupResponse:
-        r"""Create group
-        Use the *Create group* endpoint to generate a new group that you can assign your companies to.
-
-        [Groups](https://docs.codat.io/platform-api#/schemas/Group) define a set of companies that are organized based on a chosen characteristic and can be managed in the same way.
-
-        ### Tips and traps
-
-        * The maximum length for the group name is 50 characters.
-        * It's possible to create up to 20 groups per client.
+    def get_operation(self, request: operations.GetPushOperationRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetPushOperationResponse:
+        r"""Get push operation
+        Retrieve push operation.
         """
-        hook_ctx = HookContext(operation_id='create-group', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        hook_ctx = HookContext(operation_id='get-push-operation', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/groups'
-        headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, Optional[shared.GroupPrototype], "request", False, True, 'json')
-        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
-            headers['content-type'] = req_content_type
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = self.sdk_configuration.user_agent
+        url = utils.generate_url(base_url, '/companies/{companyId}/push/{pushOperationKey}', request)
         
         if callable(self.sdk_configuration.security):
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security())
+            headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security)
+            headers, query_params = utils.get_security(self.sdk_configuration.security)
         
+        headers['Accept'] = 'application/json'
+        headers['user-agent'] = self.sdk_configuration.user_agent
+        client = self.sdk_configuration.client
         
         global_retry_config = self.sdk_configuration.retry_config
         retry_config = retries
         if retry_config is None:
             if global_retry_config:
                 retry_config = global_retry_config
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
+        req = None
         def do_request():
+            nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('POST', url, data=data, files=form, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
-            if utils.match_status_codes(['401','402','403','409','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+            if utils.match_status_codes(['401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
-        content_type = http_res.headers.get('Content-Type')
         
-        res = operations.CreateGroupResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetPushOperationResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[shared.Group])
-                res.group = out
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[shared.PushOperation])
+                res.push_operation = out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code in [401, 402, 403, 409, 429, 500, 503]:
-            if utils.match_content_type(content_type, 'application/json'):
+        elif http_res.status_code in [401, 402, 403, 404, 429, 500, 503]:
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
-                out.raw_response = http_res
                 raise out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+        else:
+            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def list(self, retries: Optional[utils.RetryConfig] = None) -> operations.ListGroupsResponse:
-        r"""List groups
-        Use the *List group* endpoint to return a list of all groups that currently exist for your client.
-
-        [Groups](https://docs.codat.io/platform-api#/schemas/Group) define a set of companies that are organized based on a chosen characteristic and can be managed in the same way.
+    def list_operations(self, request: operations.GetCompanyPushHistoryRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetCompanyPushHistoryResponse:
+        r"""List push operations
+        List push operation records.
         """
-        hook_ctx = HookContext(operation_id='list-groups', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        hook_ctx = HookContext(operation_id='get-company-push-history', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/groups'
-        headers = {}
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = self.sdk_configuration.user_agent
+        url = utils.generate_url(base_url, '/companies/{companyId}/push', request)
         
         if callable(self.sdk_configuration.security):
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security())
+            headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security)
+            headers, query_params = utils.get_security(self.sdk_configuration.security)
         
+        query_params = { **utils.get_query_params(request), **query_params }
+        headers['Accept'] = 'application/json'
+        headers['user-agent'] = self.sdk_configuration.user_agent
+        client = self.sdk_configuration.client
         
         global_retry_config = self.sdk_configuration.retry_config
         retry_config = retries
         if retry_config is None:
             if global_retry_config:
                 retry_config = global_retry_config
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
+        req = None
         def do_request():
+            nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('GET', url, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
-            if utils.match_status_codes(['401','402','403','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+            if utils.match_status_codes(['400','401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
-        content_type = http_res.headers.get('Content-Type')
         
-        res = operations.ListGroupsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetCompanyPushHistoryResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[shared.Groups])
-                res.groups = out
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[shared.PushOperations])
+                res.push_operations = out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code in [401, 402, 403, 429, 500, 503]:
-            if utils.match_content_type(content_type, 'application/json'):
+        elif http_res.status_code in [400, 401, 402, 403, 404, 429, 500, 503]:
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
-                out.raw_response = http_res
                 raise out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+        else:
+            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
-    
-    def remove_company(self, request: operations.RemoveCompanyFromGroupRequest, retries: Optional[utils.RetryConfig] = None) -> operations.RemoveCompanyFromGroupResponse:
-        r"""Remove company
-        Use the *Remove company* endpoint to remove a company from a group.
-
-        [Groups](https://docs.codat.io/platform-api#/schemas/Group) define a set of companies that are organized based on a chosen characteristic and can be managed in the same way.
-        """
-        hook_ctx = HookContext(operation_id='remove-company-from-group', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
-        
-        url = utils.generate_url(operations.RemoveCompanyFromGroupRequest, base_url, '/companies/{companyId}/groups/{groupId}', request)
-        headers = {}
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = self.sdk_configuration.user_agent
-        
-        if callable(self.sdk_configuration.security):
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security())
-        else:
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security)
-        
-        
-        global_retry_config = self.sdk_configuration.retry_config
-        retry_config = retries
-        if retry_config is None:
-            if global_retry_config:
-                retry_config = global_retry_config
-            else:
-                retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
-
-        def do_request():
-            try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('DELETE', url, headers=headers).prepare(),
-                )
-                http_res = client.send(req)
-            except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
-
-            if utils.match_status_codes(['401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
-                    raise e
-            else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
-
-            return http_res
-
-        http_res = utils.retry(do_request, utils.Retries(retry_config, [
-            '408',
-            '429',
-            '5XX'
-        ]))
-        
-        content_type = http_res.headers.get('Content-Type')
-        
-        res = operations.RemoveCompanyFromGroupResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
-        
-        if http_res.status_code == 204:
-            pass
-        elif http_res.status_code in [401, 402, 403, 404, 429, 500, 503]:
-            if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
-                out.raw_response = http_res
-                raise out
-            else:
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
-            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
-
-        return res
 
-
```

### Comparing `codat-platform-3.4.0/src/codatplatform/integrations.py` & `codat-platform-3.5.0/src/codatplatform/integrations.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,255 +1,262 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from codatplatform import utils
-from codatplatform._hooks import HookContext
+from codatplatform._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from codatplatform.models import errors, operations, shared
 from typing import Optional
 
 class Integrations:
-    r"""View and manage your available integrations in Codat."""
+    r"""Get a list of integrations supported by Codat and their logos."""
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
     def get(self, request: operations.GetIntegrationRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetIntegrationResponse:
         r"""Get integration
         Get single integration, by platformKey
         """
         hook_ctx = HookContext(operation_id='get-integration', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetIntegrationRequest, base_url, '/integrations/{platformKey}', request)
-        headers = {}
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = self.sdk_configuration.user_agent
+        url = utils.generate_url(base_url, '/integrations/{platformKey}', request)
         
         if callable(self.sdk_configuration.security):
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security())
+            headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security)
+            headers, query_params = utils.get_security(self.sdk_configuration.security)
         
+        headers['Accept'] = 'application/json'
+        headers['user-agent'] = self.sdk_configuration.user_agent
+        client = self.sdk_configuration.client
         
         global_retry_config = self.sdk_configuration.retry_config
         retry_config = retries
         if retry_config is None:
             if global_retry_config:
                 retry_config = global_retry_config
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
+        req = None
         def do_request():
+            nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('GET', url, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
             if utils.match_status_codes(['401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
-        content_type = http_res.headers.get('Content-Type')
         
-        res = operations.GetIntegrationResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetIntegrationResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(content_type, 'application/json'):
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.Integration])
                 res.integration = out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [401, 402, 403, 404, 429, 500, 503]:
-            if utils.match_content_type(content_type, 'application/json'):
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
-                out.raw_response = http_res
                 raise out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+        else:
+            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
     def get_branding(self, request: operations.GetIntegrationsBrandingRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetIntegrationsBrandingResponse:
         r"""Get branding
         Get branding for platform.
         """
         hook_ctx = HookContext(operation_id='get-integrations-branding', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetIntegrationsBrandingRequest, base_url, '/integrations/{platformKey}/branding', request)
-        headers = {}
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = self.sdk_configuration.user_agent
+        url = utils.generate_url(base_url, '/integrations/{platformKey}/branding', request)
         
         if callable(self.sdk_configuration.security):
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security())
+            headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security)
+            headers, query_params = utils.get_security(self.sdk_configuration.security)
         
+        headers['Accept'] = 'application/json'
+        headers['user-agent'] = self.sdk_configuration.user_agent
+        client = self.sdk_configuration.client
         
         global_retry_config = self.sdk_configuration.retry_config
         retry_config = retries
         if retry_config is None:
             if global_retry_config:
                 retry_config = global_retry_config
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
+        req = None
         def do_request():
+            nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('GET', url, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
             if utils.match_status_codes(['401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
-        content_type = http_res.headers.get('Content-Type')
         
-        res = operations.GetIntegrationsBrandingResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetIntegrationsBrandingResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(content_type, 'application/json'):
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.Branding])
                 res.branding = out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [401, 402, 403, 404, 429, 500, 503]:
-            if utils.match_content_type(content_type, 'application/json'):
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
-                out.raw_response = http_res
                 raise out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+        else:
+            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
     def list(self, request: operations.ListIntegrationsRequest, retries: Optional[utils.RetryConfig] = None) -> operations.ListIntegrationsResponse:
         r"""List integrations
         List your available integrations
         """
         hook_ctx = HookContext(operation_id='list-integrations', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
         url = base_url + '/integrations'
-        headers = {}
-        query_params = utils.get_query_params(operations.ListIntegrationsRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = self.sdk_configuration.user_agent
         
         if callable(self.sdk_configuration.security):
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security())
+            headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security)
+            headers, query_params = utils.get_security(self.sdk_configuration.security)
         
+        query_params = { **utils.get_query_params(request), **query_params }
+        headers['Accept'] = 'application/json'
+        headers['user-agent'] = self.sdk_configuration.user_agent
+        client = self.sdk_configuration.client
         
         global_retry_config = self.sdk_configuration.retry_config
         retry_config = retries
         if retry_config is None:
             if global_retry_config:
                 retry_config = global_retry_config
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
+        req = None
         def do_request():
+            nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
             if utils.match_status_codes(['400','401','402','403','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
-        content_type = http_res.headers.get('Content-Type')
         
-        res = operations.ListIntegrationsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.ListIntegrationsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(content_type, 'application/json'):
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.Integrations])
                 res.integrations = out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [400, 401, 402, 403, 429, 500, 503]:
-            if utils.match_content_type(content_type, 'application/json'):
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
-                out.raw_response = http_res
                 raise out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+        else:
+            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
-    
+    
+
```

### Comparing `codat-platform-3.4.0/src/codatplatform/models/errors/errormessage.py` & `codat-platform-3.5.0/src/codatplatform/models/errors/errormessage.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/errors/sdkerror.py` & `codat-platform-3.5.0/src/codatplatform/models/errors/sdkerror.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/operations/__init__.py` & `codat-platform-3.5.0/src/codatplatform/models/operations/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 from .delete_company import *
 from .delete_connection import *
 from .delete_webhook_consumer import *
 from .get_company import *
 from .get_company_data_status import *
 from .get_company_push_history import *
 from .get_connection import *
+from .get_connection_management_access_token import *
+from .get_connection_management_cors_settings import *
 from .get_create_update_model_options_by_data_type import *
 from .get_custom_data_type_configuration import *
 from .get_integration import *
 from .get_integrations_branding import *
 from .get_profile import *
 from .get_profile_syncsettings import *
 from .get_pull_operation import *
@@ -36,14 +38,15 @@
 from .list_pull_operations import *
 from .list_rules import *
 from .list_webhook_consumers import *
 from .refresh_company_data import *
 from .refresh_custom_data_type import *
 from .refresh_data_type import *
 from .remove_company_from_group import *
+from .set_connection_management_cors_settings import *
 from .unlink_connection import *
 from .update_company import *
 from .update_connection_authorization import *
 from .update_profile import *
 from .update_profile_syncsettings import *
 
-__all__ = ["AddCompanyToGroupRequest","AddCompanyToGroupResponse","ConfigureCustomDataTypeRequest","ConfigureCustomDataTypeResponse","ConfigureSupplementalDataRequest","ConfigureSupplementalDataResponse","CreateAPIKeyResponse","CreateCompanyResponse","CreateConnectionRequest","CreateConnectionRequestBody","CreateConnectionResponse","CreateGroupResponse","CreateRuleResponse","CreateWebhookConsumerResponse","DataType","DeleteAPIKeyRequest","DeleteAPIKeyResponse","DeleteCompanyRequest","DeleteCompanyResponse","DeleteConnectionRequest","DeleteConnectionResponse","DeleteWebhookConsumerRequest","DeleteWebhookConsumerResponse","GetCompanyDataStatusRequest","GetCompanyDataStatusResponse","GetCompanyPushHistoryRequest","GetCompanyPushHistoryResponse","GetCompanyRequest","GetCompanyResponse","GetConnectionRequest","GetConnectionResponse","GetCreateUpdateModelOptionsByDataTypeRequest","GetCreateUpdateModelOptionsByDataTypeResponse","GetCustomDataTypeConfigurationRequest","GetCustomDataTypeConfigurationResponse","GetIntegrationRequest","GetIntegrationResponse","GetIntegrationsBrandingRequest","GetIntegrationsBrandingResponse","GetProfileResponse","GetProfileSyncSettingsResponse","GetPullOperationRequest","GetPullOperationResponse","GetPushOperationRequest","GetPushOperationResponse","GetSupplementalDataConfigurationRequest","GetSupplementalDataConfigurationResponse","GetWebhookRequest","GetWebhookResponse","ListAPIKeysResponse","ListCompaniesRequest","ListCompaniesResponse","ListConnectionsRequest","ListConnectionsResponse","ListCustomDataTypeRecordsRequest","ListCustomDataTypeRecordsResponse","ListGroupsResponse","ListIntegrationsRequest","ListIntegrationsResponse","ListPullOperationsRequest","ListPullOperationsResponse","ListRulesRequest","ListRulesResponse","ListWebhookConsumersResponse","PathParamDataType","RefreshCompanyDataRequest","RefreshCompanyDataResponse","RefreshCustomDataTypeRequest","RefreshCustomDataTypeResponse","RefreshDataTypeRequest","RefreshDataTypeResponse","RemoveCompanyFromGroupRequest","RemoveCompanyFromGroupResponse","UnlinkConnectionRequest","UnlinkConnectionResponse","UpdateCompanyRequest","UpdateCompanyResponse","UpdateConnectionAuthorizationRequest","UpdateConnectionAuthorizationResponse","UpdateProfileResponse","UpdateProfileSyncSettingsRequestBody","UpdateProfileSyncSettingsResponse"]
+__all__ = ["AddCompanyToGroupRequest","AddCompanyToGroupResponse","ConfigureCustomDataTypeRequest","ConfigureCustomDataTypeResponse","ConfigureSupplementalDataRequest","ConfigureSupplementalDataResponse","CreateAPIKeyResponse","CreateCompanyResponse","CreateConnectionRequest","CreateConnectionRequestBody","CreateConnectionResponse","CreateGroupResponse","CreateRuleResponse","CreateWebhookConsumerResponse","DataType","DeleteAPIKeyRequest","DeleteAPIKeyResponse","DeleteCompanyRequest","DeleteCompanyResponse","DeleteConnectionRequest","DeleteConnectionResponse","DeleteWebhookConsumerRequest","DeleteWebhookConsumerResponse","GetCompanyDataStatusRequest","GetCompanyDataStatusResponse","GetCompanyPushHistoryRequest","GetCompanyPushHistoryResponse","GetCompanyRequest","GetCompanyResponse","GetConnectionManagementAccessTokenRequest","GetConnectionManagementAccessTokenResponse","GetConnectionManagementCorsSettingsResponse","GetConnectionRequest","GetConnectionResponse","GetCreateUpdateModelOptionsByDataTypeRequest","GetCreateUpdateModelOptionsByDataTypeResponse","GetCustomDataTypeConfigurationRequest","GetCustomDataTypeConfigurationResponse","GetIntegrationRequest","GetIntegrationResponse","GetIntegrationsBrandingRequest","GetIntegrationsBrandingResponse","GetProfileResponse","GetProfileSyncSettingsResponse","GetPullOperationRequest","GetPullOperationResponse","GetPushOperationRequest","GetPushOperationResponse","GetSupplementalDataConfigurationRequest","GetSupplementalDataConfigurationResponse","GetWebhookRequest","GetWebhookResponse","ListAPIKeysResponse","ListCompaniesRequest","ListCompaniesResponse","ListConnectionsRequest","ListConnectionsResponse","ListCustomDataTypeRecordsRequest","ListCustomDataTypeRecordsResponse","ListGroupsResponse","ListIntegrationsRequest","ListIntegrationsResponse","ListPullOperationsRequest","ListPullOperationsResponse","ListRulesRequest","ListRulesResponse","ListWebhookConsumersResponse","PathParamDataType","RefreshCompanyDataRequest","RefreshCompanyDataResponse","RefreshCustomDataTypeRequest","RefreshCustomDataTypeResponse","RefreshDataTypeRequest","RefreshDataTypeResponse","RemoveCompanyFromGroupRequest","RemoveCompanyFromGroupResponse","SetConnectionManagementCorsSettingsResponse","UnlinkConnectionRequest","UnlinkConnectionResponse","UpdateCompanyRequest","UpdateCompanyResponse","UpdateConnectionAuthorizationRequest","UpdateConnectionAuthorizationResponse","UpdateProfileResponse","UpdateProfileSyncSettingsRequestBody","UpdateProfileSyncSettingsResponse"]
```

### Comparing `codat-platform-3.4.0/src/codatplatform/models/operations/add_company_to_group.py` & `codat-platform-3.5.0/src/codatplatform/models/operations/add_company_to_group.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/operations/configure_custom_data_type.py` & `codat-platform-3.5.0/src/codatplatform/models/operations/configure_custom_data_type.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/operations/configure_supplemental_data.py` & `codat-platform-3.5.0/src/codatplatform/models/operations/configure_supplemental_data.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/operations/create_api_key.py` & `codat-platform-3.5.0/src/codatplatform/models/operations/create_api_key.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/operations/create_company.py` & `codat-platform-3.5.0/src/codatplatform/models/operations/create_company.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/operations/create_connection.py` & `codat-platform-3.5.0/src/codatplatform/models/operations/create_connection.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/operations/create_group.py` & `codat-platform-3.5.0/src/codatplatform/models/operations/create_group.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/operations/create_rule.py` & `codat-platform-3.5.0/src/codatplatform/models/operations/create_rule.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/operations/create_webhook_consumer.py` & `codat-platform-3.5.0/src/codatplatform/models/operations/create_webhook_consumer.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/operations/delete_api_key.py` & `codat-platform-3.5.0/src/codatplatform/models/operations/delete_api_key.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/operations/delete_company.py` & `codat-platform-3.5.0/src/codatplatform/models/operations/delete_company.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/operations/delete_connection.py` & `codat-platform-3.5.0/src/codatplatform/models/operations/delete_connection.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/operations/delete_webhook_consumer.py` & `codat-platform-3.5.0/src/codatplatform/models/operations/delete_webhook_consumer.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/operations/get_company.py` & `codat-platform-3.5.0/src/codatplatform/models/operations/get_company.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/operations/get_company_data_status.py` & `codat-platform-3.5.0/src/codatplatform/models/operations/get_integration.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ...models.shared import datastatus as shared_datastatus
-from typing import Dict, Optional
+from ...models.shared import integration as shared_integration
+from typing import Optional
 
 
 @dataclasses.dataclass
-class GetCompanyDataStatusRequest:
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-    r"""Unique identifier for a company."""
+class GetIntegrationRequest:
+    platform_key: str = dataclasses.field(metadata={'path_param': { 'field_name': 'platformKey', 'style': 'simple', 'explode': False }})
+    r"""A unique 4-letter key to represent a platform in each integration."""
     
 
 
 
 @dataclasses.dataclass
-class GetCompanyDataStatusResponse:
+class GetIntegrationResponse:
     content_type: str = dataclasses.field()
     r"""HTTP response content type for this operation"""
     status_code: int = dataclasses.field()
     r"""HTTP response status code for this operation"""
     raw_response: requests_http.Response = dataclasses.field()
     r"""Raw HTTP response; suitable for custom response parsing"""
-    data_statuses: Optional[Dict[str, shared_datastatus.DataStatus]] = dataclasses.field(default=None)
+    integration: Optional[shared_integration.Integration] = dataclasses.field(default=None)
     r"""OK"""
```

### Comparing `codat-platform-3.4.0/src/codatplatform/models/operations/get_company_push_history.py` & `codat-platform-3.5.0/src/codatplatform/models/operations/get_company_push_history.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/operations/get_connection.py` & `codat-platform-3.5.0/src/codatplatform/models/operations/get_connection.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/operations/get_create_update_model_options_by_data_type.py` & `codat-platform-3.5.0/src/codatplatform/models/operations/get_create_update_model_options_by_data_type.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/operations/get_custom_data_type_configuration.py` & `codat-platform-3.5.0/src/codatplatform/models/operations/get_custom_data_type_configuration.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/operations/get_integration.py` & `codat-platform-3.5.0/src/codatplatform/models/operations/get_push_operation.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ...models.shared import integration as shared_integration
+from ...models.shared import pushoperation as shared_pushoperation
 from typing import Optional
 
 
 @dataclasses.dataclass
-class GetIntegrationRequest:
-    platform_key: str = dataclasses.field(metadata={'path_param': { 'field_name': 'platformKey', 'style': 'simple', 'explode': False }})
-    r"""A unique 4-letter key to represent a platform in each integration."""
+class GetPushOperationRequest:
+    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
+    r"""Unique identifier for a company."""
+    push_operation_key: str = dataclasses.field(metadata={'path_param': { 'field_name': 'pushOperationKey', 'style': 'simple', 'explode': False }})
+    r"""Push operation key."""
     
 
 
 
 @dataclasses.dataclass
-class GetIntegrationResponse:
+class GetPushOperationResponse:
     content_type: str = dataclasses.field()
     r"""HTTP response content type for this operation"""
     status_code: int = dataclasses.field()
     r"""HTTP response status code for this operation"""
     raw_response: requests_http.Response = dataclasses.field()
     r"""Raw HTTP response; suitable for custom response parsing"""
-    integration: Optional[shared_integration.Integration] = dataclasses.field(default=None)
+    push_operation: Optional[shared_pushoperation.PushOperation] = dataclasses.field(default=None)
     r"""OK"""
```

### Comparing `codat-platform-3.4.0/src/codatplatform/models/operations/get_integrations_branding.py` & `codat-platform-3.5.0/src/codatplatform/models/operations/get_integrations_branding.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/operations/get_profile.py` & `codat-platform-3.5.0/src/codatplatform/models/operations/get_profile.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/operations/get_profile_syncsettings.py` & `codat-platform-3.5.0/src/codatplatform/models/operations/get_profile_syncsettings.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/operations/get_pull_operation.py` & `codat-platform-3.5.0/src/codatplatform/models/operations/get_pull_operation.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/operations/get_push_operation.py` & `codat-platform-3.5.0/src/codatplatform/models/operations/refresh_data_type.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ...models.shared import pushoperation as shared_pushoperation
+from ...models.shared import pulloperation as shared_pulloperation
+from ...models.shared import schema_datatype as shared_schema_datatype
 from typing import Optional
 
 
 @dataclasses.dataclass
-class GetPushOperationRequest:
+class RefreshDataTypeRequest:
     company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
     r"""Unique identifier for a company."""
-    push_operation_key: str = dataclasses.field(metadata={'path_param': { 'field_name': 'pushOperationKey', 'style': 'simple', 'explode': False }})
-    r"""Push operation key."""
+    data_type: shared_schema_datatype.SchemaDataType = dataclasses.field(metadata={'path_param': { 'field_name': 'dataType', 'style': 'simple', 'explode': False }})
+    r"""The key of a Codat data type"""
+    connection_id: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'connectionId', 'style': 'form', 'explode': True }})
+    r"""Optionally, provide a data connection id to only queue pull operations on that connection."""
     
 
 
 
 @dataclasses.dataclass
-class GetPushOperationResponse:
+class RefreshDataTypeResponse:
     content_type: str = dataclasses.field()
     r"""HTTP response content type for this operation"""
     status_code: int = dataclasses.field()
     r"""HTTP response status code for this operation"""
     raw_response: requests_http.Response = dataclasses.field()
     r"""Raw HTTP response; suitable for custom response parsing"""
-    push_operation: Optional[shared_pushoperation.PushOperation] = dataclasses.field(default=None)
+    pull_operation: Optional[shared_pulloperation.PullOperation] = dataclasses.field(default=None)
     r"""OK"""
```

### Comparing `codat-platform-3.4.0/src/codatplatform/models/operations/get_supplemental_data_configuration.py` & `codat-platform-3.5.0/src/codatplatform/models/operations/get_supplemental_data_configuration.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/operations/get_webhook.py` & `codat-platform-3.5.0/src/codatplatform/models/operations/get_webhook.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/operations/list_api_keys.py` & `codat-platform-3.5.0/src/codatplatform/models/operations/list_api_keys.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/operations/list_companies.py` & `codat-platform-3.5.0/src/codatplatform/models/operations/list_companies.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/operations/list_connections.py` & `codat-platform-3.5.0/src/codatplatform/models/operations/list_connections.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/operations/list_custom_data_type_records.py` & `codat-platform-3.5.0/src/codatplatform/models/operations/list_custom_data_type_records.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/operations/list_groups.py` & `codat-platform-3.5.0/src/codatplatform/models/operations/list_groups.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/operations/list_integrations.py` & `codat-platform-3.5.0/src/codatplatform/models/operations/list_integrations.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/operations/list_pull_operations.py` & `codat-platform-3.5.0/src/codatplatform/models/operations/list_pull_operations.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/operations/list_rules.py` & `codat-platform-3.5.0/src/codatplatform/models/operations/list_rules.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/operations/list_webhook_consumers.py` & `codat-platform-3.5.0/src/codatplatform/models/operations/list_webhook_consumers.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/operations/refresh_company_data.py` & `codat-platform-3.5.0/src/codatplatform/models/operations/refresh_company_data.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/operations/refresh_custom_data_type.py` & `codat-platform-3.5.0/src/codatplatform/models/operations/refresh_custom_data_type.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/operations/refresh_data_type.py` & `codat-platform-3.5.0/src/codatplatform/models/operations/update_company.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ...models.shared import pulloperation as shared_pulloperation
-from ...models.shared import schema_datatype as shared_schema_datatype
+from ...models.shared import company as shared_company
+from ...models.shared import companyrequestbody as shared_companyrequestbody
 from typing import Optional
 
 
 @dataclasses.dataclass
-class RefreshDataTypeRequest:
+class UpdateCompanyRequest:
     company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
     r"""Unique identifier for a company."""
-    data_type: shared_schema_datatype.SchemaDataType = dataclasses.field(metadata={'path_param': { 'field_name': 'dataType', 'style': 'simple', 'explode': False }})
-    r"""The key of a Codat data type"""
-    connection_id: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'connectionId', 'style': 'form', 'explode': True }})
-    r"""Optionally, provide a data connection id to only queue pull operations on that connection."""
+    company_request_body: Optional[shared_companyrequestbody.CompanyRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
 
 
 @dataclasses.dataclass
-class RefreshDataTypeResponse:
+class UpdateCompanyResponse:
     content_type: str = dataclasses.field()
     r"""HTTP response content type for this operation"""
     status_code: int = dataclasses.field()
     r"""HTTP response status code for this operation"""
     raw_response: requests_http.Response = dataclasses.field()
     r"""Raw HTTP response; suitable for custom response parsing"""
-    pull_operation: Optional[shared_pulloperation.PullOperation] = dataclasses.field(default=None)
+    company: Optional[shared_company.Company] = dataclasses.field(default=None)
     r"""OK"""
```

### Comparing `codat-platform-3.4.0/src/codatplatform/models/operations/remove_company_from_group.py` & `codat-platform-3.5.0/src/codatplatform/models/operations/remove_company_from_group.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/operations/unlink_connection.py` & `codat-platform-3.5.0/src/codatplatform/models/operations/unlink_connection.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/operations/update_company.py` & `codat-platform-3.5.0/src/codatplatform/models/operations/get_connection_management_access_token.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ...models.shared import company as shared_company
-from ...models.shared import companyrequestbody as shared_companyrequestbody
+from ...models.shared import connectionmanagementaccesstoken as shared_connectionmanagementaccesstoken
 from typing import Optional
 
 
 @dataclasses.dataclass
-class UpdateCompanyRequest:
+class GetConnectionManagementAccessTokenRequest:
     company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
     r"""Unique identifier for a company."""
-    company_request_body: Optional[shared_companyrequestbody.CompanyRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
 
 
 @dataclasses.dataclass
-class UpdateCompanyResponse:
+class GetConnectionManagementAccessTokenResponse:
     content_type: str = dataclasses.field()
     r"""HTTP response content type for this operation"""
     status_code: int = dataclasses.field()
     r"""HTTP response status code for this operation"""
     raw_response: requests_http.Response = dataclasses.field()
     r"""Raw HTTP response; suitable for custom response parsing"""
-    company: Optional[shared_company.Company] = dataclasses.field(default=None)
-    r"""OK"""
+    connection_management_access_token: Optional[shared_connectionmanagementaccesstoken.ConnectionManagementAccessToken] = dataclasses.field(default=None)
+    r"""Success"""
```

### Comparing `codat-platform-3.4.0/src/codatplatform/models/operations/update_connection_authorization.py` & `codat-platform-3.5.0/src/codatplatform/models/operations/update_connection_authorization.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/operations/update_profile.py` & `codat-platform-3.5.0/src/codatplatform/models/operations/update_profile.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/operations/update_profile_syncsettings.py` & `codat-platform-3.5.0/src/codatplatform/models/operations/update_profile_syncsettings.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/__init__.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,28 +11,31 @@
 from .clientratelimitresetwebhook import *
 from .clientratelimitresetwebhookdata import *
 from .companies import *
 from .company import *
 from .companygroupassignment import *
 from .companyrequestbody import *
 from .connection import *
+from .connectionmanagementaccesstoken import *
+from .connectionmanagementallowedorigins import *
 from .connections import *
 from .connectionstatuschangedwebhook import *
 from .connectionstatuschangedwebhookdata import *
 from .createapikey import *
 from .createrule import *
 from .customdatatypeconfiguration import *
 from .customdatatyperecord import *
 from .customdatatyperecords import *
 from .dataconnectionerror import *
 from .dataconnectionstatus import *
 from .datasetdatachangedwebhook import *
 from .datasetstatuschangederrorwebhook import *
 from .datasetstatuschangederrorwebhookdata import *
 from .datastatus import *
+from .datastatuses import *
 from .datasynccompletedwebhook import *
 from .datasynccompletedwebhookdata import *
 from .datatype import *
 from .datatypefeature import *
 from .errorvalidation import *
 from .errorvalidationitem import *
 from .featurestate import *
@@ -66,22 +69,23 @@
 from .pushoptionchoice import *
 from .pushoptionproperty import *
 from .pushoptiontype import *
 from .pushvalidationinfo import *
 from .schema_datatype import *
 from .security import *
 from .sourcetype import *
+from .status import *
 from .supplementaldataconfiguration import *
 from .supportedfeature import *
 from .syncsetting import *
 from .syncsettings import *
 from .updateconnectionstatus import *
 from .validation import *
 from .validationitem import *
 from .webhook import *
 from .webhookconsumer import *
 from .webhookconsumerprototype import *
 from .webhookconsumers import *
 from .webhooknotifier import *
 from .webhooks import *
 
-__all__ = ["APIKeyDetails","APIKeys","Branding","BrandingButton","BrandingImage","BrandingLogo","ClientRateLimitReachedWebhook","ClientRateLimitReachedWebhookData","ClientRateLimitResetWebhook","ClientRateLimitResetWebhookData","Companies","Company","CompanyGroupAssignment","CompanyRequestBody","Connection","ConnectionStatusChangedWebhook","ConnectionStatusChangedWebhookData","Connections","Content","CreateAPIKey","CreateRule","CustomDataTypeConfiguration","CustomDataTypeRecord","CustomDataTypeRecords","DataConnectionError","DataConnectionStatus","DataStatus","DataSyncCompletedWebhook","DataSyncCompletedWebhookData","DataType","DataTypeFeature","DataTypes","DatasetDataChangedWebhook","DatasetDataChangedWebhookData","DatasetStatusChangedErrorWebhook","DatasetStatusChangedErrorWebhookData","ErrorValidation","ErrorValidationItem","FeatureState","FeatureType","Group","GroupPrototype","GroupRef","Groups","HalRef","ImageReference","Integration","Integrations","Links","ModifiedDate","NewCompanySynchronizedWebhook","NewCompanySynchronizedWebhookData","Profile","PullOperation","PullOperations","PushChangeType","PushFieldValidation","PushOperation","PushOperationChange","PushOperationRef","PushOperationStatus","PushOperationStatusChangedWebhook","PushOperationStatusChangedWebhookData","PushOperationTimedOutWebhook","PushOperationTimedOutWebhookData","PushOperations","PushOption","PushOptionChoice","PushOptionProperty","PushOptionType","PushValidationInfo","SchemaDataType","Security","SourceType","Status","SupplementalDataConfiguration","SupplementalDataSourceConfiguration","SupportedFeature","SyncSetting","SyncSettings","UpdateConnectionStatus","Validation","ValidationItem","Webhook","WebhookConsumer","WebhookConsumerPrototype","WebhookConsumers","WebhookNotifier","Webhooks"]
+__all__ = ["APIKeyDetails","APIKeys","Branding","BrandingButton","BrandingImage","BrandingLogo","ClientRateLimitReachedWebhook","ClientRateLimitReachedWebhookData","ClientRateLimitResetWebhook","ClientRateLimitResetWebhookData","Companies","Company","CompanyGroupAssignment","CompanyRequestBody","Connection","ConnectionManagementAccessToken","ConnectionManagementAllowedOrigins","ConnectionStatusChangedWebhook","ConnectionStatusChangedWebhookData","Connections","Content","CreateAPIKey","CreateRule","CustomDataTypeConfiguration","CustomDataTypeRecord","CustomDataTypeRecords","DataConnectionError","DataConnectionStatus","DataStatus","DataStatuses","DataSyncCompletedWebhook","DataSyncCompletedWebhookData","DataType","DataTypeFeature","DataTypes","DatasetDataChangedWebhook","DatasetDataChangedWebhookData","DatasetStatus","DatasetStatusChangedErrorWebhook","DatasetStatusChangedErrorWebhookData","ErrorValidation","ErrorValidationItem","FeatureState","FeatureType","Group","GroupPrototype","GroupRef","Groups","HalRef","ImageReference","Integration","Integrations","Links","ModifiedDate","NewCompanySynchronizedWebhook","NewCompanySynchronizedWebhookData","Profile","PullOperation","PullOperations","PushChangeType","PushFieldValidation","PushOperation","PushOperationChange","PushOperationRef","PushOperationStatus","PushOperationStatusChangedWebhook","PushOperationStatusChangedWebhookData","PushOperationTimedOutWebhook","PushOperationTimedOutWebhookData","PushOperations","PushOption","PushOptionChoice","PushOptionProperty","PushOptionType","PushValidationInfo","SchemaDataType","Security","SourceType","Status","SupplementalDataConfiguration","SupplementalDataSourceConfiguration","SupportedFeature","SyncSetting","SyncSettings","UpdateConnectionStatus","Validation","ValidationItem","Webhook","WebhookConsumer","WebhookConsumerPrototype","WebhookConsumers","WebhookNotifier","Webhooks"]
```

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/apikeydetails.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/apikeydetails.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/apikeys.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/apikeys.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/branding.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/branding.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/brandingbutton.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/brandingbutton.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/brandingimage.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/brandingimage.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/brandinglogo.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/brandinglogo.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/clientratelimitreachedwebhook.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/clientratelimitreachedwebhook.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,12 +18,15 @@
     r"""Unique identifier for your client in Codat."""
     client_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ClientName'), 'exclude': lambda f: f is None }})
     r"""Name of your client in Codat."""
     data: Optional[ClientRateLimitReachedWebhookData] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Data'), 'exclude': lambda f: f is None }})
     message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Message'), 'exclude': lambda f: f is None }})
     r"""A human-readable message about the webhook."""
     rule_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('RuleId'), 'exclude': lambda f: f is None }})
-    r"""Unique identifier for the rule."""
+    r"""Unique identifier for the rule.
+
+    Deprecated field: This will be removed in a future release, please migrate away from it as soon as possible.
+    """
     rule_type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('RuleType'), 'exclude': lambda f: f is None }})
     r"""The type of rule."""
```

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/clientratelimitreachedwebhookdata.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/clientratelimitreachedwebhookdata.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/clientratelimitresetwebhook.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/datasetstatuschangederrorwebhook.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from .clientratelimitresetwebhookdata import ClientRateLimitResetWebhookData
+from .datasetstatuschangederrorwebhookdata import DatasetStatusChangedErrorWebhookData
 from codatplatform import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class ClientRateLimitResetWebhook:
-    r"""Webhook request body for a client that has had their rate limit reset."""
+class DatasetStatusChangedErrorWebhook:
+    r"""Webhook request body to notify that a data synchronization has completed."""
     alert_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('AlertId'), 'exclude': lambda f: f is None }})
     r"""Unique identifier of the webhook event."""
     client_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ClientId'), 'exclude': lambda f: f is None }})
     r"""Unique identifier for your client in Codat."""
     client_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ClientName'), 'exclude': lambda f: f is None }})
     r"""Name of your client in Codat."""
-    data: Optional[ClientRateLimitResetWebhookData] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Data'), 'exclude': lambda f: f is None }})
+    company_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('CompanyId'), 'exclude': lambda f: f is None }})
+    r"""Unique identifier for your SMB in Codat."""
+    data: Optional[DatasetStatusChangedErrorWebhookData] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Data'), 'exclude': lambda f: f is None }})
+    data_connection_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('DataConnectionId'), 'exclude': lambda f: f is None }})
+    r"""Unique identifier for a company's data connection."""
     message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Message'), 'exclude': lambda f: f is None }})
     r"""A human-readable message about the webhook."""
     rule_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('RuleId'), 'exclude': lambda f: f is None }})
-    r"""Unique identifier for the rule."""
+    r"""Unique identifier for the rule.
+
+    Deprecated field: This will be removed in a future release, please migrate away from it as soon as possible.
+    """
     rule_type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('RuleType'), 'exclude': lambda f: f is None }})
     r"""The type of rule."""
```

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/clientratelimitresetwebhookdata.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/clientratelimitresetwebhookdata.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/companies.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/companies.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/company.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/company.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/companygroupassignment.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/companygroupassignment.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/companyrequestbody.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/companyrequestbody.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/connection.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/connection.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/connections.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/connections.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/connectionstatuschangedwebhook.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/connectionstatuschangedwebhook.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,12 +22,15 @@
     r"""Unique identifier for your SMB in Codat."""
     data: Optional[ConnectionStatusChangedWebhookData] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Data'), 'exclude': lambda f: f is None }})
     data_connection_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('DataConnectionId'), 'exclude': lambda f: f is None }})
     r"""Unique identifier for a company's data connection."""
     message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Message'), 'exclude': lambda f: f is None }})
     r"""A human-readable message about the webhook."""
     rule_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('RuleId'), 'exclude': lambda f: f is None }})
-    r"""Unique identifier for the rule."""
+    r"""Unique identifier for the rule.
+
+    Deprecated field: This will be removed in a future release, please migrate away from it as soon as possible.
+    """
     rule_type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('RuleType'), 'exclude': lambda f: f is None }})
     r"""The type of rule."""
```

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/connectionstatuschangedwebhookdata.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/connectionstatuschangedwebhookdata.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/createapikey.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/createapikey.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/createrule.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/createrule.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/customdatatypeconfiguration.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/customdatatypeconfiguration.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/customdatatyperecord.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/customdatatyperecord.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/customdatatyperecords.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/customdatatyperecords.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/dataconnectionerror.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/dataconnectionerror.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/datasetdatachangedwebhook.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/pushoperationtimedoutwebhook.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,36 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from .datatype import DataType
+from .pushoperationtimedoutwebhookdata import PushOperationTimedOutWebhookData
 from codatplatform import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class DatasetDataChangedWebhookData:
-    data_type: Optional[DataType] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataType'), 'exclude': lambda f: f is None }})
-    r"""Available data types"""
-    dataset_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('datasetId'), 'exclude': lambda f: f is None }})
-    r"""Unique identifier for the dataset that completed its sync."""
-    
-
-
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class DatasetDataChangedWebhook:
-    r"""Webhook request body to notify that a data synchronization has completed."""
+class PushOperationTimedOutWebhook:
+    r"""Webhook request body notifying that a push push operation has timed out."""
     alert_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('AlertId'), 'exclude': lambda f: f is None }})
     r"""Unique identifier of the webhook event."""
     client_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ClientId'), 'exclude': lambda f: f is None }})
     r"""Unique identifier for your client in Codat."""
     client_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ClientName'), 'exclude': lambda f: f is None }})
     r"""Name of your client in Codat."""
     company_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('CompanyId'), 'exclude': lambda f: f is None }})
     r"""Unique identifier for your SMB in Codat."""
-    data: Optional[DatasetDataChangedWebhookData] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Data'), 'exclude': lambda f: f is None }})
+    data: Optional[PushOperationTimedOutWebhookData] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Data'), 'exclude': lambda f: f is None }})
     data_connection_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('DataConnectionId'), 'exclude': lambda f: f is None }})
     r"""Unique identifier for a company's data connection."""
     message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Message'), 'exclude': lambda f: f is None }})
     r"""A human-readable message about the webhook."""
     rule_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('RuleId'), 'exclude': lambda f: f is None }})
-    r"""Unique identifier for the rule."""
+    r"""Unique identifier for the rule.
+
+    Deprecated field: This will be removed in a future release, please migrate away from it as soon as possible.
+    """
     rule_type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('RuleType'), 'exclude': lambda f: f is None }})
     r"""The type of rule."""
```

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/datasetstatuschangederrorwebhook.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/datasetdatachangedwebhook.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,47 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from .datasetstatuschangederrorwebhookdata import DatasetStatusChangedErrorWebhookData
+from .datatype import DataType
 from codatplatform import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class DatasetStatusChangedErrorWebhook:
+class DatasetDataChangedWebhookData:
+    data_type: Optional[DataType] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataType'), 'exclude': lambda f: f is None }})
+    r"""Available data types"""
+    dataset_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('datasetId'), 'exclude': lambda f: f is None }})
+    r"""Unique identifier for the dataset that completed its sync."""
+    
+
+
+
+@dataclass_json(undefined=Undefined.EXCLUDE)
+@dataclasses.dataclass
+class DatasetDataChangedWebhook:
     r"""Webhook request body to notify that a data synchronization has completed."""
     alert_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('AlertId'), 'exclude': lambda f: f is None }})
     r"""Unique identifier of the webhook event."""
     client_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ClientId'), 'exclude': lambda f: f is None }})
     r"""Unique identifier for your client in Codat."""
     client_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ClientName'), 'exclude': lambda f: f is None }})
     r"""Name of your client in Codat."""
     company_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('CompanyId'), 'exclude': lambda f: f is None }})
     r"""Unique identifier for your SMB in Codat."""
-    data: Optional[DatasetStatusChangedErrorWebhookData] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Data'), 'exclude': lambda f: f is None }})
+    data: Optional[DatasetDataChangedWebhookData] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Data'), 'exclude': lambda f: f is None }})
     data_connection_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('DataConnectionId'), 'exclude': lambda f: f is None }})
     r"""Unique identifier for a company's data connection."""
     message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Message'), 'exclude': lambda f: f is None }})
     r"""A human-readable message about the webhook."""
     rule_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('RuleId'), 'exclude': lambda f: f is None }})
-    r"""Unique identifier for the rule."""
+    r"""Unique identifier for the rule.
+
+    Deprecated field: This will be removed in a future release, please migrate away from it as soon as possible.
+    """
     rule_type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('RuleType'), 'exclude': lambda f: f is None }})
     r"""The type of rule."""
```

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/datasetstatuschangederrorwebhookdata.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/datasetstatuschangederrorwebhookdata.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/datastatus.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/datastatus.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+from .status import Status
 from codatplatform import utils
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from typing import Optional
 
 class DataTypes(str, Enum):
     r"""Available data types"""
@@ -54,16 +55,16 @@
     COMMERCE_TRANSACTIONS = 'commerce-transactions'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DataStatus:
     r"""Describes the state of data in the Codat cache for a company and data type"""
-    current_status: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('currentStatus') }})
-    r"""The current status of the dataset in Codat's cache."""
+    current_status: Status = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('currentStatus') }})
+    r"""The current status of the dataset."""
     data_type: DataTypes = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataType') }})
     r"""Available data types"""
     last_successful_sync: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastSuccessfulSync') }})
     r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
 
     ```
     2020-10-08T22:40:50Z
```

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/datasynccompletedwebhook.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/datasynccompletedwebhook.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,12 +22,15 @@
     r"""Unique identifier for your SMB in Codat."""
     data: Optional[DataSyncCompletedWebhookData] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Data'), 'exclude': lambda f: f is None }})
     data_connection_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('DataConnectionId'), 'exclude': lambda f: f is None }})
     r"""Unique identifier for a company's data connection."""
     message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Message'), 'exclude': lambda f: f is None }})
     r"""A human-readable message about the webhook."""
     rule_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('RuleId'), 'exclude': lambda f: f is None }})
-    r"""Unique identifier for the rule."""
+    r"""Unique identifier for the rule.
+
+    Deprecated field: This will be removed in a future release, please migrate away from it as soon as possible.
+    """
     rule_type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('RuleType'), 'exclude': lambda f: f is None }})
     r"""The type of rule."""
```

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/datasynccompletedwebhookdata.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/datasynccompletedwebhookdata.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/datatype.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/datatype.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/datatypefeature.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/datatypefeature.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/errorvalidation.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/errorvalidation.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/errorvalidationitem.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/errorvalidationitem.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/group.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/group.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/groupprototype.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/groupprototype.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/groupref.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/groupref.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/groups.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/groups.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/halref.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/halref.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/imagereference.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/imagereference.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/integration.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/integration.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/integrations.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/integrations.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/links.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/links.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/newcompanysynchronizedwebhook.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/pushoperationstatuschangedwebhook.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from .newcompanysynchronizedwebhookdata import NewCompanySynchronizedWebhookData
+from .pushoperationstatuschangedwebhookdata import PushOperationStatusChangedWebhookData
 from codatplatform import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class NewCompanySynchronizedWebhook:
-    r"""Webhook request body to notify that a new company has successfully synchronized at least one dataType for the first time."""
+class PushOperationStatusChangedWebhook:
+    r"""Webhook request body for a push operation status change."""
     alert_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('AlertId'), 'exclude': lambda f: f is None }})
     r"""Unique identifier of the webhook event."""
     client_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ClientId'), 'exclude': lambda f: f is None }})
     r"""Unique identifier for your client in Codat."""
     client_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ClientName'), 'exclude': lambda f: f is None }})
     r"""Name of your client in Codat."""
     company_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('CompanyId'), 'exclude': lambda f: f is None }})
     r"""Unique identifier for your SMB in Codat."""
-    data: Optional[NewCompanySynchronizedWebhookData] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Data'), 'exclude': lambda f: f is None }})
+    data: Optional[PushOperationStatusChangedWebhookData] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Data'), 'exclude': lambda f: f is None }})
     data_connection_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('DataConnectionId'), 'exclude': lambda f: f is None }})
     r"""Unique identifier for a company's data connection."""
     message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Message'), 'exclude': lambda f: f is None }})
     r"""A human-readable message about the webhook."""
     rule_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('RuleId'), 'exclude': lambda f: f is None }})
-    r"""Unique identifier for the rule."""
+    r"""Unique identifier for the rule.
+
+    Deprecated field: This will be removed in a future release, please migrate away from it as soon as possible.
+    """
     rule_type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('RuleType'), 'exclude': lambda f: f is None }})
     r"""The type of rule."""
```

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/profile.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/profile.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/pulloperation.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/pulloperation.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from __future__ import annotations
 import dataclasses
 from codatplatform import utils
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from typing import Optional
 
-class Status(str, Enum):
-    r"""The current status of the pull operation."""
+class DatasetStatus(str, Enum):
+    r"""The current status of the dataset."""
     INITIAL = 'Initial'
     QUEUED = 'Queued'
     FETCHING = 'Fetching'
     MAP_QUEUED = 'MapQueued'
     MAPPING = 'Mapping'
     COMPLETE = 'Complete'
     FETCH_ERROR = 'FetchError'
@@ -22,16 +22,14 @@
     PROCESSING = 'Processing'
     PROCESSING_ERROR = 'ProcessingError'
     VALIDATION_QUEUED = 'ValidationQueued'
     VALIDATING = 'Validating'
     VALIDATION_ERROR = 'ValidationError'
     AUTH_ERROR = 'AuthError'
     CANCELLED = 'Cancelled'
-    ROUTING = 'Routing'
-    ROUTING_ERROR = 'RoutingError'
     NOT_SUPPORTED = 'NotSupported'
     RATE_LIMIT_ERROR = 'RateLimitError'
     PERMISSIONS_ERROR = 'PermissionsError'
     PREREQUISITE_NOT_MET = 'PrerequisiteNotMet'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
@@ -72,16 +70,16 @@
     - UTC time offsets: `2021-11-15T01:00:00-05:00`
 
     > Time zones
     > 
     > Not all dates from Codat will contain information about time zones.  
     > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
     """
-    status: Status = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status') }})
-    r"""The current status of the pull operation."""
+    status: DatasetStatus = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status') }})
+    r"""The current status of the dataset."""
     completed: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('completed'), 'exclude': lambda f: f is None }})
     r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
 
     ```
     2020-10-08T22:40:50Z
     2021-01-01T00:00:00
     ```
```

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/pulloperations.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/pulloperations.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/pushfieldvalidation.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/pushfieldvalidation.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/pushoperation.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/pushoperation.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/pushoperationchange.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/pushoperationchange.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/pushoperationref.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/pushoperationref.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/pushoperations.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/pushoperations.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/pushoperationstatuschangedwebhook.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/newcompanysynchronizedwebhook.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from .pushoperationstatuschangedwebhookdata import PushOperationStatusChangedWebhookData
+from .newcompanysynchronizedwebhookdata import NewCompanySynchronizedWebhookData
 from codatplatform import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PushOperationStatusChangedWebhook:
-    r"""Webhook request body for a push operation status change."""
+class NewCompanySynchronizedWebhook:
+    r"""Webhook request body to notify that a new company has successfully synchronized at least one dataType for the first time."""
     alert_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('AlertId'), 'exclude': lambda f: f is None }})
     r"""Unique identifier of the webhook event."""
     client_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ClientId'), 'exclude': lambda f: f is None }})
     r"""Unique identifier for your client in Codat."""
     client_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ClientName'), 'exclude': lambda f: f is None }})
     r"""Name of your client in Codat."""
     company_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('CompanyId'), 'exclude': lambda f: f is None }})
     r"""Unique identifier for your SMB in Codat."""
-    data: Optional[PushOperationStatusChangedWebhookData] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Data'), 'exclude': lambda f: f is None }})
+    data: Optional[NewCompanySynchronizedWebhookData] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Data'), 'exclude': lambda f: f is None }})
     data_connection_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('DataConnectionId'), 'exclude': lambda f: f is None }})
     r"""Unique identifier for a company's data connection."""
     message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Message'), 'exclude': lambda f: f is None }})
     r"""A human-readable message about the webhook."""
     rule_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('RuleId'), 'exclude': lambda f: f is None }})
-    r"""Unique identifier for the rule."""
+    r"""Unique identifier for the rule.
+
+    Deprecated field: This will be removed in a future release, please migrate away from it as soon as possible.
+    """
     rule_type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('RuleType'), 'exclude': lambda f: f is None }})
     r"""The type of rule."""
```

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/pushoperationstatuschangedwebhookdata.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/pushoperationstatuschangedwebhookdata.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/pushoperationtimedoutwebhook.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/clientratelimitresetwebhook.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from .pushoperationtimedoutwebhookdata import PushOperationTimedOutWebhookData
+from .clientratelimitresetwebhookdata import ClientRateLimitResetWebhookData
 from codatplatform import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PushOperationTimedOutWebhook:
-    r"""Webhook request body notifying that a push push operation has timed out."""
+class ClientRateLimitResetWebhook:
+    r"""Webhook request body for a client that has had their rate limit reset."""
     alert_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('AlertId'), 'exclude': lambda f: f is None }})
     r"""Unique identifier of the webhook event."""
     client_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ClientId'), 'exclude': lambda f: f is None }})
     r"""Unique identifier for your client in Codat."""
     client_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ClientName'), 'exclude': lambda f: f is None }})
     r"""Name of your client in Codat."""
-    company_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('CompanyId'), 'exclude': lambda f: f is None }})
-    r"""Unique identifier for your SMB in Codat."""
-    data: Optional[PushOperationTimedOutWebhookData] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Data'), 'exclude': lambda f: f is None }})
-    data_connection_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('DataConnectionId'), 'exclude': lambda f: f is None }})
-    r"""Unique identifier for a company's data connection."""
+    data: Optional[ClientRateLimitResetWebhookData] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Data'), 'exclude': lambda f: f is None }})
     message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Message'), 'exclude': lambda f: f is None }})
     r"""A human-readable message about the webhook."""
     rule_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('RuleId'), 'exclude': lambda f: f is None }})
-    r"""Unique identifier for the rule."""
+    r"""Unique identifier for the rule.
+
+    Deprecated field: This will be removed in a future release, please migrate away from it as soon as possible.
+    """
     rule_type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('RuleType'), 'exclude': lambda f: f is None }})
     r"""The type of rule."""
```

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/pushoperationtimedoutwebhookdata.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/pushoperationtimedoutwebhookdata.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/pushoption.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/pushoption.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/pushoptionchoice.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/pushoptionchoice.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/pushoptionproperty.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/pushoptionproperty.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/pushvalidationinfo.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/pushvalidationinfo.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/schema_datatype.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/schema_datatype.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/supplementaldataconfiguration.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/supplementaldataconfiguration.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/supportedfeature.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/supportedfeature.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/syncsetting.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/syncsetting.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/syncsettings.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/syncsettings.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/updateconnectionstatus.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/updateconnectionstatus.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/validation.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/validation.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/validationitem.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/validationitem.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/webhook.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/webhook.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/webhookconsumer.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/webhookconsumerprototype.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,23 +5,19 @@
 from codatplatform import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import List, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class WebhookConsumer:
-    r"""A webhook consumer is an HTTP endpoint that developers can configure to subscribe to Codat's supported event types.
-
-    See our documentation for more details on [Codat's webhook service](https://docs.codat.io/using-the-api/webhooks/overview).
-    """
+class WebhookConsumerPrototype:
     UNSET='__SPEAKEASY_UNSET__'
-    disabled: Optional[bool] = dataclasses.field(default=False, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('disabled'), 'exclude': lambda f: f is WebhookConsumer.UNSET }})
+    company_id: Optional[str] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('companyId'), 'exclude': lambda f: f is WebhookConsumerPrototype.UNSET }})
+    r"""Unique identifier of the company to indicate company-specific events. The associated webhook consumer will receive events only for the specified ID."""
+    disabled: Optional[bool] = dataclasses.field(default=False, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('disabled'), 'exclude': lambda f: f is WebhookConsumerPrototype.UNSET }})
     r"""Flag that enables or disables the endpoint from receiving events. Disabled when set to `true`."""
     event_types: Optional[List[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eventTypes'), 'exclude': lambda f: f is None }})
     r"""An array of event types the webhook consumer subscribes to."""
-    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-    r"""Unique identifier for the webhook consumer."""
     url: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('url'), 'exclude': lambda f: f is None }})
     r"""The URL that will consume webhook events dispatched by Codat."""
```

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/webhookconsumerprototype.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/webhooknotifier.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,17 +5,13 @@
 from codatplatform import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import List, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class WebhookConsumerPrototype:
-    UNSET='__SPEAKEASY_UNSET__'
-    disabled: Optional[bool] = dataclasses.field(default=False, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('disabled'), 'exclude': lambda f: f is WebhookConsumerPrototype.UNSET }})
-    r"""Flag that enables or disables the endpoint from receiving events. Disabled when set to `true`."""
-    event_types: Optional[List[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eventTypes'), 'exclude': lambda f: f is None }})
-    r"""An array of event types the webhook consumer subscribes to."""
-    url: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('url'), 'exclude': lambda f: f is None }})
-    r"""The URL that will consume webhook events dispatched by Codat."""
+class WebhookNotifier:
+    emails: Optional[List[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('emails'), 'exclude': lambda f: f is None }})
+    webhook: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('webhook'), 'exclude': lambda f: f is None }})
+    r"""The URI the webhook service will use to post events."""
```

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/webhookconsumers.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/webhookconsumers.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/webhooknotifier.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/connectionmanagementaccesstoken.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from codatplatform import utils
 from dataclasses_json import Undefined, dataclass_json
-from typing import List, Optional
+from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class WebhookNotifier:
-    emails: Optional[List[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('emails'), 'exclude': lambda f: f is None }})
-    webhook: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('webhook'), 'exclude': lambda f: f is None }})
-    r"""The URI the webhook service will use to post events."""
+class ConnectionManagementAccessToken:
+    access_token: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken'), 'exclude': lambda f: f is None }})
+    r"""Access token that allows SMBs to manage connections that have access to their data."""
```

### Comparing `codat-platform-3.4.0/src/codatplatform/models/shared/webhooks.py` & `codat-platform-3.5.0/src/codatplatform/models/shared/webhooks.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/webhooks/__init__.py` & `codat-platform-3.5.0/src/codatplatform/models/webhooks/__init__.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/webhooks/client_rate_limit_reached.py` & `codat-platform-3.5.0/src/codatplatform/models/webhooks/client_rate_limit_reached.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/webhooks/client_rate_limit_reset.py` & `codat-platform-3.5.0/src/codatplatform/models/webhooks/client_rate_limit_reset.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/webhooks/company_data_connection_status_changed.py` & `codat-platform-3.5.0/src/codatplatform/models/webhooks/company_data_connection_status_changed.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/webhooks/data_sync_completed.py` & `codat-platform-3.5.0/src/codatplatform/models/webhooks/data_sync_completed.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/webhooks/dataset_data_changed.py` & `codat-platform-3.5.0/src/codatplatform/models/webhooks/dataset_data_changed.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/webhooks/dataset_status_has_changed_to_an_error_state.py` & `codat-platform-3.5.0/src/codatplatform/models/webhooks/dataset_status_has_changed_to_an_error_state.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/webhooks/new_company_synchronized.py` & `codat-platform-3.5.0/src/codatplatform/models/webhooks/new_company_synchronized.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/webhooks/push_operation_has_timed_out.py` & `codat-platform-3.5.0/src/codatplatform/models/webhooks/push_operation_has_timed_out.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/models/webhooks/push_operation_status_has_changed.py` & `codat-platform-3.5.0/src/codatplatform/models/webhooks/push_operation_status_has_changed.py`

 * *Files identical despite different names*

### Comparing `codat-platform-3.4.0/src/codatplatform/push_data.py` & `codat-platform-3.5.0/src/codatplatform/cors_settings.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,264 +1,190 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from codatplatform import utils
-from codatplatform._hooks import HookContext
+from codatplatform._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from codatplatform.models import errors, operations, shared
 from typing import Optional
 
-class PushData:
-    r"""View push options and get push statuses."""
+class CorsSettings:
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
-    def get_model_options(self, request: operations.GetCreateUpdateModelOptionsByDataTypeRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetCreateUpdateModelOptionsByDataTypeResponse:
-        r"""Get push options
-        This is the generic documentation for creation and updating of data. See the equivalent endpoint for a given data type for more specific information. 
+    def get(self, retries: Optional[utils.RetryConfig] = None) -> operations.GetConnectionManagementCorsSettingsResponse:
+        r"""Get CORS settings
+        The *Get CORS settings* endpoint returns the allowed origins (i.e. your domains) you want to allow cross-origin resource sharing ([CORS](https://en.wikipedia.org/wiki/Cross-origin_resource_sharing)) with Codat. 
 
-        Before pushing data into accounting software, it is often necessary to collect some details from the user as to how they would like the data to be inserted. This includes names and amounts on transactional entities, but also factors such as categorisation of entities, which is often handled differently between different accounting packages. A good example of this is specifying where on the balance sheet/profit and loss reports the user would like a newly-created nominal account to appear.
+        Enabling CORS with Codat is required by our embedded [connection management UI](https://docs.codat.io/auth-flow/optimize/connection-management) to access Codat's API endpoints.
 
-        Codat tries not to limit users to pushing to a very limited number of standard categories, so we have implemented \"options\" endpoints, which allow us to expose to our clients the fields which are required to be pushed for a specific linked company, and the options which may be selected for each field.
-
-
-        > **Supported Integrations**
-        > 
-        > Check out our [coverage explorer](https://knowledge.codat.io/) for integrations that support push (POST/PUT methods).
+        The embedded [connection management UI](https://docs.codat.io/auth-flow/optimize/connection-management) lets your customers control access to their data by allowing them to manage their existing connections.
         """
-        hook_ctx = HookContext(operation_id='get-create-update-model-options-by-data-type', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        hook_ctx = HookContext(operation_id='get-connection-management-cors-settings', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetCreateUpdateModelOptionsByDataTypeRequest, base_url, '/companies/{companyId}/connections/{connectionId}/options/{dataType}', request)
-        headers = {}
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = self.sdk_configuration.user_agent
+        url = base_url + '/connectionManagement/corsSettings'
         
         if callable(self.sdk_configuration.security):
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security())
+            headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security)
+            headers, query_params = utils.get_security(self.sdk_configuration.security)
         
+        headers['Accept'] = 'application/json'
+        headers['user-agent'] = self.sdk_configuration.user_agent
+        client = self.sdk_configuration.client
         
         global_retry_config = self.sdk_configuration.retry_config
         retry_config = retries
         if retry_config is None:
             if global_retry_config:
                 retry_config = global_retry_config
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
+        req = None
         def do_request():
+            nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('GET', url, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
             if utils.match_status_codes(['401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
-        content_type = http_res.headers.get('Content-Type')
         
-        res = operations.GetCreateUpdateModelOptionsByDataTypeResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetConnectionManagementCorsSettingsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[shared.PushOption])
-                res.push_option = out
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[shared.ConnectionManagementAllowedOrigins])
+                res.connection_management_allowed_origins = out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [401, 402, 403, 404, 429, 500, 503]:
-            if utils.match_content_type(content_type, 'application/json'):
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
-                out.raw_response = http_res
                 raise out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+        else:
+            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def get_operation(self, request: operations.GetPushOperationRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetPushOperationResponse:
-        r"""Get push operation
-        Retrieve push operation.
+    def set(self, request: Optional[shared.ConnectionManagementAllowedOrigins], retries: Optional[utils.RetryConfig] = None) -> operations.SetConnectionManagementCorsSettingsResponse:
+        r"""Set CORS settings
+        The *Set CORS settings* endpoint allows you to register allowed origins (i.e. your domains) for use in cross-origin resource sharing ([CORS](https://en.wikipedia.org/wiki/Cross-origin_resource_sharing)).
+
+        Enabling CORS with Codat is required by our embedded [connection management UI](https://docs.codat.io/auth-flow/optimize/connection-management) to access Codat's API endpoints. 
+
+        The embedded [connection management UI](https://docs.codat.io/auth-flow/optimize/connection-management) lets your customers control access to their data by allowing them to manage their existing connections.
         """
-        hook_ctx = HookContext(operation_id='get-push-operation', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        hook_ctx = HookContext(operation_id='set-connection-management-cors-settings', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetPushOperationRequest, base_url, '/companies/{companyId}/push/{pushOperationKey}', request)
-        headers = {}
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = self.sdk_configuration.user_agent
+        url = base_url + '/connectionManagement/corsSettings'
         
         if callable(self.sdk_configuration.security):
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security())
+            headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security)
+            headers, query_params = utils.get_security(self.sdk_configuration.security)
         
+        req_content_type, data, form = utils.serialize_request_body(request, Optional[shared.ConnectionManagementAllowedOrigins], "request", False, True, 'json')
+        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
+        headers['Accept'] = 'application/json'
+        headers['user-agent'] = self.sdk_configuration.user_agent
+        client = self.sdk_configuration.client
         
         global_retry_config = self.sdk_configuration.retry_config
         retry_config = retries
         if retry_config is None:
             if global_retry_config:
                 retry_config = global_retry_config
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
+        req = None
         def do_request():
+            nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('GET', url, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
             if utils.match_status_codes(['401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
-        content_type = http_res.headers.get('Content-Type')
         
-        res = operations.GetPushOperationResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.SetConnectionManagementCorsSettingsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[shared.PushOperation])
-                res.push_operation = out
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[shared.ConnectionManagementAllowedOrigins])
+                res.connection_management_allowed_origins = out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [401, 402, 403, 404, 429, 500, 503]:
-            if utils.match_content_type(content_type, 'application/json'):
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
-                out.raw_response = http_res
                 raise out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+        else:
+            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
-    
-    def list_operations(self, request: operations.GetCompanyPushHistoryRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetCompanyPushHistoryResponse:
-        r"""List push operations
-        List push operation records.
-        """
-        hook_ctx = HookContext(operation_id='get-company-push-history', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
-        
-        url = utils.generate_url(operations.GetCompanyPushHistoryRequest, base_url, '/companies/{companyId}/push', request)
-        headers = {}
-        query_params = utils.get_query_params(operations.GetCompanyPushHistoryRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = self.sdk_configuration.user_agent
-        
-        if callable(self.sdk_configuration.security):
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security())
-        else:
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security)
-        
-        
-        global_retry_config = self.sdk_configuration.retry_config
-        retry_config = retries
-        if retry_config is None:
-            if global_retry_config:
-                retry_config = global_retry_config
-            else:
-                retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
-
-        def do_request():
-            try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-                )
-                http_res = client.send(req)
-            except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
-
-            if utils.match_status_codes(['400','401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
-                    raise e
-            else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
-
-            return http_res
-
-        http_res = utils.retry(do_request, utils.Retries(retry_config, [
-            '408',
-            '429',
-            '5XX'
-        ]))
-        
-        content_type = http_res.headers.get('Content-Type')
-        
-        res = operations.GetCompanyPushHistoryResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
-        
-        if http_res.status_code == 200:
-            if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[shared.PushOperations])
-                res.push_operations = out
-            else:
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code in [400, 401, 402, 403, 404, 429, 500, 503]:
-            if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
-                out.raw_response = http_res
-                raise out
-            else:
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
-            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
-
-        return res
 
-
```

### Comparing `codat-platform-3.4.0/src/codatplatform/refresh_data.py` & `codat-platform-3.5.0/src/codatplatform/refresh_data.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from codatplatform import utils
-from codatplatform._hooks import HookContext
+from codatplatform._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from codatplatform.models import errors, operations, shared
-from typing import Dict, Optional
+from typing import Optional
 
 class RefreshData:
-    r"""Asynchronously retrieve data from an integration to refresh data in Codat."""
+    r"""Initiate data refreshes, view pull status and history."""
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
@@ -23,394 +23,404 @@
         This is an asynchronous operation, and will bring updated data into Codat from the linked integration for you to view.
 
         [Read more](https://docs.codat.io/core-concepts/data-type-settings) about data type settings and `fetch on first link`.
         """
         hook_ctx = HookContext(operation_id='refresh-company-data', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RefreshCompanyDataRequest, base_url, '/companies/{companyId}/data/all', request)
-        headers = {}
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = self.sdk_configuration.user_agent
+        url = utils.generate_url(base_url, '/companies/{companyId}/data/all', request)
         
         if callable(self.sdk_configuration.security):
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security())
+            headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security)
+            headers, query_params = utils.get_security(self.sdk_configuration.security)
         
+        headers['Accept'] = 'application/json'
+        headers['user-agent'] = self.sdk_configuration.user_agent
+        client = self.sdk_configuration.client
         
         global_retry_config = self.sdk_configuration.retry_config
         retry_config = retries
         if retry_config is None:
             if global_retry_config:
                 retry_config = global_retry_config
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
+        req = None
         def do_request():
+            nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('POST', url, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('POST', url, params=query_params, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
             if utils.match_status_codes(['401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
-        content_type = http_res.headers.get('Content-Type')
         
-        res = operations.RefreshCompanyDataResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.RefreshCompanyDataResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 204:
             pass
         elif http_res.status_code in [401, 402, 403, 404, 429, 500, 503]:
-            if utils.match_content_type(content_type, 'application/json'):
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
-                out.raw_response = http_res
                 raise out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+        else:
+            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
     def by_data_type(self, request: operations.RefreshDataTypeRequest, retries: Optional[utils.RetryConfig] = None) -> operations.RefreshDataTypeResponse:
         r"""Refresh data type
         Refreshes a given data type for a given company.
 
         This is an asynchronous operation, and will bring updated data into Codat from the linked integration for you to view.
         """
         hook_ctx = HookContext(operation_id='refresh-data-type', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RefreshDataTypeRequest, base_url, '/companies/{companyId}/data/queue/{dataType}', request)
-        headers = {}
-        query_params = utils.get_query_params(operations.RefreshDataTypeRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = self.sdk_configuration.user_agent
+        url = utils.generate_url(base_url, '/companies/{companyId}/data/queue/{dataType}', request)
         
         if callable(self.sdk_configuration.security):
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security())
+            headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security)
+            headers, query_params = utils.get_security(self.sdk_configuration.security)
         
+        query_params = { **utils.get_query_params(request), **query_params }
+        headers['Accept'] = 'application/json'
+        headers['user-agent'] = self.sdk_configuration.user_agent
+        client = self.sdk_configuration.client
         
         global_retry_config = self.sdk_configuration.retry_config
         retry_config = retries
         if retry_config is None:
             if global_retry_config:
                 retry_config = global_retry_config
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
+        req = None
         def do_request():
+            nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('POST', url, params=query_params, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('POST', url, params=query_params, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
             if utils.match_status_codes(['401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
-        content_type = http_res.headers.get('Content-Type')
         
-        res = operations.RefreshDataTypeResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.RefreshDataTypeResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(content_type, 'application/json'):
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.PullOperation])
                 res.pull_operation = out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [401, 402, 403, 404, 429, 500, 503]:
-            if utils.match_content_type(content_type, 'application/json'):
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
-                out.raw_response = http_res
                 raise out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+        else:
+            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
     def get(self, request: operations.GetCompanyDataStatusRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetCompanyDataStatusResponse:
         r"""Get data status
         Get the state of each data type for a company
         """
         hook_ctx = HookContext(operation_id='get-company-data-status', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetCompanyDataStatusRequest, base_url, '/companies/{companyId}/dataStatus', request)
-        headers = {}
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = self.sdk_configuration.user_agent
+        url = utils.generate_url(base_url, '/companies/{companyId}/dataStatus', request)
         
         if callable(self.sdk_configuration.security):
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security())
+            headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security)
+            headers, query_params = utils.get_security(self.sdk_configuration.security)
         
+        headers['Accept'] = 'application/json'
+        headers['user-agent'] = self.sdk_configuration.user_agent
+        client = self.sdk_configuration.client
         
         global_retry_config = self.sdk_configuration.retry_config
         retry_config = retries
         if retry_config is None:
             if global_retry_config:
                 retry_config = global_retry_config
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
+        req = None
         def do_request():
+            nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('GET', url, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
             if utils.match_status_codes(['401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
-        content_type = http_res.headers.get('Content-Type')
         
-        res = operations.GetCompanyDataStatusResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetCompanyDataStatusResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[Dict[str, shared.DataStatus]])
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[shared.DataStatuses])
                 res.data_statuses = out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [401, 402, 403, 404, 429, 500, 503]:
-            if utils.match_content_type(content_type, 'application/json'):
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
-                out.raw_response = http_res
                 raise out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+        else:
+            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
     def get_pull_operation(self, request: operations.GetPullOperationRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetPullOperationResponse:
         r"""Get pull operation
         Retrieve information about a single dataset or pull operation.
         """
         hook_ctx = HookContext(operation_id='get-pull-operation', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetPullOperationRequest, base_url, '/companies/{companyId}/data/history/{datasetId}', request)
-        headers = {}
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = self.sdk_configuration.user_agent
+        url = utils.generate_url(base_url, '/companies/{companyId}/data/history/{datasetId}', request)
         
         if callable(self.sdk_configuration.security):
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security())
+            headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security)
+            headers, query_params = utils.get_security(self.sdk_configuration.security)
         
+        headers['Accept'] = 'application/json'
+        headers['user-agent'] = self.sdk_configuration.user_agent
+        client = self.sdk_configuration.client
         
         global_retry_config = self.sdk_configuration.retry_config
         retry_config = retries
         if retry_config is None:
             if global_retry_config:
                 retry_config = global_retry_config
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
+        req = None
         def do_request():
+            nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('GET', url, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
             if utils.match_status_codes(['401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
-        content_type = http_res.headers.get('Content-Type')
         
-        res = operations.GetPullOperationResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetPullOperationResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(content_type, 'application/json'):
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.PullOperation])
                 res.pull_operation = out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [401, 402, 403, 404, 429, 500, 503]:
-            if utils.match_content_type(content_type, 'application/json'):
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
-                out.raw_response = http_res
                 raise out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+        else:
+            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
     def list_pull_operations(self, request: operations.ListPullOperationsRequest, retries: Optional[utils.RetryConfig] = None) -> operations.ListPullOperationsResponse:
         r"""List pull operations
         Gets the pull operation history (datasets) for a given company.
         """
         hook_ctx = HookContext(operation_id='list-pull-operations', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListPullOperationsRequest, base_url, '/companies/{companyId}/data/history', request)
-        headers = {}
-        query_params = utils.get_query_params(operations.ListPullOperationsRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = self.sdk_configuration.user_agent
+        url = utils.generate_url(base_url, '/companies/{companyId}/data/history', request)
         
         if callable(self.sdk_configuration.security):
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security())
+            headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security)
+            headers, query_params = utils.get_security(self.sdk_configuration.security)
         
+        query_params = { **utils.get_query_params(request), **query_params }
+        headers['Accept'] = 'application/json'
+        headers['user-agent'] = self.sdk_configuration.user_agent
+        client = self.sdk_configuration.client
         
         global_retry_config = self.sdk_configuration.retry_config
         retry_config = retries
         if retry_config is None:
             if global_retry_config:
                 retry_config = global_retry_config
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
+        req = None
         def do_request():
+            nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
             if utils.match_status_codes(['400','401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
-        content_type = http_res.headers.get('Content-Type')
         
-        res = operations.ListPullOperationsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.ListPullOperationsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(content_type, 'application/json'):
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.PullOperations])
                 res.pull_operations = out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [400, 401, 402, 403, 404, 429, 500, 503]:
-            if utils.match_content_type(content_type, 'application/json'):
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
-                out.raw_response = http_res
                 raise out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+        else:
+            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
-    
+    
+
```

### Comparing `codat-platform-3.4.0/src/codatplatform/sdkconfiguration.py` & `codat-platform-3.5.0/src/codatplatform/sdkconfiguration.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,39 +3,41 @@
 
 import requests as requests_http
 from ._hooks import SDKHooks
 from .utils import utils
 from .utils.retries import RetryConfig
 from codatplatform.models import shared
 from dataclasses import dataclass
-from typing import Callable, Dict, Tuple, Union
+from typing import Callable, Dict, Optional, Tuple, Union
 
 
 SERVERS = [
     'https://api.codat.io',
     # Production
 ]
 """Contains the list of servers available to the SDK"""
 
 @dataclass
 class SDKConfiguration:
     client: requests_http.Session
     security: Union[shared.Security,Callable[[], shared.Security]] = None
-    server_url: str = ''
-    server_idx: int = 0
+    server_url: Optional[str] = ''
+    server_idx: Optional[int] = 0
     language: str = 'python'
     openapi_doc_version: str = '3.0.0'
-    sdk_version: str = '3.4.0'
-    gen_version: str = '2.277.0'
-    user_agent: str = 'speakeasy-sdk/python 3.4.0 2.277.0 3.0.0 codat-platform'
-    retry_config: RetryConfig = None
-    _hooks: SDKHooks = None
+    sdk_version: str = '3.5.0'
+    gen_version: str = '2.314.0'
+    user_agent: str = 'speakeasy-sdk/python 3.5.0 2.314.0 3.0.0 codat-platform'
+    retry_config: Optional[RetryConfig] = None
+
+    def __post_init__(self):
+        self._hooks = SDKHooks()
 
     def get_server_details(self) -> Tuple[str, Dict[str, str]]:
-        if self.server_url:
+        if self.server_url is not None and self.server_url != '':
             return utils.remove_suffix(self.server_url, '/'), {}
         if self.server_idx is None:
             self.server_idx = 0
 
         return SERVERS[self.server_idx], {}
```

### Comparing `codat-platform-3.4.0/src/codatplatform/settings.py` & `codat-platform-3.5.0/src/codatplatform/settings.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from codatplatform import utils
-from codatplatform._hooks import HookContext
+from codatplatform._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from codatplatform.models import errors, operations, shared
 from typing import Optional
 
 class Settings:
-    r"""Manage your Codat instance."""
+    r"""Manage company profile configuration, sync settings, and API keys."""
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
@@ -30,83 +30,85 @@
         * If you require multiple API keys, perform multiple calls to the *Create API keys* endpoint. 
         * The number of API keys is limited to 10. If you have reached the maximum amount of keys, use the *Delete API key* endpoint to delete an unused key first.
         """
         hook_ctx = HookContext(operation_id='create-api-key', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
         url = base_url + '/apiKeys'
-        headers = {}
+        
+        if callable(self.sdk_configuration.security):
+            headers, query_params = utils.get_security(self.sdk_configuration.security())
+        else:
+            headers, query_params = utils.get_security(self.sdk_configuration.security)
+        
         req_content_type, data, form = utils.serialize_request_body(request, Optional[shared.CreateAPIKey], "request", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
-        
-        if callable(self.sdk_configuration.security):
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security())
-        else:
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security)
-        
+        client = self.sdk_configuration.client
         
         global_retry_config = self.sdk_configuration.retry_config
         retry_config = retries
         if retry_config is None:
             if global_retry_config:
                 retry_config = global_retry_config
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
+        req = None
         def do_request():
+            nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('POST', url, data=data, files=form, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
             if utils.match_status_codes(['400','401','402','403','409','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
-        content_type = http_res.headers.get('Content-Type')
         
-        res = operations.CreateAPIKeyResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.CreateAPIKeyResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 201:
-            if utils.match_content_type(content_type, 'application/json'):
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.APIKeyDetails])
                 res.api_key_details = out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [400, 401, 402, 403, 409, 429, 500, 503]:
-            if utils.match_content_type(content_type, 'application/json'):
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
-                out.raw_response = http_res
                 raise out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+        else:
+            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
     def delete_api_key(self, request: operations.DeleteAPIKeyRequest, retries: Optional[utils.RetryConfig] = None) -> operations.DeleteAPIKeyResponse:
         r"""Delete API key
@@ -120,239 +122,245 @@
 
         * It is possible to delete the last remaining API key. If this happens, a new key can be created via the [API key management page](https://app.codat.io/developers/api-keys) of the Portal.
         * It is possible to delete the API key used to authenticate the *Delete API key* request.
         """
         hook_ctx = HookContext(operation_id='delete-api-key', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.DeleteAPIKeyRequest, base_url, '/apiKeys/{apiKeyId}', request)
-        headers = {}
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = self.sdk_configuration.user_agent
+        url = utils.generate_url(base_url, '/apiKeys/{apiKeyId}', request)
         
         if callable(self.sdk_configuration.security):
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security())
+            headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security)
+            headers, query_params = utils.get_security(self.sdk_configuration.security)
         
+        headers['Accept'] = 'application/json'
+        headers['user-agent'] = self.sdk_configuration.user_agent
+        client = self.sdk_configuration.client
         
         global_retry_config = self.sdk_configuration.retry_config
         retry_config = retries
         if retry_config is None:
             if global_retry_config:
                 retry_config = global_retry_config
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
+        req = None
         def do_request():
+            nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('DELETE', url, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('DELETE', url, params=query_params, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
             if utils.match_status_codes(['401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
-        content_type = http_res.headers.get('Content-Type')
         
-        res = operations.DeleteAPIKeyResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.DeleteAPIKeyResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 204:
-            if utils.match_content_type(content_type, 'application/json'):
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[errors.ErrorMessage])
                 res.error_message = out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [401, 402, 403, 404, 429, 500, 503]:
-            if utils.match_content_type(content_type, 'application/json'):
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
-                out.raw_response = http_res
                 raise out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+        else:
+            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
     def get_profile(self, retries: Optional[utils.RetryConfig] = None) -> operations.GetProfileResponse:
         r"""Get profile
         Fetch your Codat profile.
         """
         hook_ctx = HookContext(operation_id='get-profile', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
         url = base_url + '/profile'
-        headers = {}
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = self.sdk_configuration.user_agent
         
         if callable(self.sdk_configuration.security):
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security())
+            headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security)
+            headers, query_params = utils.get_security(self.sdk_configuration.security)
         
+        headers['Accept'] = 'application/json'
+        headers['user-agent'] = self.sdk_configuration.user_agent
+        client = self.sdk_configuration.client
         
         global_retry_config = self.sdk_configuration.retry_config
         retry_config = retries
         if retry_config is None:
             if global_retry_config:
                 retry_config = global_retry_config
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
+        req = None
         def do_request():
+            nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('GET', url, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
             if utils.match_status_codes(['401','402','403','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
-        content_type = http_res.headers.get('Content-Type')
         
-        res = operations.GetProfileResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetProfileResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(content_type, 'application/json'):
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.Profile])
                 res.profile = out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [401, 402, 403, 429, 500, 503]:
-            if utils.match_content_type(content_type, 'application/json'):
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
-                out.raw_response = http_res
                 raise out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+        else:
+            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
     def get_sync_settings(self, retries: Optional[utils.RetryConfig] = None) -> operations.GetProfileSyncSettingsResponse:
         r"""Get sync settings
         Retrieve the [sync settings](https://docs.codat.io/knowledge-base/advanced-sync-settings) for your client. This includes how often data types should be queued to be updated, and how much history should be fetched.
         """
         hook_ctx = HookContext(operation_id='get-profile-syncSettings', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
         url = base_url + '/profile/syncSettings'
-        headers = {}
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = self.sdk_configuration.user_agent
         
         if callable(self.sdk_configuration.security):
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security())
+            headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security)
+            headers, query_params = utils.get_security(self.sdk_configuration.security)
         
+        headers['Accept'] = 'application/json'
+        headers['user-agent'] = self.sdk_configuration.user_agent
+        client = self.sdk_configuration.client
         
         global_retry_config = self.sdk_configuration.retry_config
         retry_config = retries
         if retry_config is None:
             if global_retry_config:
                 retry_config = global_retry_config
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
+        req = None
         def do_request():
+            nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('GET', url, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
             if utils.match_status_codes(['401','402','403','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
-        content_type = http_res.headers.get('Content-Type')
         
-        res = operations.GetProfileSyncSettingsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetProfileSyncSettingsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(content_type, 'application/json'):
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.SyncSettings])
                 res.sync_settings = out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [401, 402, 403, 429, 500, 503]:
-            if utils.match_content_type(content_type, 'application/json'):
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
-                out.raw_response = http_res
                 raise out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+        else:
+            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
     def list_api_keys(self, retries: Optional[utils.RetryConfig] = None) -> operations.ListAPIKeysResponse:
         r"""List API keys
@@ -362,237 +370,243 @@
 
         You can [read more](https://docs.codat.io/using-the-api/authentication) about authentication at Codat and managing API keys via the Portal UI or API.
         """
         hook_ctx = HookContext(operation_id='list-api-keys', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
         url = base_url + '/apiKeys'
-        headers = {}
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = self.sdk_configuration.user_agent
         
         if callable(self.sdk_configuration.security):
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security())
+            headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security)
+            headers, query_params = utils.get_security(self.sdk_configuration.security)
         
+        headers['Accept'] = 'application/json'
+        headers['user-agent'] = self.sdk_configuration.user_agent
+        client = self.sdk_configuration.client
         
         global_retry_config = self.sdk_configuration.retry_config
         retry_config = retries
         if retry_config is None:
             if global_retry_config:
                 retry_config = global_retry_config
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
+        req = None
         def do_request():
+            nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('GET', url, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
             if utils.match_status_codes(['401','402','403','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
-        content_type = http_res.headers.get('Content-Type')
         
-        res = operations.ListAPIKeysResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.ListAPIKeysResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(content_type, 'application/json'):
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.APIKeys])
                 res.api_keys = out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [401, 402, 403, 429, 500, 503]:
-            if utils.match_content_type(content_type, 'application/json'):
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
-                out.raw_response = http_res
                 raise out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+        else:
+            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
     def update_profile(self, request: Optional[shared.Profile], retries: Optional[utils.RetryConfig] = None) -> operations.UpdateProfileResponse:
         r"""Update profile
         Update your Codat profile
         """
         hook_ctx = HookContext(operation_id='update-profile', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
         url = base_url + '/profile'
-        headers = {}
+        
+        if callable(self.sdk_configuration.security):
+            headers, query_params = utils.get_security(self.sdk_configuration.security())
+        else:
+            headers, query_params = utils.get_security(self.sdk_configuration.security)
+        
         req_content_type, data, form = utils.serialize_request_body(request, Optional[shared.Profile], "request", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
-        
-        if callable(self.sdk_configuration.security):
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security())
-        else:
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security)
-        
+        client = self.sdk_configuration.client
         
         global_retry_config = self.sdk_configuration.retry_config
         retry_config = retries
         if retry_config is None:
             if global_retry_config:
                 retry_config = global_retry_config
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
+        req = None
         def do_request():
+            nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('PUT', url, data=data, files=form, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('PUT', url, params=query_params, data=data, files=form, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
             if utils.match_status_codes(['401','402','403','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
-        content_type = http_res.headers.get('Content-Type')
         
-        res = operations.UpdateProfileResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.UpdateProfileResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(content_type, 'application/json'):
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.Profile])
                 res.profile = out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [401, 402, 403, 429, 500, 503]:
-            if utils.match_content_type(content_type, 'application/json'):
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
-                out.raw_response = http_res
                 raise out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+        else:
+            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
     def update_sync_settings(self, request: Optional[operations.UpdateProfileSyncSettingsRequestBody], retries: Optional[utils.RetryConfig] = None) -> operations.UpdateProfileSyncSettingsResponse:
         r"""Update all sync settings
         Update sync settings for all data types.
         """
         hook_ctx = HookContext(operation_id='update-profile-syncSettings', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
         url = base_url + '/profile/syncSettings'
-        headers = {}
+        
+        if callable(self.sdk_configuration.security):
+            headers, query_params = utils.get_security(self.sdk_configuration.security())
+        else:
+            headers, query_params = utils.get_security(self.sdk_configuration.security)
+        
         req_content_type, data, form = utils.serialize_request_body(request, Optional[operations.UpdateProfileSyncSettingsRequestBody], "request", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
-        
-        if callable(self.sdk_configuration.security):
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security())
-        else:
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security)
-        
+        client = self.sdk_configuration.client
         
         global_retry_config = self.sdk_configuration.retry_config
         retry_config = retries
         if retry_config is None:
             if global_retry_config:
                 retry_config = global_retry_config
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
+        req = None
         def do_request():
+            nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('POST', url, data=data, files=form, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
             if utils.match_status_codes(['401','402','403','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
-        content_type = http_res.headers.get('Content-Type')
         
-        res = operations.UpdateProfileSyncSettingsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.UpdateProfileSyncSettingsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 204:
             pass
         elif http_res.status_code in [401, 402, 403, 429, 500, 503]:
-            if utils.match_content_type(content_type, 'application/json'):
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
-                out.raw_response = http_res
                 raise out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+        else:
+            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
-    
+    
+
```

### Comparing `codat-platform-3.4.0/src/codatplatform/supplemental_data.py` & `codat-platform-3.5.0/src/codatplatform/supplemental_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from codatplatform import utils
-from codatplatform._hooks import HookContext
+from codatplatform._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from codatplatform.models import errors, operations, shared
 from typing import Optional
 
 class SupplementalData:
-    r"""View and configure supplemental data for supported data types."""
+    r"""Configure and pull additional data you can include in Codat's standard data types."""
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
@@ -24,158 +24,162 @@
 
         **Integration-specific behaviour**
         See the *examples* for integration-specific frequently requested properties.
         """
         hook_ctx = HookContext(operation_id='configure-supplemental-data', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ConfigureSupplementalDataRequest, base_url, '/integrations/{platformKey}/dataTypes/{dataType}/supplementalDataConfig', request)
-        headers = {}
+        url = utils.generate_url(base_url, '/integrations/{platformKey}/dataTypes/{dataType}/supplementalDataConfig', request)
+        
+        if callable(self.sdk_configuration.security):
+            headers, query_params = utils.get_security(self.sdk_configuration.security())
+        else:
+            headers, query_params = utils.get_security(self.sdk_configuration.security)
+        
         req_content_type, data, form = utils.serialize_request_body(request, operations.ConfigureSupplementalDataRequest, "supplemental_data_configuration", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
-        
-        if callable(self.sdk_configuration.security):
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security())
-        else:
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security)
-        
+        client = self.sdk_configuration.client
         
         global_retry_config = self.sdk_configuration.retry_config
         retry_config = retries
         if retry_config is None:
             if global_retry_config:
                 retry_config = global_retry_config
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
+        req = None
         def do_request():
+            nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('PUT', url, data=data, files=form, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('PUT', url, params=query_params, data=data, files=form, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
             if utils.match_status_codes(['401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
-        content_type = http_res.headers.get('Content-Type')
         
-        res = operations.ConfigureSupplementalDataResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.ConfigureSupplementalDataResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code in [401, 402, 403, 404, 429, 500, 503]:
-            if utils.match_content_type(content_type, 'application/json'):
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
-                out.raw_response = http_res
                 raise out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+        else:
+            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
     def get_configuration(self, request: operations.GetSupplementalDataConfigurationRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetSupplementalDataConfigurationResponse:
         r"""Get configuration
         The *Get configuration* endpoint returns supplemental data configuration previously created for each integration and data type combination.
 
         [Supplemental data](https://docs.codat.io/using-the-api/additional-data) is additional data you can include in Codat's standard data types.
         """
         hook_ctx = HookContext(operation_id='get-supplemental-data-configuration', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetSupplementalDataConfigurationRequest, base_url, '/integrations/{platformKey}/dataTypes/{dataType}/supplementalDataConfig', request)
-        headers = {}
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = self.sdk_configuration.user_agent
+        url = utils.generate_url(base_url, '/integrations/{platformKey}/dataTypes/{dataType}/supplementalDataConfig', request)
         
         if callable(self.sdk_configuration.security):
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security())
+            headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security)
+            headers, query_params = utils.get_security(self.sdk_configuration.security)
         
+        headers['Accept'] = 'application/json'
+        headers['user-agent'] = self.sdk_configuration.user_agent
+        client = self.sdk_configuration.client
         
         global_retry_config = self.sdk_configuration.retry_config
         retry_config = retries
         if retry_config is None:
             if global_retry_config:
                 retry_config = global_retry_config
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
+        req = None
         def do_request():
+            nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('GET', url, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
             if utils.match_status_codes(['401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
-        content_type = http_res.headers.get('Content-Type')
         
-        res = operations.GetSupplementalDataConfigurationResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetSupplementalDataConfigurationResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(content_type, 'application/json'):
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.SupplementalDataConfiguration])
                 res.supplemental_data_configuration = out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [401, 402, 403, 404, 429, 500, 503]:
-            if utils.match_content_type(content_type, 'application/json'):
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
-                out.raw_response = http_res
                 raise out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+        else:
+            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
-    
+    
+
```

### Comparing `codat-platform-3.4.0/src/codatplatform/utils/retries.py` & `codat-platform-3.5.0/src/codatplatform/utils/retries.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,20 +71,20 @@
                             raise TemporaryError(res)
                     else:
                         parsed_code = int(code)
 
                         if res.status_code == parsed_code:
                             raise TemporaryError(res)
             except requests.exceptions.ConnectionError as exception:
-                if retries.config.config.retry_connection_errors:
+                if retries.config.retry_connection_errors:
                     raise
 
                 raise PermanentError(exception) from exception
             except requests.exceptions.Timeout as exception:
-                if retries.config.config.retry_connection_errors:
+                if retries.config.retry_connection_errors:
                     raise
 
                 raise PermanentError(exception) from exception
             except TemporaryError:
                 raise
             except Exception as exception:
                 raise PermanentError(exception) from exception
@@ -110,11 +110,10 @@
             if now - start > max_elapsed_time:
                 if isinstance(exception, TemporaryError):
                     return exception.response
 
                 raise
             sleep = ((initial_interval/1000) *
                      exponent**retries + random.uniform(0, 1))
-            if sleep > max_interval/1000:
-                sleep = max_interval/1000
+            sleep = min(sleep, max_interval / 1000)
             time.sleep(sleep)
             retries += 1
```

### Comparing `codat-platform-3.4.0/src/codatplatform/utils/utils.py` & `codat-platform-3.5.0/src/codatplatform/utils/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,512 +1,636 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import base64
 import json
 import re
 import sys
-from dataclasses import Field, dataclass, fields, is_dataclass, make_dataclass
+from dataclasses import Field, fields, is_dataclass, make_dataclass
 from datetime import date, datetime
 from decimal import Decimal
 from email.message import Message
 from enum import Enum
-from typing import (Any, Callable, Dict, List, Optional, Tuple, Union,
-                    get_args, get_origin)
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    List,
+    Optional,
+    Tuple,
+    Union,
+    get_args,
+    get_origin,
+)
 from xmlrpc.client import boolean
 from typing_inspect import is_optional_type
 import dateutil.parser
-import requests
 from dataclasses_json import DataClassJsonMixin
 
 
-class SecurityClient:
-    client: requests.Session
-    query_params: Dict[str, str] = {}
+def get_security(security: Any) -> Tuple[Dict[str, str], Dict[str, str]]:
     headers: Dict[str, str] = {}
-
-    def __init__(self, client: requests.Session):
-        self.client = client
-
-    def send(self, request: requests.PreparedRequest, **kwargs):
-        request.prepare_url(url=request.url, params=self.query_params)
-        request.headers.update(self.headers)
-
-        return self.client.send(request, **kwargs)
-
-
-def configure_security_client(client: requests.Session, security: dataclass):
-    client = SecurityClient(client)
+    query_params: Dict[str, str] = {}
 
     if security is None:
-        return client
+        return headers, query_params
 
     sec_fields: Tuple[Field, ...] = fields(security)
     for sec_field in sec_fields:
         value = getattr(security, sec_field.name)
         if value is None:
             continue
 
-        metadata = sec_field.metadata.get('security')
+        metadata = sec_field.metadata.get("security")
         if metadata is None:
             continue
-        if metadata.get('option'):
-            _parse_security_option(client, value)
-            return client
-        if metadata.get('scheme'):
+        if metadata.get("option"):
+            _parse_security_option(headers, query_params, value)
+            return headers, query_params
+        if metadata.get("scheme"):
             # Special case for basic auth which could be a flattened struct
             if metadata.get("sub_type") == "basic" and not is_dataclass(value):
-                _parse_security_scheme(client, metadata, security)
+                _parse_security_scheme(headers, query_params, metadata, security)
             else:
-                _parse_security_scheme(client, metadata, value)
+                _parse_security_scheme(headers, query_params, metadata, value)
 
-    return client
+    return headers, query_params
 
 
-def _parse_security_option(client: SecurityClient, option: dataclass):
+def _parse_security_option(
+    headers: Dict[str, str], query_params: Dict[str, str], option: Any
+):
     opt_fields: Tuple[Field, ...] = fields(option)
     for opt_field in opt_fields:
-        metadata = opt_field.metadata.get('security')
-        if metadata is None or metadata.get('scheme') is None:
+        metadata = opt_field.metadata.get("security")
+        if metadata is None or metadata.get("scheme") is None:
             continue
         _parse_security_scheme(
-            client, metadata, getattr(option, opt_field.name))
+            headers, query_params, metadata, getattr(option, opt_field.name)
+        )
 
 
-def _parse_security_scheme(client: SecurityClient, scheme_metadata: Dict, scheme: any):
-    scheme_type = scheme_metadata.get('type')
-    sub_type = scheme_metadata.get('sub_type')
+def _parse_security_scheme(
+    headers: Dict[str, str],
+    query_params: Dict[str, str],
+    scheme_metadata: Dict,
+    scheme: Any,
+):
+    scheme_type = scheme_metadata.get("type")
+    sub_type = scheme_metadata.get("sub_type")
 
     if is_dataclass(scheme):
-        if scheme_type == 'http' and sub_type == 'basic':
-            _parse_basic_auth_scheme(client, scheme)
+        if scheme_type == "http" and sub_type == "basic":
+            _parse_basic_auth_scheme(headers, scheme)
             return
 
         scheme_fields: Tuple[Field, ...] = fields(scheme)
         for scheme_field in scheme_fields:
-            metadata = scheme_field.metadata.get('security')
-            if metadata is None or metadata.get('field_name') is None:
+            metadata = scheme_field.metadata.get("security")
+            if metadata is None or metadata.get("field_name") is None:
                 continue
 
             value = getattr(scheme, scheme_field.name)
 
             _parse_security_scheme_value(
-                client, scheme_metadata, metadata, value)
+                headers, query_params, scheme_metadata, metadata, value
+            )
     else:
         _parse_security_scheme_value(
-            client, scheme_metadata, scheme_metadata, scheme)
+            headers, query_params, scheme_metadata, scheme_metadata, scheme
+        )
 
 
-def _parse_security_scheme_value(client: SecurityClient, scheme_metadata: Dict, security_metadata: Dict, value: any):
-    scheme_type = scheme_metadata.get('type')
-    sub_type = scheme_metadata.get('sub_type')
+def _parse_security_scheme_value(
+    headers: Dict[str, str],
+    query_params: Dict[str, str],
+    scheme_metadata: Dict,
+    security_metadata: Dict,
+    value: Any,
+):
+    scheme_type = scheme_metadata.get("type")
+    sub_type = scheme_metadata.get("sub_type")
 
-    header_name = security_metadata.get('field_name')
+    header_name = str(security_metadata.get("field_name"))
 
     if scheme_type == "apiKey":
-        if sub_type == 'header':
-            client.headers[header_name] = value
-        elif sub_type == 'query':
-            client.query_params[header_name] = value
+        if sub_type == "header":
+            headers[header_name] = value
+        elif sub_type == "query":
+            query_params[header_name] = value
         else:
-            raise Exception('not supported')
+            raise Exception("not supported")
     elif scheme_type == "openIdConnect":
-        client.headers[header_name] = _apply_bearer(value)
-    elif scheme_type == 'oauth2':
-        if sub_type != 'client_credentials':
-            client.headers[header_name] = _apply_bearer(value)
-    elif scheme_type == 'http':
-        if sub_type == 'bearer':
-            client.headers[header_name] = _apply_bearer(value)
+        headers[header_name] = _apply_bearer(value)
+    elif scheme_type == "oauth2":
+        if sub_type != "client_credentials":
+            headers[header_name] = _apply_bearer(value)
+    elif scheme_type == "http":
+        if sub_type == "bearer":
+            headers[header_name] = _apply_bearer(value)
         else:
-            raise Exception('not supported')
+            raise Exception("not supported")
     else:
-        raise Exception('not supported')
+        raise Exception("not supported")
 
 
 def _apply_bearer(token: str) -> str:
-    return token.lower().startswith('bearer ') and token or f'Bearer {token}'
+    return token.lower().startswith("bearer ") and token or f"Bearer {token}"
 
 
-def _parse_basic_auth_scheme(client: SecurityClient, scheme: dataclass):
+def _parse_basic_auth_scheme(headers: Dict[str, str], scheme: Any):
     username = ""
     password = ""
 
     scheme_fields: Tuple[Field, ...] = fields(scheme)
     for scheme_field in scheme_fields:
-        metadata = scheme_field.metadata.get('security')
-        if metadata is None or metadata.get('field_name') is None:
+        metadata = scheme_field.metadata.get("security")
+        if metadata is None or metadata.get("field_name") is None:
             continue
 
-        field_name = metadata.get('field_name')
+        field_name = metadata.get("field_name")
         value = getattr(scheme, scheme_field.name)
 
-        if field_name == 'username':
+        if field_name == "username":
             username = value
-        if field_name == 'password':
+        if field_name == "password":
             password = value
 
-    data = f'{username}:{password}'.encode()
-    client.headers['Authorization'] = f'Basic {base64.b64encode(data).decode()}'
+    data = f"{username}:{password}".encode()
+    headers["Authorization"] = f"Basic {base64.b64encode(data).decode()}"
+
 
+def generate_url(
+    server_url: str,
+    path: str,
+    path_params: Any,
+    gbls: Optional[Any] = None,
+) -> str:
+    path_param_values: Dict[str, str] = {}
+
+    globals_already_populated = _populate_path_params(
+        path_params, gbls, path_param_values, []
+    )
+    if gbls is not None:
+        _populate_path_params(gbls, None, path_param_values, globals_already_populated)
+
+    for key, value in path_param_values.items():
+        path = path.replace("{" + key + "}", value, 1)
+
+    return remove_suffix(server_url, "/") + path
+
+
+def _populate_path_params(
+    path_params: Any,
+    gbls: Any,
+    path_param_values: Dict[str, str],
+    skip_fields: List[str],
+) -> List[str]:
+    globals_already_populated: List[str] = []
 
-def generate_url(clazz: type, server_url: str, path: str, path_params: dataclass,
-                 gbls: Dict[str, Dict[str, Dict[str, Any]]] = None) -> str:
-    path_param_fields: Tuple[Field, ...] = fields(clazz)
+    path_param_fields: Tuple[Field, ...] = fields(path_params)
     for field in path_param_fields:
-        request_metadata = field.metadata.get('request')
-        if request_metadata is not None:
+        if field.name in skip_fields:
             continue
 
-        param_metadata = field.metadata.get('path_param')
+        param_metadata = field.metadata.get("path_param")
         if param_metadata is None:
             continue
 
-        param = getattr(
-            path_params, field.name) if path_params is not None else None
-        param = _populate_from_globals(
-            field.name, param, 'pathParam', gbls)
+        param = getattr(path_params, field.name) if path_params is not None else None
+        param, global_found = _populate_from_globals(
+            field.name, param, "path_param", gbls
+        )
+        if global_found:
+            globals_already_populated.append(field.name)
 
         if param is None:
             continue
 
         f_name = param_metadata.get("field_name", field.name)
-        serialization = param_metadata.get('serialization', '')
-        if serialization != '':
+        serialization = param_metadata.get("serialization", "")
+        if serialization != "":
             serialized_params = _get_serialized_params(
-                param_metadata, field.type, f_name, param)
+                param_metadata, field.type, f_name, param
+            )
             for key, value in serialized_params.items():
-                path = path.replace(
-                    '{' + key + '}', value, 1)
+                path_param_values[key] = value
         else:
-            if param_metadata.get('style', 'simple') == 'simple':
+            if param_metadata.get("style", "simple") == "simple":
                 if isinstance(param, List):
                     pp_vals: List[str] = []
                     for pp_val in param:
                         if pp_val is None:
                             continue
                         pp_vals.append(_val_to_string(pp_val))
-                    path = path.replace(
-                        '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
+                    path_param_values[param_metadata.get("field_name", field.name)] = (
+                        ",".join(pp_vals)
+                    )
                 elif isinstance(param, Dict):
                     pp_vals: List[str] = []
                     for pp_key in param:
                         if param[pp_key] is None:
                             continue
-                        if param_metadata.get('explode'):
-                            pp_vals.append(
-                                f"{pp_key}={_val_to_string(param[pp_key])}")
+                        if param_metadata.get("explode"):
+                            pp_vals.append(f"{pp_key}={_val_to_string(param[pp_key])}")
                         else:
-                            pp_vals.append(
-                                f"{pp_key},{_val_to_string(param[pp_key])}")
-                    path = path.replace(
-                        '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
+                            pp_vals.append(f"{pp_key},{_val_to_string(param[pp_key])}")
+                    path_param_values[param_metadata.get("field_name", field.name)] = (
+                        ",".join(pp_vals)
+                    )
                 elif not isinstance(param, (str, int, float, complex, bool, Decimal)):
                     pp_vals: List[str] = []
                     param_fields: Tuple[Field, ...] = fields(param)
                     for param_field in param_fields:
-                        param_value_metadata = param_field.metadata.get(
-                            'path_param')
+                        param_value_metadata = param_field.metadata.get("path_param")
                         if not param_value_metadata:
                             continue
 
-                        parm_name = param_value_metadata.get(
-                            'field_name', field.name)
+                        param_name = param_value_metadata.get("field_name", field.name)
 
                         param_field_val = getattr(param, param_field.name)
                         if param_field_val is None:
                             continue
-                        if param_metadata.get('explode'):
+                        if param_metadata.get("explode"):
                             pp_vals.append(
-                                f"{parm_name}={_val_to_string(param_field_val)}")
+                                f"{param_name}={_val_to_string(param_field_val)}"
+                            )
                         else:
                             pp_vals.append(
-                                f"{parm_name},{_val_to_string(param_field_val)}")
-                    path = path.replace(
-                        '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
+                                f"{param_name},{_val_to_string(param_field_val)}"
+                            )
+                    path_param_values[param_metadata.get("field_name", field.name)] = (
+                        ",".join(pp_vals)
+                    )
                 else:
-                    path = path.replace(
-                        '{' + param_metadata.get('field_name', field.name) + '}', _val_to_string(param), 1)
+                    path_param_values[param_metadata.get("field_name", field.name)] = (
+                        _val_to_string(param)
+                    )
 
-    return remove_suffix(server_url, '/') + path
+    return globals_already_populated
 
 
 def is_optional(field):
     return get_origin(field) is Union and type(None) in get_args(field)
 
 
 def template_url(url_with_params: str, params: Dict[str, str]) -> str:
     for key, value in params.items():
-        url_with_params = url_with_params.replace(
-            '{' + key + '}', value)
+        url_with_params = url_with_params.replace("{" + key + "}", value)
 
     return url_with_params
 
 
-def get_query_params(clazz: type, query_params: dataclass, gbls: Dict[str, Dict[str, Dict[str, Any]]] = None) -> Dict[
-        str, List[str]]:
+def get_query_params(
+    query_params: Any,
+    gbls: Optional[Any] = None,
+) -> Dict[str, List[str]]:
     params: Dict[str, List[str]] = {}
 
-    param_fields: Tuple[Field, ...] = fields(clazz)
+    globals_already_populated = _populate_query_params(query_params, gbls, params, [])
+    if gbls is not None:
+        _populate_query_params(gbls, None, params, globals_already_populated)
+
+    return params
+
+
+def _populate_query_params(
+    query_params: Any,
+    gbls: Any,
+    query_param_values: Dict[str, List[str]],
+    skip_fields: List[str],
+) -> List[str]:
+    globals_already_populated: List[str] = []
+
+    param_fields: Tuple[Field, ...] = fields(query_params)
     for field in param_fields:
-        request_metadata = field.metadata.get('request')
-        if request_metadata is not None:
+        if field.name in skip_fields:
             continue
 
-        metadata = field.metadata.get('query_param')
+        metadata = field.metadata.get("query_param")
         if not metadata:
             continue
 
         param_name = field.name
-        value = getattr(
-            query_params, param_name) if query_params is not None else None
+        value = getattr(query_params, param_name) if query_params is not None else None
 
-        value = _populate_from_globals(param_name, value, 'queryParam', gbls)
+        value, global_found = _populate_from_globals(
+            param_name, value, "query_param", gbls
+        )
+        if global_found:
+            globals_already_populated.append(param_name)
 
         f_name = metadata.get("field_name")
-        serialization = metadata.get('serialization', '')
-        if serialization != '':
+        serialization = metadata.get("serialization", "")
+        if serialization != "":
             serialized_parms = _get_serialized_params(
-                metadata, field.type, f_name, value)
+                metadata, field.type, f_name, value
+            )
             for key, value in serialized_parms.items():
-                if key in params:
-                    params[key].extend(value)
+                if key in query_param_values:
+                    query_param_values[key].extend(value)
                 else:
-                    params[key] = [value]
+                    query_param_values[key] = [value]
         else:
-            style = metadata.get('style', 'form')
-            if style == 'deepObject':
-                params = {**params, **_get_deep_object_query_params(
-                    metadata, f_name, value)}
-            elif style == 'form':
-                params = {**params, **_get_delimited_query_params(
-                    metadata, f_name, value, ",")}
-            elif style == 'pipeDelimited':
-                params = {**params, **_get_delimited_query_params(
-                    metadata, f_name, value, "|")}
+            style = metadata.get("style", "form")
+            if style == "deepObject":
+                _populate_deep_object_query_params(
+                    metadata, f_name, value, query_param_values
+                )
+            elif style == "form":
+                _populate_delimited_query_params(
+                    metadata, f_name, value, ",", query_param_values
+                )
+            elif style == "pipeDelimited":
+                _populate_delimited_query_params(
+                    metadata, f_name, value, "|", query_param_values
+                )
             else:
-                raise Exception('not yet implemented')
-    return params
+                raise Exception("not yet implemented")
 
+    return globals_already_populated
 
-def get_headers(headers_params: dataclass) -> Dict[str, str]:
-    if headers_params is None:
-        return {}
 
+def get_headers(headers_params: Any, gbls: Optional[Any] = None) -> Dict[str, str]:
     headers: Dict[str, str] = {}
 
-    param_fields: Tuple[Field, ...] = fields(headers_params)
-    for field in param_fields:
-        metadata = field.metadata.get('header')
-        if not metadata:
-            continue
+    globals_already_populated = []
+    if headers_params is not None:
+        globals_already_populated = _populate_headers(headers_params, gbls, headers, [])
+    if gbls is not None:
+        _populate_headers(gbls, None, headers, globals_already_populated)
+
+    return headers
 
-        value = _serialize_header(metadata.get(
-            'explode', False), getattr(headers_params, field.name))
 
-        if value != '':
-            headers[metadata.get('field_name', field.name)] = value
+def _populate_headers(
+    headers_params: Any,
+    gbls: Any,
+    header_values: Dict[str, str],
+    skip_fields: List[str],
+) -> List[str]:
+    globals_already_populated: List[str] = []
 
-    return headers
+    param_fields: Tuple[Field, ...] = fields(headers_params)
+    for field in param_fields:
+        if field.name in skip_fields:
+            continue
 
+        metadata = field.metadata.get("header")
+        if not metadata:
+            continue
 
-def _get_serialized_params(metadata: Dict, field_type: type, field_name: str, obj: any) -> Dict[str, str]:
+        value, global_found = _populate_from_globals(
+            field.name, getattr(headers_params, field.name), "header", gbls
+        )
+        if global_found:
+            globals_already_populated.append(field.name)
+        value = _serialize_header(metadata.get("explode", False), value)
+
+        if value != "":
+            header_values[metadata.get("field_name", field.name)] = value
+
+    return globals_already_populated
+
+
+def _get_serialized_params(
+    metadata: Dict, field_type: type, field_name: str, obj: Any
+) -> Dict[str, str]:
     params: Dict[str, str] = {}
 
-    serialization = metadata.get('serialization', '')
-    if serialization == 'json':
-        params[metadata.get("field_name", field_name)
-               ] = marshal_json(obj, field_type)
+    serialization = metadata.get("serialization", "")
+    if serialization == "json":
+        params[metadata.get("field_name", field_name)] = marshal_json(obj, field_type)
 
     return params
 
 
-def _get_deep_object_query_params(metadata: Dict, field_name: str, obj: any) -> Dict[str, List[str]]:
-    params: Dict[str, List[str]] = {}
-
+def _populate_deep_object_query_params(
+    metadata: Dict, field_name: str, obj: Any, params: Dict[str, List[str]]
+):
     if obj is None:
-        return params
+        return
 
     if is_dataclass(obj):
         obj_fields: Tuple[Field, ...] = fields(obj)
         for obj_field in obj_fields:
-            obj_param_metadata = obj_field.metadata.get('query_param')
+            obj_param_metadata = obj_field.metadata.get("query_param")
             if not obj_param_metadata:
                 continue
 
             obj_val = getattr(obj, obj_field.name)
             if obj_val is None:
                 continue
 
             if isinstance(obj_val, List):
                 for val in obj_val:
                     if val is None:
                         continue
 
-                    if params.get(
-                            f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]') is None:
+                    if (
+                        params.get(
+                            f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'
+                        )
+                        is None
+                    ):
                         params[
-                            f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'] = [
-                        ]
+                            f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'
+                        ] = []
 
                     params[
-                        f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'].append(
-                        _val_to_string(val))
+                        f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'
+                    ].append(_val_to_string(val))
             else:
                 params[
-                    f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'] = [
-                    _val_to_string(obj_val)]
+                    f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'
+                ] = [_val_to_string(obj_val)]
     elif isinstance(obj, Dict):
         for key, value in obj.items():
             if value is None:
                 continue
 
             if isinstance(value, List):
                 for val in value:
                     if val is None:
                         continue
 
-                    if params.get(f'{metadata.get("field_name", field_name)}[{key}]') is None:
-                        params[f'{metadata.get("field_name", field_name)}[{key}]'] = [
-                        ]
-
-                    params[
-                        f'{metadata.get("field_name", field_name)}[{key}]'].append(_val_to_string(val))
+                    if (
+                        params.get(f'{metadata.get("field_name", field_name)}[{key}]')
+                        is None
+                    ):
+                        params[f'{metadata.get("field_name", field_name)}[{key}]'] = []
+
+                    params[f'{metadata.get("field_name", field_name)}[{key}]'].append(
+                        _val_to_string(val)
+                    )
             else:
                 params[f'{metadata.get("field_name", field_name)}[{key}]'] = [
-                    _val_to_string(value)]
-    return params
+                    _val_to_string(value)
+                ]
 
 
 def _get_query_param_field_name(obj_field: Field) -> str:
-    obj_param_metadata = obj_field.metadata.get('query_param')
+    obj_param_metadata = obj_field.metadata.get("query_param")
 
     if not obj_param_metadata:
         return ""
 
     return obj_param_metadata.get("field_name", obj_field.name)
 
 
-def _get_delimited_query_params(metadata: Dict, field_name: str, obj: any, delimiter: str) -> Dict[
-        str, List[str]]:
-    return _populate_form(field_name, metadata.get("explode", True), obj, _get_query_param_field_name, delimiter)
+def _populate_delimited_query_params(
+    metadata: Dict,
+    field_name: str,
+    obj: Any,
+    delimiter: str,
+    query_param_values: Dict[str, List[str]],
+):
+    _populate_form(
+        field_name,
+        metadata.get("explode", True),
+        obj,
+        _get_query_param_field_name,
+        delimiter,
+        query_param_values,
+    )
 
 
 SERIALIZATION_METHOD_TO_CONTENT_TYPE = {
-    'json': 'application/json',
-    'form': 'application/x-www-form-urlencoded',
-    'multipart': 'multipart/form-data',
-    'raw': 'application/octet-stream',
-    'string': 'text/plain',
+    "json": "application/json",
+    "form": "application/x-www-form-urlencoded",
+    "multipart": "multipart/form-data",
+    "raw": "application/octet-stream",
+    "string": "text/plain",
 }
 
 
-def serialize_request_body(request: dataclass, request_type: type, request_field_name: str, nullable: bool, optional: bool, serialization_method: str, encoder=None) -> Tuple[
-        str, any, any]:
+def serialize_request_body(
+    request: Any,
+    request_type: type,
+    request_field_name: str,
+    nullable: bool,
+    optional: bool,
+    serialization_method: str,
+    encoder=None,
+) -> Tuple[Optional[str], Optional[Any], Optional[Any]]:
     if request is None:
         if not nullable and optional:
             return None, None, None
 
     if not is_dataclass(request) or not hasattr(request, request_field_name):
-        return serialize_content_type(request_field_name, request_type, SERIALIZATION_METHOD_TO_CONTENT_TYPE[serialization_method],
-                                      request, encoder)
+        return serialize_content_type(
+            request_field_name,
+            request_type,
+            SERIALIZATION_METHOD_TO_CONTENT_TYPE[serialization_method],
+            request,
+            encoder,
+        )
 
     request_val = getattr(request, request_field_name)
 
     if request_val is None:
         if not nullable and optional:
             return None, None, None
 
     request_fields: Tuple[Field, ...] = fields(request)
     request_metadata = None
 
     for field in request_fields:
         if field.name == request_field_name:
-            request_metadata = field.metadata.get('request')
+            request_metadata = field.metadata.get("request")
             break
 
     if request_metadata is None:
-        raise Exception('invalid request type')
+        raise Exception("invalid request type")
 
-    return serialize_content_type(request_field_name, request_type, request_metadata.get('media_type', 'application/octet-stream'),
-                                  request_val)
+    return serialize_content_type(
+        request_field_name,
+        request_type,
+        request_metadata.get("media_type", "application/octet-stream"),
+        request_val,
+    )
 
 
-def serialize_content_type(field_name: str, request_type: any, media_type: str, request: dataclass, encoder=None) -> Tuple[str, any, List[List[any]]]:
-    if re.match(r'(application|text)\/.*?\+*json.*', media_type) is not None:
+def serialize_content_type(
+    field_name: str, request_type: Any, media_type: str, request: Any, encoder=None
+) -> Tuple[Optional[str], Optional[Any], Optional[List[List[Any]]]]:
+    if re.match(r"(application|text)\/.*?\+*json.*", media_type) is not None:
         return media_type, marshal_json(request, request_type, encoder), None
-    if re.match(r'multipart\/.*', media_type) is not None:
+    if re.match(r"multipart\/.*", media_type) is not None:
         return serialize_multipart_form(media_type, request)
-    if re.match(r'application\/x-www-form-urlencoded.*', media_type) is not None:
+    if re.match(r"application\/x-www-form-urlencoded.*", media_type) is not None:
         return media_type, serialize_form_data(field_name, request), None
     if isinstance(request, (bytes, bytearray)):
         return media_type, request, None
     if isinstance(request, str):
         return media_type, request, None
 
     raise Exception(
-        f"invalid request body type {type(request)} for mediaType {media_type}")
+        f"invalid request body type {type(request)} for mediaType {media_type}"
+    )
 
 
-def serialize_multipart_form(media_type: str, request: dataclass) -> Tuple[str, any, List[List[any]]]:
-    form: List[List[any]] = []
+def serialize_multipart_form(
+    media_type: str, request: Any
+) -> Tuple[str, Any, List[List[Any]]]:
+    form: List[List[Any]] = []
     request_fields = fields(request)
 
     for field in request_fields:
         val = getattr(request, field.name)
         if val is None:
             continue
 
-        field_metadata = field.metadata.get('multipart_form')
+        field_metadata = field.metadata.get("multipart_form")
         if not field_metadata:
             continue
 
         if field_metadata.get("file") is True:
             file_fields = fields(val)
 
             file_name = ""
             field_name = ""
             content = bytes()
 
             for file_field in file_fields:
-                file_metadata = file_field.metadata.get('multipart_form')
+                file_metadata = file_field.metadata.get("multipart_form")
                 if file_metadata is None:
                     continue
 
                 if file_metadata.get("content") is True:
                     content = getattr(val, file_field.name)
                 else:
-                    field_name = file_metadata.get(
-                        "field_name", file_field.name)
+                    field_name = file_metadata.get("field_name", file_field.name)
                     file_name = getattr(val, file_field.name)
             if field_name == "" or file_name == "" or content == bytes():
-                raise Exception('invalid multipart/form-data file')
+                raise Exception("invalid multipart/form-data file")
 
             form.append([field_name, [file_name, content]])
         elif field_metadata.get("json") is True:
-            to_append = [field_metadata.get("field_name", field.name), [
-                None, marshal_json(val, field.type), "application/json"]]
+            to_append = [
+                field_metadata.get("field_name", field.name),
+                [None, marshal_json(val, field.type), "application/json"],
+            ]
             form.append(to_append)
         else:
-            field_name = field_metadata.get(
-                "field_name", field.name)
+            field_name = field_metadata.get("field_name", field.name)
             if isinstance(val, List):
                 for value in val:
                     if value is None:
                         continue
-                    form.append(
-                        [field_name + "[]", [None, _val_to_string(value)]])
+                    form.append([field_name + "[]", [None, _val_to_string(value)]])
             else:
                 form.append([field_name, [None, _val_to_string(val)]])
     return media_type, None, form
 
 
-def serialize_dict(original: Dict, explode: bool, field_name, existing: Optional[Dict[str, List[str]]]) -> Dict[
-        str, List[str]]:
+def serialize_dict(
+    original: Dict, explode: bool, field_name, existing: Optional[Dict[str, List[str]]]
+) -> Dict[str, List[str]]:
     if existing is None:
-        existing = []
+        existing = {}
 
     if explode is True:
         for key, val in original.items():
             if key not in existing:
                 existing[key] = []
             existing[key].append(val)
     else:
@@ -516,224 +640,227 @@
             temp.append(str(val))
         if field_name not in existing:
             existing[field_name] = []
         existing[field_name].append(",".join(temp))
     return existing
 
 
-def serialize_form_data(field_name: str, data: dataclass) -> Dict[str, any]:
+def serialize_form_data(field_name: str, data: Any) -> Dict[str, Any]:
     form: Dict[str, List[str]] = {}
 
     if is_dataclass(data):
         for field in fields(data):
             val = getattr(data, field.name)
             if val is None:
                 continue
 
-            metadata = field.metadata.get('form')
+            metadata = field.metadata.get("form")
             if metadata is None:
                 continue
 
-            field_name = metadata.get('field_name', field.name)
+            field_name = metadata.get("field_name", field.name)
 
-            if metadata.get('json'):
+            if metadata.get("json"):
                 form[field_name] = [marshal_json(val, field.type)]
             else:
-                if metadata.get('style', 'form') == 'form':
-                    form = {**form, **_populate_form(
-                        field_name, metadata.get('explode', True), val, _get_form_field_name, ",")}
+                if metadata.get("style", "form") == "form":
+                    _populate_form(
+                        field_name,
+                        metadata.get("explode", True),
+                        val,
+                        _get_form_field_name,
+                        ",",
+                        form,
+                    )
                 else:
-                    raise Exception(
-                        f'Invalid form style for field {field.name}')
+                    raise Exception(f"Invalid form style for field {field.name}")
     elif isinstance(data, Dict):
         for key, value in data.items():
             form[key] = [_val_to_string(value)]
     else:
-        raise Exception(f'Invalid request body type for field {field_name}')
+        raise Exception(f"Invalid request body type for field {field_name}")
 
     return form
 
 
 def _get_form_field_name(obj_field: Field) -> str:
-    obj_param_metadata = obj_field.metadata.get('form')
+    obj_param_metadata = obj_field.metadata.get("form")
 
     if not obj_param_metadata:
         return ""
 
     return obj_param_metadata.get("field_name", obj_field.name)
 
 
-def _populate_form(field_name: str, explode: boolean, obj: any, get_field_name_func: Callable, delimiter: str) -> \
-        Dict[str, List[str]]:
-    params: Dict[str, List[str]] = {}
-
+def _populate_form(
+    field_name: str,
+    explode: boolean,
+    obj: Any,
+    get_field_name_func: Callable,
+    delimiter: str,
+    form: Dict[str, List[str]],
+):
     if obj is None:
-        return params
+        return form
 
     if is_dataclass(obj):
         items = []
 
         obj_fields: Tuple[Field, ...] = fields(obj)
         for obj_field in obj_fields:
             obj_field_name = get_field_name_func(obj_field)
-            if obj_field_name == '':
+            if obj_field_name == "":
                 continue
 
             val = getattr(obj, obj_field.name)
             if val is None:
                 continue
 
             if explode:
-                params[obj_field_name] = [_val_to_string(val)]
+                form[obj_field_name] = [_val_to_string(val)]
             else:
-                items.append(
-                    f'{obj_field_name}{delimiter}{_val_to_string(val)}')
+                items.append(f"{obj_field_name}{delimiter}{_val_to_string(val)}")
 
         if len(items) > 0:
-            params[field_name] = [delimiter.join(items)]
+            form[field_name] = [delimiter.join(items)]
     elif isinstance(obj, Dict):
         items = []
         for key, value in obj.items():
             if value is None:
                 continue
 
             if explode:
-                params[key] = _val_to_string(value)
+                form[key] = [_val_to_string(value)]
             else:
-                items.append(f'{key}{delimiter}{_val_to_string(value)}')
+                items.append(f"{key}{delimiter}{_val_to_string(value)}")
 
         if len(items) > 0:
-            params[field_name] = [delimiter.join(items)]
+            form[field_name] = [delimiter.join(items)]
     elif isinstance(obj, List):
         items = []
 
         for value in obj:
             if value is None:
                 continue
 
             if explode:
-                if not field_name in params:
-                    params[field_name] = []
-                params[field_name].append(_val_to_string(value))
+                if not field_name in form:
+                    form[field_name] = []
+                form[field_name].append(_val_to_string(value))
             else:
                 items.append(_val_to_string(value))
 
         if len(items) > 0:
-            params[field_name] = [delimiter.join(
-                [str(item) for item in items])]
+            form[field_name] = [delimiter.join([str(item) for item in items])]
     else:
-        params[field_name] = [_val_to_string(obj)]
+        form[field_name] = [_val_to_string(obj)]
 
-    return params
+    return form
 
 
-def _serialize_header(explode: bool, obj: any) -> str:
+def _serialize_header(explode: bool, obj: Any) -> str:
     if obj is None:
-        return ''
+        return ""
 
     if is_dataclass(obj):
         items = []
         obj_fields: Tuple[Field, ...] = fields(obj)
         for obj_field in obj_fields:
-            obj_param_metadata = obj_field.metadata.get('header')
+            obj_param_metadata = obj_field.metadata.get("header")
 
             if not obj_param_metadata:
                 continue
 
-            obj_field_name = obj_param_metadata.get(
-                'field_name', obj_field.name)
-            if obj_field_name == '':
+            obj_field_name = obj_param_metadata.get("field_name", obj_field.name)
+            if obj_field_name == "":
                 continue
 
             val = getattr(obj, obj_field.name)
             if val is None:
                 continue
 
             if explode:
-                items.append(
-                    f'{obj_field_name}={_val_to_string(val)}')
+                items.append(f"{obj_field_name}={_val_to_string(val)}")
             else:
                 items.append(obj_field_name)
                 items.append(_val_to_string(val))
 
         if len(items) > 0:
-            return ','.join(items)
+            return ",".join(items)
     elif isinstance(obj, Dict):
         items = []
 
         for key, value in obj.items():
             if value is None:
                 continue
 
             if explode:
-                items.append(f'{key}={_val_to_string(value)}')
+                items.append(f"{key}={_val_to_string(value)}")
             else:
                 items.append(key)
                 items.append(_val_to_string(value))
 
         if len(items) > 0:
-            return ','.join([str(item) for item in items])
+            return ",".join([str(item) for item in items])
     elif isinstance(obj, List):
         items = []
 
         for value in obj:
             if value is None:
                 continue
 
             items.append(_val_to_string(value))
 
         if len(items) > 0:
-            return ','.join(items)
+            return ",".join(items)
     else:
-        return f'{_val_to_string(obj)}'
+        return f"{_val_to_string(obj)}"
 
-    return ''
+    return ""
 
 
 def unmarshal_json(data, typ, decoder=None):
-    unmarshal = make_dataclass('Unmarshal', [('res', typ)],
-                               bases=(DataClassJsonMixin,))
+    unmarshal = make_dataclass("Unmarshal", [("res", typ)], bases=(DataClassJsonMixin,))
     json_dict = json.loads(data)
     try:
         out = unmarshal.from_dict({"res": json_dict})
     except AttributeError as attr_err:
         raise AttributeError(
-            f'unable to unmarshal {data} as {typ} - {attr_err}') from attr_err
+            f"unable to unmarshal {data} as {typ} - {attr_err}"
+        ) from attr_err
 
     return out.res if decoder is None else decoder(out.res)
 
 
 def marshal_json(val, typ, encoder=None):
     if not is_optional_type(typ) and val is None:
-        raise ValueError(
-            f"Could not marshal None into non-optional type: {typ}")
+        raise ValueError(f"Could not marshal None into non-optional type: {typ}")
 
-    marshal = make_dataclass('Marshal', [('res', typ)],
-                             bases=(DataClassJsonMixin,))
+    marshal = make_dataclass("Marshal", [("res", typ)], bases=(DataClassJsonMixin,))
     marshaller = marshal(res=val)
     json_dict = marshaller.to_dict()
     val = json_dict["res"] if encoder is None else encoder(json_dict["res"])
 
-    return json.dumps(val, separators=(',', ':'), sort_keys=True)
+    return json.dumps(val, separators=(",", ":"), sort_keys=True)
 
 
 def match_content_type(content_type: str, pattern: str) -> boolean:
     if pattern in (content_type, "*", "*/*"):
         return True
 
     msg = Message()
-    msg['content-type'] = content_type
+    msg["content-type"] = content_type
     media_type = msg.get_content_type()
 
     if media_type == pattern:
         return True
 
     parts = media_type.split("/")
     if len(parts) == 2:
-        if pattern in (f'{parts[0]}/*', f'*/{parts[1]}'):
+        if pattern in (f"{parts[0]}/*", f"*/{parts[1]}"):
             return True
 
     return False
 
 
 def match_status_codes(status_codes: List[str], status_code: int) -> bool:
     for code in status_codes:
@@ -846,68 +973,88 @@
 
         return decoded
 
     return list_decode
 
 
 def union_encoder(all_encoders: Dict[str, Callable]):
-    def selective_encoder(val: any):
+    def selective_encoder(val: Any):
         if type(val) in all_encoders:
             return all_encoders[type(val)](val)
         return val
+
     return selective_encoder
 
 
 def union_decoder(all_decoders: List[Callable]):
-    def selective_decoder(val: any):
+    def selective_decoder(val: Any):
         decoded = val
         for decoder in all_decoders:
             try:
                 decoded = decoder(val)
                 break
             except (TypeError, ValueError):
                 continue
         return decoded
+
     return selective_decoder
 
 
 def get_field_name(name):
     def override(_, _field_name=name):
         return _field_name
 
     return override
 
 
-def _val_to_string(val):
+def _val_to_string(val) -> str:
     if isinstance(val, bool):
         return str(val).lower()
     if isinstance(val, datetime):
-        return val.isoformat().replace('+00:00', 'Z')
+        return str(val.isoformat().replace("+00:00", "Z"))
     if isinstance(val, Enum):
         return str(val.value)
 
     return str(val)
 
 
-def _populate_from_globals(param_name: str, value: any, param_type: str, gbls: Dict[str, Dict[str, Dict[str, Any]]]):
-    if value is None and gbls is not None:
-        if 'parameters' in gbls:
-            if param_type in gbls['parameters']:
-                if param_name in gbls['parameters'][param_type]:
-                    global_value = gbls['parameters'][param_type][param_name]
-                    if global_value is not None:
-                        value = global_value
+def _populate_from_globals(
+    param_name: str, value: Any, param_type: str, gbls: Any
+) -> Tuple[Any, bool]:
+    if gbls is None:
+        return value, False
+
+    global_fields = fields(gbls)
+
+    found = False
+    for field in global_fields:
+        if field.name is not param_name:
+            continue
+
+        found = True
+
+        if value is not None:
+            return value, True
+
+        global_value = getattr(gbls, field.name)
+
+        param_metadata = field.metadata.get(param_type)
+        if param_metadata is None:
+            return value, True
+
+        return global_value, True
 
-    return value
+    return value, found
 
 
 def decoder_with_discriminator(field_name):
     def decode_fx(obj):
-        kls = getattr(sys.modules['sdk.models.shared'], obj[field_name])
+        kls = getattr(sys.modules["sdk.models.shared"], obj[field_name])
         return unmarshal_json(json.dumps(obj), kls)
+
     return decode_fx
 
 
 def remove_suffix(input_string, suffix):
     if suffix and input_string.endswith(suffix):
-        return input_string[:-len(suffix)]
+        return input_string[: -len(suffix)]
     return input_string
```

### Comparing `codat-platform-3.4.0/src/codatplatform/webhooks.py` & `codat-platform-3.5.0/src/codatplatform/connections.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,506 +1,512 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from codatplatform import utils
-from codatplatform._hooks import HookContext
+from codatplatform._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from codatplatform.models import errors, operations, shared
 from typing import Optional
 
-class Webhooks:
-    r"""Manage webhooks, rules, and events."""
+class Connections:
+    r"""Create new and manage existing data connections for a company."""
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
-    def create(self, request: Optional[shared.CreateRule], retries: Optional[utils.RetryConfig] = None) -> operations.CreateRuleResponse:
-        r"""Create webhook
-        Create a new webhook configuration
+    def create(self, request: operations.CreateConnectionRequest, retries: Optional[utils.RetryConfig] = None) -> operations.CreateConnectionResponse:
+        r"""Create connection
+        Creates a connection for the company by providing a valid `platformKey`. 
 
-        Deprecated method: This will be removed in a future release, please migrate away from it as soon as possible.
+        Use the [List Integrations](https://docs.codat.io/platform-api#/operations/list-integrations) endpoint to access valid platform keys.
         """
-        hook_ctx = HookContext(operation_id='create-rule', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        hook_ctx = HookContext(operation_id='create-connection', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/rules'
-        headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, Optional[shared.CreateRule], "request", False, True, 'json')
-        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
-            headers['content-type'] = req_content_type
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = self.sdk_configuration.user_agent
+        url = utils.generate_url(base_url, '/companies/{companyId}/connections', request)
         
         if callable(self.sdk_configuration.security):
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security())
+            headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security)
+            headers, query_params = utils.get_security(self.sdk_configuration.security)
         
+        req_content_type, data, form = utils.serialize_request_body(request, operations.CreateConnectionRequest, "request_body", False, True, 'json')
+        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
+        headers['Accept'] = 'application/json'
+        headers['user-agent'] = self.sdk_configuration.user_agent
+        client = self.sdk_configuration.client
         
         global_retry_config = self.sdk_configuration.retry_config
         retry_config = retries
         if retry_config is None:
             if global_retry_config:
                 retry_config = global_retry_config
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
+        req = None
         def do_request():
+            nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('POST', url, data=data, files=form, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
-            if utils.match_status_codes(['401','402','403','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+            if utils.match_status_codes(['401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
-        content_type = http_res.headers.get('Content-Type')
         
-        res = operations.CreateRuleResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.CreateConnectionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[shared.Webhook])
-                res.webhook = out
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Connection])
+                res.connection = out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code in [401, 402, 403, 429, 500, 503]:
-            if utils.match_content_type(content_type, 'application/json'):
+        elif http_res.status_code in [401, 402, 403, 404, 429, 500, 503]:
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
-                out.raw_response = http_res
                 raise out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+        else:
+            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def create_consumer(self, request: Optional[shared.WebhookConsumerPrototype], retries: Optional[utils.RetryConfig] = None) -> operations.CreateWebhookConsumerResponse:
-        r"""Create webhook consumer
-        Use the *Create webhook consumer* endpoint to create a new webhook consumer that will listen to messages we send you.
-
-        [Webhook consumer](https://docs.codat.io/platform-api#/schemas/WebhookConsumer) is an HTTP endpoint that you configure to subscribe to specific events. See our documentation for more details on [Codat's webhook service](https://docs.codat.io/using-the-api/webhooks/overview).
+    def delete(self, request: operations.DeleteConnectionRequest, retries: Optional[utils.RetryConfig] = None) -> operations.DeleteConnectionResponse:
+        r"""Delete connection
+        Revoke and remove a connection from a company.
+        This operation is not reversible. The end user would need to reauthorize a new data connection if you wish to view new data for this company.
         """
-        hook_ctx = HookContext(operation_id='create-webhook-consumer', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        hook_ctx = HookContext(operation_id='delete-connection', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/webhooks'
-        headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, Optional[shared.WebhookConsumerPrototype], "request", False, True, 'json')
-        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
-            headers['content-type'] = req_content_type
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = self.sdk_configuration.user_agent
+        url = utils.generate_url(base_url, '/companies/{companyId}/connections/{connectionId}', request)
         
         if callable(self.sdk_configuration.security):
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security())
+            headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security)
+            headers, query_params = utils.get_security(self.sdk_configuration.security)
         
+        headers['Accept'] = 'application/json'
+        headers['user-agent'] = self.sdk_configuration.user_agent
+        client = self.sdk_configuration.client
         
         global_retry_config = self.sdk_configuration.retry_config
         retry_config = retries
         if retry_config is None:
             if global_retry_config:
                 retry_config = global_retry_config
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
+        req = None
         def do_request():
+            nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('POST', url, data=data, files=form, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('DELETE', url, params=query_params, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
-            if utils.match_status_codes(['401','402','403','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+            if utils.match_status_codes(['401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
-        content_type = http_res.headers.get('Content-Type')
         
-        res = operations.CreateWebhookConsumerResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.DeleteConnectionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
-        if http_res.status_code == 201:
-            if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[shared.WebhookConsumer])
-                res.webhook_consumer = out
-            else:
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code in [401, 402, 403, 429, 500, 503]:
-            if utils.match_content_type(content_type, 'application/json'):
+        if http_res.status_code == 200:
+            pass
+        elif http_res.status_code in [401, 402, 403, 404, 429, 500, 503]:
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
-                out.raw_response = http_res
                 raise out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+        else:
+            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def delete_consumer(self, request: operations.DeleteWebhookConsumerRequest, retries: Optional[utils.RetryConfig] = None) -> operations.DeleteWebhookConsumerResponse:
-        r"""Delete webhook consumer
-        Use the *Delete webhook consumer* endpoint to delete an existing webhoook consumer, providing its valid `id` as a parameter.
-
-        [Webhook consumer](https://docs.codat.io/platform-api#/schemas/WebhookConsumer) is an HTTP endpoint that you configure to subscribe to specific events. See our documentation for more details on [Codat's webhook service](https://docs.codat.io/using-the-api/webhooks/overview).
+    def get(self, request: operations.GetConnectionRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetConnectionResponse:
+        r"""Get connection
+        Returns a specific connection for a company when valid identifiers are provided. If the identifiers are for a deleted company and/or connection, a not found response is returned.
         """
-        hook_ctx = HookContext(operation_id='delete-webhook-consumer', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        hook_ctx = HookContext(operation_id='get-connection', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.DeleteWebhookConsumerRequest, base_url, '/webhooks/{webhookId}', request)
-        headers = {}
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = self.sdk_configuration.user_agent
+        url = utils.generate_url(base_url, '/companies/{companyId}/connections/{connectionId}', request)
         
         if callable(self.sdk_configuration.security):
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security())
+            headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security)
+            headers, query_params = utils.get_security(self.sdk_configuration.security)
         
+        headers['Accept'] = 'application/json'
+        headers['user-agent'] = self.sdk_configuration.user_agent
+        client = self.sdk_configuration.client
         
         global_retry_config = self.sdk_configuration.retry_config
         retry_config = retries
         if retry_config is None:
             if global_retry_config:
                 retry_config = global_retry_config
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
+        req = None
         def do_request():
+            nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('DELETE', url, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
             if utils.match_status_codes(['401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
-        content_type = http_res.headers.get('Content-Type')
         
-        res = operations.DeleteWebhookConsumerResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetConnectionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
-        if http_res.status_code == 204:
-            pass
+        if http_res.status_code == 200:
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Connection])
+                res.connection = out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [401, 402, 403, 404, 429, 500, 503]:
-            if utils.match_content_type(content_type, 'application/json'):
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
-                out.raw_response = http_res
                 raise out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+        else:
+            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def get(self, request: operations.GetWebhookRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetWebhookResponse:
-        r"""Get webhook
-        Get a single webhook
-
-        Deprecated method: This will be removed in a future release, please migrate away from it as soon as possible.
+    def list(self, request: operations.ListConnectionsRequest, retries: Optional[utils.RetryConfig] = None) -> operations.ListConnectionsResponse:
+        r"""List connections
+        List the connections for a company.
         """
-        hook_ctx = HookContext(operation_id='get-webhook', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        hook_ctx = HookContext(operation_id='list-connections', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetWebhookRequest, base_url, '/rules/{ruleId}', request)
-        headers = {}
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = self.sdk_configuration.user_agent
+        url = utils.generate_url(base_url, '/companies/{companyId}/connections', request)
         
         if callable(self.sdk_configuration.security):
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security())
+            headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security)
+            headers, query_params = utils.get_security(self.sdk_configuration.security)
         
+        query_params = { **utils.get_query_params(request), **query_params }
+        headers['Accept'] = 'application/json'
+        headers['user-agent'] = self.sdk_configuration.user_agent
+        client = self.sdk_configuration.client
         
         global_retry_config = self.sdk_configuration.retry_config
         retry_config = retries
         if retry_config is None:
             if global_retry_config:
                 retry_config = global_retry_config
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
+        req = None
         def do_request():
+            nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('GET', url, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
-            if utils.match_status_codes(['401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+            if utils.match_status_codes(['400','401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
-        content_type = http_res.headers.get('Content-Type')
         
-        res = operations.GetWebhookResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.ListConnectionsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[shared.Webhook])
-                res.webhook = out
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Connections])
+                res.connections = out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code in [401, 402, 403, 404, 429, 500, 503]:
-            if utils.match_content_type(content_type, 'application/json'):
+        elif http_res.status_code in [400, 401, 402, 403, 404, 429, 500, 503]:
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
-                out.raw_response = http_res
                 raise out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+        else:
+            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def list(self, request: operations.ListRulesRequest, retries: Optional[utils.RetryConfig] = None) -> operations.ListRulesResponse:
-        r"""List webhooks
-        List webhooks that you are subscribed to.
-
-        Deprecated method: This will be removed in a future release, please migrate away from it as soon as possible.
+    def unlink(self, request: operations.UnlinkConnectionRequest, retries: Optional[utils.RetryConfig] = None) -> operations.UnlinkConnectionResponse:
+        r"""Unlink connection
+        This allows you to deauthorize a connection, without deleting it from Codat. This means you can still view any data that has previously been pulled into Codat, and also lets you re-authorize in future if your customer wishes to resume sharing their data.
         """
-        hook_ctx = HookContext(operation_id='list-rules', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        hook_ctx = HookContext(operation_id='unlink-connection', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/rules'
-        headers = {}
-        query_params = utils.get_query_params(operations.ListRulesRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = self.sdk_configuration.user_agent
+        url = utils.generate_url(base_url, '/companies/{companyId}/connections/{connectionId}', request)
         
         if callable(self.sdk_configuration.security):
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security())
+            headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security)
+            headers, query_params = utils.get_security(self.sdk_configuration.security)
         
+        req_content_type, data, form = utils.serialize_request_body(request, operations.UnlinkConnectionRequest, "update_connection_status", False, True, 'json')
+        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
+        headers['Accept'] = 'application/json'
+        headers['user-agent'] = self.sdk_configuration.user_agent
+        client = self.sdk_configuration.client
         
         global_retry_config = self.sdk_configuration.retry_config
         retry_config = retries
         if retry_config is None:
             if global_retry_config:
                 retry_config = global_retry_config
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
+        req = None
         def do_request():
+            nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('PATCH', url, params=query_params, data=data, files=form, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
-            if utils.match_status_codes(['400','401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+            if utils.match_status_codes(['401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
-        content_type = http_res.headers.get('Content-Type')
         
-        res = operations.ListRulesResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.UnlinkConnectionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[shared.Webhooks])
-                res.webhooks = out
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Connection])
+                res.connection = out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code in [400, 401, 402, 403, 404, 429, 500, 503]:
-            if utils.match_content_type(content_type, 'application/json'):
+        elif http_res.status_code in [401, 402, 403, 404, 429, 500, 503]:
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
-                out.raw_response = http_res
                 raise out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+        else:
+            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def list_consumers(self, retries: Optional[utils.RetryConfig] = None) -> operations.ListWebhookConsumersResponse:
-        r"""List webhook consumers
-        Use the *List webhook consumers* endpoint to return a list of all webhook consumers that currently exist for your client.
-
-        [Webhook consumer](https://docs.codat.io/platform-api#/schemas/WebhookConsumer) is an HTTP endpoint that you configure to subscribe to specific events. See our documentation for more details on [Codat's webhook service](https://docs.codat.io/using-the-api/webhooks/overview).
+    def update_authorization(self, request: operations.UpdateConnectionAuthorizationRequest, retries: Optional[utils.RetryConfig] = None) -> operations.UpdateConnectionAuthorizationResponse:
+        r"""Update authorization
+        Update data connection's authorization.
         """
-        hook_ctx = HookContext(operation_id='list-webhook-consumers', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        hook_ctx = HookContext(operation_id='update-connection-authorization', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/webhooks'
-        headers = {}
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = self.sdk_configuration.user_agent
+        url = utils.generate_url(base_url, '/companies/{companyId}/connections/{connectionId}/authorization', request)
         
         if callable(self.sdk_configuration.security):
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security())
+            headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security)
+            headers, query_params = utils.get_security(self.sdk_configuration.security)
         
+        req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateConnectionAuthorizationRequest, "request_body", False, True, 'json')
+        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
+        headers['Accept'] = 'application/json'
+        headers['user-agent'] = self.sdk_configuration.user_agent
+        client = self.sdk_configuration.client
         
         global_retry_config = self.sdk_configuration.retry_config
         retry_config = retries
         if retry_config is None:
             if global_retry_config:
                 retry_config = global_retry_config
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
+        req = None
         def do_request():
+            nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('GET', url, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('PUT', url, params=query_params, data=data, files=form, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
-            if utils.match_status_codes(['400','401','402','403','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+            if utils.match_status_codes(['401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
-        content_type = http_res.headers.get('Content-Type')
         
-        res = operations.ListWebhookConsumersResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.UpdateConnectionAuthorizationResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[shared.WebhookConsumers])
-                res.webhook_consumers = out
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Connection])
+                res.connection = out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code in [400, 401, 402, 403, 429, 500, 503]:
-            if utils.match_content_type(content_type, 'application/json'):
+        elif http_res.status_code in [401, 402, 403, 404, 429, 500, 503]:
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
-                out.raw_response = http_res
                 raise out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+        else:
+            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
-    
+    
+
```

