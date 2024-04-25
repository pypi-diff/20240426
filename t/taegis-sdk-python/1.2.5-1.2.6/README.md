# Comparing `tmp/taegis-sdk-python-1.2.5.tar.gz` & `tmp/taegis_sdk_python-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taegis-sdk-python-1.2.5.tar", last modified: Mon Apr  8 15:02:18 2024, max compression
+gzip compressed data, was "taegis_sdk_python-1.2.6.tar", last modified: Thu Apr 25 22:08:51 2024, max compression
```

## Comparing `taegis-sdk-python-1.2.5.tar` & `taegis_sdk_python-1.2.6.tar`

### file list

```diff
@@ -1,262 +1,274 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.426053 taegis-sdk-python-1.2.5/
--rw-rw-rw-   0 root         (0) root         (0)    10173 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       84 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2839 2024-04-08 15:02:18.426053 taegis-sdk-python-1.2.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2119 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/README.md
--rw-rw-rw-   0 root         (0) root         (0)       12 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/requirements-dev.txt
--rw-rw-rw-   0 root         (0) root         (0)       39 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/requirements-test.txt
--rw-rw-rw-   0 root         (0) root         (0)      134 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-08 15:02:18.426053 taegis-sdk-python-1.2.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1571 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.370065 taegis-sdk-python-1.2.5/taegis_sdk_python/
--rw-rw-rw-   0 root         (0) root         (0)      895 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1135 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/_consts.py
--rw-rw-rw-   0 root         (0) root         (0)       23 2024-04-08 15:02:17.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     8742 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/authentication.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/config.py
--rw-rw-rw-   0 root         (0) root         (0)     2636 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/errors.py
--rw-rw-rw-   0 root         (0) root         (0)    14018 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/service_core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.370065 taegis-sdk-python-1.2.5/taegis_sdk_python/services/
--rw-rw-rw-   0 root         (0) root         (0)    17514 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.370065 taegis-sdk-python-1.2.5/taegis_sdk_python/services/access_points/
--rw-rw-rw-   0 root         (0) root         (0)      976 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/access_points/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2419 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/access_points/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     2313 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/access_points/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      893 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/access_points/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1377 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/access_points/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.374064 taegis-sdk-python-1.2.5/taegis_sdk_python/services/agent/
--rw-rw-rw-   0 root         (0) root         (0)     1154 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/agent/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      829 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/agent/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     3167 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/agent/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      841 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/agent/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     5316 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/agent/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.374064 taegis-sdk-python-1.2.5/taegis_sdk_python/services/alerts/
--rw-rw-rw-   0 root         (0) root         (0)      892 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/alerts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4785 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/alerts/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     6011 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/alerts/queries.py
--rw-rw-rw-   0 root         (0) root         (0)     1724 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/alerts/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    78668 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/alerts/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.374064 taegis-sdk-python-1.2.5/taegis_sdk_python/services/assets/
--rw-rw-rw-   0 root         (0) root         (0)      893 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/assets/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7235 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/assets/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    16354 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/assets/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      848 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/assets/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    23548 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/assets/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.378063 taegis-sdk-python-1.2.5/taegis_sdk_python/services/assets2/
--rw-rw-rw-   0 root         (0) root         (0)      905 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/assets2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9308 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/assets2/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    16070 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/assets2/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      855 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/assets2/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    42319 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/assets2/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.378063 taegis-sdk-python-1.2.5/taegis_sdk_python/services/audits/
--rw-rw-rw-   0 root         (0) root         (0)      893 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/audits/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1361 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/audits/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     3909 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/audits/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      848 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/audits/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    12825 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/audits/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.378063 taegis-sdk-python-1.2.5/taegis_sdk_python/services/authz/
--rw-rw-rw-   0 root         (0) root         (0)      881 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/authz/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3484 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/authz/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    14226 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/authz/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      841 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/authz/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    13254 2024-04-08 15:01:05.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/authz/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.382062 taegis-sdk-python-1.2.5/taegis_sdk_python/services/byoti/
--rw-rw-rw-   0 root         (0) root         (0)      881 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/byoti/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2761 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/byoti/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     3010 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/byoti/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      841 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/byoti/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    10026 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/byoti/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.382062 taegis-sdk-python-1.2.5/taegis_sdk_python/services/clients/
--rw-rw-rw-   0 root         (0) root         (0)      905 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/clients/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4001 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/clients/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     2562 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/clients/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      855 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/clients/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     7361 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/clients/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.386062 taegis-sdk-python-1.2.5/taegis_sdk_python/services/collector/
--rw-rw-rw-   0 root         (0) root         (0)      929 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/collector/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17250 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/collector/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    27472 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/collector/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      869 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/collector/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    43430 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/collector/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.386062 taegis-sdk-python-1.2.5/taegis_sdk_python/services/comments/
--rw-rw-rw-   0 root         (0) root         (0)      917 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/comments/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4946 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/comments/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     7300 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/comments/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      862 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/comments/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     5118 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/comments/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.386062 taegis-sdk-python-1.2.5/taegis_sdk_python/services/datasources/
--rw-rw-rw-   0 root         (0) root         (0)      962 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/datasources/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1794 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/datasources/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     1807 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/datasources/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      883 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/datasources/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2862 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/datasources/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.390061 taegis-sdk-python-1.2.5/taegis_sdk_python/services/detector_registry/
--rw-rw-rw-   0 root         (0) root         (0)     1034 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/detector_registry/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      909 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/detector_registry/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     3194 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/detector_registry/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      921 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/detector_registry/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3164 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/detector_registry/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.390061 taegis-sdk-python-1.2.5/taegis_sdk_python/services/endpoint_command_manager/
--rw-rw-rw-   0 root         (0) root         (0)     1381 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/endpoint_command_manager/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7325 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/endpoint_command_manager/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     3523 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/endpoint_command_manager/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      983 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/endpoint_command_manager/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     8618 2024-04-08 15:01:05.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/endpoint_command_manager/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.390061 taegis-sdk-python-1.2.5/taegis_sdk_python/services/endpoint_management_service/
--rw-rw-rw-   0 root         (0) root         (0)     1417 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/endpoint_management_service/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6935 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/endpoint_management_service/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     7179 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/endpoint_management_service/queries.py
--rw-rw-rw-   0 root         (0) root         (0)     1004 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/endpoint_management_service/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    21447 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/endpoint_management_service/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.394060 taegis-sdk-python-1.2.5/taegis_sdk_python/services/event_search/
--rw-rw-rw-   0 root         (0) root         (0)      965 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/event_search/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      874 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/event_search/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     2805 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/event_search/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      886 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/event_search/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3609 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/event_search/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.394060 taegis-sdk-python-1.2.5/taegis_sdk_python/services/events/
--rw-rw-rw-   0 root         (0) root         (0)     1215 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/events/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1346 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/events/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     2775 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/events/queries.py
--rw-rw-rw-   0 root         (0) root         (0)     2508 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/events/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    11022 2024-04-08 15:01:05.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/events/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.394060 taegis-sdk-python-1.2.5/taegis_sdk_python/services/exports/
--rw-rw-rw-   0 root         (0) root         (0)      905 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/exports/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13614 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/exports/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    10457 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/exports/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      855 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/exports/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    25646 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/exports/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.394060 taegis-sdk-python-1.2.5/taegis_sdk_python/services/fast_ioc/
--rw-rw-rw-   0 root         (0) root         (0)     1201 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/fast_ioc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      846 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/fast_ioc/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     3177 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/fast_ioc/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      858 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/fast_ioc/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3467 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/fast_ioc/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.398059 taegis-sdk-python-1.2.5/taegis_sdk_python/services/file_info/
--rw-rw-rw-   0 root         (0) root         (0)     1088 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/file_info/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4508 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/file_info/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     2911 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/file_info/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      865 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/file_info/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    39710 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/file_info/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.398059 taegis-sdk-python-1.2.5/taegis_sdk_python/services/investigations/
--rw-rw-rw-   0 root         (0) root         (0)     1007 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/investigations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22228 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/investigations/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    28039 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/investigations/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      904 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/investigations/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    37546 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/investigations/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.398059 taegis-sdk-python-1.2.5/taegis_sdk_python/services/investigations2/
--rw-rw-rw-   0 root         (0) root         (0)     1019 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/investigations2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15493 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/investigations2/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     8585 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/investigations2/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      911 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/investigations2/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    59951 2024-04-08 15:01:05.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/investigations2/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.402058 taegis-sdk-python-1.2.5/taegis_sdk_python/services/mitre_attack_info/
--rw-rw-rw-   0 root         (0) root         (0)     1025 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/mitre_attack_info/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      905 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/mitre_attack_info/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     9291 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/mitre_attack_info/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      917 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/mitre_attack_info/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3202 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/mitre_attack_info/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.402058 taegis-sdk-python-1.2.5/taegis_sdk_python/services/multi_tenant_context/
--rw-rw-rw-   0 root         (0) root         (0)     1061 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/multi_tenant_context/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4584 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/multi_tenant_context/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     4704 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/multi_tenant_context/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      955 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/multi_tenant_context/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     6279 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/multi_tenant_context/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.406057 taegis-sdk-python-1.2.5/taegis_sdk_python/services/multi_tenant_ioc/
--rw-rw-rw-   0 root         (0) root         (0)     1313 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/multi_tenant_ioc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      898 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/multi_tenant_ioc/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     3229 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/multi_tenant_ioc/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      910 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/multi_tenant_ioc/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3901 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/multi_tenant_ioc/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.406057 taegis-sdk-python-1.2.5/taegis_sdk_python/services/notebooks/
--rw-rw-rw-   0 root         (0) root         (0)      928 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/notebooks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2253 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/notebooks/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     1286 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/notebooks/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      869 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/notebooks/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1085 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/notebooks/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.406057 taegis-sdk-python-1.2.5/taegis_sdk_python/services/notifications/
--rw-rw-rw-   0 root         (0) root         (0)      986 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/notifications/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6906 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/notifications/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     2462 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/notifications/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      897 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/notifications/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     8811 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/notifications/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.406057 taegis-sdk-python-1.2.5/taegis_sdk_python/services/preferences/
--rw-rw-rw-   0 root         (0) root         (0)      962 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/preferences/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7272 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/preferences/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     7360 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/preferences/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      883 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/preferences/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    16267 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/preferences/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.410056 taegis-sdk-python-1.2.5/taegis_sdk_python/services/queries/
--rw-rw-rw-   0 root         (0) root         (0)      915 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/queries/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3852 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/queries/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     4382 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/queries/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      855 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/queries/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    10778 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/queries/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.410056 taegis-sdk-python-1.2.5/taegis_sdk_python/services/roadrunner/
--rw-rw-rw-   0 root         (0) root         (0)      941 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/roadrunner/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6287 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/roadrunner/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     6420 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/roadrunner/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      876 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/roadrunner/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    14157 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/roadrunner/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.414056 taegis-sdk-python-1.2.5/taegis_sdk_python/services/rules/
--rw-rw-rw-   0 root         (0) root         (0)      881 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/rules/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14238 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/rules/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    17159 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/rules/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      841 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/rules/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    24776 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/rules/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.414056 taegis-sdk-python-1.2.5/taegis_sdk_python/services/sharelinks/
--rw-rw-rw-   0 root         (0) root         (0)      941 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/sharelinks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1426 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/sharelinks/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     1381 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/sharelinks/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      876 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/sharelinks/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2578 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/sharelinks/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.414056 taegis-sdk-python-1.2.5/taegis_sdk_python/services/subjects/
--rw-rw-rw-   0 root         (0) root         (0)      917 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/subjects/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      850 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/subjects/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     1451 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/subjects/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      862 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/subjects/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3651 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/subjects/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.418055 taegis-sdk-python-1.2.5/taegis_sdk_python/services/tenant_profiles/
--rw-rw-rw-   0 root         (0) root         (0)     1010 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/tenant_profiles/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    19209 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/tenant_profiles/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    11166 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/tenant_profiles/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      907 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/tenant_profiles/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    23270 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/tenant_profiles/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.418055 taegis-sdk-python-1.2.5/taegis_sdk_python/services/tenants/
--rw-rw-rw-   0 root         (0) root         (0)     1349 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/tenants/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17846 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/tenants/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     7989 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/tenants/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      855 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/tenants/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    46328 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/tenants/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.418055 taegis-sdk-python-1.2.5/taegis_sdk_python/services/threat/
--rw-rw-rw-   0 root         (0) root         (0)      894 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/threat/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1906 2024-04-08 15:01:05.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/threat/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    13551 2024-04-08 15:01:05.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/threat/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      848 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/threat/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    46416 2024-04-08 15:01:05.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/threat/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.422054 taegis-sdk-python-1.2.5/taegis_sdk_python/services/threat_score/
--rw-rw-rw-   0 root         (0) root         (0)      966 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/threat_score/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      874 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/threat_score/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     2208 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/threat_score/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      886 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/threat_score/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     4092 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/threat_score/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.422054 taegis-sdk-python-1.2.5/taegis_sdk_python/services/trip/
--rw-rw-rw-   0 root         (0) root         (0)      869 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/trip/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4135 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/trip/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     3993 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/trip/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      834 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/trip/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     8879 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/trip/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.422054 taegis-sdk-python-1.2.5/taegis_sdk_python/services/users/
--rw-rw-rw-   0 root         (0) root         (0)      881 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/users/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12152 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/users/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     7321 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/users/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      841 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/users/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    25986 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/services/users/types.py
--rw-rw-rw-   0 root         (0) root         (0)      979 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/tokens.py
--rw-rw-rw-   0 root         (0) root         (0)     7548 2024-04-08 08:10:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:02:18.422054 taegis-sdk-python-1.2.5/taegis_sdk_python.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2839 2024-04-08 15:02:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10499 2024-04-08 15:02:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 15:02:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      135 2024-04-08 15:02:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2024-04-08 15:02:18.000000 taegis-sdk-python-1.2.5/taegis_sdk_python.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.603420 taegis_sdk_python-1.2.6/
+-rw-rw-rw-   0 root         (0) root         (0)    10173 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       84 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2871 2024-04-25 22:08:51.603420 taegis_sdk_python-1.2.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2119 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       12 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/requirements-dev.txt
+-rw-rw-rw-   0 root         (0) root         (0)       39 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/requirements-test.txt
+-rw-rw-rw-   0 root         (0) root         (0)      151 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-25 22:08:51.603420 taegis_sdk_python-1.2.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1571 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.575420 taegis_sdk_python-1.2.6/taegis_sdk_python/
+-rw-rw-rw-   0 root         (0) root         (0)      895 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1135 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/_consts.py
+-rw-rw-rw-   0 root         (0) root         (0)       23 2024-04-25 22:08:51.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     9120 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/authentication.py
+-rw-rw-rw-   0 root         (0) root         (0)     1740 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2636 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)    15383 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/service_core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.575420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/
+-rw-rw-rw-   0 root         (0) root         (0)    18716 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.575420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/access_points/
+-rw-rw-rw-   0 root         (0) root         (0)      976 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/access_points/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2419 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/access_points/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2313 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/access_points/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      893 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/access_points/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1377 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/access_points/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.575420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/agent/
+-rw-rw-rw-   0 root         (0) root         (0)     1154 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/agent/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      829 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/agent/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3167 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/agent/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      841 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/agent/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     5316 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/agent/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.575420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/alerts/
+-rw-rw-rw-   0 root         (0) root         (0)      892 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/alerts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4785 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/alerts/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     6011 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/alerts/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)     1724 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/alerts/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    80085 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/alerts/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.579420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/assets/
+-rw-rw-rw-   0 root         (0) root         (0)      893 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/assets/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7235 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/assets/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    16354 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/assets/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      848 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/assets/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    23548 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/assets/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.579420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/assets2/
+-rw-rw-rw-   0 root         (0) root         (0)      905 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/assets2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9308 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/assets2/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    16070 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/assets2/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      855 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/assets2/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    44413 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/assets2/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.579420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/audits/
+-rw-rw-rw-   0 root         (0) root         (0)      893 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/audits/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1361 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/audits/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3909 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/audits/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      848 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/audits/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    12825 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/audits/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.579420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/authz/
+-rw-rw-rw-   0 root         (0) root         (0)      881 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/authz/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3484 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/authz/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    14226 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/authz/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      841 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/authz/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    13254 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/authz/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.579420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/byoti/
+-rw-rw-rw-   0 root         (0) root         (0)      881 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/byoti/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2761 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/byoti/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3010 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/byoti/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      841 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/byoti/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    10026 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/byoti/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.583420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/clients/
+-rw-rw-rw-   0 root         (0) root         (0)      905 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/clients/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4001 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/clients/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2562 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/clients/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      855 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/clients/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     7361 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/clients/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.583420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/collector/
+-rw-rw-rw-   0 root         (0) root         (0)      929 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/collector/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17250 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/collector/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    27472 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/collector/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      869 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/collector/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    43430 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/collector/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.583420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/comments/
+-rw-rw-rw-   0 root         (0) root         (0)      917 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/comments/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4946 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/comments/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     7300 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/comments/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      862 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/comments/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     5118 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/comments/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.583420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/contracted_endpoint/
+-rw-rw-rw-   0 root         (0) root         (0)     1059 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/contracted_endpoint/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      923 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/contracted_endpoint/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2717 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/contracted_endpoint/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      935 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/contracted_endpoint/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1866 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/contracted_endpoint/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.583420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/datasources/
+-rw-rw-rw-   0 root         (0) root         (0)      962 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/datasources/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1794 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/datasources/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     1807 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/datasources/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      883 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/datasources/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2862 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/datasources/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.583420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/detector_registry/
+-rw-rw-rw-   0 root         (0) root         (0)     1034 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/detector_registry/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      909 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/detector_registry/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3194 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/detector_registry/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      921 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/detector_registry/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3164 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/detector_registry/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.583420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/endpoint_command_manager/
+-rw-rw-rw-   0 root         (0) root         (0)     1381 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/endpoint_command_manager/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7325 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/endpoint_command_manager/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3523 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/endpoint_command_manager/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      983 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/endpoint_command_manager/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     8618 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/endpoint_command_manager/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.587420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/endpoint_management_service/
+-rw-rw-rw-   0 root         (0) root         (0)     1417 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/endpoint_management_service/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6935 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/endpoint_management_service/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     7179 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/endpoint_management_service/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)     1004 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/endpoint_management_service/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    21447 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/endpoint_management_service/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.587420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/event_search/
+-rw-rw-rw-   0 root         (0) root         (0)      965 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/event_search/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      874 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/event_search/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2805 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/event_search/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      886 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/event_search/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3609 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/event_search/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.587420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/events/
+-rw-rw-rw-   0 root         (0) root         (0)     1215 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/events/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1346 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/events/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2775 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/events/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)     2508 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/events/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    11022 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/events/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.587420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/exports/
+-rw-rw-rw-   0 root         (0) root         (0)      905 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/exports/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14201 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/exports/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    10873 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/exports/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      855 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/exports/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    25813 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/exports/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.587420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/fast_ioc/
+-rw-rw-rw-   0 root         (0) root         (0)     1201 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/fast_ioc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      846 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/fast_ioc/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3177 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/fast_ioc/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      858 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/fast_ioc/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3467 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/fast_ioc/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.587420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/file_info/
+-rw-rw-rw-   0 root         (0) root         (0)     1088 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/file_info/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4508 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/file_info/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3510 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/file_info/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      865 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/file_info/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    39710 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/file_info/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.591420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/ingest_stats/
+-rw-rw-rw-   0 root         (0) root         (0)      966 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/ingest_stats/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      874 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/ingest_stats/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     4123 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/ingest_stats/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      886 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/ingest_stats/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3947 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/ingest_stats/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.591420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/investigations/
+-rw-rw-rw-   0 root         (0) root         (0)     1007 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/investigations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    26132 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/investigations/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    32299 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/investigations/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      904 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/investigations/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    37546 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/investigations/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.591420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/investigations2/
+-rw-rw-rw-   0 root         (0) root         (0)     1019 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/investigations2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15493 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/investigations2/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     8585 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/investigations2/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      911 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/investigations2/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    59951 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/investigations2/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.591420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/mitre_attack_info/
+-rw-rw-rw-   0 root         (0) root         (0)     1025 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/mitre_attack_info/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      905 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/mitre_attack_info/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     9291 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/mitre_attack_info/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      917 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/mitre_attack_info/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3202 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/mitre_attack_info/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.591420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/multi_tenant_context/
+-rw-rw-rw-   0 root         (0) root         (0)     1061 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/multi_tenant_context/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4584 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/multi_tenant_context/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     4704 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/multi_tenant_context/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      955 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/multi_tenant_context/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     6279 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/multi_tenant_context/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.595420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/multi_tenant_ioc/
+-rw-rw-rw-   0 root         (0) root         (0)     1313 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/multi_tenant_ioc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      898 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/multi_tenant_ioc/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3229 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/multi_tenant_ioc/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      910 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/multi_tenant_ioc/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3901 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/multi_tenant_ioc/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.595420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/notebooks/
+-rw-rw-rw-   0 root         (0) root         (0)      928 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/notebooks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2253 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/notebooks/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     1286 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/notebooks/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      869 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/notebooks/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1085 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/notebooks/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.595420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/notifications/
+-rw-rw-rw-   0 root         (0) root         (0)      986 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/notifications/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6906 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/notifications/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2462 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/notifications/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      897 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/notifications/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     8811 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/notifications/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.595420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/preferences/
+-rw-rw-rw-   0 root         (0) root         (0)      962 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/preferences/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7272 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/preferences/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     7360 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/preferences/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      883 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/preferences/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    17016 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/preferences/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.595420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/queries/
+-rw-rw-rw-   0 root         (0) root         (0)      915 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/queries/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3852 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/queries/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     4382 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/queries/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      855 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/queries/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    10778 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/queries/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.595420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/roadrunner/
+-rw-rw-rw-   0 root         (0) root         (0)      941 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/roadrunner/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6287 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/roadrunner/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     6420 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/roadrunner/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      876 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/roadrunner/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    14157 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/roadrunner/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.599420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/rules/
+-rw-rw-rw-   0 root         (0) root         (0)      881 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/rules/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14238 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/rules/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    17159 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/rules/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      841 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/rules/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    25560 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/rules/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.599420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/sharelinks/
+-rw-rw-rw-   0 root         (0) root         (0)      941 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/sharelinks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1426 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/sharelinks/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     1381 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/sharelinks/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      876 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/sharelinks/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2578 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/sharelinks/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.599420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/subjects/
+-rw-rw-rw-   0 root         (0) root         (0)      917 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/subjects/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      850 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/subjects/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     1451 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/subjects/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      862 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/subjects/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3651 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/subjects/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.599420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/tenant_profiles/
+-rw-rw-rw-   0 root         (0) root         (0)     1010 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/tenant_profiles/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    19209 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/tenant_profiles/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    11166 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/tenant_profiles/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      907 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/tenant_profiles/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    23270 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/tenant_profiles/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.599420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/tenants/
+-rw-rw-rw-   0 root         (0) root         (0)     1349 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/tenants/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17846 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/tenants/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     7989 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/tenants/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      855 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/tenants/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    46328 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/tenants/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.599420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/threat/
+-rw-rw-rw-   0 root         (0) root         (0)      894 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/threat/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1906 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/threat/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    12121 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/threat/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      848 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/threat/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    46398 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/threat/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.603420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/threat_score/
+-rw-rw-rw-   0 root         (0) root         (0)      966 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/threat_score/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      874 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/threat_score/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2208 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/threat_score/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      886 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/threat_score/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     4092 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/threat_score/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.603420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/trip/
+-rw-rw-rw-   0 root         (0) root         (0)      869 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/trip/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4135 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/trip/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3447 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/trip/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      834 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/trip/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     6813 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/trip/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.603420 taegis_sdk_python-1.2.6/taegis_sdk_python/services/users/
+-rw-rw-rw-   0 root         (0) root         (0)      881 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/users/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12152 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/users/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     7321 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/users/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      841 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/users/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    26696 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/services/users/types.py
+-rw-rw-rw-   0 root         (0) root         (0)      979 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/tokens.py
+-rw-rw-rw-   0 root         (0) root         (0)     7548 2024-04-25 22:08:38.000000 taegis_sdk_python-1.2.6/taegis_sdk_python/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 22:08:51.603420 taegis_sdk_python-1.2.6/taegis_sdk_python.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2871 2024-04-25 22:08:51.000000 taegis_sdk_python-1.2.6/taegis_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11058 2024-04-25 22:08:51.000000 taegis_sdk_python-1.2.6/taegis_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 22:08:51.000000 taegis_sdk_python-1.2.6/taegis_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      152 2024-04-25 22:08:51.000000 taegis_sdk_python-1.2.6/taegis_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-04-25 22:08:51.000000 taegis_sdk_python-1.2.6/taegis_sdk_python.egg-info/top_level.txt
```

### Comparing `taegis-sdk-python-1.2.5/LICENSE` & `taegis_sdk_python-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/PKG-INFO` & `taegis_sdk_python-1.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taegis-sdk-python
-Version: 1.2.5
+Version: 1.2.6
 Summary: Taegis Python SDK
 Home-page: https://github.com/secureworks/taegis-sdk-python
 Author: Secureworks
 Author-email: sdks@secureworks.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,14 +17,15 @@
 Requires-Dist: oauthlib
 Requires-Dist: requests
 Requires-Dist: requests-oauthlib
 Requires-Dist: dataclasses-json
 Requires-Dist: pyjwt>=2.8.0
 Requires-Dist: requests-toolbelt
 Requires-Dist: websockets
+Requires-Dist: filelock>=3.12.4
 
 # Taegis SDK for Python
 
 The Taegis SDK is a Python library for interfacing with the GraphQL APIs in Taegis.
 
 ## Prerequisites
```

### Comparing `taegis-sdk-python-1.2.5/README.md` & `taegis_sdk_python-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/setup.py` & `taegis_sdk_python-1.2.6/setup.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/__init__.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/_consts.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/_consts.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/authentication.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/authentication.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 """
 
 import logging
 import os
 from getpass import getpass
 from time import time
 from typing import Any, Dict, Tuple, Union, Optional
+import threading
 
 from oauthlib.oauth2 import BackendApplicationClient
 from requests import HTTPError, post
 from requests_oauthlib import OAuth2Session
 from taegis_sdk_python.config import get_config, write_to_config
 from taegis_sdk_python.errors import (
     InvalidAuthenticationMethod,
@@ -22,14 +23,16 @@
 try:
     from simplejson import JSONDecodeError
 except ImportError:  # pragma: no cover
     from json.decoder import JSONDecodeError
 
 logger = logging.getLogger(__name__)
 
+LOCK = threading.RLock()
+
 
 def check_username(
     request_url: str, username: str
 ) -> Dict[str, Any]:  # pragma: no cover
     """Check if the user needs to login via password or sso.
 
     Parameters
@@ -99,42 +102,50 @@
     -------
     str
         access token
     """
     access_token = get_cached_token(environment)
 
     if not access_token:
-        client_id, client_secret = get_oauth_from_env(environment)
-        if client_id and client_secret:
-            access_token = get_token_by_oauth(request_url, client_id, client_secret)
-        else:
-            username = input("Username: ")
-            response = check_username(request_url, username)
-
-            if response.get("login_type") == "username-password":
-                access_token = get_token_by_password_grant(request_url, username)
-            elif response.get("login_type") == "sso":
-                access_token = get_token_by_sso_device_code(request_url)
-            else:
-                raise InvalidAuthenticationMethod(
-                    message="No known authenticition method for user"
-                )
+        with LOCK:
+            access_token = get_cached_token(environment)
+
+            if not access_token:
+                client_id, client_secret = get_oauth_from_env(environment)
+                if client_id and client_secret:
+                    access_token = get_token_by_oauth(
+                        request_url, client_id, client_secret
+                    )
+                else:
+                    username = input("Username: ")
+                    response = check_username(request_url, username)
+
+                    if response.get("login_type") == "username-password":
+                        access_token = get_token_by_password_grant(
+                            request_url, username
+                        )
+                    elif response.get("login_type") == "sso":
+                        access_token = get_token_by_sso_device_code(request_url)
+                    else:
+                        raise InvalidAuthenticationMethod(
+                            message="No known authentication method for user"
+                        )
 
-        write_to_config(environment, "access_token", access_token)
+                write_to_config(environment, "access_token", access_token)
 
     return access_token
 
 
 def get_cached_token(env: str) -> Union[str, None]:  # pragma: no cover
     """Get cached token from config file."""
     config = get_config()
 
     # check for token and expiry in config
     token = str(config.get(env, "access_token", fallback=""))
-    if token and get_token_exp(token) >= int(time()):
+    if token and get_token_exp(token) >= int(time()) + 15:
         return token
 
     return None
 
 
 def get_token_by_oauth(
     request_url: str, client_id: str, client_secret: str
```

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/config.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 """config.py
 
 Taegis SDK Configuration management.
 """
+
 from configparser import ConfigParser
 from pathlib import Path
+import threading
+from filelock import FileLock
+
+LOCK = threading.RLock()
 
 
 def get_config_file() -> Path:
     """Return config file path and ensure config file exists.
 
     Returns
     -------
@@ -40,17 +45,22 @@
 
     Parameters
     ----------
     config : ConfigParser
         Config object
     """
     config_fp = get_config_file()
+    lock_file = config_fp.with_suffix(".lock")
+    file_lock = FileLock(lock_file)
+
+    with file_lock:
+        with config_fp.open(mode="w") as f:  # pylint: disable=invalid-name
+            config.write(f)
 
-    with config_fp.open(mode="w") as f:  # pylint: disable=invalid-name
-        config.write(f)
+    lock_file.unlink(missing_ok=True)
 
 
 def write_to_config(section: str, key: str, value: str):
     """Write a key/value pair to config file under section.
 
     Parameters
     ----------
```

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/errors.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/errors.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/service_core.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/service_core.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,16 +4,18 @@
 """
 
 from __future__ import annotations
 
 import logging
 from datetime import datetime, timedelta
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union
+import threading
 
 from gql import Client, gql
+from gql.transport import Transport
 from gql.transport.requests import RequestsHTTPTransport
 from gql.transport.websockets import WebsocketsTransport
 from graphql import GraphQLError, GraphQLField, GraphQLSchema
 from taegis_sdk_python._version import __version__
 from taegis_sdk_python.errors import InvalidGraphQLEndpoint
 from taegis_sdk_python.utils import async_block, prepare_variables, remove_node
 
@@ -21,78 +23,156 @@
     from taegis_sdk_python.services import GraphQLService
 
 
 log = logging.getLogger(__name__)
 
 
 class SchemaCache:
-    """GraphQL Schema Cache."""
+    """Taegis GraphQL Schema Cache."""
 
-    def __init__(self, schema: Optional[GraphQLSchema] = None, expires: int = 5):
-        """Initialize SchemaCache.
+    _lock = threading.RLock()
 
-        Parameters
-        ----------
-        schema : Optional[GraphQLSchema], optional
-            GraphQL schema object, by default None
-        expires : int, optional
-            Schema expires in minutes, by default 5
-        """
+    def __init__(self, expires: int, schema: Optional[GraphQLSchema] = None):
+        self._expires = expires
         self._schema = schema
         self._inserted_at = datetime.now()
-        self.expires = expires
+
+    def is_expired(self) -> bool:
+        """Returns if the schema is expired.
+
+        Returns
+        -------
+        bool
+            Is schema expired?
+        """
+        return self._inserted_at + timedelta(minutes=self._expires) <= datetime.now()
 
     @property
-    def schema(self) -> Union[GraphQLSchema, None]:
-        """Return GraphQLSchema if it exists and is not expired.
+    def schema(self) -> Optional[GraphQLSchema]:
+        """Get the schema.
 
         Returns
         -------
-        Union[GraphQLSchema, None]
-            GraphQL Schema
+        Optional[GraphQLSchema]
         """
-        if self._inserted_at + timedelta(minutes=self.expires) < datetime.now():
-            self.schema = None
+        log.debug(f"Schema is expired: {self.is_expired()}")
+
         return self._schema
 
-    @schema.setter
-    def schema(self, schema: Optional[GraphQLSchema]):
-        """Set schema and update inserted_at.
+
+class SchemaCacheMap:
+    """Taegis Schema Cache Map.
+
+    This is a singleton class that will cache the introspection schema for a given
+    GraphQL server.  The schema will be cached for a given amount of time and will
+    be retrieved from the transport if expired.
+    """
+
+    _instance = None
+    _lock = threading.RLock()
+
+    def __new__(cls, *args, **kwargs):
+        if cls._instance is None:
+            with cls._lock:
+                if cls._instance is None:
+                    cls._instance = super(SchemaCacheMap, cls).__new__(cls)
+                    cls._instance.__post_init__(*args, **kwargs)
+        return cls._instance
+
+    def __post_init__(self, expires: int = 5):
+        self._map = {}
+        self._expires = expires
+
+    def get(
+        self, transport: Transport, introspection_args: Dict[str, Any]
+    ) -> GraphQLSchema:
+        """Get the schema from the map.
+
+        Retrieves new schema if expired, thread locks to prevent another service
+        from retrieving the schema at the same time.
+
+        Parameters
+        ----------
+        transport : Transport
+            gql Transport
+        introspection_args : Dict[str, Any]
+            Introspection Query arguments
+
+        Returns
+        -------
+        GraphQLSchema
+        """
+        if transport.url not in self._map or self._map[transport.url].is_expired():
+            log.debug("Schema not in map or expired...")
+            with self._lock:
+                if (
+                    transport.url not in self._map
+                    or self._map[transport.url].is_expired()
+                ):
+                    self._map[transport.url] = SchemaCache(
+                        expires=self._expires,
+                        schema=self.retrieve_schema(transport, introspection_args),
+                    )
+
+        return self._map.get(transport.url).schema
+
+    def clear(self, transport: Transport):
+        """Clear the schema from the map.
 
         Parameters
         ----------
-        schema :
-            _description_
+        transport : Transport
+            gql Transport
         """
-        if self._schema is not schema:
-            self._schema = schema
-            self._inserted_at = datetime.now()
+        if transport.url in self._map:
+            with self._lock:
+                if transport.url in self._map:
+                    del self._map[transport.url]
+
+    @staticmethod
+    def retrieve_schema(
+        transport: Transport, introspection_args: Dict[str, Any]
+    ) -> GraphQLSchema:
+        """Retrieve the schema from a gql Client with the provided transport and
+        introspection query arguments.
 
-    def should_fetch_schema(self) -> bool:
-        """Return True if schema is should be fetched in transport.
+        Parameters
+        ----------
+        transport : Transport
+        introspection_args : Dict[str, Any]
 
         Returns
         -------
-        bool
-            True if schema is should be fetched in transport.
+        GraphQLSchema
         """
-        return not self.schema
+        log.debug(f"Retrieving schema for {transport.url}...")
+
+        client = Client(
+            transport=transport,
+            fetch_schema_from_transport=True,
+            introspection_args=introspection_args,
+        )
+
+        with client:
+            schema = client.schema
+
+        return schema
 
 
 class ServiceCore:
     """Taegis GraphQL Service core functionality."""
 
     def __init__(self, service: GraphQLService):
         self.service = service
 
         self._urls = self.service._environments
         self._gateway = self.service._gateway
         self._input_value_deprecation = True
 
-        self._schema = SchemaCache(schema=None, expires=self.service.schema_expiry)
+        self._cache_map = SchemaCacheMap(expires=self.service.schema_expiry)
 
         self._queries = None
         self._mutations = None
         self._subscriptions = None
 
     @property
     def sync_url(self) -> str:
@@ -130,96 +210,75 @@
         transport = RequestsHTTPTransport(
             f"{self.sync_url}{self.gateway}",
             headers=self.service.headers,
         )
 
         client = Client(
             transport=transport,
-            schema=self._schema.schema,
-            fetch_schema_from_transport=self._schema.should_fetch_schema(),
-            introspection_args={
-                "input_value_deprecation": (
-                    bool(self.service.input_value_deprecation)
-                    if self.service.input_value_deprecation is not None
-                    else self._input_value_deprecation
-                )
-            },
+            schema=self._cache_map.get(
+                transport,
+                introspection_args={
+                    "input_value_deprecation": (
+                        bool(self.service.input_value_deprecation)
+                        if self.service.input_value_deprecation is not None
+                        else self._input_value_deprecation
+                    )
+                },
+            ),
         )
 
-        with client:
-            self._schema.schema = client.schema
-
         return client
 
     @property
     def ws_client(self) -> Client:
         """GraphQL WebSockets Transport with Client."""
         subprotocols = [
             "graphql-ws",
             f"access-token-{self.service.access_token}",
         ]
 
-        # we cannot build the async client and use it to fetch the schema
-        # due to async issues with the transport.  This will grab the schema
-        # from a sync client and use it to build the async client.
-        if not self._schema.schema:
-            self.sync_client  # pylint: disable=pointless-statement
-
         if self.service.tenant_id:
             subprotocols.append(f"x-tenant-context-{self.service.tenant_id}")
 
         transport = WebsocketsTransport(
             f"{self.wss_url}{self.gateway}",
             headers=self.service.headers,
             subprotocols=subprotocols,
             connect_args={"max_size": None},
         )
 
         client = Client(
             transport=transport,
-            schema=self._schema.schema,
-            fetch_schema_from_transport=self._schema.should_fetch_schema(),
-            introspection_args={
-                "input_value_deprecation": (
-                    bool(self.service.input_value_deprecation)
-                    if self.service.input_value_deprecation is not None
-                    else self._input_value_deprecation
-                )
-            },
+            schema=self.schema,
         )
 
         return client
 
     @property
     def schema(self) -> GraphQLSchema:
         """Retrieves introspection schema from Synchronous endpoint.
 
         Returns
         -------
         GraphQLSchema
         """
-        if not self._schema.schema:
-            self.sync_client  # pylint: disable=pointless-statement
-        return self._schema.schema
+        return self.sync_client.schema
 
     def clear_schema(self):
         """Clears the introspection schema."""
-        self._schema.schema = None
+        self._cache_map.clear(self.sync_client.transport)
 
     def get_sync_schema(self) -> Union[GraphQLSchema, None]:
         """Retrieves introspection schema from Synchronous endpoint.
 
         Returns
         -------
         GraphQLSchema
         """
-        client = self.sync_client
-        with client:
-            schema = client.schema
-        return schema
+        return self.schema
 
     @async_block
     async def get_ws_schema(self) -> Union[GraphQLSchema, None]:
         """Retrieves introspection schema from WebSockets endpoint.
 
         Returns
         -------
```

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/__init__.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 This needs to be a generated file.  Need to make jinja template.
 """
 
 from typing import Dict, Optional, Any
+import threading
 
 from taegis_sdk_python._consts import TAEGIS_ENVIRONMENT_URLS
 from taegis_sdk_python._version import __version__
 from taegis_sdk_python.authentication import get_token
 from taegis_sdk_python.config import write_to_config
 from taegis_sdk_python.service_core import ServiceCore
 from taegis_sdk_python.services.access_points import AccessPointsService
@@ -16,27 +17,29 @@
 from taegis_sdk_python.services.assets2 import Assets2Service
 from taegis_sdk_python.services.audits import AuditsService
 from taegis_sdk_python.services.authz import AuthzService
 from taegis_sdk_python.services.byoti import ByotiService
 from taegis_sdk_python.services.clients import ClientsService
 from taegis_sdk_python.services.collector import CollectorService
 from taegis_sdk_python.services.comments import CommentsService
+from taegis_sdk_python.services.contracted_endpoint import ContractedEndpointService
 from taegis_sdk_python.services.datasources import DatasourcesService
 from taegis_sdk_python.services.detector_registry import DetectorRegistryService
 from taegis_sdk_python.services.endpoint_command_manager import (
     EndpointCommandManagerService,
 )
 from taegis_sdk_python.services.endpoint_management_service import (
     EndpointManagementServiceService,
 )
 from taegis_sdk_python.services.event_search import EventSearchService
 from taegis_sdk_python.services.events import EventsService
 from taegis_sdk_python.services.exports import ExportsService
 from taegis_sdk_python.services.fast_ioc import FastIocService
 from taegis_sdk_python.services.file_info import FileInfoService
+from taegis_sdk_python.services.ingest_stats import IngestStatsService
 from taegis_sdk_python.services.investigations import InvestigationsService
 from taegis_sdk_python.services.investigations2 import Investigations2Service
 from taegis_sdk_python.services.mitre_attack_info import MitreAttackInfoService
 from taegis_sdk_python.services.multi_tenant_context import MultiTenantContextService
 from taegis_sdk_python.services.multi_tenant_ioc import MultiTenantIocService
 from taegis_sdk_python.services.notebooks import NotebooksService
 from taegis_sdk_python.services.notifications import NotificationsService
@@ -96,16 +99,16 @@
         self._environment = environment or list(self._environments)[0]
 
         if self._environment not in self._environments:
             raise ValueError(f"environment must be in {self._environments.keys()}")
 
         self._tenant_id = tenant_id
         self._gateway = gateway or "/graphql"
-        self._context_manager = {}
-        self._context_kwargs = []
+        self._thread_id = threading.get_ident()
+        self._context_kwargs = {}
         if not extra_headers:
             self._extra_headers = {}
         else:
             self._extra_headers = extra_headers
         self._schema_expiry = schema_expiry
         self._input_value_deprecation = None
 
@@ -116,23 +119,25 @@
         self._assets2 = None
         self._audits = None
         self._authz = None
         self._byoti = None
         self._clients = None
         self._collector = None
         self._comments = None
+        self._contracted_endpoint = None
         self._datasources = None
         self._detector_registry = None
         self._endpoint_command_manager = None
         self._endpoint_management_service = None
         self._event_search = None
         self._events = None
         self._exports = None
         self._fast_ioc = None
         self._file_info = None
+        self._ingest_stats = None
         self._investigations = None
         self._investigations2 = None
         self._mitre_attack_info = None
         self._multi_tenant_context = None
         self._multi_tenant_ioc = None
         self._notebooks = None
         self._notifications = None
@@ -147,30 +152,42 @@
         self._tenants = None
         self._threat = None
         self._threat_score = None
         self._trip = None
         self._users = None
 
     def __call__(self, **kwargs):
-        self._context_kwargs.append(kwargs)
+        if threading.get_ident() not in self._context_kwargs:
+            self._context_kwargs[threading.get_ident()] = []
+
+        self._context_kwargs[threading.get_ident()].append(kwargs)
         return self
 
     def __enter__(self):
-        for kwarg in self._context_kwargs:
-            self._context_manager.update(kwarg)
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
-        self._context_manager.clear()
+        if self._context_kwargs[threading.get_ident()]:
+            self._context_kwargs[threading.get_ident()].pop()
+
+        else:
+            del self._context_kwargs[threading.get_ident()]
+
+    @property
+    def _context_manager(self):
+        """Internal Context Manager property."""
+        temp_context = {}
 
-        if self._context_kwargs:
-            self._context_kwargs.pop()
+        for kwarg in self._context_kwargs.get(self._thread_id, []):
+            temp_context.update(kwarg)
+        if self._thread_id != threading.get_ident():
+            for kwarg in self._context_kwargs.get(threading.get_ident(), []):
+                temp_context.update(kwarg)
 
-            for kwarg in self._context_kwargs:
-                self._context_manager.update(kwarg)
+        return temp_context
 
     @property
     def environment(self):
         """Taegis Environment."""
         return self._context_manager.get("environment", self._environment)
 
     @property
@@ -322,14 +339,21 @@
     def comments(self):
         """Comments Service Endpoint."""
         if not self._comments:
             self._comments = CommentsService(self)
         return self._comments
 
     @property
+    def contracted_endpoint(self):
+        """ContractedEndpoint Service Endpoint."""
+        if not self._contracted_endpoint:
+            self._contracted_endpoint = ContractedEndpointService(self)
+        return self._contracted_endpoint
+
+    @property
     def datasources(self):
         """Datasources Service Endpoint."""
         if not self._datasources:
             self._datasources = DatasourcesService(self)
         return self._datasources
 
     @property
@@ -385,14 +409,21 @@
     def file_info(self):
         """FileInfo Service Endpoint."""
         if not self._file_info:
             self._file_info = FileInfoService(self)
         return self._file_info
 
     @property
+    def ingest_stats(self):
+        """IngestStats Service Endpoint."""
+        if not self._ingest_stats:
+            self._ingest_stats = IngestStatsService(self)
+        return self._ingest_stats
+
+    @property
     def investigations(self):
         """Investigations Service Endpoint."""
         if not self._investigations:
             self._investigations = InvestigationsService(self)
         return self._investigations
 
     @property
```

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/access_points/__init__.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/access_points/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/access_points/mutations.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/access_points/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/access_points/queries.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/access_points/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/access_points/subscriptions.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/access_points/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/access_points/types.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/access_points/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/agent/__init__.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/agent/mutations.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/agent/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/agent/queries.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/agent/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/agent/subscriptions.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/agent/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/agent/types.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/agent/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/alerts/__init__.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/alerts/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/alerts/mutations.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/alerts/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/alerts/queries.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/alerts/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/alerts/subscriptions.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/alerts/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/alerts/types.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/alerts/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1348,14 +1348,43 @@
     status: Optional[ResponseStatus] = field(
         default=None, metadata=config(field_name="status")
     )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
+class MatchedYaraRule:
+    """MatchedYaraRule."""
+
+    rule_name: Optional[str] = field(
+        default=None, metadata=config(field_name="rule_name")
+    )
+    rule_description: Optional[str] = field(
+        default=None, metadata=config(field_name="rule_description")
+    )
+    classification: Optional[str] = field(
+        default=None, metadata=config(field_name="classification")
+    )
+    confidence: Optional[float] = field(
+        default=None, metadata=config(field_name="confidence")
+    )
+    severity: Optional[float] = field(
+        default=None, metadata=config(field_name="severity")
+    )
+    attack_technique_ids: Optional[List[str]] = field(
+        default=None, metadata=config(field_name="attack_technique_ids")
+    )
+    vid: Optional[str] = field(default=None, metadata=config(field_name="vid"))
+    rule_created_date: Optional[Timestamp] = field(
+        default=None, metadata=config(field_name="rule_created_date")
+    )
+
+
+@dataclass_json
+@dataclass(order=True, eq=True, frozen=True)
 class DDosIpCount:
     """DDosIpCount."""
 
     count: Optional[int] = field(default=None, metadata=config(field_name="count"))
     date: Optional[Timestamp] = field(default=None, metadata=config(field_name="date"))
 
 
@@ -2006,14 +2035,24 @@
     initial_access_vector_info: Optional[List[InitialAccessVectorInfo]] = field(
         default=None, metadata=config(field_name="initial_access_vector_info")
     )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
+class FileAnalysisDetail:
+    """FileAnalysisDetail."""
+
+    matched_yara_rule: Optional[List[MatchedYaraRule]] = field(
+        default=None, metadata=config(field_name="matched_yara_rule")
+    )
+
+
+@dataclass_json
+@dataclass(order=True, eq=True, frozen=True)
 class HandsOnKeyboardDetails:
     """HandsOnKeyboardDetails."""
 
     total_num_events: Optional[int] = field(
         default=None, metadata=config(field_name="total_num_events")
     )
     matched_num_events: Optional[int] = field(
@@ -2174,14 +2213,17 @@
         default=None, metadata=config(field_name="business_email_compromise")
     )
     account_compromise_detector_detail: Optional[
         AccountCompromiseDetectorDetail
     ] = field(
         default=None, metadata=config(field_name="account_compromise_detector_detail")
     )
+    file_analysis_detail: Optional[FileAnalysisDetail] = field(
+        default=None, metadata=config(field_name="file_analysis_detail")
+    )
     generic: Optional[GenericDetail] = field(
         default=None, metadata=config(field_name="generic")
     )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
```

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/assets/__init__.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/assets/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/assets/mutations.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/assets/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/assets/queries.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/assets/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/assets/subscriptions.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/assets/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/assets/types.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/assets/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/assets2/__init__.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/assets2/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/assets2/mutations.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/assets2/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/assets2/queries.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/assets2/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/assets2/subscriptions.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/assets2/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/assets2/types.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/assets2/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -344,15 +344,19 @@
     updated_at: Optional[str] = field(
         default=None, metadata=config(field_name="updatedAt")
     )
     deleted_at: Optional[str] = field(
         default=None, metadata=config(field_name="deletedAt")
     )
     last_seen_at: Optional[str] = field(
-        default=None, metadata=config(field_name="lastSeenAt")
+        default=None,
+        metadata=config(
+            metadata={"deprecated": True, "deprecation_reason": "use updatedAt"},
+            field_name="lastSeenAt",
+        ),
     )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
 class AssetIPAddress:
     """AssetIPAddress."""
@@ -368,15 +372,19 @@
     updated_at: Optional[str] = field(
         default=None, metadata=config(field_name="updatedAt")
     )
     deleted_at: Optional[str] = field(
         default=None, metadata=config(field_name="deletedAt")
     )
     last_seen_at: Optional[str] = field(
-        default=None, metadata=config(field_name="lastSeenAt")
+        default=None,
+        metadata=config(
+            metadata={"deprecated": True, "deprecation_reason": "use updatedAt"},
+            field_name="lastSeenAt",
+        ),
     )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
 class AssetMacAddress:
     """AssetMacAddress."""
@@ -392,15 +400,19 @@
     updated_at: Optional[str] = field(
         default=None, metadata=config(field_name="updatedAt")
     )
     deleted_at: Optional[str] = field(
         default=None, metadata=config(field_name="deletedAt")
     )
     last_seen_at: Optional[str] = field(
-        default=None, metadata=config(field_name="lastSeenAt")
+        default=None,
+        metadata=config(
+            metadata={"deprecated": True, "deprecation_reason": "use updatedAt"},
+            field_name="lastSeenAt",
+        ),
     )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
 class KVTagInputV2:
     """KVTagInputV2."""
@@ -590,27 +602,47 @@
     hostname_contains: Optional[str] = field(
         default=None, metadata=config(field_name="hostname_contains")
     )
     hostname_autocomplete: Optional[str] = field(
         default=None, metadata=config(field_name="hostname_autocomplete")
     )
     last_seen_at: Optional[str] = field(
-        default=None, metadata=config(field_name="lastSeenAt")
+        default=None,
+        metadata=config(
+            metadata={"deprecated": True, "deprecation_reason": "use updatedAt"},
+            field_name="lastSeenAt",
+        ),
     )
     last_seen_at_lt: Optional[str] = field(
-        default=None, metadata=config(field_name="lastSeenAt_lt")
+        default=None,
+        metadata=config(
+            metadata={"deprecated": True, "deprecation_reason": "use updatedAt_lt"},
+            field_name="lastSeenAt_lt",
+        ),
     )
     last_seen_at_lte: Optional[str] = field(
-        default=None, metadata=config(field_name="lastSeenAt_lte")
+        default=None,
+        metadata=config(
+            metadata={"deprecated": True, "deprecation_reason": "use updatedAt_lte"},
+            field_name="lastSeenAt_lte",
+        ),
     )
     last_seen_at_gt: Optional[str] = field(
-        default=None, metadata=config(field_name="lastSeenAt_gt")
+        default=None,
+        metadata=config(
+            metadata={"deprecated": True, "deprecation_reason": "use updatedAt_gt"},
+            field_name="lastSeenAt_gt",
+        ),
     )
     last_seen_at_gte: Optional[str] = field(
-        default=None, metadata=config(field_name="lastSeenAt_gte")
+        default=None,
+        metadata=config(
+            metadata={"deprecated": True, "deprecation_reason": "use updatedAt_gte"},
+            field_name="lastSeenAt_gte",
+        ),
     )
     updated_at: Optional[str] = field(
         default=None, metadata=config(field_name="updatedAt")
     )
     updated_at_lt: Optional[str] = field(
         default=None, metadata=config(field_name="updatedAt_lt")
     )
@@ -665,27 +697,47 @@
     ip_contains: Optional[str] = field(
         default=None, metadata=config(field_name="ip_contains")
     )
     ip_autocomplete: Optional[str] = field(
         default=None, metadata=config(field_name="ip_autocomplete")
     )
     last_seen_at: Optional[str] = field(
-        default=None, metadata=config(field_name="lastSeenAt")
+        default=None,
+        metadata=config(
+            metadata={"deprecated": True, "deprecation_reason": "use updatedAt"},
+            field_name="lastSeenAt",
+        ),
     )
     last_seen_at_lt: Optional[str] = field(
-        default=None, metadata=config(field_name="lastSeenAt_lt")
+        default=None,
+        metadata=config(
+            metadata={"deprecated": True, "deprecation_reason": "use updatedAt_lt"},
+            field_name="lastSeenAt_lt",
+        ),
     )
     last_seen_at_lte: Optional[str] = field(
-        default=None, metadata=config(field_name="lastSeenAt_lte")
+        default=None,
+        metadata=config(
+            metadata={"deprecated": True, "deprecation_reason": "use updatedAt_lte"},
+            field_name="lastSeenAt_lte",
+        ),
     )
     last_seen_at_gt: Optional[str] = field(
-        default=None, metadata=config(field_name="lastSeenAt_gt")
+        default=None,
+        metadata=config(
+            metadata={"deprecated": True, "deprecation_reason": "use updatedAt_gt"},
+            field_name="lastSeenAt_gt",
+        ),
     )
     last_seen_at_gte: Optional[str] = field(
-        default=None, metadata=config(field_name="lastSeenAt_gte")
+        default=None,
+        metadata=config(
+            metadata={"deprecated": True, "deprecation_reason": "use updatedAt_gte"},
+            field_name="lastSeenAt_gte",
+        ),
     )
     updated_at: Optional[str] = field(
         default=None, metadata=config(field_name="updatedAt")
     )
     updated_at_lt: Optional[str] = field(
         default=None, metadata=config(field_name="updatedAt_lt")
     )
@@ -740,27 +792,47 @@
     mac_contains: Optional[str] = field(
         default=None, metadata=config(field_name="mac_contains")
     )
     mac_autocomplete: Optional[str] = field(
         default=None, metadata=config(field_name="mac_autocomplete")
     )
     last_seen_at: Optional[str] = field(
-        default=None, metadata=config(field_name="lastSeenAt")
+        default=None,
+        metadata=config(
+            metadata={"deprecated": True, "deprecation_reason": "use updatedAt"},
+            field_name="lastSeenAt",
+        ),
     )
     last_seen_at_lt: Optional[str] = field(
-        default=None, metadata=config(field_name="lastSeenAt_lt")
+        default=None,
+        metadata=config(
+            metadata={"deprecated": True, "deprecation_reason": "use updatedAt_lt"},
+            field_name="lastSeenAt_lt",
+        ),
     )
     last_seen_at_lte: Optional[str] = field(
-        default=None, metadata=config(field_name="lastSeenAt_lte")
+        default=None,
+        metadata=config(
+            metadata={"deprecated": True, "deprecation_reason": "use updatedAt_lte"},
+            field_name="lastSeenAt_lte",
+        ),
     )
     last_seen_at_gt: Optional[str] = field(
-        default=None, metadata=config(field_name="lastSeenAt_gt")
+        default=None,
+        metadata=config(
+            metadata={"deprecated": True, "deprecation_reason": "use updatedAt_gt"},
+            field_name="lastSeenAt_gt",
+        ),
     )
     last_seen_at_gte: Optional[str] = field(
-        default=None, metadata=config(field_name="lastSeenAt_gte")
+        default=None,
+        metadata=config(
+            metadata={"deprecated": True, "deprecation_reason": "use updatedAt_gte"},
+            field_name="lastSeenAt_gte",
+        ),
     )
     updated_at: Optional[str] = field(
         default=None, metadata=config(field_name="updatedAt")
     )
     updated_at_lt: Optional[str] = field(
         default=None, metadata=config(field_name="updatedAt_lt")
     )
```

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/audits/__init__.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/audits/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/audits/mutations.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/audits/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/audits/queries.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/audits/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/audits/subscriptions.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/audits/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/audits/types.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/audits/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/authz/__init__.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/authz/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/authz/mutations.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/authz/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/authz/queries.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/authz/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/authz/subscriptions.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/authz/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/authz/types.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/authz/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/byoti/__init__.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/byoti/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/byoti/mutations.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/byoti/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/byoti/queries.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/byoti/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/byoti/subscriptions.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/byoti/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/byoti/types.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/byoti/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/clients/__init__.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/clients/mutations.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/clients/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/clients/queries.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/clients/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/clients/subscriptions.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/clients/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/clients/types.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/clients/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/collector/__init__.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/collector/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/collector/mutations.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/collector/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/collector/queries.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/collector/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/collector/subscriptions.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/collector/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/collector/types.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/collector/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/comments/__init__.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/comments/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/comments/mutations.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/comments/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/comments/queries.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/comments/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/comments/subscriptions.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/comments/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/comments/types.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/comments/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/datasources/__init__.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/datasources/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/datasources/mutations.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/datasources/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/datasources/queries.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/datasources/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/datasources/subscriptions.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/datasources/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/datasources/types.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/datasources/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/detector_registry/__init__.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/detector_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/detector_registry/mutations.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/detector_registry/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/detector_registry/queries.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/detector_registry/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/detector_registry/subscriptions.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/detector_registry/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/detector_registry/types.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/detector_registry/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/endpoint_command_manager/__init__.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/endpoint_command_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/endpoint_command_manager/mutations.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/endpoint_command_manager/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/endpoint_command_manager/queries.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/endpoint_command_manager/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/endpoint_command_manager/subscriptions.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/endpoint_command_manager/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/endpoint_command_manager/types.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/endpoint_command_manager/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/endpoint_management_service/__init__.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/endpoint_management_service/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/endpoint_management_service/mutations.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/endpoint_management_service/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/endpoint_management_service/queries.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/endpoint_management_service/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/endpoint_management_service/subscriptions.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/endpoint_management_service/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/endpoint_management_service/types.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/endpoint_management_service/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/event_search/__init__.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/event_search/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/event_search/mutations.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/event_search/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/event_search/queries.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/event_search/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/event_search/subscriptions.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/event_search/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/event_search/types.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/event_search/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/events/__init__.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/events/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/events/mutations.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/events/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/events/queries.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/events/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/events/subscriptions.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/events/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/events/types.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/events/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/exports/__init__.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/exports/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/exports/mutations.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/exports/mutations.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,14 +30,18 @@
     def __init__(self, service: ExportsService):
         self.service = service
 
     def new_export(self, input_: NewExportInput) -> Export:
         """None."""
         endpoint = "newExport"
 
+        log.warning(
+            f"GraphQL Mutation `{endpoint}` is deprecated: 'Migration to V2 backend; Use 'createReportSpecV2''"
+        )
+
         result = self.service.execute_mutation(
             endpoint=endpoint,
             variables={
                 "input": prepare_input(input_),
             },
             output=build_output_string(Export),
         )
@@ -45,14 +49,18 @@
             return Export.from_dict(result.get(endpoint))
         raise GraphQLNoRowsInResultSetError("for mutation newExport")
 
     def cancel_export(self, input_: str) -> Export:
         """None."""
         endpoint = "cancelExport"
 
+        log.warning(
+            f"GraphQL Mutation `{endpoint}` is deprecated: 'Migration to V2 backend; Use 'cancelReportArtifactV2''"
+        )
+
         result = self.service.execute_mutation(
             endpoint=endpoint,
             variables={
                 "input": prepare_input(input_),
             },
             output=build_output_string(Export),
         )
@@ -60,14 +68,18 @@
             return Export.from_dict(result.get(endpoint))
         raise GraphQLNoRowsInResultSetError("for mutation cancelExport")
 
     def delete_export(self, id_: str) -> Export:
         """None."""
         endpoint = "deleteExport"
 
+        log.warning(
+            f"GraphQL Mutation `{endpoint}` is deprecated: 'Migration to V2 backend; Use 'deleteReportArtifactV2''"
+        )
+
         result = self.service.execute_mutation(
             endpoint=endpoint,
             variables={
                 "id": prepare_input(id_),
             },
             output=build_output_string(Export),
         )
@@ -75,14 +87,18 @@
             return Export.from_dict(result.get(endpoint))
         raise GraphQLNoRowsInResultSetError("for mutation deleteExport")
 
     def retry_export(self, id_: str) -> Export:
         """None."""
         endpoint = "retryExport"
 
+        log.warning(
+            f"GraphQL Mutation `{endpoint}` is deprecated: 'Migration to V2 backend; Use 'retryReportArtifactV2''"
+        )
+
         result = self.service.execute_mutation(
             endpoint=endpoint,
             variables={
                 "id": prepare_input(id_),
             },
             output=build_output_string(Export),
         )
```

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/exports/queries.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/exports/queries.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,14 +32,18 @@
 
     def all_exports(
         self, include_connected_exports: Optional[bool] = None
     ) -> List[Export]:
         """None."""
         endpoint = "allExports"
 
+        log.warning(
+            f"GraphQL Query `{endpoint}` is deprecated: 'Migration to V2 backend; Use 'searchReportsV2''"
+        )
+
         result = self.service.execute_query(
             endpoint=endpoint,
             variables={
                 "includeConnectedExports": prepare_input(include_connected_exports),
             },
             output=build_output_string(Export),
         )
@@ -49,14 +53,18 @@
             )
         raise GraphQLNoRowsInResultSetError("for query allExports")
 
     def single_export(self, id_: str) -> Export:
         """None."""
         endpoint = "singleExport"
 
+        log.warning(
+            f"GraphQL Query `{endpoint}` is deprecated: 'Migration to V2 backend; Use 'reportV2''"
+        )
+
         result = self.service.execute_query(
             endpoint=endpoint,
             variables={
                 "id": prepare_input(id_),
             },
             output=build_output_string(Export),
         )
@@ -64,14 +72,18 @@
             return Export.from_dict(result.get(endpoint))
         raise GraphQLNoRowsInResultSetError("for query singleExport")
 
     def get_export_url(self, input_: str) -> str:
         """None."""
         endpoint = "getExportURL"
 
+        log.warning(
+            f"GraphQL Query `{endpoint}` is deprecated: 'Migration to V2 backend; Use 'downloadReportArtifactV2''"
+        )
+
         result = self.service.execute_query(
             endpoint=endpoint,
             variables={
                 "input": prepare_input(input_),
             },
             output="",
         )
```

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/exports/subscriptions.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/exports/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/exports/types.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/exports/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,16 +26,18 @@
     ERRORED = "Errored"
     PAUSED = "Paused"
 
 
 class RelativeTimeRange(str, Enum):
     """RelativeTimeRange."""
 
-    LAST_MONTH = "LAST_MONTH"
     CURRENT_MONTH_TO_DATE = "CURRENT_MONTH_TO_DATE"
+    LAST_MONTH = "LAST_MONTH"
+    LAST_QUARTER = "LAST_QUARTER"
+    LAST_YEAR = "LAST_YEAR"
 
 
 class ExportType(str, Enum):
     """ExportType."""
 
     CSV = "CSV"
     JSON = "JSON"
@@ -259,14 +261,17 @@
 class QueryWithTimeRangeInput:
     """QueryWithTimeRangeInput."""
 
     query: Optional[str] = field(default=None, metadata=config(field_name="query"))
     reference_time: Optional[str] = field(
         default=None, metadata=config(field_name="referenceTime")
     )
+    time_zone: Optional[str] = field(
+        default=None, metadata=config(field_name="timeZone")
+    )
     time_range: Optional[RelativeTimeRange] = field(
         default=None, metadata=config(field_name="timeRange")
     )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
```

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/fast_ioc/__init__.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/fast_ioc/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/fast_ioc/mutations.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/fast_ioc/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/fast_ioc/queries.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/fast_ioc/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/fast_ioc/subscriptions.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/fast_ioc/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/fast_ioc/types.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/fast_ioc/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/file_info/__init__.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/file_info/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/file_info/mutations.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/file_info/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/file_info/queries.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/threat/mutations.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""FileInfo Query."""
+"""Threat Mutation."""
 # pylint: disable=no-member, unused-argument, too-many-locals, duplicate-code, wildcard-import, unused-wildcard-import, cyclic-import
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
@@ -12,82 +12,50 @@
 
 from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
     parse_union_result,
     prepare_input,
 )
-from taegis_sdk_python.services.file_info.types import *
+from taegis_sdk_python.services.threat.types import *
 
 if TYPE_CHECKING:  # pragma: no cover
-    from taegis_sdk_python.services.file_info import FileInfoService
+    from taegis_sdk_python.services.threat import ThreatService
 
 log = logging.getLogger(__name__)
 
 
-class TaegisSDKFileInfoQuery:
-    """Taegis File_info Query operations."""
+class TaegisSDKThreatMutation:
+    """Taegis Threat Mutation operations."""
 
-    def __init__(self, service: FileInfoService):
+    def __init__(self, service: ThreatService):
         self.service = service
 
-    def file_info(self, file_hash: str) -> File:
+    def indicator(self, id_: str) -> ThreatIndicator:
         """None."""
-        endpoint = "fileInfo"
+        endpoint = "indicator"
 
-        result = self.service.execute_query(
+        result = self.service.execute_mutation(
             endpoint=endpoint,
             variables={
-                "fileHash": prepare_input(file_hash),
+                "id": prepare_input(id_),
             },
-            output=build_output_string(File),
+            output=build_output_string(ThreatIndicator),
         )
         if result.get(endpoint) is not None:
-            return File.from_dict(result.get(endpoint))
-        raise GraphQLNoRowsInResultSetError("for query fileInfo")
+            return ThreatIndicator.from_dict(result.get(endpoint))
+        raise GraphQLNoRowsInResultSetError("for mutation indicator")
 
-    def file_info_counts(self, file_hash: str) -> FileCounts:
-        """None."""
-        endpoint = "fileInfoCounts"
-
-        result = self.service.execute_query(
-            endpoint=endpoint,
-            variables={
-                "fileHash": prepare_input(file_hash),
-            },
-            output=build_output_string(FileCounts),
-        )
-        if result.get(endpoint) is not None:
-            return FileCounts.from_dict(result.get(endpoint))
-        raise GraphQLNoRowsInResultSetError("for query fileInfoCounts")
-
-    def search_file_info(self, query: str) -> List[File]:
-        """None."""
-        endpoint = "searchFileInfo"
-
-        result = self.service.execute_query(
-            endpoint=endpoint,
-            variables={
-                "query": prepare_input(query),
-            },
-            output=build_output_string(File),
-        )
-        if result.get(endpoint) is not None:
-            return File.schema().load(
-                [r or {} for r in result.get(endpoint)], many=True
-            )
-        raise GraphQLNoRowsInResultSetError("for query searchFileInfo")
-
-    def file_info_exists(self, file_hash: str) -> bool:
-        """None."""
-        endpoint = "fileInfoExists"
+    def threat_delete_document(self, id_: str) -> bool:
+        """threatDeleteDocument is used to delete a document by id in the configured index."""
+        endpoint = "threatDeleteDocument"
 
-        result = self.service.execute_query(
+        result = self.service.execute_mutation(
             endpoint=endpoint,
             variables={
-                "fileHash": prepare_input(file_hash),
+                "id": prepare_input(id_),
             },
             output="",
         )
         if result.get(endpoint) is not None:
             return result.get(endpoint)
-        raise GraphQLNoRowsInResultSetError("for query fileInfoExists")
+        raise GraphQLNoRowsInResultSetError("for mutation threatDeleteDocument")
```

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/file_info/subscriptions.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/file_info/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/file_info/types.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/file_info/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/investigations/__init__.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/investigations/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/investigations/mutations.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/investigations/mutations.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,14 +30,18 @@
     def __init__(self, service: InvestigationsService):
         self.service = service
 
     def create_investigation(self, investigation: InvestigationInput) -> Investigation:
         """Create new investigation."""
         endpoint = "createInvestigation"
 
+        log.warning(
+            f"GraphQL Mutation `{endpoint}` is deprecated: 'Use the createInvestigationV2 mutation'"
+        )
+
         result = self.service.execute_mutation(
             endpoint=endpoint,
             variables={
                 "investigation": prepare_input(investigation),
             },
             output=build_output_string(Investigation),
         )
@@ -47,14 +51,18 @@
 
     def update_investigation(
         self, investigation_id: str, investigation: UpdateInvestigationInput
     ) -> Investigation:
         """Update investigation."""
         endpoint = "updateInvestigation"
 
+        log.warning(
+            f"GraphQL Mutation `{endpoint}` is deprecated: 'Use the updateInvestigationV2 mutation'"
+        )
+
         result = self.service.execute_mutation(
             endpoint=endpoint,
             variables={
                 "investigation_id": prepare_input(investigation_id),
                 "investigation": prepare_input(investigation),
             },
             output=build_output_string(Investigation),
@@ -63,14 +71,18 @@
             return Investigation.from_dict(result.get(endpoint))
         raise GraphQLNoRowsInResultSetError("for mutation updateInvestigation")
 
     def archive_investigation(self, investigation_id: str) -> Investigation:
         """Archive investigation."""
         endpoint = "archiveInvestigation"
 
+        log.warning(
+            f"GraphQL Mutation `{endpoint}` is deprecated: 'Use the archiveInvestigationV2 mutation'"
+        )
+
         result = self.service.execute_mutation(
             endpoint=endpoint,
             variables={
                 "investigation_id": prepare_input(investigation_id),
             },
             output=build_output_string(Investigation),
         )
@@ -78,14 +90,18 @@
             return Investigation.from_dict(result.get(endpoint))
         raise GraphQLNoRowsInResultSetError("for mutation archiveInvestigation")
 
     def bulk_archive_investigations(self, ids: List[str]) -> List[str]:
         """Bulk Archive Investigations."""
         endpoint = "bulkArchiveInvestigations"
 
+        log.warning(
+            f"GraphQL Mutation `{endpoint}` is deprecated: 'Use the archiveInvestigationsV2 mutation'"
+        )
+
         result = self.service.execute_mutation(
             endpoint=endpoint,
             variables={
                 "ids": prepare_input(ids),
             },
             output="",
         )
@@ -93,14 +109,18 @@
             return result.get(endpoint)
         raise GraphQLNoRowsInResultSetError("for mutation bulkArchiveInvestigations")
 
     def un_archive_investigation(self, investigation_id: str) -> Investigation:
         """UnArchive Investigation."""
         endpoint = "unArchiveInvestigation"
 
+        log.warning(
+            f"GraphQL Mutation `{endpoint}` is deprecated: 'Use the unarchiveInvestigationV2 mutation'"
+        )
+
         result = self.service.execute_mutation(
             endpoint=endpoint,
             variables={
                 "investigation_id": prepare_input(investigation_id),
             },
             output=build_output_string(Investigation),
         )
@@ -108,14 +128,18 @@
             return Investigation.from_dict(result.get(endpoint))
         raise GraphQLNoRowsInResultSetError("for mutation unArchiveInvestigation")
 
     def bulk_un_archive_investigations(self, ids: List[str]) -> List[str]:
         """Bulk UnArchive Investigations."""
         endpoint = "bulkUnArchiveInvestigations"
 
+        log.warning(
+            f"GraphQL Mutation `{endpoint}` is deprecated: 'Use the unarchiveInvestigationsV2 mutation'"
+        )
+
         result = self.service.execute_mutation(
             endpoint=endpoint,
             variables={
                 "ids": prepare_input(ids),
             },
             output="",
         )
@@ -149,14 +173,18 @@
 
     def add_assets_to_investigation(
         self, investigation_id: str, assets: List[str]
     ) -> Investigation:
         """Add assets to investigation."""
         endpoint = "addAssetsToInvestigation"
 
+        log.warning(
+            f"GraphQL Mutation `{endpoint}` is deprecated: 'Use the addEvidenceToInvestigation mutation'"
+        )
+
         result = self.service.execute_mutation(
             endpoint=endpoint,
             variables={
                 "investigation_id": prepare_input(investigation_id),
                 "assets": prepare_input(assets),
             },
             output=build_output_string(Investigation),
@@ -167,14 +195,18 @@
 
     def add_events_to_investigation(
         self, investigation_id: str, events: List[str]
     ) -> Investigation:
         """Add events to investigation."""
         endpoint = "addEventsToInvestigation"
 
+        log.warning(
+            f"GraphQL Mutation `{endpoint}` is deprecated: 'Use the addEvidenceToInvestigation mutation'"
+        )
+
         result = self.service.execute_mutation(
             endpoint=endpoint,
             variables={
                 "investigation_id": prepare_input(investigation_id),
                 "events": prepare_input(events),
             },
             output=build_output_string(Investigation),
@@ -185,14 +217,18 @@
 
     def add_alerts_to_investigation(
         self, investigation_id: str, alerts: List[str]
     ) -> Investigation:
         """Add alerts to investigation."""
         endpoint = "addAlertsToInvestigation"
 
+        log.warning(
+            f"GraphQL Mutation `{endpoint}` is deprecated: 'Use the addEvidenceToInvestigation mutation'"
+        )
+
         result = self.service.execute_mutation(
             endpoint=endpoint,
             variables={
                 "investigation_id": prepare_input(investigation_id),
                 "alerts": prepare_input(alerts),
             },
             output=build_output_string(Investigation),
@@ -203,14 +239,18 @@
 
     def add_genesis_events_to_investigation(
         self, investigation_id: str, genesis_events: List[str]
     ) -> Investigation:
         """Add genesis events to investigation."""
         endpoint = "addGenesisEventsToInvestigation"
 
+        log.warning(
+            f"GraphQL Mutation `{endpoint}` is deprecated: 'Use the addEvidenceToInvestigation mutation'"
+        )
+
         result = self.service.execute_mutation(
             endpoint=endpoint,
             variables={
                 "investigation_id": prepare_input(investigation_id),
                 "genesis_events": prepare_input(genesis_events),
             },
             output=build_output_string(Investigation),
@@ -223,14 +263,18 @@
 
     def add_genesis_alerts_to_investigation(
         self, investigation_id: str, genesis_alerts: List[str]
     ) -> Investigation:
         """Add genesis alerts to investigation."""
         endpoint = "addGenesisAlertsToInvestigation"
 
+        log.warning(
+            f"GraphQL Mutation `{endpoint}` is deprecated: 'Use the addEvidenceToInvestigation mutation'"
+        )
+
         result = self.service.execute_mutation(
             endpoint=endpoint,
             variables={
                 "investigation_id": prepare_input(investigation_id),
                 "genesis_alerts": prepare_input(genesis_alerts),
             },
             output=build_output_string(Investigation),
@@ -243,14 +287,18 @@
 
     def add_auth_credentials_to_investigation(
         self, investigation_id: str, auth_credentials: List[str]
     ) -> Investigation:
         """Add auth credentials to investigation."""
         endpoint = "addAuthCredentialsToInvestigation"
 
+        log.warning(
+            f"GraphQL Mutation `{endpoint}` is deprecated: 'Use the addEvidenceToInvestigation mutation'"
+        )
+
         result = self.service.execute_mutation(
             endpoint=endpoint,
             variables={
                 "investigation_id": prepare_input(investigation_id),
                 "auth_credentials": prepare_input(auth_credentials),
             },
             output=build_output_string(Investigation),
@@ -263,14 +311,18 @@
 
     def add_search_queries_to_investigation(
         self, investigation_id: str, search_queries: List[str]
     ) -> Investigation:
         """Add search queries to investigation."""
         endpoint = "addSearchQueriesToInvestigation"
 
+        log.warning(
+            f"GraphQL Mutation `{endpoint}` is deprecated: 'Use the addEvidenceToInvestigation mutation'"
+        )
+
         result = self.service.execute_mutation(
             endpoint=endpoint,
             variables={
                 "investigation_id": prepare_input(investigation_id),
                 "search_queries": prepare_input(search_queries),
             },
             output=build_output_string(Investigation),
@@ -287,14 +339,18 @@
         vector_name: str,
         created_at: Optional[str] = None,
         updated_at: Optional[str] = None,
     ) -> AccessVector:
         """Access Vectors."""
         endpoint = "addAccessVector"
 
+        log.warning(
+            f"GraphQL Mutation `{endpoint}` is deprecated: 'Not currently supported and may not be supported in the future.'"
+        )
+
         result = self.service.execute_mutation(
             endpoint=endpoint,
             variables={
                 "investigation_id": prepare_input(investigation_id),
                 "vectorName": prepare_input(vector_name),
                 "created_at": prepare_input(created_at),
                 "updated_at": prepare_input(updated_at),
@@ -305,14 +361,18 @@
             return AccessVector.from_dict(result.get(endpoint))
         raise GraphQLNoRowsInResultSetError("for mutation addAccessVector")
 
     def remove_access_vector(self, id_: str) -> AccessVector:
         """None."""
         endpoint = "removeAccessVector"
 
+        log.warning(
+            f"GraphQL Mutation `{endpoint}` is deprecated: 'Not currently supported and may not be supported in the future.'"
+        )
+
         result = self.service.execute_mutation(
             endpoint=endpoint,
             variables={
                 "id": prepare_input(id_),
             },
             output=build_output_string(AccessVector),
         )
@@ -322,14 +382,18 @@
 
     def remove_assets_from_investigation(
         self, investigation_id: str, assets: List[str]
     ) -> Investigation:
         """Remove assets from investigation."""
         endpoint = "removeAssetsFromInvestigation"
 
+        log.warning(
+            f"GraphQL Mutation `{endpoint}` is deprecated: 'Use the removeEvidenceFromInvestigation mutation'"
+        )
+
         result = self.service.execute_mutation(
             endpoint=endpoint,
             variables={
                 "investigation_id": prepare_input(investigation_id),
                 "assets": prepare_input(assets),
             },
             output=build_output_string(Investigation),
@@ -342,14 +406,18 @@
 
     def remove_events_from_investigation(
         self, investigation_id: str, events: List[str]
     ) -> Investigation:
         """Remove events from investigation."""
         endpoint = "removeEventsFromInvestigation"
 
+        log.warning(
+            f"GraphQL Mutation `{endpoint}` is deprecated: 'Use the removeEvidenceFromInvestigation mutation'"
+        )
+
         result = self.service.execute_mutation(
             endpoint=endpoint,
             variables={
                 "investigation_id": prepare_input(investigation_id),
                 "events": prepare_input(events),
             },
             output=build_output_string(Investigation),
@@ -362,14 +430,18 @@
 
     def remove_alerts_from_investigation(
         self, investigation_id: str, alerts: List[str]
     ) -> Investigation:
         """Remove alerts from investigation."""
         endpoint = "removeAlertsFromInvestigation"
 
+        log.warning(
+            f"GraphQL Mutation `{endpoint}` is deprecated: 'Use the removeEvidenceFromInvestigation mutation'"
+        )
+
         result = self.service.execute_mutation(
             endpoint=endpoint,
             variables={
                 "investigation_id": prepare_input(investigation_id),
                 "alerts": prepare_input(alerts),
             },
             output=build_output_string(Investigation),
@@ -382,14 +454,18 @@
 
     def remove_search_queries_from_investigation(
         self, investigation_id: str, search_queries: List[str]
     ) -> Investigation:
         """Remove search queries from investigation."""
         endpoint = "removeSearchQueriesFromInvestigation"
 
+        log.warning(
+            f"GraphQL Mutation `{endpoint}` is deprecated: 'Use the removeEvidenceFromInvestigation mutation'"
+        )
+
         result = self.service.execute_mutation(
             endpoint=endpoint,
             variables={
                 "investigation_id": prepare_input(investigation_id),
                 "search_queries": prepare_input(search_queries),
             },
             output=build_output_string(Investigation),
@@ -405,14 +481,18 @@
         search_query: str,
         investigation_id: Optional[str] = None,
         new_investigation: Optional[InvestigationInput] = None,
     ) -> Investigation:
         """Bulk add alerts to an investigation using restdb search query."""
         endpoint = "addBulkAlertsToInvestigation"
 
+        log.warning(
+            f"GraphQL Mutation `{endpoint}` is deprecated: 'Use the addEvidenceToInvestigation mutation'"
+        )
+
         result = self.service.execute_mutation(
             endpoint=endpoint,
             variables={
                 "investigation_id": prepare_input(investigation_id),
                 "new_investigation": prepare_input(new_investigation),
                 "search_query": prepare_input(search_query),
             },
@@ -424,14 +504,18 @@
 
     def add_bulk_alerts2_to_investigation(
         self, new_investigation: InvestigationInput, cql: str
     ) -> Investigation:
         """Bulk add alerts2 to an new investigation using cql query."""
         endpoint = "addBulkAlerts2ToInvestigation"
 
+        log.warning(
+            f"GraphQL Mutation `{endpoint}` is deprecated: 'Use the addEvidenceToInvestigation mutation'"
+        )
+
         result = self.service.execute_mutation(
             endpoint=endpoint,
             variables={
                 "new_investigation": prepare_input(new_investigation),
                 "cql": prepare_input(cql),
             },
             output=build_output_string(Investigation),
@@ -444,14 +528,18 @@
 
     def add_bulk_alerts2_to_existing_investigation(
         self, investigation_id: str, cql: str
     ) -> Investigation:
         """Bulk add alerts2 to an existing investigation using cql query."""
         endpoint = "addBulkAlerts2ToExistingInvestigation"
 
+        log.warning(
+            f"GraphQL Mutation `{endpoint}` is deprecated: 'Use the addEvidenceToInvestigation mutation'"
+        )
+
         result = self.service.execute_mutation(
             endpoint=endpoint,
             variables={
                 "investigation_id": prepare_input(investigation_id),
                 "cql": prepare_input(cql),
             },
             output=build_output_string(Investigation),
@@ -482,14 +570,18 @@
             "for mutation reProcessInvestigationBackgroundJob"
         )
 
     def delete_investigation(self, investigation_id: str) -> str:
         """Hard delete of investigation (Supported only in development environments)."""
         endpoint = "deleteInvestigation"
 
+        log.warning(
+            f"GraphQL Mutation `{endpoint}` is deprecated: 'Not supported - deleting investigations is not allowed'"
+        )
+
         result = self.service.execute_mutation(
             endpoint=endpoint,
             variables={
                 "investigation_id": prepare_input(investigation_id),
             },
             output="",
         )
@@ -497,14 +589,18 @@
             return result.get(endpoint)
         raise GraphQLNoRowsInResultSetError("for mutation deleteInvestigation")
 
     def acknowledge_investigation(self, investigation_id: str) -> str:
         """Update state_transitions table to acknowledge if current state is handoff, without changing the investigation itself."""
         endpoint = "acknowledgeInvestigation"
 
+        log.warning(
+            f"GraphQL Mutation `{endpoint}` is deprecated: 'Use the investigationV2 query'"
+        )
+
         result = self.service.execute_mutation(
             endpoint=endpoint,
             variables={
                 "investigation_id": prepare_input(investigation_id),
             },
             output="",
         )
@@ -512,14 +608,18 @@
             return result.get(endpoint)
         raise GraphQLNoRowsInResultSetError("for mutation acknowledgeInvestigation")
 
     def file_upload(self, input_: FileUploadInput) -> InvestigationFile:
         """Upload File for an investigation."""
         endpoint = "fileUpload"
 
+        log.warning(
+            f"GraphQL Mutation `{endpoint}` is deprecated: 'Use the initInvestigationFileUpload query'"
+        )
+
         result = self.service.execute_mutation(
             endpoint=endpoint,
             variables={
                 "input": prepare_input(input_),
             },
             output=build_output_string(InvestigationFile),
         )
@@ -527,14 +627,18 @@
             return InvestigationFile.from_dict(result.get(endpoint))
         raise GraphQLNoRowsInResultSetError("for mutation fileUpload")
 
     def delete_file(self, investigation_id: str, file_id: str) -> bool:
         """Delete investigation files from S3 bucket."""
         endpoint = "deleteFile"
 
+        log.warning(
+            f"GraphQL Mutation `{endpoint}` is deprecated: 'Use the deleteInvestigationFile query'"
+        )
+
         result = self.service.execute_mutation(
             endpoint=endpoint,
             variables={
                 "investigation_id": prepare_input(investigation_id),
                 "file_id": prepare_input(file_id),
             },
             output="",
@@ -543,14 +647,18 @@
             return result.get(endpoint)
         raise GraphQLNoRowsInResultSetError("for mutation deleteFile")
 
     def init_file_upload(self, input_: FileUploadRequest) -> FileUploadResponse:
         """Initialize file upload to get Presigned URL to upload file."""
         endpoint = "initFileUpload"
 
+        log.warning(
+            f"GraphQL Mutation `{endpoint}` is deprecated: 'Use the initInvestigationFileUpload query'"
+        )
+
         result = self.service.execute_mutation(
             endpoint=endpoint,
             variables={
                 "input": prepare_input(input_),
             },
             output=build_output_string(FileUploadResponse),
         )
@@ -560,14 +668,18 @@
 
     def update_file_status(
         self, investigation_id: str, file_id: str, status: str
     ) -> InvestigationFile:
         """Update investigation file  status."""
         endpoint = "updateFileStatus"
 
+        log.warning(
+            f"GraphQL Mutation `{endpoint}` is deprecated: 'No longer supported, migrate to the InvestigationsV2-API'"
+        )
+
         result = self.service.execute_mutation(
             endpoint=endpoint,
             variables={
                 "investigation_id": prepare_input(investigation_id),
                 "file_id": prepare_input(file_id),
                 "status": prepare_input(status),
             },
```

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/investigations/queries.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/investigations/queries.py`

 * *Files 17% similar despite different names*

```diff
@@ -30,14 +30,18 @@
     def __init__(self, service: InvestigationsService):
         self.service = service
 
     def investigation_summary(self) -> List[InvestigationSummary]:
         """Get summary of investigations (tag and counts for each tag)."""
         endpoint = "investigationSummary"
 
+        log.warning(
+            f"GraphQL Query `{endpoint}` is deprecated: 'No longer supported, migrate to the InvestigationsV2-API'"
+        )
+
         result = self.service.execute_query(
             endpoint=endpoint,
             variables={},
             output=build_output_string(InvestigationSummary),
         )
         if result.get(endpoint) is not None:
             return InvestigationSummary.schema().load(
@@ -45,14 +49,18 @@
             )
         raise GraphQLNoRowsInResultSetError("for query investigationSummary")
 
     def investigation(self, investigation_id: str) -> Investigation:
         """Get an investigation by id."""
         endpoint = "investigation"
 
+        log.warning(
+            f"GraphQL Query `{endpoint}` is deprecated: 'Use the investigationV2 query'"
+        )
+
         result = self.service.execute_query(
             endpoint=endpoint,
             variables={
                 "investigation_id": prepare_input(investigation_id),
             },
             output=build_output_string(Investigation),
         )
@@ -62,14 +70,18 @@
 
     def investigations(
         self, investigation_ids: Optional[List[str]] = None
     ) -> List[Investigation]:
         """Get investigations for the list of ids."""
         endpoint = "investigations"
 
+        log.warning(
+            f"GraphQL Query `{endpoint}` is deprecated: 'Use the investigationsV2 query'"
+        )
+
         result = self.service.execute_query(
             endpoint=endpoint,
             variables={
                 "investigation_ids": prepare_input(investigation_ids),
             },
             output=build_output_string(Investigation),
         )
@@ -96,15 +108,15 @@
         """Get all investigations
         Max perPage Value is 100. If requesting over 100, only the first 100 will be returned.
         deprecated: Use `investigationsSearch` for better investigations query experience..
         """
         endpoint = "allInvestigations"
 
         log.warning(
-            f"GraphQL Query `{endpoint}` is deprecated: 'replaced by investigationsSearch'"
+            f"GraphQL Query `{endpoint}` is deprecated: 'Use the investigationsV2 query'"
         )
 
         result = self.service.execute_query(
             endpoint=endpoint,
             variables={
                 "status": prepare_input(status),
                 "page": prepare_input(page),
@@ -133,14 +145,18 @@
         transition_status: Optional[str] = None,
         after: Optional[str] = None,
         before: Optional[str] = None,
     ) -> Count:
         """Get the number of investigations created during a given time frame. Can optionslly pass in a desired 'transition_status' (handoff, acknowledge, resolution)."""
         endpoint = "investigationCountOverTime"
 
+        log.warning(
+            f"GraphQL Query `{endpoint}` is deprecated: 'No longer supported, migrate to the InvestigationsV2-API'"
+        )
+
         result = self.service.execute_query(
             endpoint=endpoint,
             variables={
                 "transition_status": prepare_input(transition_status),
                 "after": prepare_input(after),
                 "before": prepare_input(before),
             },
@@ -155,14 +171,18 @@
         after: Optional[str] = None,
         before: Optional[str] = None,
         include_threat_hunt_types: Optional[bool] = None,
     ) -> TimeSummaryForGroup:
         """Get the average times it took to hand off, acknowledge, and resolve all investigations over the course of the period."""
         endpoint = "meanTimeSummaryOverPeriod"
 
+        log.warning(
+            f"GraphQL Query `{endpoint}` is deprecated: 'No longer supported, migrate to the InvestigationsV2-API'"
+        )
+
         result = self.service.execute_query(
             endpoint=endpoint,
             variables={
                 "after": prepare_input(after),
                 "before": prepare_input(before),
                 "includeThreatHuntTypes": prepare_input(include_threat_hunt_types),
             },
@@ -177,14 +197,18 @@
         investigation_id: str,
         page: Optional[int] = None,
         per_page: Optional[int] = None,
     ) -> InvestigationAssetOutput:
         """Get investigation assets by investigation id."""
         endpoint = "investigationAssets"
 
+        log.warning(
+            f"GraphQL Query `{endpoint}` is deprecated: 'No longer supported, migrate to the InvestigationsV2-API'"
+        )
+
         result = self.service.execute_query(
             endpoint=endpoint,
             variables={
                 "investigation_id": prepare_input(investigation_id),
                 "page": prepare_input(page),
                 "perPage": prepare_input(per_page),
             },
@@ -199,14 +223,18 @@
         investigation_id: str,
         page: Optional[int] = None,
         per_page: Optional[int] = None,
     ) -> InvestigationEventOutput:
         """Get investigation events by investigation id."""
         endpoint = "investigationEvents"
 
+        log.warning(
+            f"GraphQL Query `{endpoint}` is deprecated: 'No longer supported, migrate to the InvestigationsV2-API'"
+        )
+
         result = self.service.execute_query(
             endpoint=endpoint,
             variables={
                 "investigation_id": prepare_input(investigation_id),
                 "page": prepare_input(page),
                 "perPage": prepare_input(per_page),
             },
@@ -226,14 +254,18 @@
         order_direction: Optional[OrderDirection] = None,
     ) -> InvestigationAlertOutput:
         """Get investigation alerts by investigation id
         deprecated: Use `investigation` query or alerts2 search query (paginated) to get alerts by investigation id.
         """
         endpoint = "investigationAlerts"
 
+        log.warning(
+            f"GraphQL Query `{endpoint}` is deprecated: 'No longer supported, migrate to the InvestigationsV2-API'"
+        )
+
         result = self.service.execute_query(
             endpoint=endpoint,
             variables={
                 "investigation_id": prepare_input(investigation_id),
                 "page": prepare_input(page),
                 "perPage": prepare_input(per_page),
                 "filterQuery": prepare_input(filter_query),
@@ -246,14 +278,18 @@
             return InvestigationAlertOutput.from_dict(result.get(endpoint))
         raise GraphQLNoRowsInResultSetError("for query investigationAlerts")
 
     def investigation_genesis_events(self, investigation_id: str) -> List[Event]:
         """Get investigation genesis events by investigation id."""
         endpoint = "investigationGenesisEvents"
 
+        log.warning(
+            f"GraphQL Query `{endpoint}` is deprecated: 'No longer supported, migrate to the InvestigationsV2-API'"
+        )
+
         result = self.service.execute_query(
             endpoint=endpoint,
             variables={
                 "investigation_id": prepare_input(investigation_id),
             },
             output=build_output_string(Event),
         )
@@ -263,14 +299,18 @@
             )
         raise GraphQLNoRowsInResultSetError("for query investigationGenesisEvents")
 
     def investigation_genesis_alerts(self, investigation_id: str) -> List[Alert]:
         """Get investigation genesis alerts by investigation id."""
         endpoint = "investigationGenesisAlerts"
 
+        log.warning(
+            f"GraphQL Query `{endpoint}` is deprecated: 'No longer supported, migrate to the InvestigationsV2-API'"
+        )
+
         result = self.service.execute_query(
             endpoint=endpoint,
             variables={
                 "investigation_id": prepare_input(investigation_id),
             },
             output=build_output_string(Alert),
         )
@@ -280,14 +320,18 @@
             )
         raise GraphQLNoRowsInResultSetError("for query investigationGenesisAlerts")
 
     def investigation_auth_credentials(self, investigation_id: str) -> List[str]:
         """Get investigation auth credentials by investigation id."""
         endpoint = "investigationAuthCredentials"
 
+        log.warning(
+            f"GraphQL Query `{endpoint}` is deprecated: 'No longer supported, migrate to the InvestigationsV2-API'"
+        )
+
         result = self.service.execute_query(
             endpoint=endpoint,
             variables={
                 "investigation_id": prepare_input(investigation_id),
             },
             output="",
         )
@@ -295,14 +339,18 @@
             return result.get(endpoint)
         raise GraphQLNoRowsInResultSetError("for query investigationAuthCredentials")
 
     def investigation_search_queries(self, investigation_id: str) -> List[SearchQuery]:
         """Get investigation search queries by investigation id."""
         endpoint = "investigationSearchQueries"
 
+        log.warning(
+            f"GraphQL Query `{endpoint}` is deprecated: 'No longer supported, migrate to the InvestigationsV2-API'"
+        )
+
         result = self.service.execute_query(
             endpoint=endpoint,
             variables={
                 "investigation_id": prepare_input(investigation_id),
             },
             output=build_output_string(SearchQuery),
         )
@@ -314,14 +362,18 @@
 
     def investigations_bulk_events_alerts(
         self, query_strings: List[str]
     ) -> List[InvestigationBulkResponse]:
         """Get investigations by quering a string on events/alerts/genesis events/genesis alerts fields."""
         endpoint = "investigationsBulkEventsAlerts"
 
+        log.warning(
+            f"GraphQL Query `{endpoint}` is deprecated: 'No longer supported, migrate to the InvestigationsV2-API'"
+        )
+
         result = self.service.execute_query(
             endpoint=endpoint,
             variables={
                 "queryStrings": prepare_input(query_strings),
             },
             output=build_output_string(InvestigationBulkResponse),
         )
@@ -331,25 +383,33 @@
             )
         raise GraphQLNoRowsInResultSetError("for query investigationsBulkEventsAlerts")
 
     def investigations_bulk_update_alerts(self) -> str:
         """Updates Investigation Alerts and Investigation information from Alerts (ie Access Vectors)."""
         endpoint = "investigationsBulkUpdateAlerts"
 
+        log.warning(
+            f"GraphQL Query `{endpoint}` is deprecated: 'No longer supported, migrate to the InvestigationsV2-API'"
+        )
+
         result = self.service.execute_query(endpoint=endpoint, variables={}, output="")
         if result.get(endpoint) is not None:
             return result.get(endpoint)
         raise GraphQLNoRowsInResultSetError("for query investigationsBulkUpdateAlerts")
 
     def investigation_status_summary(
         self, updated_after: Optional[str] = None, updated_before: Optional[str] = None
     ) -> List[SummaryGroup]:
         """Get summary of investigations and status filtered by updated_at."""
         endpoint = "investigationStatusSummary"
 
+        log.warning(
+            f"GraphQL Query `{endpoint}` is deprecated: 'No longer supported, migrate to the InvestigationsV2-API'"
+        )
+
         result = self.service.execute_query(
             endpoint=endpoint,
             variables={
                 "updatedAfter": prepare_input(updated_after),
                 "updatedBefore": prepare_input(updated_before),
             },
             output=build_output_string(SummaryGroup),
@@ -371,14 +431,18 @@
     ) -> InvestigationsOutput:
         """Investigations Search.
         Query fields accepts a CQL string (non aggregations). Use filterText for free text search.
         Max perPage Value is 100. If requesting over 100, only the first 100 will be returned..
         """
         endpoint = "investigationsSearch"
 
+        log.warning(
+            f"GraphQL Query `{endpoint}` is deprecated: 'Use the investigationsV2 query'"
+        )
+
         result = self.service.execute_query(
             endpoint=endpoint,
             variables={
                 "page": prepare_input(page),
                 "perPage": prepare_input(per_page),
                 "query": prepare_input(query),
                 "filterText": prepare_input(filter_text),
@@ -391,14 +455,18 @@
             return InvestigationsOutput.from_dict(result.get(endpoint))
         raise GraphQLNoRowsInResultSetError("for query investigationsSearch")
 
     def investigations_advanced_search(self, cql: str) -> List[Dict[str, Any]]:
         """Investigations Advanced Search can perform aggregations/sorting/filtering on investigations using CQL."""
         endpoint = "investigationsAdvancedSearch"
 
+        log.warning(
+            f"GraphQL Query `{endpoint}` is deprecated: 'Use the investigationsV2 query'"
+        )
+
         result = self.service.execute_query(
             endpoint=endpoint,
             variables={
                 "cql": prepare_input(cql),
             },
             output="",
         )
@@ -408,14 +476,18 @@
 
     def investigation_processing_status(
         self, investigation_id: str
     ) -> InvestigationProcessingResponse:
         """Get investigation processing status by id."""
         endpoint = "investigationProcessingStatus"
 
+        log.warning(
+            f"GraphQL Query `{endpoint}` is deprecated: 'No longer supported, migrate to the InvestigationsV2-API'"
+        )
+
         result = self.service.execute_query(
             endpoint=endpoint,
             variables={
                 "investigation_id": prepare_input(investigation_id),
             },
             output=build_output_string(InvestigationProcessingResponse),
         )
@@ -423,14 +495,18 @@
             return InvestigationProcessingResponse.from_dict(result.get(endpoint))
         raise GraphQLNoRowsInResultSetError("for query investigationProcessingStatus")
 
     def get_false_positives(self, after: str, before: str) -> Dict[str, Any]:
         """MDR - false positives widget."""
         endpoint = "getFalsePositives"
 
+        log.warning(
+            f"GraphQL Query `{endpoint}` is deprecated: 'No longer supported, migrate to the InvestigationsV2-API'"
+        )
+
         result = self.service.execute_query(
             endpoint=endpoint,
             variables={
                 "after": prepare_input(after),
                 "before": prepare_input(before),
             },
             output="",
@@ -439,14 +515,18 @@
             return result.get(endpoint)
         raise GraphQLNoRowsInResultSetError("for query getFalsePositives")
 
     def investigations_count(self, query: Optional[str] = None) -> int:
         """Get aggregated investigations counts based on CQL query."""
         endpoint = "investigationsCount"
 
+        log.warning(
+            f"GraphQL Query `{endpoint}` is deprecated: 'No longer supported, migrate to the InvestigationsV2-API'"
+        )
+
         result = self.service.execute_query(
             endpoint=endpoint,
             variables={
                 "query": prepare_input(query),
             },
             output="",
         )
@@ -454,14 +534,18 @@
             return result.get(endpoint)
         raise GraphQLNoRowsInResultSetError("for query investigationsCount")
 
     def investigations_status_count(self) -> InvestigationStatusCountResponse:
         """Get aggregated investigations status counts."""
         endpoint = "investigationsStatusCount"
 
+        log.warning(
+            f"GraphQL Query `{endpoint}` is deprecated: 'No longer supported, migrate to the InvestigationsV2-API'"
+        )
+
         result = self.service.execute_query(
             endpoint=endpoint,
             variables={},
             output=build_output_string(InvestigationStatusCountResponse),
         )
         if result.get(endpoint) is not None:
             return InvestigationStatusCountResponse.from_dict(result.get(endpoint))
@@ -477,14 +561,18 @@
         order_direction: Optional[OrderDirectionInput] = None,
     ) -> InvestigationsExportOutput:
         """Export investigations Search Raw Content
         Max perPage Value is 100. If requesting over 100, only the first 100 will be returned..
         """
         endpoint = "exportInvestigationsSearch"
 
+        log.warning(
+            f"GraphQL Query `{endpoint}` is deprecated: 'Use the investigationsV2 query'"
+        )
+
         result = self.service.execute_query(
             endpoint=endpoint,
             variables={
                 "page": prepare_input(page),
                 "perPage": prepare_input(per_page),
                 "query": prepare_input(query),
                 "filterText": prepare_input(filter_text),
@@ -497,14 +585,18 @@
             return InvestigationsExportOutput.from_dict(result.get(endpoint))
         raise GraphQLNoRowsInResultSetError("for query exportInvestigationsSearch")
 
     def investigation_file(self, file_id: str) -> InvestigationFile:
         """Get investigation file details."""
         endpoint = "investigationFile"
 
+        log.warning(
+            f"GraphQL Query `{endpoint}` is deprecated: 'Use the investigationFileV2 query'"
+        )
+
         result = self.service.execute_query(
             endpoint=endpoint,
             variables={
                 "file_id": prepare_input(file_id),
             },
             output=build_output_string(InvestigationFile),
         )
@@ -512,14 +604,18 @@
             return InvestigationFile.from_dict(result.get(endpoint))
         raise GraphQLNoRowsInResultSetError("for query investigationFile")
 
     def investigation_files(self, investigation_id: str) -> List[InvestigationFile]:
         """Get investigation files details."""
         endpoint = "investigationFiles"
 
+        log.warning(
+            f"GraphQL Query `{endpoint}` is deprecated: 'Use the investigationFilesV2 query'"
+        )
+
         result = self.service.execute_query(
             endpoint=endpoint,
             variables={
                 "investigation_id": prepare_input(investigation_id),
             },
             output=build_output_string(InvestigationFile),
         )
@@ -529,14 +625,18 @@
             )
         raise GraphQLNoRowsInResultSetError("for query investigationFiles")
 
     def download_investigation_file(self, investigation_id: str, file_id: str) -> str:
         """Presigned URL to Download investigation file."""
         endpoint = "downloadInvestigationFile"
 
+        log.warning(
+            f"GraphQL Query `{endpoint}` is deprecated: 'Use the investigationFileV2 query'"
+        )
+
         result = self.service.execute_query(
             endpoint=endpoint,
             variables={
                 "investigation_id": prepare_input(investigation_id),
                 "file_id": prepare_input(file_id),
             },
             output="",
@@ -554,15 +654,15 @@
         """Get investigations by multi-tenant session
         DO NOT USE, this query is unsupported. Use investigationsSearch instead.
         Max perPage Value is 100. If requesting over 100, only the first 100 will be returned..
         """
         endpoint = "investigationsBySession"
 
         log.warning(
-            f"GraphQL Query `{endpoint}` is deprecated: 'Not Supported - use investigationsSearch'"
+            f"GraphQL Query `{endpoint}` is deprecated: 'Use the investigationsV2 query'"
         )
 
         result = self.service.execute_query(
             endpoint=endpoint,
             variables={
                 "session_id": prepare_input(session_id),
                 "page": prepare_input(page),
@@ -586,14 +686,18 @@
         exclude_threat_hunt_types: Optional[bool] = None,
     ) -> InvestigationsOutput:
         """Return list of Investigations which are handed off at least once for the the given dates and status
         Max perPage Value is 100. If requesting over 100, only the first 100 will be returned..
         """
         endpoint = "getHandoffInvestigations"
 
+        log.warning(
+            f"GraphQL Query `{endpoint}` is deprecated: 'Use the investigationsV2 query'"
+        )
+
         result = self.service.execute_query(
             endpoint=endpoint,
             variables={
                 "page": prepare_input(page),
                 "perPage": prepare_input(per_page),
                 "createdAfter": prepare_input(created_after),
                 "createdBefore": prepare_input(created_before),
@@ -608,14 +712,18 @@
             return InvestigationsOutput.from_dict(result.get(endpoint))
         raise GraphQLNoRowsInResultSetError("for query getHandoffInvestigations")
 
     def investigation_types(self) -> List[InvestigationKeyValuePair]:
         """Return investigation types list based on user."""
         endpoint = "investigationTypes"
 
+        log.warning(
+            f"GraphQL Query `{endpoint}` is deprecated: 'Use the investigationV2Types query'"
+        )
+
         result = self.service.execute_query(
             endpoint=endpoint,
             variables={},
             output=build_output_string(InvestigationKeyValuePair),
         )
         if result.get(endpoint) is not None:
             return InvestigationKeyValuePair.schema().load(
@@ -623,14 +731,18 @@
             )
         raise GraphQLNoRowsInResultSetError("for query investigationTypes")
 
     def investigation_status_list(self) -> List[InvestigationKeyValuePair]:
         """Return investigation status static list."""
         endpoint = "investigationStatusList"
 
+        log.warning(
+            f"GraphQL Query `{endpoint}` is deprecated: 'No longer supported, migrate to the InvestigationsV2-API enums'"
+        )
+
         result = self.service.execute_query(
             endpoint=endpoint,
             variables={},
             output=build_output_string(InvestigationKeyValuePair),
         )
         if result.get(endpoint) is not None:
             return InvestigationKeyValuePair.schema().load(
@@ -638,14 +750,18 @@
             )
         raise GraphQLNoRowsInResultSetError("for query investigationStatusList")
 
     def investigation_priority_list(self) -> List[InvestigationKeyValuePair]:
         """Return investigation priority static list."""
         endpoint = "investigationPriorityList"
 
+        log.warning(
+            f"GraphQL Query `{endpoint}` is deprecated: 'No longer supported, migrate to the InvestigationsV2-API enums'"
+        )
+
         result = self.service.execute_query(
             endpoint=endpoint,
             variables={},
             output=build_output_string(InvestigationKeyValuePair),
         )
         if result.get(endpoint) is not None:
             return InvestigationKeyValuePair.schema().load(
@@ -655,14 +771,18 @@
 
     def investigation_timeline(
         self, arguments: InvestigationTimelineArguments
     ) -> InvestigationTimeline:
         """Return investigation timeline."""
         endpoint = "investigationTimeline"
 
+        log.warning(
+            f"GraphQL Query `{endpoint}` is deprecated: 'Use the investigationV2Types query'"
+        )
+
         result = self.service.execute_query(
             endpoint=endpoint,
             variables={
                 "arguments": prepare_input(arguments),
             },
             output=build_output_string(InvestigationTimeline),
         )
@@ -672,14 +792,16 @@
 
     def investigation_entities(
         self, arguments: InvestigationEntitiesArguments
     ) -> InvestigationEntities:
         """Get an investigation by id."""
         endpoint = "investigationEntities"
 
+        log.warning(f"GraphQL Query `{endpoint}` is deprecated: 'No longer supported'")
+
         result = self.service.execute_query(
             endpoint=endpoint,
             variables={
                 "arguments": prepare_input(arguments),
             },
             output=build_output_string(InvestigationEntities),
         )
```

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/investigations/subscriptions.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/investigations/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/investigations/types.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/investigations/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/investigations2/__init__.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/investigations2/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/investigations2/mutations.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/investigations2/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/investigations2/queries.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/investigations2/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/investigations2/subscriptions.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/investigations2/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/investigations2/types.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/investigations2/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/mitre_attack_info/__init__.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/mitre_attack_info/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/mitre_attack_info/mutations.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/mitre_attack_info/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/mitre_attack_info/queries.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/mitre_attack_info/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/mitre_attack_info/subscriptions.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/mitre_attack_info/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/mitre_attack_info/types.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/mitre_attack_info/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/multi_tenant_context/__init__.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/multi_tenant_context/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/multi_tenant_context/mutations.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/multi_tenant_context/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/multi_tenant_context/queries.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/multi_tenant_context/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/multi_tenant_context/subscriptions.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/multi_tenant_context/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/multi_tenant_context/types.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/multi_tenant_context/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/multi_tenant_ioc/__init__.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/multi_tenant_ioc/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/multi_tenant_ioc/mutations.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/multi_tenant_ioc/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/multi_tenant_ioc/queries.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/multi_tenant_ioc/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/multi_tenant_ioc/subscriptions.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/multi_tenant_ioc/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/multi_tenant_ioc/types.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/multi_tenant_ioc/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/notebooks/__init__.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/notebooks/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/notebooks/mutations.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/notebooks/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/notebooks/queries.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/notebooks/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/notebooks/subscriptions.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/notebooks/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/notebooks/types.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/notebooks/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/notifications/__init__.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/notifications/mutations.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/notifications/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/notifications/queries.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/notifications/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/notifications/subscriptions.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/notifications/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/notifications/types.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/notifications/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/preferences/__init__.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/preferences/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/preferences/mutations.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/preferences/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/preferences/queries.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/preferences/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/preferences/subscriptions.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/preferences/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/preferences/types.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/preferences/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -228,15 +228,24 @@
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
 class UserPreferenceDictionary:
     """UserPreferenceDictionary."""
 
     id: Optional[str] = field(default=None, metadata=config(field_name="id"))
-    user_id: Optional[str] = field(default=None, metadata=config(field_name="userID"))
+    user_id: Optional[str] = field(
+        default=None,
+        metadata=config(
+            metadata={"deprecated": True, "deprecation_reason": "Use `taegisUserId`"},
+            field_name="userID",
+        ),
+    )
+    taegis_user_id: Optional[str] = field(
+        default=None, metadata=config(field_name="taegisUserID")
+    )
     category: Optional[str] = field(
         default=None, metadata=config(field_name="category")
     )
     sub_key: Optional[str] = field(default=None, metadata=config(field_name="subKey"))
     preferences: Optional[dict] = field(
         default=None, metadata=config(field_name="preferences")
     )
@@ -281,30 +290,48 @@
     id: Optional[str] = field(default=None, metadata=config(field_name="id"))
     created_at: Optional[str] = field(
         default=None, metadata=config(field_name="created_at")
     )
     updated_at: Optional[str] = field(
         default=None, metadata=config(field_name="updated_at")
     )
-    user_id: Optional[str] = field(default=None, metadata=config(field_name="user_id"))
+    user_id: Optional[str] = field(
+        default=None,
+        metadata=config(
+            metadata={"deprecated": True, "deprecation_reason": "Use `taegis_user_id`"},
+            field_name="user_id",
+        ),
+    )
+    taegis_user_id: Optional[str] = field(
+        default=None, metadata=config(field_name="taegis_user_id")
+    )
     key: Optional[str] = field(default=None, metadata=config(field_name="key"))
     environment: Optional[str] = field(
         default=None, metadata=config(field_name="environment")
     )
     preference_items: Optional[List[UserPreferenceItem]] = field(
         default=None, metadata=config(field_name="preference_items")
     )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
 class UserNotificationPreferencesResponse:
     """UserNotificationPreferencesResponse."""
 
-    user_id: Optional[str] = field(default=None, metadata=config(field_name="user_id"))
+    user_id: Optional[str] = field(
+        default=None,
+        metadata=config(
+            metadata={"deprecated": True, "deprecation_reason": "Use `taegis_user_id`"},
+            field_name="user_id",
+        ),
+    )
+    taegis_user_id: Optional[str] = field(
+        default=None, metadata=config(field_name="taegis_user_id")
+    )
     error: Optional[str] = field(default=None, metadata=config(field_name="error"))
     user_notification_preference: Optional[UserPreference] = field(
         default=None, metadata=config(field_name="user_notification_preference")
     )
 
 
 @dataclass_json
```

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/queries/__init__.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/queries/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/queries/mutations.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/queries/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/queries/queries.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/queries/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/queries/subscriptions.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/queries/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/queries/types.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/queries/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/roadrunner/__init__.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/roadrunner/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/roadrunner/mutations.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/roadrunner/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/roadrunner/queries.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/roadrunner/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/roadrunner/subscriptions.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/roadrunner/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/roadrunner/types.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/roadrunner/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/rules/__init__.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/rules/mutations.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/rules/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/rules/queries.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/rules/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/rules/subscriptions.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/rules/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/rules/types.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/rules/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,14 +87,33 @@
     """RuleSource."""
 
     WATCHLIST = "WATCHLIST"
     DETECTOR = "DETECTOR"
     CUSTOM = "CUSTOM"
 
 
+class AlertOrigin(str, Enum):
+    """AlertOrigin."""
+
+    INTERNAL = "INTERNAL"
+    CUSTOMER = "CUSTOMER"
+    EXTERNAL = "EXTERNAL"
+    PARTNER = "PARTNER"
+
+
+class AlertSeverity(str, Enum):
+    """AlertSeverity."""
+
+    INFO = "INFO"
+    LOW = "LOW"
+    MEDIUM = "MEDIUM"
+    HIGH = "HIGH"
+    CRITICAL = "CRITICAL"
+
+
 class RuleVisibility(str, Enum):
     """RuleVisibility."""
 
     VISIBLE = "visible"
     HIDDEN = "hidden"
 
 
@@ -649,14 +668,20 @@
     )
     result_visibility: Optional[RuleVisibility] = field(
         default=None, metadata=config(field_name="resultVisibility")
     )
     status: Optional[RuleResolutionStatus] = field(
         default=None, metadata=config(field_name="status")
     )
+    origin: Optional[AlertOrigin] = field(
+        default=None, metadata=config(field_name="origin")
+    )
+    alert_severity: Optional[AlertSeverity] = field(
+        default=None, metadata=config(field_name="alertSeverity")
+    )
     rule_source: Optional[RuleSource] = field(
         default=None, metadata=config(field_name="ruleSource")
     )
     rule_action: Optional[RuleAction] = field(
         default=None, metadata=config(field_name="ruleAction")
     )
     endpoint_platform: Optional[List[RuleEndpointPlatform]] = field(
@@ -729,14 +754,20 @@
     )
     result_visibility: Optional[RuleVisibility] = field(
         default=None, metadata=config(field_name="resultVisibility")
     )
     status: Optional[RuleResolutionStatus] = field(
         default=None, metadata=config(field_name="status")
     )
+    origin: Optional[AlertOrigin] = field(
+        default=None, metadata=config(field_name="origin")
+    )
+    alert_severity: Optional[AlertSeverity] = field(
+        default=None, metadata=config(field_name="alertSeverity")
+    )
     attack_categories_details: Optional[List[AttackCategoryDetail]] = field(
         default=None, metadata=config(field_name="attackCategoriesDetails")
     )
     endpoint_platform: Optional[List[RuleEndpointPlatform]] = field(
         default=None, metadata=config(field_name="endpointPlatform")
     )
     references: Optional[List[RuleReference]] = field(
```

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/sharelinks/__init__.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/sharelinks/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/sharelinks/mutations.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/sharelinks/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/sharelinks/queries.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/sharelinks/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/sharelinks/subscriptions.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/sharelinks/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/sharelinks/types.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/sharelinks/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/subjects/__init__.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/subjects/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/subjects/mutations.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/subjects/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/subjects/queries.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/subjects/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/subjects/subscriptions.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/subjects/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/subjects/types.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/subjects/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/tenant_profiles/__init__.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/tenant_profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/tenant_profiles/mutations.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/tenant_profiles/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/tenant_profiles/queries.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/tenant_profiles/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/tenant_profiles/subscriptions.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/tenant_profiles/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/tenant_profiles/types.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/tenant_profiles/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/tenants/__init__.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/tenants/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/tenants/mutations.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/tenants/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/tenants/queries.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/tenants/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/tenants/subscriptions.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/tenants/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/tenants/types.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/tenants/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/threat/__init__.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/threat/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/threat/mutations.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/contracted_endpoint/queries.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Threat Mutation."""
+"""ContractedEndpoint Query."""
 # pylint: disable=no-member, unused-argument, too-many-locals, duplicate-code, wildcard-import, unused-wildcard-import, cyclic-import
 
 
 # Autogenerated
 # DO NOT MODIFY
 
 from __future__ import annotations
@@ -12,50 +12,68 @@
 
 from taegis_sdk_python import GraphQLNoRowsInResultSetError
 from taegis_sdk_python.utils import (
     build_output_string,
     parse_union_result,
     prepare_input,
 )
-from taegis_sdk_python.services.threat.types import *
+from taegis_sdk_python.services.contracted_endpoint.types import *
 
 if TYPE_CHECKING:  # pragma: no cover
-    from taegis_sdk_python.services.threat import ThreatService
+    from taegis_sdk_python.services.contracted_endpoint import ContractedEndpointService
 
 log = logging.getLogger(__name__)
 
 
-class TaegisSDKThreatMutation:
-    """Taegis Threat Mutation operations."""
+class TaegisSDKContractedEndpointQuery:
+    """Taegis Contracted_endpoint Query operations."""
 
-    def __init__(self, service: ThreatService):
+    def __init__(self, service: ContractedEndpointService):
         self.service = service
 
-    def indicator(self, id_: str) -> ThreatIndicator:
+    def endpoint_count_for_tenant_id(
+        self, service_date: Optional[str] = None
+    ) -> ContractedEndpoints:
         """None."""
-        endpoint = "indicator"
+        endpoint = "endpointCountForTenantID"
 
-        result = self.service.execute_mutation(
+        result = self.service.execute_query(
             endpoint=endpoint,
             variables={
-                "id": prepare_input(id_),
+                "serviceDate": prepare_input(service_date),
             },
-            output=build_output_string(ThreatIndicator),
+            output=build_output_string(ContractedEndpoints),
         )
         if result.get(endpoint) is not None:
-            return ThreatIndicator.from_dict(result.get(endpoint))
-        raise GraphQLNoRowsInResultSetError("for mutation indicator")
+            return ContractedEndpoints.from_dict(result.get(endpoint))
+        raise GraphQLNoRowsInResultSetError("for query endpointCountForTenantID")
 
-    def threat_delete_document(self, id_: str) -> bool:
-        """threatDeleteDocument is used to delete a document by id in the configured index."""
-        endpoint = "threatDeleteDocument"
+    def project_ir_hours_for_tenant_id(self) -> float:
+        """None."""
+        endpoint = "projectIRHoursForTenantID"
+
+        result = self.service.execute_query(endpoint=endpoint, variables={}, output="")
+        if result.get(endpoint) is not None:
+            return result.get(endpoint)
+        raise GraphQLNoRowsInResultSetError("for query projectIRHoursForTenantID")
 
-        result = self.service.execute_mutation(
+    def get_historical_endpoint_count_for_tenant_id(
+        self, start_date: str, end_date: str
+    ) -> List[EndpointHistory]:
+        """None."""
+        endpoint = "getHistoricalEndpointCountForTenantID"
+
+        result = self.service.execute_query(
             endpoint=endpoint,
             variables={
-                "id": prepare_input(id_),
+                "startDate": prepare_input(start_date),
+                "endDate": prepare_input(end_date),
             },
-            output="",
+            output=build_output_string(EndpointHistory),
         )
         if result.get(endpoint) is not None:
-            return result.get(endpoint)
-        raise GraphQLNoRowsInResultSetError("for mutation threatDeleteDocument")
+            return EndpointHistory.schema().load(
+                [r or {} for r in result.get(endpoint)], many=True
+            )
+        raise GraphQLNoRowsInResultSetError(
+            "for query getHistoricalEndpointCountForTenantID"
+        )
```

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/threat/queries.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/threat/queries.py`

 * *Files 7% similar despite different names*

```diff
@@ -95,34 +95,14 @@
         )
         if result.get(endpoint) is not None:
             return ThreatPublication.schema().load(
                 [r or {} for r in result.get(endpoint)], many=True
             )
         raise GraphQLNoRowsInResultSetError("for query threatLatestPublications")
 
-    def threat_object_by_id(
-        self, id_: str, object_type: ThreatObjectType
-    ) -> ThreatResult:
-        """Gets an object by `id`, `name` or `sharing_id`.."""
-        endpoint = "threatObjectById"
-
-        log.warning(f"GraphQL Query `{endpoint}` is deprecated: 'No longer supported'")
-
-        result = self.service.execute_query(
-            endpoint=endpoint,
-            variables={
-                "id": prepare_input(id_),
-                "objectType": prepare_input(object_type),
-            },
-            output=build_output_string(ThreatResult),
-        )
-        if result.get(endpoint) is not None:
-            return parse_union_result(ThreatResult, result.get(endpoint))
-        raise GraphQLNoRowsInResultSetError("for query threatObjectById")
-
     def threat_identities_by_confidence(self, confidence: int) -> List[ThreatResult]:
         """Gets identities by confidence score.."""
         endpoint = "threatIdentitiesByConfidence"
 
         result = self.service.execute_query(
             endpoint=endpoint,
             variables={
@@ -130,53 +110,18 @@
             },
             output=build_output_string(ThreatResult),
         )
         if result.get(endpoint) is not None:
             return [parse_union_result(ThreatResult, r) for r in result.get(endpoint)]
         raise GraphQLNoRowsInResultSetError("for query threatIdentitiesByConfidence")
 
-    def threat_objects_related(self, source_id: str, target_id: str) -> bool:
-        """Checks if a relationship between source and target exists.."""
-        endpoint = "threatObjectsRelated"
-
-        log.warning(f"GraphQL Query `{endpoint}` is deprecated: 'No longer supported'")
-
-        result = self.service.execute_query(
-            endpoint=endpoint,
-            variables={
-                "sourceID": prepare_input(source_id),
-                "targetID": prepare_input(target_id),
-            },
-            output="",
-        )
-        if result.get(endpoint) is not None:
-            return result.get(endpoint)
-        raise GraphQLNoRowsInResultSetError("for query threatObjectsRelated")
-
-    def threat_get_related(self, source_id: str) -> List[ThreatResult]:
-        """Gets relationship(s) between source and target(s).."""
-        endpoint = "threatGetRelated"
-
-        log.warning(f"GraphQL Query `{endpoint}` is deprecated: 'No longer supported'")
-
-        result = self.service.execute_query(
-            endpoint=endpoint,
-            variables={
-                "sourceID": prepare_input(source_id),
-            },
-            output=build_output_string(ThreatResult),
-        )
-        if result.get(endpoint) is not None:
-            return [parse_union_result(ThreatResult, r) for r in result.get(endpoint)]
-        raise GraphQLNoRowsInResultSetError("for query threatGetRelated")
-
     def threat_watchlist(self, type_: ThreatParentType) -> List[ThreatRelationship]:
         """Gets a watchlist by type. All results are considered **high confidence**.
-        Only IP and DOMAIN types are supported. Used the paged service threatTimsMalwareFiles for FILE types..
-        """
+        Only IP and DOMAIN types are supported. FILE type has been removed from this endpoint.
+        Instead, use the paged endpoint threatTimsMalwareFiles for FILE types.."""
         endpoint = "threatWatchlist"
 
         result = self.service.execute_query(
             endpoint=endpoint,
             variables={
                 "type": prepare_input(type_),
             },
@@ -225,14 +170,31 @@
         )
         if result.get(endpoint) is not None:
             return ThreatReport.schema().load(
                 [r or {} for r in result.get(endpoint)], many=True
             )
         raise GraphQLNoRowsInResultSetError("for query threatIndicatorPublications")
 
+    def threat_publications_indicators(self, id_: List[str]) -> List[ThreatIndicator]:
+        """Get list of indicators related to list of publications."""
+        endpoint = "threatPublicationsIndicators"
+
+        result = self.service.execute_query(
+            endpoint=endpoint,
+            variables={
+                "ID": prepare_input(id_),
+            },
+            output=build_output_string(ThreatIndicator),
+        )
+        if result.get(endpoint) is not None:
+            return ThreatIndicator.schema().load(
+                [r or {} for r in result.get(endpoint)], many=True
+            )
+        raise GraphQLNoRowsInResultSetError("for query threatPublicationsIndicators")
+
     def threat_indicator_intelligence(self, id_: str) -> ThreatIndicatorIntelligence:
         """Retrieves all intelligence associated with an indicator.."""
         endpoint = "threatIndicatorIntelligence"
 
         result = self.service.execute_query(
             endpoint=endpoint,
             variables={
```

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/threat/subscriptions.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/threat/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/threat/types.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/threat/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 
 
 class ThreatParentType(str, Enum):
     """ThreatParentType."""
 
     IP = "IP"
     DOMAIN = "DOMAIN"
-    FILE = "FILE"
 
 
 class ThreatIndicatorClass(str, Enum):
     """ThreatIndicatorClass."""
 
     IPV4 = "ipv4"
     IPV6 = "ipv6"
```

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/threat_score/__init__.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/threat_score/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/threat_score/mutations.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/threat_score/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/threat_score/queries.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/threat_score/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/threat_score/subscriptions.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/threat_score/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/threat_score/types.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/threat_score/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/trip/__init__.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/trip/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/trip/mutations.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/trip/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/trip/queries.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/trip/queries.py`

 * *Files 13% similar despite different names*

```diff
@@ -95,22 +95,7 @@
                 "pageSize": prepare_input(page_size),
             },
             output=build_output_string(ApiIntegrationHistoryPage),
         )
         if result.get(endpoint) is not None:
             return ApiIntegrationHistoryPage.from_dict(result.get(endpoint))
         raise GraphQLNoRowsInResultSetError("for query listApiIntegrationHistory")
-
-    def get_api_integration_form(self, product_id: int) -> ApiForm:
-        """None."""
-        endpoint = "getApiIntegrationForm"
-
-        result = self.service.execute_query(
-            endpoint=endpoint,
-            variables={
-                "productId": prepare_input(product_id),
-            },
-            output=build_output_string(ApiForm),
-        )
-        if result.get(endpoint) is not None:
-            return ApiForm.from_dict(result.get(endpoint))
-        raise GraphQLNoRowsInResultSetError("for query getApiIntegrationForm")
```

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/trip/subscriptions.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/trip/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/trip/types.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/trip/types.py`

 * *Files 16% similar despite different names*

```diff
@@ -61,21 +61,14 @@
     """ApiFormItemType."""
 
     TEXT = "Text"
     TEXT_INPUT = "TextInput"
     OPTION = "Option"
 
 
-class ApiFormItemValidatorType(str, Enum):
-    """ApiFormItemValidatorType."""
-
-    PATTERN = "Pattern"
-    JSON = "Json"
-
-
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
 class ApiIntegrationParameterInput:
     """ApiIntegrationParameterInput."""
 
     name: Optional[str] = field(default=None, metadata=config(field_name="name"))
     value: Optional[str] = field(default=None, metadata=config(field_name="value"))
@@ -91,44 +84,20 @@
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
 class ApiIntegrationParameter:
     """ApiIntegrationParameter."""
 
     name: Optional[str] = field(default=None, metadata=config(field_name="name"))
+    caption: Optional[str] = field(default=None, metadata=config(field_name="caption"))
     value: Optional[str] = field(default=None, metadata=config(field_name="value"))
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
-class ApiFormItemOption:
-    """ApiFormItemOption."""
-
-    order: Optional[int] = field(default=None, metadata=config(field_name="order"))
-    code: Optional[str] = field(default=None, metadata=config(field_name="code"))
-    description: Optional[str] = field(
-        default=None, metadata=config(field_name="description")
-    )
-
-
-@dataclass_json
-@dataclass(order=True, eq=True, frozen=True)
-class ApiFormItemValidator:
-    """ApiFormItemValidator."""
-
-    parameter: Optional[str] = field(
-        default=None, metadata=config(field_name="parameter")
-    )
-    type: Optional[ApiFormItemValidatorType] = field(
-        default=None, metadata=config(field_name="type")
-    )
-
-
-@dataclass_json
-@dataclass(order=True, eq=True, frozen=True)
 class ApiIntegrationHistory:
     """ApiIntegrationHistory."""
 
     id: Optional[int] = field(default=None, metadata=config(field_name="id"))
     created_at: Optional[str] = field(
         default=None, metadata=config(field_name="createdAt")
     )
@@ -178,34 +147,16 @@
     )
     product: Optional[ApiProduct] = field(
         default=None, metadata=config(field_name="product")
     )
     status: Optional[ApiIntegrationHealthStatus] = field(
         default=None, metadata=config(field_name="status")
     )
-
-
-@dataclass_json
-@dataclass(order=True, eq=True, frozen=True)
-class ApiFormItem:
-    """ApiFormItem."""
-
-    order: Optional[int] = field(default=None, metadata=config(field_name="order"))
-    label: Optional[str] = field(default=None, metadata=config(field_name="label"))
-    caption: Optional[str] = field(default=None, metadata=config(field_name="caption"))
-    content: Optional[str] = field(default=None, metadata=config(field_name="content"))
-    secret: Optional[bool] = field(default=None, metadata=config(field_name="secret"))
-    type: Optional[ApiFormItemType] = field(
-        default=None, metadata=config(field_name="type")
-    )
-    options: Optional[List[ApiFormItemOption]] = field(
-        default=None, metadata=config(field_name="options")
-    )
-    validators: Optional[List[ApiFormItemValidator]] = field(
-        default=None, metadata=config(field_name="validators")
+    child_summaries: Optional[List["ApiIntegrationSummary"]] = field(
+        default=None, metadata=config(field_name="childSummaries")
     )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
 class ApiIntegration:
     """ApiIntegration."""
@@ -226,43 +177,27 @@
     )
     product: Optional[ApiProduct] = field(
         default=None, metadata=config(field_name="product")
     )
     parent_integration: Optional["ApiIntegration"] = field(
         default=None, metadata=config(field_name="parentIntegration")
     )
+    child_integrations: Optional[List["ApiIntegration"]] = field(
+        default=None, metadata=config(field_name="childIntegrations")
+    )
     status: Optional[ApiIntegrationStatus] = field(
         default=None, metadata=config(field_name="status")
     )
     parameters: Optional[List[ApiIntegrationParameter]] = field(
         default=None, metadata=config(field_name="parameters")
     )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
-class ApiForm:
-    """ApiForm."""
-
-    id: Optional[int] = field(default=None, metadata=config(field_name="id"))
-    active: Optional[bool] = field(default=None, metadata=config(field_name="active"))
-    title: Optional[str] = field(default=None, metadata=config(field_name="title"))
-    description: Optional[str] = field(
-        default=None, metadata=config(field_name="description")
-    )
-    product_id: Optional[int] = field(
-        default=None, metadata=config(field_name="productId")
-    )
-    items: Optional[List[ApiFormItem]] = field(
-        default=None, metadata=config(field_name="Items")
-    )
-
-
-@dataclass_json
-@dataclass(order=True, eq=True, frozen=True)
 class ApiIntegrationHistoryPage:
     """ApiIntegrationHistoryPage."""
 
     start_time: Optional[str] = field(
         default=None, metadata=config(field_name="startTime")
     )
     end_time: Optional[str] = field(default=None, metadata=config(field_name="endTime"))
```

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/users/__init__.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/users/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/users/mutations.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/users/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/users/queries.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/users/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/users/subscriptions.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/users/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/services/users/types.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/services/users/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -583,18 +583,43 @@
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
 class TDRUser:
     """TDRUser."""
 
     id: Optional[str] = field(default=None, metadata=config(field_name="id"))
-    id_uuid: Optional[str] = field(default=None, metadata=config(field_name="id_uuid"))
-    user_id: Optional[str] = field(default=None, metadata=config(field_name="user_id"))
+    idp_user_id: Optional[str] = field(
+        default=None, metadata=config(field_name="idp_user_id")
+    )
+    id_uuid: Optional[str] = field(
+        default=None,
+        metadata=config(
+            metadata={"deprecated": True, "deprecation_reason": "prefer `id`"},
+            field_name="id_uuid",
+        ),
+    )
+    user_id: Optional[str] = field(
+        default=None,
+        metadata=config(
+            metadata={
+                "deprecated": True,
+                "deprecation_reason": "will no longer be valid after migration to Cognito, migrate to `id`, or `idp_user_id` if the IDP ID is required",
+            },
+            field_name="user_id",
+        ),
+    )
     user_id_v1: Optional[str] = field(
-        default=None, metadata=config(field_name="user_id_v1")
+        default=None,
+        metadata=config(
+            metadata={
+                "deprecated": True,
+                "deprecation_reason": "superseded by `user_id`, which is also now deprecated",
+            },
+            field_name="user_id_v1",
+        ),
     )
     created_at: Optional[str] = field(
         default=None, metadata=config(field_name="created_at")
     )
     updated_at: Optional[str] = field(
         default=None, metadata=config(field_name="updated_at")
     )
```

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/tokens.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/tokens.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python/utils.py` & `taegis_sdk_python-1.2.6/taegis_sdk_python/utils.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python.egg-info/PKG-INFO` & `taegis_sdk_python-1.2.6/taegis_sdk_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taegis-sdk-python
-Version: 1.2.5
+Version: 1.2.6
 Summary: Taegis Python SDK
 Home-page: https://github.com/secureworks/taegis-sdk-python
 Author: Secureworks
 Author-email: sdks@secureworks.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,14 +17,15 @@
 Requires-Dist: oauthlib
 Requires-Dist: requests
 Requires-Dist: requests-oauthlib
 Requires-Dist: dataclasses-json
 Requires-Dist: pyjwt>=2.8.0
 Requires-Dist: requests-toolbelt
 Requires-Dist: websockets
+Requires-Dist: filelock>=3.12.4
 
 # Taegis SDK for Python
 
 The Taegis SDK is a Python library for interfacing with the GraphQL APIs in Taegis.
 
 ## Prerequisites
```

### Comparing `taegis-sdk-python-1.2.5/taegis_sdk_python.egg-info/SOURCES.txt` & `taegis_sdk_python-1.2.6/taegis_sdk_python.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -71,14 +71,19 @@
 taegis_sdk_python/services/collector/subscriptions.py
 taegis_sdk_python/services/collector/types.py
 taegis_sdk_python/services/comments/__init__.py
 taegis_sdk_python/services/comments/mutations.py
 taegis_sdk_python/services/comments/queries.py
 taegis_sdk_python/services/comments/subscriptions.py
 taegis_sdk_python/services/comments/types.py
+taegis_sdk_python/services/contracted_endpoint/__init__.py
+taegis_sdk_python/services/contracted_endpoint/mutations.py
+taegis_sdk_python/services/contracted_endpoint/queries.py
+taegis_sdk_python/services/contracted_endpoint/subscriptions.py
+taegis_sdk_python/services/contracted_endpoint/types.py
 taegis_sdk_python/services/datasources/__init__.py
 taegis_sdk_python/services/datasources/mutations.py
 taegis_sdk_python/services/datasources/queries.py
 taegis_sdk_python/services/datasources/subscriptions.py
 taegis_sdk_python/services/datasources/types.py
 taegis_sdk_python/services/detector_registry/__init__.py
 taegis_sdk_python/services/detector_registry/mutations.py
@@ -116,14 +121,19 @@
 taegis_sdk_python/services/fast_ioc/subscriptions.py
 taegis_sdk_python/services/fast_ioc/types.py
 taegis_sdk_python/services/file_info/__init__.py
 taegis_sdk_python/services/file_info/mutations.py
 taegis_sdk_python/services/file_info/queries.py
 taegis_sdk_python/services/file_info/subscriptions.py
 taegis_sdk_python/services/file_info/types.py
+taegis_sdk_python/services/ingest_stats/__init__.py
+taegis_sdk_python/services/ingest_stats/mutations.py
+taegis_sdk_python/services/ingest_stats/queries.py
+taegis_sdk_python/services/ingest_stats/subscriptions.py
+taegis_sdk_python/services/ingest_stats/types.py
 taegis_sdk_python/services/investigations/__init__.py
 taegis_sdk_python/services/investigations/mutations.py
 taegis_sdk_python/services/investigations/queries.py
 taegis_sdk_python/services/investigations/subscriptions.py
 taegis_sdk_python/services/investigations/types.py
 taegis_sdk_python/services/investigations2/__init__.py
 taegis_sdk_python/services/investigations2/mutations.py
```

