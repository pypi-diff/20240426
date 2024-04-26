# Comparing `tmp/infuzu_python_sdk-0.81.tar.gz` & `tmp/infuzu-python-sdk-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "infuzu_python_sdk-0.81.tar", last modified: Thu Apr 25 19:49:39 2024, max compression
+gzip compressed data, was "infuzu-python-sdk-0.9.tar", last modified: Tue Dec  5 23:50:28 2023, max compression
```

## Comparing `infuzu_python_sdk-0.81.tar` & `infuzu-python-sdk-0.9.tar`

### file list

```diff
@@ -1,83 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:49:39.408952 infuzu_python_sdk-0.81/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-25 19:49:35.000000 infuzu_python_sdk-0.81/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     6168 2024-04-25 19:49:39.404952 infuzu_python_sdk-0.81/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-04-25 19:49:35.000000 infuzu_python_sdk-0.81/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:49:39.396952 infuzu_python_sdk-0.81/infuzu/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-25 19:49:35.000000 infuzu_python_sdk-0.81/infuzu/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:49:39.396952 infuzu_python_sdk-0.81/infuzu/access/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:49:35.000000 infuzu_python_sdk-0.81/infuzu/access/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9010 2024-04-25 19:49:35.000000 infuzu_python_sdk-0.81/infuzu/access/instance_access_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-25 19:49:35.000000 infuzu_python_sdk-0.81/infuzu/access/object_access_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-25 19:49:35.000000 infuzu_python_sdk-0.81/infuzu/access/user_access_profile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:49:39.396952 infuzu_python_sdk-0.81/infuzu/authentication/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-25 19:49:35.000000 infuzu_python_sdk-0.81/infuzu/authentication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-25 19:49:35.000000 infuzu_python_sdk-0.81/infuzu/authentication/authenticate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6821 2024-04-25 19:49:35.000000 infuzu_python_sdk-0.81/infuzu/authentication/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-04-25 19:49:35.000000 infuzu_python_sdk-0.81/infuzu/authentication/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-04-25 19:49:35.000000 infuzu_python_sdk-0.81/infuzu/authentication/shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-25 19:49:35.000000 infuzu_python_sdk-0.81/infuzu/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:49:39.396952 infuzu_python_sdk-0.81/infuzu/clockwise/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-25 19:49:35.000000 infuzu_python_sdk-0.81/infuzu/clockwise/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:49:39.400952 infuzu_python_sdk-0.81/infuzu/clockwise/assignments/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-25 19:49:35.000000 infuzu_python_sdk-0.81/infuzu/clockwise/assignments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-25 19:49:35.000000 infuzu_python_sdk-0.81/infuzu/clockwise/assignments/complete_assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-04-25 19:49:35.000000 infuzu_python_sdk-0.81/infuzu/clockwise/assignments/retrieve_assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-25 19:49:35.000000 infuzu_python_sdk-0.81/infuzu/clockwise/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:49:39.400952 infuzu_python_sdk-0.81/infuzu/clockwise/rules/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-25 19:49:35.000000 infuzu_python_sdk-0.81/infuzu/clockwise/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-25 19:49:35.000000 infuzu_python_sdk-0.81/infuzu/clockwise/rules/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-25 19:49:35.000000 infuzu_python_sdk-0.81/infuzu/clockwise/rules/calls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-25 19:49:35.000000 infuzu_python_sdk-0.81/infuzu/clockwise/rules/execution_log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:49:39.400952 infuzu_python_sdk-0.81/infuzu/cogitobot/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:49:35.000000 infuzu_python_sdk-0.81/infuzu/cogitobot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-25 19:49:35.000000 infuzu_python_sdk-0.81/infuzu/cogitobot/document_version.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-25 19:49:35.000000 infuzu_python_sdk-0.81/infuzu/constant_access.py
--rw-r--r--   0 runner    (1001) docker     (127)     5059 2024-04-25 19:49:35.000000 infuzu_python_sdk-0.81/infuzu/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:49:39.400952 infuzu_python_sdk-0.81/infuzu/errors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:49:35.000000 infuzu_python_sdk-0.81/infuzu/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-25 19:49:35.000000 infuzu_python_sdk-0.81/infuzu/errors/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-25 19:49:35.000000 infuzu_python_sdk-0.81/infuzu/errors/subscription_overviews.py
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-25 19:49:35.000000 infuzu_python_sdk-0.81/infuzu/errors/subscription_plans.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-25 19:49:35.000000 infuzu_python_sdk-0.81/infuzu/errors/subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-25 19:49:35.000000 infuzu_python_sdk-0.81/infuzu/errors/user_and_subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-25 19:49:35.000000 infuzu_python_sdk-0.81/infuzu/errors/user_subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-25 19:49:35.000000 infuzu_python_sdk-0.81/infuzu/errors/users.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:49:39.400952 infuzu_python_sdk-0.81/infuzu/http_requests/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-25 19:49:35.000000 infuzu_python_sdk-0.81/infuzu/http_requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-25 19:49:35.000000 infuzu_python_sdk-0.81/infuzu/http_requests/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:49:39.400952 infuzu_python_sdk-0.81/infuzu/subscriptions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:49:35.000000 infuzu_python_sdk-0.81/infuzu/subscriptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-04-25 19:49:35.000000 infuzu_python_sdk-0.81/infuzu/subscriptions/overview.py
--rw-r--r--   0 runner    (1001) docker     (127)     7344 2024-04-25 19:49:35.000000 infuzu_python_sdk-0.81/infuzu/subscriptions/subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-04-25 19:49:35.000000 infuzu_python_sdk-0.81/infuzu/subscriptions/subscription_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     6534 2024-04-25 19:49:35.000000 infuzu_python_sdk-0.81/infuzu/subscriptions/user_subscription.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:49:39.404952 infuzu_python_sdk-0.81/infuzu/users/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:49:35.000000 infuzu_python_sdk-0.81/infuzu/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-25 19:49:35.000000 infuzu_python_sdk-0.81/infuzu/users/marketing_preference.py
--rw-r--r--   0 runner    (1001) docker     (127)     5555 2024-04-25 19:49:35.000000 infuzu_python_sdk-0.81/infuzu/users/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:49:39.404952 infuzu_python_sdk-0.81/infuzu/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:49:35.000000 infuzu_python_sdk-0.81/infuzu/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:49:39.404952 infuzu_python_sdk-0.81/infuzu/utils/api_calls/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:49:35.000000 infuzu_python_sdk-0.81/infuzu/utils/api_calls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6966 2024-04-25 19:49:35.000000 infuzu_python_sdk-0.81/infuzu/utils/api_calls/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-25 19:49:35.000000 infuzu_python_sdk-0.81/infuzu/utils/api_calls/serialize.py
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-25 19:49:35.000000 infuzu_python_sdk-0.81/infuzu/utils/caching.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:49:39.404952 infuzu_python_sdk-0.81/infuzu/utils/django/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:49:35.000000 infuzu_python_sdk-0.81/infuzu/utils/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-04-25 19:49:35.000000 infuzu_python_sdk-0.81/infuzu/utils/django/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-25 19:49:35.000000 infuzu_python_sdk-0.81/infuzu/utils/django/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-25 19:49:35.000000 infuzu_python_sdk-0.81/infuzu/utils/encryption.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:49:39.404952 infuzu_python_sdk-0.81/infuzu/utils/enums/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:49:35.000000 infuzu_python_sdk-0.81/infuzu/utils/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-25 19:49:35.000000 infuzu_python_sdk-0.81/infuzu/utils/enums/api_calls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-25 19:49:35.000000 infuzu_python_sdk-0.81/infuzu/utils/enums/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-25 19:49:35.000000 infuzu_python_sdk-0.81/infuzu/utils/enums/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-25 19:49:35.000000 infuzu_python_sdk-0.81/infuzu/utils/random.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:49:39.404952 infuzu_python_sdk-0.81/infuzu_python_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6168 2024-04-25 19:49:39.000000 infuzu_python_sdk-0.81/infuzu_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-25 19:49:39.000000 infuzu_python_sdk-0.81/infuzu_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:49:39.000000 infuzu_python_sdk-0.81/infuzu_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-25 19:49:39.000000 infuzu_python_sdk-0.81/infuzu_python_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-25 19:49:35.000000 infuzu_python_sdk-0.81/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 19:49:39.408952 infuzu_python_sdk-0.81/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-25 19:49:35.000000 infuzu_python_sdk-0.81/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 23:50:28.163313 infuzu-python-sdk-0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2023-12-05 23:50:16.000000 infuzu-python-sdk-0.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6167 2023-12-05 23:50:28.163313 infuzu-python-sdk-0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5685 2023-12-05 23:50:16.000000 infuzu-python-sdk-0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 23:50:28.155313 infuzu-python-sdk-0.9/infuzu/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-05 23:50:16.000000 infuzu-python-sdk-0.9/infuzu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 23:50:28.155313 infuzu-python-sdk-0.9/infuzu/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-05 23:50:16.000000 infuzu-python-sdk-0.9/infuzu/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3943 2023-12-05 23:50:16.000000 infuzu-python-sdk-0.9/infuzu/auth/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 23:50:28.155313 infuzu-python-sdk-0.9/infuzu/clockwise/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2023-12-05 23:50:16.000000 infuzu-python-sdk-0.9/infuzu/clockwise/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 23:50:28.155313 infuzu-python-sdk-0.9/infuzu/clockwise/assignments/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2023-12-05 23:50:16.000000 infuzu-python-sdk-0.9/infuzu/clockwise/assignments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2023-12-05 23:50:16.000000 infuzu-python-sdk-0.9/infuzu/clockwise/assignments/complete_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5665 2023-12-05 23:50:16.000000 infuzu-python-sdk-0.9/infuzu/clockwise/assignments/retrieve_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2023-12-05 23:50:16.000000 infuzu-python-sdk-0.9/infuzu/clockwise/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 23:50:28.155313 infuzu-python-sdk-0.9/infuzu/clockwise/rules/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2023-12-05 23:50:16.000000 infuzu-python-sdk-0.9/infuzu/clockwise/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2023-12-05 23:50:16.000000 infuzu-python-sdk-0.9/infuzu/clockwise/rules/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2023-12-05 23:50:16.000000 infuzu-python-sdk-0.9/infuzu/clockwise/rules/calls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2023-12-05 23:50:16.000000 infuzu-python-sdk-0.9/infuzu/clockwise/rules/execution_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2023-12-05 23:50:16.000000 infuzu-python-sdk-0.9/infuzu/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 23:50:28.159313 infuzu-python-sdk-0.9/infuzu/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-05 23:50:16.000000 infuzu-python-sdk-0.9/infuzu/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 23:50:28.159313 infuzu-python-sdk-0.9/infuzu/utils/api_calls/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-05 23:50:16.000000 infuzu-python-sdk-0.9/infuzu/utils/api_calls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8049 2023-12-05 23:50:16.000000 infuzu-python-sdk-0.9/infuzu/utils/api_calls/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2023-12-05 23:50:16.000000 infuzu-python-sdk-0.9/infuzu/utils/api_calls/clockwise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2023-12-05 23:50:16.000000 infuzu-python-sdk-0.9/infuzu/utils/api_calls/infuzu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2023-12-05 23:50:16.000000 infuzu-python-sdk-0.9/infuzu/utils/api_calls/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2023-12-05 23:50:16.000000 infuzu-python-sdk-0.9/infuzu/utils/encryption.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 23:50:28.159313 infuzu-python-sdk-0.9/infuzu/utils/enums/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-05 23:50:16.000000 infuzu-python-sdk-0.9/infuzu/utils/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2023-12-05 23:50:16.000000 infuzu-python-sdk-0.9/infuzu/utils/enums/api_calls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2023-12-05 23:50:16.000000 infuzu-python-sdk-0.9/infuzu/utils/enums/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2023-12-05 23:50:16.000000 infuzu-python-sdk-0.9/infuzu/utils/random.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 23:50:28.159313 infuzu-python-sdk-0.9/infuzu_python_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6167 2023-12-05 23:50:28.000000 infuzu-python-sdk-0.9/infuzu_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2023-12-05 23:50:28.000000 infuzu-python-sdk-0.9/infuzu_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-05 23:50:28.000000 infuzu-python-sdk-0.9/infuzu_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2023-12-05 23:50:28.000000 infuzu-python-sdk-0.9/infuzu_python_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2023-12-05 23:50:16.000000 infuzu-python-sdk-0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-05 23:50:28.163313 infuzu-python-sdk-0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2023-12-05 23:50:16.000000 infuzu-python-sdk-0.9/setup.py
```

### Comparing `infuzu_python_sdk-0.81/LICENSE.md` & `infuzu-python-sdk-0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `infuzu_python_sdk-0.81/PKG-INFO` & `infuzu-python-sdk-0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infuzu-python-sdk
-Version: 0.81
+Version: 0.9
 Summary: This SDK provides a set of tools to manage assignments from Clockwise. Primarily, it allows you to fetch, represent, and mark assignments as complete.
 Home-page: https://github.com/Infuzu/InfuzuPythonSDK
 Author: Infuzu
 Author-email: help@infuzu.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

### Comparing `infuzu_python_sdk-0.81/README.md` & `infuzu-python-sdk-0.9/README.md`

 * *Files identical despite different names*

### Comparing `infuzu_python_sdk-0.81/infuzu/access/instance_access_profile.py` & `infuzu-python-sdk-0.9/infuzu/utils/api_calls/base.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,208 +1,190 @@
-import datetime
-from enum import Enum
-from pydantic import Field
-from requests import Response
-from .user_access_profile import UserAccessProfile
-from .. import constants
-from ..base import BaseInfuzuObject
-from ..errors.base import InfuzuError
-from ..http_requests import signed_requests
-from ..utils.caching import CacheSystem
-from ..utils.enums.checks import validate_enum_value
-
-
-INSTANCE_ACCESS_PROFILE_CACHE: CacheSystem = CacheSystem(default_expiry_time=60)
-
-
-class WhoHasAccessEnum(Enum):
-    RESTRICTED: str = "R"
-    ANYONE_SIGNED_IN: str = "S"
-    ANYONE_WITH_LINK: str = "A"
-
-
-class LinkAccessEnum(Enum):
-    DEFINITION_EDITOR: str = "DE"
-    DEFINITION_VIEWER: str = "DV"
-    PRODUCT_USER: str = "PU"
-
-
-class PaymentOptionEnum(Enum):
-    OWNER: str = "O"
-    OWNER_AND_SUBSCRIPTION: str = "OS"
-    USER: str = "U"
-    OWNER_AND_SUBSCRIPTION_WITH_USER_AS_BACKUP: str = "OB"
-
-
-class InstanceAccessProfile(BaseInfuzuObject):
-    id: str | None = Field(frozen=True, default=None)
-    object_type: str | None = Field(frozen=True, default=None)
-    who_has_access: str | None = Field(frozen=True, default=None)
-    link_access: str | None = Field(frozen=True, default=None)
-    owner_id: str | None = Field(frozen=True, default=None)
-    definition_editors: list[str] | None = Field(frozen=True, default=None)
-    definition_viewers: list[str] | None = Field(frozen=True, default=None)
-    product_users: list[str] | None = Field(frozen=True, default=None)
-    payment_option: str | None = Field(frozen=True, default=None)
-    subscribed_users: list[str] | None = Field(frozen=True, default=None)
-    subscription_list: list[str] | None = Field(frozen=True, default=None)
-    last_updated: str | None = Field(frozen=True, default=None)
+import json
+import time
+from types import NoneType
+import requests
+from PythonAdvancedTyping import check_type
+from .serialize import class_str_serializer
+from ..enums.api_calls import HttpMethod
+
+
+class APIResponse:
+    """
+    Wrapper class around the response object returned by the requests library.
+
+    Attributes:
+        response_object (requests.Response): The raw response object from the requests library.
+        attempts_count (int): The number of attempts made to get the response.
+
+    Methods:
+        success: Property indicating if the response was successful (HTTP 200).
+        response_dict: Property returning the response details as a dictionary.
+        execution_dict: Property returning details about the execution (e.g., attempts).
+    """
+
+    def __init__(self, response_object: requests.Response, attempts_count: int) -> None:
+        """
+        Initialize an APIResponse instance.
+
+        Args:
+            response_object (requests.Response): The raw response object.
+            attempts_count (int): The number of attempts made to get the response.
+        """
+        check_type((response_object, "response_object", requests.Response), (attempts_count, "attempts_count", int))
+        self.response_object: requests.Response = response_object
+        self.attempts_count: int = attempts_count
 
     @property
-    def who_has_access_enum(self) -> WhoHasAccessEnum:
-        return WhoHasAccessEnum(self.who_has_access)
+    def success(self) -> bool:
+        return self.response_object.status_code == 200
 
     @property
-    def link_access_enum(self) -> LinkAccessEnum:
-        return LinkAccessEnum(self.link_access)
+    def response_dict(self) -> dict[str, any]:
+        return {
+            "status_code": self.response_object.status_code,
+            "headers": self._headers_dict,
+            "content": self._content,
+            "url": self.response_object.url,
+            "history": [{"url": resp.url, "status": resp.status_code} for resp in self.response_object.history],
+            "encoding": self.response_object.encoding,
+            "elapsed": str(self.response_object.elapsed),
+            "cookies": self._cookies_dict,
+        }
 
     @property
-    def payment_option_enum(self) -> PaymentOptionEnum:
-        return PaymentOptionEnum(self.payment_option)
+    def execution_dict(self) -> dict[str, any]:
+        return {
+            "attempts": self.attempts_count
+        }
 
     @property
-    def last_updated_datetime(self) -> datetime.datetime:
-        return datetime.datetime.fromisoformat(self.last_updated)
-
-    def is_owner(self, user_id: str | None) -> bool:
-        return self.owner_id == user_id
-
-    def is_explicit_definition_editor(self, user_id: str | None) -> bool:
-        return user_id in self.definition_editors
-
-    def is_explicit_definition_viewer(self, user_id: str | None) -> bool:
-        return user_id in self.definition_viewers
-
-    def is_explicit_product_user(self, user_id: str | None) -> bool:
-        return user_id in self.product_users
-
-    def has_link_access(self, user_id: str | None) -> bool:
-        return self.who_has_access_enum == WhoHasAccessEnum.ANYONE_WITH_LINK or (
-            self.who_has_access_enum == WhoHasAccessEnum.ANYONE_SIGNED_IN and user_id
-        )
-
-    def is_implicit_definition_editor(self, user_id: str | None) -> bool:
-        return self.has_link_access(user_id) and self.link_access_enum == LinkAccessEnum.DEFINITION_EDITOR
-
-    def is_implicit_definition_viewer(self, user_id: str | None) -> bool:
-        return self.has_link_access(user_id) and self.link_access_enum == LinkAccessEnum.DEFINITION_VIEWER
-
-    def is_implicit_product_user(self, user_id: str | None) -> bool:
-        return self.has_link_access(user_id) and self.link_access_enum == LinkAccessEnum.PRODUCT_USER
-
-    def is_definition_editor(self, user_id: str | None) -> bool:
-        return (
-            self.is_explicit_definition_editor(user_id) or
-            self.is_implicit_definition_editor(user_id) or
-            self.is_owner(user_id)
-        )
-
-    def is_definition_viewer(self, user_id: str | None) -> bool:
-        return (
-            self.is_explicit_definition_viewer(user_id) or
-            self.is_implicit_definition_viewer(user_id) or
-            self.is_definition_editor(user_id)
-        )
-
-    def is_product_user(self, user_id: str | None) -> bool:
-        return (
-                self.is_explicit_product_user(user_id) or
-                self.is_implicit_product_user(user_id) or
-                self.is_definition_viewer(user_id)
-        )
-
-    def has_subscription(self, user_id: str | None) -> bool:
-        return user_id in self.subscribed_users
+    def _headers_dict(self) -> dict[str, any]:
+        return dict(self.response_object.headers)
 
     @property
-    def requires_subscription(self) -> bool:
-        return self.payment_option_enum == PaymentOptionEnum.OWNER_AND_SUBSCRIPTION
+    def _cookies_dict(self) -> dict[str, any]:
+        cookies_dict: dict[str, any] = {}
+        for cookie in self.response_object.cookies:
+            cookies_dict[cookie.name] = cookie.value
+        return cookies_dict
 
-    def has_use_access(self, user_id: str | None) -> bool:
-        if self.payment_option_enum == PaymentOptionEnum.OWNER:
-            return self.is_product_user(user_id)
-        elif self.payment_option_enum == PaymentOptionEnum.OWNER_AND_SUBSCRIPTION:
-            return self.is_product_user(user_id) and self.has_subscription(user_id)
-        elif self.payment_option_enum == PaymentOptionEnum.USER:
-            return self.is_product_user(user_id) and UserAccessProfile.retrieve(user_id).billing_in_good_standing
-        elif self.payment_option_enum == PaymentOptionEnum.OWNER_AND_SUBSCRIPTION_WITH_USER_AS_BACKUP:
-            return self.is_product_user(user_id) and (
-                    self.has_subscription(user_id) or UserAccessProfile.retrieve(user_id).billing_in_good_standing
-            )
-        else:
-            raise NotImplementedError(f"Payment option {self.payment_option_enum} not implemented.")
+    @property
+    def _content(self) -> str:
+        try:
+            if 'json' in self._headers_dict.get('content-type', ''):
+                content: str = self.response_object.json()
+            else:
+                content: str = self.response_object.text
+        except (json.JSONDecodeError, UnicodeDecodeError):
+            content: str = "Error decoding content"
+        return content
 
-    def user_id_to_charge(self, user_id: str | None) -> str | None:
-        if self.payment_option_enum == PaymentOptionEnum.OWNER:
-            return self.owner_id
-        elif self.payment_option_enum == PaymentOptionEnum.OWNER_AND_SUBSCRIPTION:
-            return self.owner_id
-        elif self.payment_option_enum == PaymentOptionEnum.USER:
-            return user_id
-        elif self.payment_option_enum == PaymentOptionEnum.OWNER_AND_SUBSCRIPTION_WITH_USER_AS_BACKUP:
-            return self.owner_id if self.has_subscription(user_id) else user_id
-        else:
-            raise NotImplementedError(f"Payment option {self.payment_option_enum} not implemented.")
-
-    @classmethod
-    def create(
-            cls,
-            id: str,
-            object_type: str,
-            owner_id: str,
-            who_has_access: str | None = None,
-            link_access: str | None = None
-    ) -> 'InstanceAccessProfile':
-        def create_instance_access_profile() -> 'InstanceAccessProfile':
-            data: dict[str, any] = {"id": id, "object_type": object_type, "owner_id": owner_id}
-            if who_has_access is not None:
-                validate_enum_value(who_has_access, WhoHasAccessEnum)
-                data["who_has_access"] = who_has_access
-            if link_access is not None:
-                validate_enum_value(link_access, LinkAccessEnum)
-                data["link_access"] = link_access
-            api_response: Response = signed_requests.request(
-                method="POST",
-                url=f"{constants.ACCESS_BASE_URL}"
-                    f"{constants.ACCESS_CREATE_INSTANCE_ACCESS_PROFILE_ENDPOINT}",
-                json=data
-            )
-            if api_response.status_code == 201:
-                return cls(**api_response.json())
-            raise InfuzuError(f"Error creating instance access profile: {api_response.text}")
-        return INSTANCE_ACCESS_PROFILE_CACHE.get(
-            cache_key_name=f'{id}', specialized_fetch_function=create_instance_access_profile
-        )
-
-    @classmethod
-    def retrieve(cls, id: str) -> 'InstanceAccessProfile':
-        def get_instance_access_profile() -> 'InstanceAccessProfile':
-            api_response: Response = signed_requests.request(
-                method="GET",
-                url=f"{constants.ACCESS_BASE_URL}"
-                    f"{constants.ACCESS_RETRIEVE_INSTANCE_ACCESS_PROFILE_ENDPOINT}"
-                .replace('<str:instance_id>', id)
-            )
-            if api_response.status_code == 200:
-                return cls(**api_response.json())
-            raise InfuzuError(f"Error retrieving instance access profile: {api_response.text}")
-        return INSTANCE_ACCESS_PROFILE_CACHE.get(
-            cache_key_name=f'{id}', specialized_fetch_function=get_instance_access_profile
-        )
-
-    @classmethod
-    def delete(cls, id: str) -> bool:
-        def delete_instance_access_profile() -> bool:
-            api_response: Response = signed_requests.request(
-                method="DELETE",
-                url=f"{constants.ACCESS_BASE_URL}"
-                    f"{constants.ACCESS_DELETE_INSTANCE_ACCESS_PROFILE_ENDPOINT}"
-                .replace('<str:instance_id>', id)
+    @property
+    def response_content(self) -> any:
+        try:
+            if 'json' in self._headers_dict.get('Content-Type', ''):
+                return self.response_object.json()
+            else:
+                return self.response_object.text
+        except (json.JSONDecodeError, UnicodeDecodeError):
+            return "Error decoding content"
+
+
+def api_call(
+        url: str,
+        headers: dict | None,
+        params: dict | None = None,
+        body: dict | None = None,
+        method: HttpMethod = HttpMethod.GET,
+        tries: int = 1,
+        retry_wait: int = 0,
+        timeout: int = 10
+) -> APIResponse:
+    """
+    Make an API call with the provided details and retry mechanism.
+
+    Args:
+        url (str): The API endpoint to call.
+        headers (dict | None): Dictionary containing headers for the API request.
+        params (dict | None, optional): Dictionary containing query parameters for the API request. Defaults to None.
+        body (dict | None, optional): Dictionary containing request body (used for POST, PUT, etc.). Defaults to None.
+        method (HttpMethod, optional): The HTTP method to use. Defaults to HttpMethod.GET.
+        tries (int, optional): The number of tries to attempt the call. Defaults to 1.
+        retry_wait (int, optional): The number of seconds to wait between retries. Defaults to 0.
+        timeout (int, optional): The timeout for the API call in seconds. Defaults to 10.
+
+    Returns:
+        APIResponse: A wrapper around the response object with additional metadata.
+    """
+    check_type(
+        (url, "url", str),
+        (headers, "headers", (dict, NoneType)),
+        (params, "params", (dict, NoneType)),
+        (body, "body", (dict, NoneType)),
+        (method, "method", HttpMethod),
+        (tries, "tries", int),
+        (retry_wait, "retry_wait", int),
+        (timeout, "timeout", int)
+    )
+    attempts_made: int = 0
+    while attempts_made < tries:
+        attempts_made += 1
+        try:
+            if body is None:
+                json_body: None = None
+            else:
+                json_body: str = json.dumps(body, default=class_str_serializer)
+            response: requests.Response = requests.request(
+                method.name, url, headers=headers, params=params, data=json_body, timeout=timeout
             )
-            if api_response.status_code == 204:
-                return True
-            raise InfuzuError(f"Error creating instance access profile: {api_response.text}")
-        return INSTANCE_ACCESS_PROFILE_CACHE.get(
-            cache_key_name=f'delete__{id}',
-            specialized_fetch_function=delete_instance_access_profile,
-            specialized_expiry_time=1
-        )
+            if attempts_made < tries:
+                response.raise_for_status()
+            return APIResponse(response, attempts_made)
+        except requests.ConnectionError:
+            print("Failed to connect to the URL.")
+            if attempts_made < tries:
+                print(f"Attempt {attempts_made} failed due to connection error. Retrying in {retry_wait} seconds...")
+                time.sleep(retry_wait)
+            else:
+                custom_response_data: dict[str, any] = {
+                    "status_code": 503, "content": "Failed to connect after all attempts.",
+                }
+                custom_response: requests.Response = requests.Response()
+                for key, value in custom_response_data.items():
+                    setattr(custom_response, key, value)
+                return APIResponse(custom_response, attempts_made)
+        except requests.TooManyRedirects:
+            print("Too many redirects.")
+            if attempts_made < tries:
+                print(f"Attempt {attempts_made} failed due to too many redirects. Retrying in {retry_wait} seconds...")
+                time.sleep(retry_wait)
+            else:
+                custom_response_data: dict[str, any] = {
+                    "status_code": 508, "content": "Too many redirects after all attempts.",
+                }
+                custom_response: requests.Response = requests.Response()
+                for key, value in custom_response_data.items():
+                    setattr(custom_response, key, value)
+                return APIResponse(custom_response, attempts_made)
+        except requests.RequestException:
+            if attempts_made < tries:
+                print(f"Attempt {attempts_made} failed. Retrying in {retry_wait} seconds...")
+                time.sleep(retry_wait)
+            else:
+                try:
+                    # noinspection PyUnboundLocalVariable
+                    return APIResponse(response, attempts_made)
+                except NameError:
+                    print("An unexpected error occurred. Unable to get a response.")
+                    custom_response_data: dict[str, any] = {
+                        "status_code": 500, "content": "An unexpected error occurred after all attempts.",
+                    }
+                    custom_response: requests.Response = requests.Response()
+                    for key, value in custom_response_data.items():
+                        setattr(custom_response, key, value)
+                    return APIResponse(custom_response, attempts_made)
+
+    custom_response_data: dict[str, any] = {"status_code": 400, "content": "Unexpected failure"}
+    custom_response: requests.Response = requests.Response()
+    for key, value in custom_response_data.items():
+        setattr(custom_response, key, value)
+    return APIResponse(custom_response, attempts_made)
```

### Comparing `infuzu_python_sdk-0.81/infuzu/clockwise/assignments/retrieve_assignment.py` & `infuzu-python-sdk-0.9/infuzu/utils/api_calls/clockwise.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,77 +1,61 @@
-from typing import Any
-from deprecated import deprecated
-from pydantic import (Field, PositiveInt)
-from pydantic_core import Url
-from requests import Response
+"""
+utils/api_calls/clockwise.py
+This module provides utilities to interact with the Clockwise API.
+
+Dependencies:
+    - `PythonAdvancedTyping` for static type checking.
+    - `constants` module for default values and constants, including CLOCKWISE_BASE_URL.
+    - `InfuzuCredentials` for generating authentication tokens for Clockwise, even though the name suggests it's for Infuzu.
+    - `APIResponse` and `api_call` from the base module to handle API interactions.
+    - `HttpMethod` from the enums module for HTTP method typing.
+"""
+from types import NoneType
+from PythonAdvancedTyping import check_type
+from .base import (APIResponse, api_call)
 from ... import constants
-from ...base import BaseInfuzuObject
-from ...errors.base import InfuzuError
-from ...http_requests import signed_requests
-from ...utils.enums.api_calls import HttpMethod
-from ..errors import NoContentError
-
-
-class Assignment(BaseInfuzuObject):
-    rule_id: str | None = Field(frozen=True, default=None)
-    url: Url | None = Field(frozen=True, default=None)
-    private_key_b64: str | None = Field(frozen=True, default=None)
-    http_method: HttpMethod | None = Field(frozen=True, default=HttpMethod.GET)
-    headers: dict[str, Any] | None = Field(frozen=True, default=None)
-    body: dict[str, Any] | None = Field(frozen=True, default=None)
-    max_retries: PositiveInt | None = Field(frozen=True, default=0)
-    timeout: PositiveInt | None = Field(frozen=True, default=30)
-
-    @classmethod
-    @deprecated(version='0.77', reason="Use standard pydantic options instead")
-    def from_dict(cls, assignment_dict: dict[str, any]) -> 'Assignment':
-        rule_id: str = assignment_dict.get("rule_id")
-        url: str = assignment_dict.get("url")
-        private_key_b64: str = assignment_dict.get("private_key_b64")
-        http_method: str = assignment_dict.get("http_method")
-        headers: dict[str, any] | None = assignment_dict.get("headers")
-        body: dict[str, any] | None = assignment_dict.get("body")
-        max_retries: int = assignment_dict.get("max_retries")
-        timeout: int = assignment_dict.get("timeout")
-
-        http_method: HttpMethod = HttpMethod(http_method)
-
-        return cls(
-            rule_id=rule_id,
-            url=url,
-            private_key_b64=private_key_b64,
-            http_method=http_method,
-            headers=headers,
-            body=body,
-            max_retries=max_retries,
-            timeout=timeout
-        )
-
-    @deprecated(version='0.77', reason="Use standard pydantic options instead")
-    def to_dict(self) -> dict[str, any]:
-        return {
-            "rule_id": self.rule_id,
-            "url": self.url,
-            "http_method": self.http_method,
-            "headers": self.headers,
-            "body": self.body,
-            "max_retries": self.max_retries,
-            "timeout": self.timeout
-        }
-
-    @classmethod
-    def retrieve(cls):
-        response: Response = signed_requests.get(
-            url=f"{constants.CLOCKWISE_BASE_URL}{constants.CLOCKWISE_RETRIEVE_ASSIGNMENT_ENDPOINT}"
-        )
-        if response.status_code == 200:
-            return Assignment(**response.json())
-        elif response.status_code == 204:
-            raise NoContentError()
-        raise InfuzuError(
-            f"Status Code: {response.status_code}, Content: {response.content}"
-        )
-
-
-@deprecated(version='0.77', reason="Use Assignment.retrieve() instead")
-def get_assignment() -> Assignment:
-    return Assignment.retrieve()
+from ..enums.api_calls import HttpMethod
+from ...auth import InfuzuCredentials
+
+
+def clockwise_api_call(
+        credentials: InfuzuCredentials,
+        endpoint: str,
+        method: HttpMethod,
+        timeout: int = constants.DEFAULT_REQUEST_TIMEOUT,
+        headers: dict[str, any] = None,
+        params: dict[str, any] = None,
+        body: dict[str, any] = None
+) -> APIResponse:
+    """
+    Makes an authenticated API call to Clockwise.
+
+    Args:
+        credentials (InfuzuCredentials): Clockwise authentication credentials object, though it's named InfuzuCredentials.
+        endpoint (str): The specific API endpoint for Clockwise (e.g., "/users").
+        method (HttpMethod): The HTTP method for the API call.
+        timeout (int, optional): The maximum duration (in seconds) to wait for a response. Defaults to `DEFAULT_REQUEST_TIMEOUT`.
+        headers (dict[str, any], optional): Additional headers to send with the request.
+        params (dict[str, any], optional): Query parameters to send with the request.
+        body (dict[str, any], optional): The body of the request if applicable.
+
+    Returns:
+        APIResponse: An object containing the details of the API response.
+
+    Raises:
+        RequestException: If there's an issue with making the request.
+        ValueError: For invalid input types.
+    """
+    if headers is None:
+        headers: dict[str, any] = {}
+    check_type(
+        (credentials, "credentials", InfuzuCredentials),
+        (endpoint, "endpoint", str),
+        (headers, "headers", dict),
+        (params, "params", (dict, NoneType)),
+        (body, "body", (dict, NoneType)),
+        (method, "method", HttpMethod),
+        (timeout, "timeout", int)
+    )
+    url: str = constants.CLOCKWISE_BASE_URL + endpoint
+    headers[constants.INFUZU_AUTH_TOKEN_HEADER_NAME] = credentials.infuzu_auth_signature
+    return api_call(url=url, method=method, headers=headers, timeout=timeout, body=body)
```

### Comparing `infuzu_python_sdk-0.81/infuzu/utils/encryption.py` & `infuzu-python-sdk-0.9/infuzu/utils/encryption.py`

 * *Files identical despite different names*

### Comparing `infuzu_python_sdk-0.81/infuzu/utils/enums/api_calls.py` & `infuzu-python-sdk-0.9/infuzu/utils/enums/api_calls.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """
 utils/enums/api_calls.py
 This module contains the HttpMethod enumeration which represents the various HTTP methods
 used in making API calls.
 """
-from enum import Enum
 
+from .base import SerializableEnum
 
-class HttpMethod(str, Enum):
+
+class HttpMethod(SerializableEnum):
     """
     Enumeration representing the different HTTP methods commonly used in RESTful API calls.
 
     Inherits:
         SerializableEnum: The custom Enum class which allows for serialization.
 
     Members:
```

### Comparing `infuzu_python_sdk-0.81/infuzu/utils/enums/base.py` & `infuzu-python-sdk-0.9/infuzu/utils/enums/base.py`

 * *Files identical despite different names*

### Comparing `infuzu_python_sdk-0.81/infuzu_python_sdk.egg-info/PKG-INFO` & `infuzu-python-sdk-0.9/infuzu_python_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infuzu-python-sdk
-Version: 0.81
+Version: 0.9
 Summary: This SDK provides a set of tools to manage assignments from Clockwise. Primarily, it allows you to fetch, represent, and mark assignments as complete.
 Home-page: https://github.com/Infuzu/InfuzuPythonSDK
 Author: Infuzu
 Author-email: help@infuzu.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

### Comparing `infuzu_python_sdk-0.81/setup.py` & `infuzu-python-sdk-0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import (setup, find_packages)
 
 setup(
     name="infuzu-python-sdk",
-    version="0.81",
+    version="0.9",
     packages=find_packages(),
     install_requires=[],
     author="Infuzu",
     author_email="help@infuzu.com",
     description="This SDK provides a set of tools to manage assignments from Clockwise. Primarily, it allows you to fetch, represent, and mark assignments as complete.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
```

