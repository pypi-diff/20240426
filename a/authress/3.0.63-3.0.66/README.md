# Comparing `tmp/authress-3.0.63.tar.gz` & `tmp/authress-3.0.66.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "authress-3.0.63.tar", last modified: Tue Mar  5 09:55:54 2024, max compression
+gzip compressed data, was "authress-3.0.66.tar", last modified: Fri Apr 26 10:02:51 2024, max compression
```

## Comparing `authress-3.0.63.tar` & `authress-3.0.66.tar`

### file list

```diff
@@ -1,187 +1,187 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 09:55:54.594892 authress-3.0.63/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-05 09:55:32.000000 authress-3.0.63/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-03-05 09:55:54.594892 authress-3.0.63/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-03-05 09:55:32.000000 authress-3.0.63/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 09:55:54.570892 authress-3.0.63/authress/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-05 09:55:33.000000 authress-3.0.63/authress/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)     6596 2024-03-05 09:55:32.000000 authress-3.0.63/authress/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 09:55:54.574892 authress-3.0.63/authress/api/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-03-05 09:55:32.000000 authress-3.0.63/authress/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    78077 2024-03-05 09:55:32.000000 authress-3.0.63/authress/api/access_records_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    26872 2024-03-05 09:55:32.000000 authress-3.0.63/authress/api/accounts_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     9116 2024-03-05 09:55:32.000000 authress-3.0.63/authress/api/applications_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    40628 2024-03-05 09:55:32.000000 authress-3.0.63/authress/api/connections_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    54954 2024-03-05 09:55:32.000000 authress-3.0.63/authress/api/extensions_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    36052 2024-03-05 09:55:32.000000 authress-3.0.63/authress/api/groups_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    27251 2024-03-05 09:55:32.000000 authress-3.0.63/authress/api/invites_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    30337 2024-03-05 09:55:32.000000 authress-3.0.63/authress/api/resource_permissions_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    32205 2024-03-05 09:55:32.000000 authress-3.0.63/authress/api/roles_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-03-05 09:55:32.000000 authress-3.0.63/authress/api/service_client_token_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    47502 2024-03-05 09:55:32.000000 authress-3.0.63/authress/api/service_clients_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    32499 2024-03-05 09:55:32.000000 authress-3.0.63/authress/api/tenants_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-03-05 09:55:32.000000 authress-3.0.63/authress/api/token_verifier.py
--rw-r--r--   0 runner    (1001) docker     (127)    37628 2024-03-05 09:55:32.000000 authress-3.0.63/authress/api/user_permissions_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    23156 2024-03-05 09:55:32.000000 authress-3.0.63/authress/api/users_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-03-05 09:55:32.000000 authress-3.0.63/authress/api_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-03-05 09:55:32.000000 authress-3.0.63/authress/authress_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6002 2024-03-05 09:55:32.000000 authress-3.0.63/authress/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    30455 2024-03-05 09:55:32.000000 authress-3.0.63/authress/http_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 09:55:54.582892 authress-3.0.63/authress/models/
--rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-03-05 09:55:32.000000 authress-3.0.63/authress/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9112 2024-03-05 09:55:32.000000 authress-3.0.63/authress/models/access_record.py
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-03-05 09:55:32.000000 authress-3.0.63/authress/models/access_record_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-03-05 09:55:32.000000 authress-3.0.63/authress/models/access_record_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     5063 2024-03-05 09:55:32.000000 authress-3.0.63/authress/models/access_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-03-05 09:55:32.000000 authress-3.0.63/authress/models/access_request_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-03-05 09:55:32.000000 authress-3.0.63/authress/models/access_request_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3721 2024-03-05 09:55:32.000000 authress-3.0.63/authress/models/access_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-03-05 09:55:32.000000 authress-3.0.63/authress/models/account.py
--rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-03-05 09:55:32.000000 authress-3.0.63/authress/models/account_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-03-05 09:55:32.000000 authress-3.0.63/authress/models/account_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-03-05 09:55:32.000000 authress-3.0.63/authress/models/application_delegation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-03-05 09:55:32.000000 authress-3.0.63/authress/models/claim_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4840 2024-03-05 09:55:32.000000 authress-3.0.63/authress/models/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-03-05 09:55:32.000000 authress-3.0.63/authress/models/client_access_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-03-05 09:55:32.000000 authress-3.0.63/authress/models/client_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-03-05 09:55:32.000000 authress-3.0.63/authress/models/client_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-03-05 09:55:32.000000 authress-3.0.63/authress/models/collection_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     8169 2024-03-05 09:55:32.000000 authress-3.0.63/authress/models/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-03-05 09:55:32.000000 authress-3.0.63/authress/models/connection_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-03-05 09:55:32.000000 authress-3.0.63/authress/models/connection_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-03-05 09:55:32.000000 authress-3.0.63/authress/models/connection_default_connection_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-03-05 09:55:32.000000 authress-3.0.63/authress/models/extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-03-05 09:55:32.000000 authress-3.0.63/authress/models/extension_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-03-05 09:55:32.000000 authress-3.0.63/authress/models/extension_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-03-05 09:55:32.000000 authress-3.0.63/authress/models/extension_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-03-05 09:55:32.000000 authress-3.0.63/authress/models/group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-03-05 09:55:32.000000 authress-3.0.63/authress/models/group_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-03-05 09:55:32.000000 authress-3.0.63/authress/models/identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-03-05 09:55:32.000000 authress-3.0.63/authress/models/identity_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-03-05 09:55:32.000000 authress-3.0.63/authress/models/identity_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4233 2024-03-05 09:55:32.000000 authress-3.0.63/authress/models/invite.py
--rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-03-05 09:55:32.000000 authress-3.0.63/authress/models/link.py
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-03-05 09:55:32.000000 authress-3.0.63/authress/models/linked_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-03-05 09:55:32.000000 authress-3.0.63/authress/models/links.py
--rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-03-05 09:55:32.000000 authress-3.0.63/authress/models/metadata_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-03-05 09:55:32.000000 authress-3.0.63/authress/models/metadata_object_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-03-05 09:55:32.000000 authress-3.0.63/authress/models/o_auth_authorize_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-03-05 09:55:32.000000 authress-3.0.63/authress/models/o_auth_token_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-03-05 09:55:32.000000 authress-3.0.63/authress/models/o_auth_token_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-03-05 09:55:32.000000 authress-3.0.63/authress/models/pagination.py
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-03-05 09:55:32.000000 authress-3.0.63/authress/models/pagination_next.py
--rw-r--r--   0 runner    (1001) docker     (127)     3940 2024-03-05 09:55:32.000000 authress-3.0.63/authress/models/permission_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-03-05 09:55:32.000000 authress-3.0.63/authress/models/permission_collection_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     3862 2024-03-05 09:55:32.000000 authress-3.0.63/authress/models/permission_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-03-05 09:55:32.000000 authress-3.0.63/authress/models/permissioned_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     4023 2024-03-05 09:55:32.000000 authress-3.0.63/authress/models/permissioned_resource_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-03-05 09:55:32.000000 authress-3.0.63/authress/models/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-03-05 09:55:32.000000 authress-3.0.63/authress/models/resource_permission.py
--rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-03-05 09:55:32.000000 authress-3.0.63/authress/models/resource_users_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4302 2024-03-05 09:55:32.000000 authress-3.0.63/authress/models/role.py
--rw-r--r--   0 runner    (1001) docker     (127)     3802 2024-03-05 09:55:32.000000 authress-3.0.63/authress/models/role_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-03-05 09:55:32.000000 authress-3.0.63/authress/models/statement.py
--rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-03-05 09:55:32.000000 authress-3.0.63/authress/models/tenant.py
--rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-03-05 09:55:32.000000 authress-3.0.63/authress/models/tenant_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-03-05 09:55:32.000000 authress-3.0.63/authress/models/tenant_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-03-05 09:55:32.000000 authress-3.0.63/authress/models/tenant_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-03-05 09:55:32.000000 authress-3.0.63/authress/models/token_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-03-05 09:55:32.000000 authress-3.0.63/authress/models/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-03-05 09:55:32.000000 authress-3.0.63/authress/models/user_connection_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-03-05 09:55:32.000000 authress-3.0.63/authress/models/user_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-03-05 09:55:32.000000 authress-3.0.63/authress/models/user_identity_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-03-05 09:55:32.000000 authress-3.0.63/authress/models/user_resources_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-03-05 09:55:32.000000 authress-3.0.63/authress/models/user_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-03-05 09:55:32.000000 authress-3.0.63/authress/models/user_role_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-03-05 09:55:32.000000 authress-3.0.63/authress/models/user_token.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 09:55:32.000000 authress-3.0.63/authress/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    12268 2024-03-05 09:55:32.000000 authress-3.0.63/authress/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 09:55:54.594892 authress-3.0.63/authress.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-03-05 09:55:54.000000 authress-3.0.63/authress.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5665 2024-03-05 09:55:54.000000 authress-3.0.63/authress.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-05 09:55:54.000000 authress-3.0.63/authress.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-05 09:55:54.000000 authress-3.0.63/authress.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-05 09:55:54.000000 authress-3.0.63/authress.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-03-05 09:55:32.000000 authress-3.0.63/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-05 09:55:54.594892 authress-3.0.63/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-03-05 09:55:32.000000 authress-3.0.63/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 09:55:54.594892 authress-3.0.63/test/
--rw-r--r--   0 runner    (1001) docker     (127)     5163 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_access_record.py
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_access_record_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     6953 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_access_record_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_access_records_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_access_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_access_request_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_access_request_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_access_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_account_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_account_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_accounts_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_application_delegation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_applications_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_claim_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_client_access_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     5113 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_client_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_client_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_collection_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4448 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_connection_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_connection_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_connection_default_connection_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_connections_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_extension_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_extension_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_extension_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_extensions_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_group_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_groups_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_identity_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_identity_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_invite.py
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_invites_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_link.py
--rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_linked_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_metadata_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_metadata_object_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_o_auth_authorize_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_o_auth_token_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_o_auth_token_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_pagination.py
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_pagination_next.py
--rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_permission_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_permission_collection_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_permission_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_permissioned_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     3943 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_permissioned_resource_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_resource_permission.py
--rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_resource_permissions_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_resource_users_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_role_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_roles_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_service_client_token_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_service_clients_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_statement.py
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_tenant.py
--rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_tenant_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_tenant_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_tenant_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_tenants_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_token_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_token_verifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_user_connection_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_user_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_user_identity_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_user_permissions_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_user_resources_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_user_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_user_role_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_user_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-03-05 09:55:32.000000 authress-3.0.63/test/test_users_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:02:51.727112 authress-3.0.66/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-26 10:02:31.000000 authress-3.0.66/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-04-26 10:02:51.727112 authress-3.0.66/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-04-26 10:02:31.000000 authress-3.0.66/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:02:51.699112 authress-3.0.66/authress/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-26 10:02:31.000000 authress-3.0.66/authress/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)     6596 2024-04-26 10:02:31.000000 authress-3.0.66/authress/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:02:51.703112 authress-3.0.66/authress/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-26 10:02:31.000000 authress-3.0.66/authress/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78077 2024-04-26 10:02:31.000000 authress-3.0.66/authress/api/access_records_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26872 2024-04-26 10:02:31.000000 authress-3.0.66/authress/api/accounts_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9116 2024-04-26 10:02:31.000000 authress-3.0.66/authress/api/applications_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40628 2024-04-26 10:02:31.000000 authress-3.0.66/authress/api/connections_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54954 2024-04-26 10:02:31.000000 authress-3.0.66/authress/api/extensions_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36052 2024-04-26 10:02:31.000000 authress-3.0.66/authress/api/groups_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27251 2024-04-26 10:02:31.000000 authress-3.0.66/authress/api/invites_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30337 2024-04-26 10:02:31.000000 authress-3.0.66/authress/api/resource_permissions_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32205 2024-04-26 10:02:31.000000 authress-3.0.66/authress/api/roles_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-04-26 10:02:31.000000 authress-3.0.66/authress/api/service_client_token_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47502 2024-04-26 10:02:31.000000 authress-3.0.66/authress/api/service_clients_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32499 2024-04-26 10:02:31.000000 authress-3.0.66/authress/api/tenants_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-04-26 10:02:31.000000 authress-3.0.66/authress/api/token_verifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37628 2024-04-26 10:02:31.000000 authress-3.0.66/authress/api/user_permissions_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23156 2024-04-26 10:02:31.000000 authress-3.0.66/authress/api/users_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-26 10:02:31.000000 authress-3.0.66/authress/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-04-26 10:02:31.000000 authress-3.0.66/authress/authress_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6002 2024-04-26 10:02:31.000000 authress-3.0.66/authress/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30455 2024-04-26 10:02:31.000000 authress-3.0.66/authress/http_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:02:51.715112 authress-3.0.66/authress/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-04-26 10:02:31.000000 authress-3.0.66/authress/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9112 2024-04-26 10:02:31.000000 authress-3.0.66/authress/models/access_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-04-26 10:02:31.000000 authress-3.0.66/authress/models/access_record_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-04-26 10:02:31.000000 authress-3.0.66/authress/models/access_record_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5063 2024-04-26 10:02:31.000000 authress-3.0.66/authress/models/access_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-04-26 10:02:31.000000 authress-3.0.66/authress/models/access_request_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-26 10:02:31.000000 authress-3.0.66/authress/models/access_request_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3721 2024-04-26 10:02:31.000000 authress-3.0.66/authress/models/access_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-04-26 10:02:31.000000 authress-3.0.66/authress/models/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-04-26 10:02:31.000000 authress-3.0.66/authress/models/account_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-04-26 10:02:31.000000 authress-3.0.66/authress/models/account_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-04-26 10:02:31.000000 authress-3.0.66/authress/models/application_delegation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-04-26 10:02:31.000000 authress-3.0.66/authress/models/claim_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4840 2024-04-26 10:02:31.000000 authress-3.0.66/authress/models/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-04-26 10:02:31.000000 authress-3.0.66/authress/models/client_access_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-04-26 10:02:31.000000 authress-3.0.66/authress/models/client_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-04-26 10:02:31.000000 authress-3.0.66/authress/models/client_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-04-26 10:02:31.000000 authress-3.0.66/authress/models/collection_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8169 2024-04-26 10:02:31.000000 authress-3.0.66/authress/models/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-04-26 10:02:31.000000 authress-3.0.66/authress/models/connection_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-04-26 10:02:31.000000 authress-3.0.66/authress/models/connection_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-04-26 10:02:31.000000 authress-3.0.66/authress/models/connection_default_connection_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-04-26 10:02:31.000000 authress-3.0.66/authress/models/extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-04-26 10:02:31.000000 authress-3.0.66/authress/models/extension_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-04-26 10:02:31.000000 authress-3.0.66/authress/models/extension_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-04-26 10:02:31.000000 authress-3.0.66/authress/models/extension_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-04-26 10:02:31.000000 authress-3.0.66/authress/models/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-04-26 10:02:31.000000 authress-3.0.66/authress/models/group_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-26 10:02:31.000000 authress-3.0.66/authress/models/identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-04-26 10:02:31.000000 authress-3.0.66/authress/models/identity_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-04-26 10:02:31.000000 authress-3.0.66/authress/models/identity_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4233 2024-04-26 10:02:31.000000 authress-3.0.66/authress/models/invite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-04-26 10:02:31.000000 authress-3.0.66/authress/models/link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-04-26 10:02:31.000000 authress-3.0.66/authress/models/linked_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-04-26 10:02:31.000000 authress-3.0.66/authress/models/links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-04-26 10:02:31.000000 authress-3.0.66/authress/models/metadata_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-04-26 10:02:31.000000 authress-3.0.66/authress/models/metadata_object_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-04-26 10:02:31.000000 authress-3.0.66/authress/models/o_auth_authorize_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-04-26 10:02:31.000000 authress-3.0.66/authress/models/o_auth_token_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-04-26 10:02:31.000000 authress-3.0.66/authress/models/o_auth_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-26 10:02:31.000000 authress-3.0.66/authress/models/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-04-26 10:02:31.000000 authress-3.0.66/authress/models/pagination_next.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3940 2024-04-26 10:02:31.000000 authress-3.0.66/authress/models/permission_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-26 10:02:31.000000 authress-3.0.66/authress/models/permission_collection_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3862 2024-04-26 10:02:31.000000 authress-3.0.66/authress/models/permission_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-04-26 10:02:31.000000 authress-3.0.66/authress/models/permissioned_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4023 2024-04-26 10:02:31.000000 authress-3.0.66/authress/models/permissioned_resource_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-04-26 10:02:31.000000 authress-3.0.66/authress/models/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-26 10:02:31.000000 authress-3.0.66/authress/models/resource_permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-04-26 10:02:31.000000 authress-3.0.66/authress/models/resource_users_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4302 2024-04-26 10:02:31.000000 authress-3.0.66/authress/models/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3802 2024-04-26 10:02:31.000000 authress-3.0.66/authress/models/role_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-04-26 10:02:31.000000 authress-3.0.66/authress/models/statement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-04-26 10:02:31.000000 authress-3.0.66/authress/models/tenant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-26 10:02:31.000000 authress-3.0.66/authress/models/tenant_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-04-26 10:02:31.000000 authress-3.0.66/authress/models/tenant_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-04-26 10:02:31.000000 authress-3.0.66/authress/models/tenant_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-04-26 10:02:31.000000 authress-3.0.66/authress/models/token_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-04-26 10:02:31.000000 authress-3.0.66/authress/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-04-26 10:02:31.000000 authress-3.0.66/authress/models/user_connection_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-04-26 10:02:31.000000 authress-3.0.66/authress/models/user_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-04-26 10:02:31.000000 authress-3.0.66/authress/models/user_identity_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-04-26 10:02:31.000000 authress-3.0.66/authress/models/user_resources_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-26 10:02:31.000000 authress-3.0.66/authress/models/user_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-04-26 10:02:31.000000 authress-3.0.66/authress/models/user_role_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-04-26 10:02:31.000000 authress-3.0.66/authress/models/user_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:02:31.000000 authress-3.0.66/authress/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    12268 2024-04-26 10:02:31.000000 authress-3.0.66/authress/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:02:51.727112 authress-3.0.66/authress.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-04-26 10:02:51.000000 authress-3.0.66/authress.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5665 2024-04-26 10:02:51.000000 authress-3.0.66/authress.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 10:02:51.000000 authress-3.0.66/authress.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-26 10:02:51.000000 authress-3.0.66/authress.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-26 10:02:51.000000 authress-3.0.66/authress.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-26 10:02:31.000000 authress-3.0.66/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-26 10:02:51.727112 authress-3.0.66/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-26 10:02:31.000000 authress-3.0.66/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:02:51.727112 authress-3.0.66/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     5163 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_access_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_access_record_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6953 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_access_record_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_access_records_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_access_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_access_request_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_access_request_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_access_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_account_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_account_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_accounts_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_application_delegation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_applications_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_claim_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_client_access_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5113 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_client_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_client_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_collection_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4448 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_connection_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_connection_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_connection_default_connection_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_connections_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_extension_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_extension_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_extension_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_extensions_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_group_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_groups_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_identity_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_identity_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_invite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_invites_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_linked_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_metadata_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_metadata_object_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_o_auth_authorize_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_o_auth_token_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_o_auth_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_pagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_pagination_next.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_permission_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_permission_collection_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_permission_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_permissioned_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3943 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_permissioned_resource_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_resource_permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_resource_permissions_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_resource_users_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_role_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_roles_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_service_client_token_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_service_clients_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_statement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_tenant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_tenant_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_tenant_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_tenant_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_tenants_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_token_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_token_verifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_user_connection_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_user_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_user_identity_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_user_permissions_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_user_resources_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_user_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_user_role_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_user_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-04-26 10:02:31.000000 authress-3.0.66/test/test_users_api.py
```

### Comparing `authress-3.0.63/LICENSE` & `authress-3.0.66/LICENSE`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/PKG-INFO` & `authress-3.0.66/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: authress
-Version: 3.0.63
+Version: 3.0.66
 Summary: Authress SDK for authorization as a service and interact with the Authress API.
 Home-page: https://github.com/Authress/authress-sdk.py.git
 Author: Authress Developers
 Author-email: developers@authress.io
 License: Apache-2.0
 Keywords: Authorization as a service,Security,authorization,authorization as a service,authentication,user authentication,Authress,Authress client,access management,access management as a service,user security,oso,polar,open source policy engine,embedded authorization,batteries included authorization,verified,verified access,verified permissions
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: authress Version: 3.0.63 Summary: Authress SDK for
+Metadata-Version: 2.1 Name: authress Version: 3.0.66 Summary: Authress SDK for
 authorization as a service and interact with the Authress API. Home-page:
 https://github.com/Authress/authress-sdk.py.git Author: Authress Developers
 Author-email: developers@authress.io License: Apache-2.0 Keywords:
 Authorization as a service,Security,authorization,authorization as a
 service,authentication,user authentication,Authress,Authress client,access
 management,access management as a service,user security,oso,polar,open source
 policy engine,embedded authorization,batteries included
```

### Comparing `authress-3.0.63/README.md` & `authress-3.0.66/README.md`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/__init__.py` & `authress-3.0.66/authress/__init__.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/api/__init__.py` & `authress-3.0.66/authress/api/__init__.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/api/access_records_api.py` & `authress-3.0.66/authress/api/access_records_api.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/api/accounts_api.py` & `authress-3.0.66/authress/api/accounts_api.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/api/applications_api.py` & `authress-3.0.66/authress/api/applications_api.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/api/connections_api.py` & `authress-3.0.66/authress/api/connections_api.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/api/extensions_api.py` & `authress-3.0.66/authress/api/extensions_api.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/api/groups_api.py` & `authress-3.0.66/authress/api/groups_api.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/api/invites_api.py` & `authress-3.0.66/authress/api/invites_api.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/api/resource_permissions_api.py` & `authress-3.0.66/authress/api/resource_permissions_api.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/api/roles_api.py` & `authress-3.0.66/authress/api/roles_api.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/api/service_client_token_provider.py` & `authress-3.0.66/authress/api/service_client_token_provider.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/api/service_clients_api.py` & `authress-3.0.66/authress/api/service_clients_api.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/api/tenants_api.py` & `authress-3.0.66/authress/api/tenants_api.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/api/token_verifier.py` & `authress-3.0.66/authress/api/token_verifier.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,25 +47,25 @@
       raise Exception("Unauthorized", "Issuer does not match")
 
     # Handle service client checking
     clientIdMatcher = re.match(r"^/v\d/clients/([^/]+)$", urlparse(issuer).path)
     if (clientIdMatcher is not None and clientIdMatcher.group(1) != unverifiedPayload['sub']):
       raise Exception("Unauthorized", "Service ID does not match token sub claim")
 
-    jwk = options['expectedPublicKey'] if options is not None and 'expectedPublicKey' in options else self.get_public_key(f"{issuer}/.well-known/openid-configuration/jwks", kid)
+    jwk = self.get_public_key(f"{issuer}/.well-known/openid-configuration/jwks", kid)
 
     try:
       return jwt.decode(authenticationToken, jwt.api_jwk.PyJWK.from_dict(jwk).key, algorithms=['EdDSA'], options = { 'verify_aud': False })
     except jwt.ExpiredSignatureError:
       raise Exception("Unauthorized", "Token is invalid")
 
   def get_public_key(self, jwkKeyListUrl, kid):
     hashKey = f"{jwkKeyListUrl}|{kid}"
 
-    if hashKey in self.keyMap is not None:
+    if hashKey in self.keyMap is None:
       self.keyMap[hashKey] = self.get_key_uncached(jwkKeyListUrl, kid)
 
     try:
       key = self.keyMap[hashKey]
       return key
     except:
       self.keyMap[hashKey] = self.get_key_uncached(jwkKeyListUrl, kid)
```

### Comparing `authress-3.0.63/authress/api/user_permissions_api.py` & `authress-3.0.66/authress/api/user_permissions_api.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/api/users_api.py` & `authress-3.0.66/authress/api/users_api.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/api_response.py` & `authress-3.0.66/authress/api_response.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/authress_client.py` & `authress-3.0.66/authress/authress_client.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/exceptions.py` & `authress-3.0.66/authress/exceptions.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/http_client.py` & `authress-3.0.66/authress/http_client.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/models/__init__.py` & `authress-3.0.66/authress/models/__init__.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/models/access_record.py` & `authress-3.0.66/authress/models/access_record.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/models/access_record_account.py` & `authress-3.0.66/authress/models/access_record_account.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/models/access_record_collection.py` & `authress-3.0.66/authress/models/access_record_collection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/models/access_request.py` & `authress-3.0.66/authress/models/access_request.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/models/access_request_collection.py` & `authress-3.0.66/authress/models/access_request_collection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/models/access_request_response.py` & `authress-3.0.66/authress/models/access_request_response.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/models/access_template.py` & `authress-3.0.66/authress/models/access_template.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/models/account.py` & `authress-3.0.66/authress/models/account.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/models/account_collection.py` & `authress-3.0.66/authress/models/account_collection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/models/account_links.py` & `authress-3.0.66/authress/models/account_links.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/models/application_delegation.py` & `authress-3.0.66/authress/models/application_delegation.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/models/claim_request.py` & `authress-3.0.66/authress/models/claim_request.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/models/client.py` & `authress-3.0.66/authress/models/client.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/models/client_access_key.py` & `authress-3.0.66/authress/models/client_access_key.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/models/client_collection.py` & `authress-3.0.66/authress/models/client_collection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/models/client_options.py` & `authress-3.0.66/authress/models/client_options.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/models/collection_links.py` & `authress-3.0.66/authress/models/collection_links.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/models/connection.py` & `authress-3.0.66/authress/models/connection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/models/connection_collection.py` & `authress-3.0.66/authress/models/connection_collection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/models/connection_data.py` & `authress-3.0.66/authress/models/connection_data.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/models/connection_default_connection_properties.py` & `authress-3.0.66/authress/models/connection_default_connection_properties.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/models/extension.py` & `authress-3.0.66/authress/models/extension.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/models/extension_application.py` & `authress-3.0.66/authress/models/extension_application.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/models/extension_client.py` & `authress-3.0.66/authress/models/extension_client.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/models/extension_collection.py` & `authress-3.0.66/authress/models/extension_collection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/models/group.py` & `authress-3.0.66/authress/models/group.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/models/group_collection.py` & `authress-3.0.66/authress/models/group_collection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/models/identity.py` & `authress-3.0.66/authress/models/identity.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/models/identity_collection.py` & `authress-3.0.66/authress/models/identity_collection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/models/identity_request.py` & `authress-3.0.66/authress/models/identity_request.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/models/invite.py` & `authress-3.0.66/authress/models/invite.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/models/link.py` & `authress-3.0.66/authress/models/link.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/models/linked_group.py` & `authress-3.0.66/authress/models/linked_group.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/models/links.py` & `authress-3.0.66/authress/models/links.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/models/metadata_object.py` & `authress-3.0.66/authress/models/metadata_object.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/models/metadata_object_account.py` & `authress-3.0.66/authress/models/metadata_object_account.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/models/o_auth_authorize_response.py` & `authress-3.0.66/authress/models/o_auth_authorize_response.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/models/o_auth_token_request.py` & `authress-3.0.66/authress/models/o_auth_token_request.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/models/o_auth_token_response.py` & `authress-3.0.66/authress/models/o_auth_token_response.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/models/pagination.py` & `authress-3.0.66/authress/models/pagination.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/models/pagination_next.py` & `authress-3.0.66/authress/models/pagination_next.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/models/permission_collection.py` & `authress-3.0.66/authress/models/permission_collection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/models/permission_collection_account.py` & `authress-3.0.66/authress/models/permission_collection_account.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/models/permission_object.py` & `authress-3.0.66/authress/models/permission_object.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/models/permissioned_resource.py` & `authress-3.0.66/authress/models/permissioned_resource.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/models/permissioned_resource_collection.py` & `authress-3.0.66/authress/models/permissioned_resource_collection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/models/resource.py` & `authress-3.0.66/authress/models/resource.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/models/resource_permission.py` & `authress-3.0.66/authress/models/resource_permission.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/models/resource_users_collection.py` & `authress-3.0.66/authress/models/resource_users_collection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/models/role.py` & `authress-3.0.66/authress/models/role.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/models/role_collection.py` & `authress-3.0.66/authress/models/role_collection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/models/statement.py` & `authress-3.0.66/authress/models/statement.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/models/tenant.py` & `authress-3.0.66/authress/models/tenant.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/models/tenant_collection.py` & `authress-3.0.66/authress/models/tenant_collection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/models/tenant_connection.py` & `authress-3.0.66/authress/models/tenant_connection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/models/tenant_data.py` & `authress-3.0.66/authress/models/tenant_data.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/models/token_request.py` & `authress-3.0.66/authress/models/token_request.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/models/user.py` & `authress-3.0.66/authress/models/user.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/models/user_connection_credentials.py` & `authress-3.0.66/authress/models/user_connection_credentials.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/models/user_identity.py` & `authress-3.0.66/authress/models/user_identity.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/models/user_identity_collection.py` & `authress-3.0.66/authress/models/user_identity_collection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/models/user_resources_collection.py` & `authress-3.0.66/authress/models/user_resources_collection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/models/user_role.py` & `authress-3.0.66/authress/models/user_role.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/models/user_role_collection.py` & `authress-3.0.66/authress/models/user_role_collection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/models/user_token.py` & `authress-3.0.66/authress/models/user_token.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress/rest.py` & `authress-3.0.66/authress/rest.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/authress.egg-info/PKG-INFO` & `authress-3.0.66/authress.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: authress
-Version: 3.0.63
+Version: 3.0.66
 Summary: Authress SDK for authorization as a service and interact with the Authress API.
 Home-page: https://github.com/Authress/authress-sdk.py.git
 Author: Authress Developers
 Author-email: developers@authress.io
 License: Apache-2.0
 Keywords: Authorization as a service,Security,authorization,authorization as a service,authentication,user authentication,Authress,Authress client,access management,access management as a service,user security,oso,polar,open source policy engine,embedded authorization,batteries included authorization,verified,verified access,verified permissions
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: authress Version: 3.0.63 Summary: Authress SDK for
+Metadata-Version: 2.1 Name: authress Version: 3.0.66 Summary: Authress SDK for
 authorization as a service and interact with the Authress API. Home-page:
 https://github.com/Authress/authress-sdk.py.git Author: Authress Developers
 Author-email: developers@authress.io License: Apache-2.0 Keywords:
 Authorization as a service,Security,authorization,authorization as a
 service,authentication,user authentication,Authress,Authress client,access
 management,access management as a service,user security,oso,polar,open source
 policy engine,embedded authorization,batteries included
```

### Comparing `authress-3.0.63/authress.egg-info/SOURCES.txt` & `authress-3.0.66/authress.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/pyproject.toml` & `authress-3.0.66/pyproject.toml`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/setup.py` & `authress-3.0.66/setup.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_access_record.py` & `authress-3.0.66/test/test_access_record.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_access_record_account.py` & `authress-3.0.66/test/test_access_record_account.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_access_record_collection.py` & `authress-3.0.66/test/test_access_record_collection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_access_records_api.py` & `authress-3.0.66/test/test_access_records_api.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_access_request.py` & `authress-3.0.66/test/test_access_request.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_access_request_collection.py` & `authress-3.0.66/test/test_access_request_collection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_access_request_response.py` & `authress-3.0.66/test/test_access_request_response.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_access_template.py` & `authress-3.0.66/test/test_access_template.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_account.py` & `authress-3.0.66/test/test_account.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_account_collection.py` & `authress-3.0.66/test/test_account_collection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_account_links.py` & `authress-3.0.66/test/test_account_links.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_accounts_api.py` & `authress-3.0.66/test/test_accounts_api.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_application_delegation.py` & `authress-3.0.66/test/test_application_delegation.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_applications_api.py` & `authress-3.0.66/test/test_applications_api.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_claim_request.py` & `authress-3.0.66/test/test_claim_request.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_client.py` & `authress-3.0.66/test/test_client.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_client_access_key.py` & `authress-3.0.66/test/test_client_access_key.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_client_collection.py` & `authress-3.0.66/test/test_client_collection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_client_options.py` & `authress-3.0.66/test/test_client_options.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_collection_links.py` & `authress-3.0.66/test/test_collection_links.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_connection.py` & `authress-3.0.66/test/test_connection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_connection_collection.py` & `authress-3.0.66/test/test_connection_collection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_connection_data.py` & `authress-3.0.66/test/test_connection_data.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_connection_default_connection_properties.py` & `authress-3.0.66/test/test_connection_default_connection_properties.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_connections_api.py` & `authress-3.0.66/test/test_connections_api.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_extension.py` & `authress-3.0.66/test/test_extension.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_extension_application.py` & `authress-3.0.66/test/test_extension_application.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_extension_client.py` & `authress-3.0.66/test/test_extension_client.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_extension_collection.py` & `authress-3.0.66/test/test_extension_collection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_extensions_api.py` & `authress-3.0.66/test/test_extensions_api.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_group.py` & `authress-3.0.66/test/test_group.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_group_collection.py` & `authress-3.0.66/test/test_group_collection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_groups_api.py` & `authress-3.0.66/test/test_groups_api.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_identity.py` & `authress-3.0.66/test/test_identity.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_identity_collection.py` & `authress-3.0.66/test/test_identity_collection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_identity_request.py` & `authress-3.0.66/test/test_identity_request.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_invite.py` & `authress-3.0.66/test/test_invite.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_invites_api.py` & `authress-3.0.66/test/test_invites_api.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_link.py` & `authress-3.0.66/test/test_link.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_linked_group.py` & `authress-3.0.66/test/test_linked_group.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_links.py` & `authress-3.0.66/test/test_links.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_metadata_object.py` & `authress-3.0.66/test/test_metadata_object.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_metadata_object_account.py` & `authress-3.0.66/test/test_metadata_object_account.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_o_auth_authorize_response.py` & `authress-3.0.66/test/test_o_auth_authorize_response.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_o_auth_token_request.py` & `authress-3.0.66/test/test_o_auth_token_request.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_o_auth_token_response.py` & `authress-3.0.66/test/test_o_auth_token_response.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_pagination.py` & `authress-3.0.66/test/test_pagination.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_pagination_next.py` & `authress-3.0.66/test/test_pagination_next.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_permission_collection.py` & `authress-3.0.66/test/test_permission_collection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_permission_collection_account.py` & `authress-3.0.66/test/test_permission_collection_account.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_permission_object.py` & `authress-3.0.66/test/test_permission_object.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_permissioned_resource.py` & `authress-3.0.66/test/test_permissioned_resource.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_permissioned_resource_collection.py` & `authress-3.0.66/test/test_permissioned_resource_collection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_resource.py` & `authress-3.0.66/test/test_resource.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_resource_permission.py` & `authress-3.0.66/test/test_resource_permission.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_resource_permissions_api.py` & `authress-3.0.66/test/test_resource_permissions_api.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_resource_users_collection.py` & `authress-3.0.66/test/test_resource_users_collection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_role.py` & `authress-3.0.66/test/test_role.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_role_collection.py` & `authress-3.0.66/test/test_role_collection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_roles_api.py` & `authress-3.0.66/test/test_roles_api.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_service_client_token_provider.py` & `authress-3.0.66/test/test_service_client_token_provider.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_service_clients_api.py` & `authress-3.0.66/test/test_service_clients_api.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_statement.py` & `authress-3.0.66/test/test_statement.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_tenant.py` & `authress-3.0.66/test/test_tenant.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_tenant_collection.py` & `authress-3.0.66/test/test_tenant_collection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_tenant_connection.py` & `authress-3.0.66/test/test_tenant_connection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_tenant_data.py` & `authress-3.0.66/test/test_tenant_data.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_tenants_api.py` & `authress-3.0.66/test/test_tenants_api.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_token_request.py` & `authress-3.0.66/test/test_token_request.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_user.py` & `authress-3.0.66/test/test_user.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_user_connection_credentials.py` & `authress-3.0.66/test/test_user_connection_credentials.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_user_identity.py` & `authress-3.0.66/test/test_user_identity.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_user_identity_collection.py` & `authress-3.0.66/test/test_user_identity_collection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_user_permissions_api.py` & `authress-3.0.66/test/test_user_permissions_api.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_user_resources_collection.py` & `authress-3.0.66/test/test_user_resources_collection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_user_role.py` & `authress-3.0.66/test/test_user_role.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_user_role_collection.py` & `authress-3.0.66/test/test_user_role_collection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_user_token.py` & `authress-3.0.66/test/test_user_token.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.63/test/test_users_api.py` & `authress-3.0.66/test/test_users_api.py`

 * *Files identical despite different names*

