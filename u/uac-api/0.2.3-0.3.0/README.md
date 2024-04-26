# Comparing `tmp/uac-api-0.2.3.tar.gz` & `tmp/uac-api-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uac-api-0.2.3.tar", last modified: Tue Apr 23 20:50:46 2024, max compression
+gzip compressed data, was "uac-api-0.3.0.tar", last modified: Fri Apr 26 02:49:10 2024, max compression
```

## Comparing `uac-api-0.2.3.tar` & `uac-api-0.3.0.tar`

### file list

```diff
@@ -1,45 +1,48 @@
-drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-04-23 20:50:46.339602 uac-api-0.2.3/
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     8608 2024-04-23 20:50:46.339184 uac-api-0.2.3/PKG-INFO
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     8224 2024-04-23 20:30:56.000000 uac-api-0.2.3/README.md
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-04-22 17:21:03.000000 uac-api-0.2.3/pyproject.toml
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       38 2024-04-23 20:50:46.339673 uac-api-0.2.3/setup.cfg
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      904 2024-04-22 21:21:10.000000 uac-api-0.2.3/setup.py
-drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-04-23 20:50:46.321411 uac-api-0.2.3/uac_api.egg-info/
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     8608 2024-04-23 20:50:46.000000 uac-api-0.2.3/uac_api.egg-info/PKG-INFO
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      854 2024-04-23 20:50:46.000000 uac-api-0.2.3/uac_api.egg-info/SOURCES.txt
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        1 2024-04-23 20:50:46.000000 uac-api-0.2.3/uac_api.egg-info/dependency_links.txt
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        9 2024-04-23 20:50:46.000000 uac-api-0.2.3/uac_api.egg-info/requires.txt
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        7 2024-04-23 20:50:46.000000 uac-api-0.2.3/uac_api.egg-info/top_level.txt
-drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-04-23 20:50:46.338610 uac-api-0.2.3/uacapi/
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     5393 2024-04-23 20:50:40.000000 uac-api-0.2.3/uacapi/__init__.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2353 2024-04-23 20:18:59.000000 uac-api-0.2.3/uacapi/agents.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1399 2024-04-23 20:20:02.000000 uac-api-0.2.3/uacapi/audits.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      602 2024-04-23 20:20:20.000000 uac-api-0.2.3/uacapi/bundles.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      522 2024-04-23 20:21:12.000000 uac-api-0.2.3/uacapi/business_services.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      344 2024-04-23 20:21:22.000000 uac-api-0.2.3/uacapi/calendars.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      143 2024-04-23 20:21:32.000000 uac-api-0.2.3/uacapi/connections.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      312 2024-04-23 20:21:49.000000 uac-api-0.2.3/uacapi/credentials.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1110 2024-04-23 20:24:21.000000 uac-api-0.2.3/uacapi/custom_days.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-04-22 15:23:03.000000 uac-api-0.2.3/uacapi/groups.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      109 2024-04-23 20:24:40.000000 uac-api-0.2.3/uacapi/ldap.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       45 2024-04-23 20:24:47.000000 uac-api-0.2.3/uacapi/metrics.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      174 2024-04-23 20:24:56.000000 uac-api-0.2.3/uacapi/oauth_clients.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1270 2024-04-23 19:59:52.000000 uac-api-0.2.3/uacapi/oms_servers.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3257 2024-04-22 12:58:51.000000 uac-api-0.2.3/uacapi/payload.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       96 2024-04-23 20:25:32.000000 uac-api-0.2.3/uacapi/properties.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       27 2024-04-23 20:25:40.000000 uac-api-0.2.3/uacapi/reports.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1510 2024-04-23 20:29:44.000000 uac-api-0.2.3/uacapi/scripts.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      140 2024-04-23 20:29:55.000000 uac-api-0.2.3/uacapi/simulations.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       30 2024-04-23 20:30:38.000000 uac-api-0.2.3/uacapi/system.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     5034 2024-04-23 20:36:25.000000 uac-api-0.2.3/uacapi/task_instances.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2568 2024-04-23 20:44:17.000000 uac-api-0.2.3/uacapi/tasks.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      602 2024-04-23 20:44:36.000000 uac-api-0.2.3/uacapi/triggers.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      242 2024-04-23 20:47:20.000000 uac-api-0.2.3/uacapi/universal_event_templates.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      491 2024-04-22 16:25:20.000000 uac-api-0.2.3/uacapi/universal_events.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      605 2024-04-23 20:45:40.000000 uac-api-0.2.3/uacapi/universal_templates.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      273 2024-04-23 20:45:51.000000 uac-api-0.2.3/uacapi/users.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     5769 2024-04-23 19:42:21.000000 uac-api-0.2.3/uacapi/utils.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      260 2024-04-23 20:45:59.000000 uac-api-0.2.3/uacapi/variables.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      609 2024-04-23 20:46:26.000000 uac-api-0.2.3/uacapi/virtual_resources.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      404 2024-04-23 20:46:36.000000 uac-api-0.2.3/uacapi/webhooks.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      324 2024-04-23 20:48:30.000000 uac-api-0.2.3/uacapi/workflows.py
+drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-04-26 02:49:10.383056 uac-api-0.3.0/
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    18836 2024-04-26 02:49:10.382826 uac-api-0.3.0/PKG-INFO
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    18448 2024-04-26 02:47:32.000000 uac-api-0.3.0/README.md
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-04-22 17:21:03.000000 uac-api-0.3.0/pyproject.toml
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       38 2024-04-26 02:49:10.383101 uac-api-0.3.0/setup.cfg
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      909 2024-04-26 01:06:22.000000 uac-api-0.3.0/setup.py
+drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-04-26 02:49:10.380544 uac-api-0.3.0/uac_api/
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     7184 2024-04-26 02:48:58.000000 uac-api-0.3.0/uac_api/__init__.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     8745 2024-04-26 00:55:46.000000 uac-api-0.3.0/uac_api/agents.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1192 2024-04-26 01:02:08.000000 uac-api-0.3.0/uac_api/audits.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    10234 2024-04-26 00:58:46.000000 uac-api-0.3.0/uac_api/bundles.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2068 2024-04-26 00:56:32.000000 uac-api-0.3.0/uac_api/business_services.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     4997 2024-04-26 00:56:41.000000 uac-api-0.3.0/uac_api/calendars.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      402 2024-04-24 20:55:02.000000 uac-api-0.3.0/uac_api/cluster_nodes.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     8909 2024-04-26 00:59:35.000000 uac-api-0.3.0/uac_api/connections.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2953 2024-04-26 00:56:58.000000 uac-api-0.3.0/uac_api/credentials.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3398 2024-04-26 00:57:08.000000 uac-api-0.3.0/uac_api/custom_days.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1851 2024-04-26 00:57:56.000000 uac-api-0.3.0/uac_api/email_templates.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      536 2024-04-24 20:59:01.000000 uac-api-0.3.0/uac_api/ldap.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      216 2024-04-25 17:28:13.000000 uac-api-0.3.0/uac_api/metrics.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2059 2024-04-26 00:58:08.000000 uac-api-0.3.0/uac_api/oauth_clients.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1891 2024-04-26 00:58:22.000000 uac-api-0.3.0/uac_api/oms_servers.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3257 2024-04-22 12:58:51.000000 uac-api-0.3.0/uac_api/payload.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      818 2024-04-25 17:33:25.000000 uac-api-0.3.0/uac_api/properties.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      669 2024-04-25 17:33:50.000000 uac-api-0.3.0/uac_api/reports.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1746 2024-04-26 00:59:12.000000 uac-api-0.3.0/uac_api/scripts.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      722 2024-04-25 21:56:36.000000 uac-api-0.3.0/uac_api/server_operations.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2571 2024-04-26 00:59:23.000000 uac-api-0.3.0/uac_api/simulations.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      305 2024-04-25 17:38:45.000000 uac-api-0.3.0/uac_api/system.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    43174 2024-04-26 02:35:39.000000 uac-api-0.3.0/uac_api/task_instances.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    21888 2024-04-26 02:36:45.000000 uac-api-0.3.0/uac_api/tasks.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     5587 2024-04-26 00:59:56.000000 uac-api-0.3.0/uac_api/triggers.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2471 2024-04-26 01:00:11.000000 uac-api-0.3.0/uac_api/universal_event_templates.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2233 2024-04-25 17:51:48.000000 uac-api-0.3.0/uac_api/universal_events.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     4942 2024-04-26 01:00:20.000000 uac-api-0.3.0/uac_api/universal_templates.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1760 2024-04-26 01:00:31.000000 uac-api-0.3.0/uac_api/user_groups.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     4091 2024-04-26 01:00:50.000000 uac-api-0.3.0/uac_api/users.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     6779 2024-04-26 00:41:23.000000 uac-api-0.3.0/uac_api/utils.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3787 2024-04-26 01:01:04.000000 uac-api-0.3.0/uac_api/variables.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3208 2024-04-26 01:01:22.000000 uac-api-0.3.0/uac_api/virtual_resources.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     4221 2024-04-26 01:01:36.000000 uac-api-0.3.0/uac_api/webhooks.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     6115 2024-04-26 00:33:44.000000 uac-api-0.3.0/uac_api/workflows.py
+drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-04-26 02:49:10.382504 uac-api-0.3.0/uac_api.egg-info/
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    18836 2024-04-26 02:49:10.000000 uac-api-0.3.0/uac_api.egg-info/PKG-INFO
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      972 2024-04-26 02:49:10.000000 uac-api-0.3.0/uac_api.egg-info/SOURCES.txt
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        1 2024-04-26 02:49:10.000000 uac-api-0.3.0/uac_api.egg-info/dependency_links.txt
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        9 2024-04-26 02:49:10.000000 uac-api-0.3.0/uac_api.egg-info/requires.txt
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        8 2024-04-26 02:49:10.000000 uac-api-0.3.0/uac_api.egg-info/top_level.txt
```

### Comparing `uac-api-0.2.3/setup.py` & `uac-api-0.3.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from setuptools import setup, find_packages
-from uacapi import __version__
+from uac_api import __version__
 version = __version__
 
 def main():
     with open('README.md', 'r') as readme:
         long_description = readme.read()
     setup(
         name='uac-api',
@@ -11,15 +11,15 @@
         author_email="huseyin.gomleksizoglu@stonebranch.com",
         packages=find_packages(),
         include_package_data=True,
         install_requires=[
             "requests"
         ],
         author='Stonebranch',
-        description='A Python wrapper for the Stonebranch API',
+        description='A Python wrapper for the Stonebranch UAC API',
         python_requires='>=3.7',
         classifiers=[
             "Programming Language :: Python :: 3",
             "License :: OSI Approved :: MIT License",
             "Operating System :: OS Independent",
         ],
         long_description=long_description,
```

### Comparing `uac-api-0.2.3/uac_api.egg-info/SOURCES.txt` & `uac-api-0.3.0/uac_api.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 README.md
 pyproject.toml
 setup.py
+uac_api/__init__.py
+uac_api/agents.py
+uac_api/audits.py
+uac_api/bundles.py
+uac_api/business_services.py
+uac_api/calendars.py
+uac_api/cluster_nodes.py
+uac_api/connections.py
+uac_api/credentials.py
+uac_api/custom_days.py
+uac_api/email_templates.py
+uac_api/ldap.py
+uac_api/metrics.py
+uac_api/oauth_clients.py
+uac_api/oms_servers.py
+uac_api/payload.py
+uac_api/properties.py
+uac_api/reports.py
+uac_api/scripts.py
+uac_api/server_operations.py
+uac_api/simulations.py
+uac_api/system.py
+uac_api/task_instances.py
+uac_api/tasks.py
+uac_api/triggers.py
+uac_api/universal_event_templates.py
+uac_api/universal_events.py
+uac_api/universal_templates.py
+uac_api/user_groups.py
+uac_api/users.py
+uac_api/utils.py
+uac_api/variables.py
+uac_api/virtual_resources.py
+uac_api/webhooks.py
+uac_api/workflows.py
 uac_api.egg-info/PKG-INFO
 uac_api.egg-info/SOURCES.txt
 uac_api.egg-info/dependency_links.txt
 uac_api.egg-info/requires.txt
-uac_api.egg-info/top_level.txt
-uacapi/__init__.py
-uacapi/agents.py
-uacapi/audits.py
-uacapi/bundles.py
-uacapi/business_services.py
-uacapi/calendars.py
-uacapi/connections.py
-uacapi/credentials.py
-uacapi/custom_days.py
-uacapi/groups.py
-uacapi/ldap.py
-uacapi/metrics.py
-uacapi/oauth_clients.py
-uacapi/oms_servers.py
-uacapi/payload.py
-uacapi/properties.py
-uacapi/reports.py
-uacapi/scripts.py
-uacapi/simulations.py
-uacapi/system.py
-uacapi/task_instances.py
-uacapi/tasks.py
-uacapi/triggers.py
-uacapi/universal_event_templates.py
-uacapi/universal_events.py
-uacapi/universal_templates.py
-uacapi/users.py
-uacapi/utils.py
-uacapi/variables.py
-uacapi/virtual_resources.py
-uacapi/webhooks.py
-uacapi/workflows.py
+uac_api.egg-info/top_level.txt
```

### Comparing `uac-api-0.2.3/uacapi/audits.py` & `uac-api-0.3.0/uac_api/audits.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,42 +2,36 @@
 
 class Audits:
     def __init__(self, uc):
         self.log = uc.log
         self.headers = uc.headers
         self.uc = uc
 
-    def list_audits(self, payload=None, **args):
+    def list_audit(self, payload=None, **args):
         '''
-        payload: Payload of the request
-        Args Mapping:
-        - type: auditType
-        - source: source
-        - updated_time: updatedTime
-        - updated_time_type: updatedTimeType
-        - include_child_audit: includeChildAudits
-        - created_by: createdBy
-        - status: status
-        - table_record_name(or name): tableRecordName
-        - table_name (or table): tableName
-        - table_key (or key): tableKey
+        Arguments:
+        - auditType: auditType 
+        - source: source 
+        - status: status 
+        - createdBy: createdBy 
+        - tableName: tableName 
+        - tableRecordName: tableRecordName 
+        - updatedTimeType: updatedTimeType 
+        - updatedTime: updatedTime 
+        - tableKey: tableKey 
+        - includeChildAudits: includeChildAudits 
         '''
-        url = "/audit/list"
-        field_mapping = {
-            "type": "auditType",
-            "source": "source",
-            "updated_time": "updatedTime",
-            "updated_time_type": "updatedTimeType",
-            "include_child_audit": "includeChildAudits",
-            "created_by": "createdBy",
-            "status": "status",
-            "table_record_name": "tableRecordName",
-            "table_name": "tableName",
-            "table_key": "tableKey",
-            "name": "tableRecordName",
-            "table": "tableName",
-            "key": "tableKey"
+        url="/resources/audit/list"
+        field_mapping={
+          "auditType": "auditType", 
+          "source": "source", 
+          "status": "status", 
+          "createdBy": "createdBy", 
+          "tableName": "tableName", 
+          "tableRecordName": "tableRecordName", 
+          "updatedTimeType": "updatedTimeType", 
+          "updatedTime": "updatedTime", 
+          "tableKey": "tableKey", 
+          "includeChildAudits": "includeChildAudits", 
         }
         _payload = prepare_payload(payload, field_mapping, args)
-
-        response = self.uc.post(url, json_data=_payload)
-        return response
+        return self.uc.post(url, json_data=_payload)
```

### Comparing `uac-api-0.2.3/uacapi/oms_servers.py` & `uac-api-0.3.0/uac_api/oms_servers.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,39 +7,56 @@
 
 class OmsServers:
     def __init__(self, uc) -> None:
         self.log = uc.log
         self.headers = uc.headers
         self.uc = uc
 
-    def list_oms_servers(self):
-        url = "/omsserver/list"
-        response = self.uc.get(url)
-        return response
-
-    def read_oms_server(self, query=None, **args):
-        """
-        Read OMS server details.
-        Args:
-        - query: Query parameters
-        Args:
-        - server_id: Server ID
-        - server_address: Server address
-        """
-        url = "/omsserver"
-        field_mapping = {
-            "server_id": "serverid", 
-            "server_address": "serveraddress" 
+    def get_oms_server(self, query=None, **args):
+        '''
+        Arguments:
+        - serveraddress: serveraddress 
+        - serverid: serverid 
+        '''
+        url="/resources/omsserver"
+        field_mapping={
+            "serveraddress": "serveraddress", 
+            "serverid": "serverid", 
         }
         parameters = prepare_query_params(query, field_mapping, args)
+        return self.uc.get(url, query=parameters)
 
-        response = self.uc.get(url, query=parameters)
-        return response
+    def update_oms_server(self, payload=None, **args):
+        url="/resources/omsserver"
+        _payload = payload
+        return self.uc.put(url, json_data=_payload)
 
     def create_oms_server(self, payload=None, **args):
-        url = "/omsserver"
-        field_mapping = {
-            "server_address": "serverAddress"
+        '''
+        Arguments:
+        - retainSysIds: retainSysIds 
+            False will ignore sysIds in the payload and create a new task  
+        '''
+        url="/resources/omsserver"
+        field_mapping={
+          "retainSysIds": "retainSysIds", 
+        }
+        _payload = prepare_payload(payload, field_mapping, args)
+        return self.uc.post(url, json_data=_payload)
+
+    def delete_oms_server(self, query=None, **args):
+        '''
+        Arguments:
+        - serveraddress: serveraddress 
+        - serverid: serverid 
+        '''
+        url="/resources/omsserver"
+        field_mapping={
+          "serveraddress": "serveraddress", 
+          "serverid": "serverid", 
         }
-        payload = prepare_payload(payload, field_mapping, args)
-        response = self.uc.post(url, json_data=payload, parse_response=False)
-        return response
+        parameters = prepare_query_params(query, field_mapping, args)
+        return self.uc.delete(url, query=parameters, parse_response=False)
+
+    def list_oms_servers(self):
+        url="/resources/omsserver/list"
+        return self.uc.get(url)
```

### Comparing `uac-api-0.2.3/uacapi/payload.py` & `uac-api-0.3.0/uac_api/payload.py`

 * *Files identical despite different names*

### Comparing `uac-api-0.2.3/uacapi/scripts.py` & `uac-api-0.3.0/uac_api/scripts.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,54 +1,57 @@
-from .utils import prepare_payload
+from .utils import prepare_payload, prepare_query_params
 
 class Scripts:
     def __init__(self, uc) -> None:
         self.log = uc.log
         self.headers = uc.headers
         self.uc = uc
-        self.field_mapping = {
-            "script_name": "scriptname",
-            "script_id": "scriptid",
+
+    def get_script(self, query=None, **args):
+        '''
+        Arguments:
+        - scriptid: scriptid 
+        - scriptname: scriptname 
+        '''
+        url="/resources/script"
+        field_mapping={
+            "scriptid": "scriptid", 
+            "scriptname": "scriptname", 
         }
+        parameters = prepare_query_params(query, field_mapping, args)
+        return self.uc.get(url, query=parameters)
 
-    def list_scripts(self):
-        url = "/script/list"
-        response = self.uc.get(url)
-        return response
-
-    def read_script(self, query=None, **args):
-        """
-        Read script details.
-        Args:
-        - query: Query parameters
-        Args:
-        - script_id: Script ID
-        - script_name: Script name
-        """
-        url = "/script"
-        parameters = prepare_payload(query, self.field_mapping, args)
-        response = self.uc.get(url, query=parameters)
-        return response
-
-    def modify_script(self, payload):
-        url = "/script"
-        response = self.uc.put(url, query="", json_data=payload)
-        return response
-
-    def create_script(self, payload):
-        url = "/script"
-        response = self.uc.post(url, query="", json_data=payload)
-        return response
+    def update_script(self, payload=None, **args):
+        url="/resources/script"
+        _payload = payload
+        return self.uc.put(url, json_data=_payload)
+
+    def create_script(self, payload=None, **args):
+        '''
+        Arguments:
+        - retainSysIds: retainSysIds 
+            False will ignore sysIds in the payload and create a new task  
+        '''
+        url="/resources/script"
+        field_mapping={
+          "retainSysIds": "retainSysIds", 
+        }
+        _payload = prepare_payload(payload, field_mapping, args)
+        return self.uc.post(url, json_data=_payload)
 
     def delete_script(self, query=None, **args):
-        """
-        Delete script.
-        Args:
-        - query: Query parameters
-        Args:
-        - script_id: Script ID
-        - script_name: Script name
-        """
-        url = "/script"
-        parameters = prepare_payload(query, self.field_mapping, args)
-        response = self.uc.delete(url, query=parameters)
-        return response
+        '''
+        Arguments:
+        - scriptid: scriptid 
+        - scriptname: scriptname 
+        '''
+        url="/resources/script"
+        field_mapping={
+          "scriptid": "scriptid", 
+          "scriptname": "scriptname", 
+        }
+        parameters = prepare_query_params(query, field_mapping, args)
+        return self.uc.delete(url, query=parameters, parse_response=False)
+
+    def list_scripts(self):
+        url="/resources/script/list"
+        return self.uc.get(url)
```

### Comparing `uac-api-0.2.3/uacapi/utils.py` & `uac-api-0.3.0/uac_api/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -169,32 +169,56 @@
             program_name["value"] = "${program_name}"
 
         program_short_name = json_content.get("textField7")
         if program_short_name.get("name") == "program_short_name":
             program_short_name["value"] = "${program_short_name}"
     finally:
         return json_content
+
+def snake_to_camel(snake_case_str):
+    """Converts a snake_case string to camelCase.
+
+    Args:
+        snake_case_str: The string in snake_case format.
+
+    Returns:
+        The converted string in camelCase format.
+    """
+    components = snake_case_str.split('_')
+    return components[0] + ''.join(x.title() for x in components[1:])
     
 def prepare_payload(payload, field_mapping, args):
     _payload = None
     if payload is not None:
         _payload = payload
     else:
         _payload = { }
-        # Process additional arguments (**args)
-        for arg_key, arg_value in args.items():
-            if arg_key in field_mapping:
-                _payload[field_mapping[arg_key]] = arg_value
     
+    # Process additional arguments (**args)
+    for arg_key, arg_value in args.items():
+        if arg_key in field_mapping:
+            _payload[field_mapping[arg_key]] = arg_value
+        elif snake_to_camel(arg_key) in field_mapping:
+            _payload[field_mapping[snake_to_camel(arg_key)]] = arg_value
+        else:
+            for key, value in field_mapping.items():
+                if key.lower() == snake_to_camel(arg_key).lower():
+                    _payload[key] = arg_value
     return _payload
 
 def prepare_query_params(query, field_mapping, args):
     if query is not None:
         parameters = query
     else:
         parameters = []
         
         for field, var in args.items():
             if field in field_mapping:
                 append_if_not_none(parameters, var, field_mapping[field] + "={var}")
+            elif snake_to_camel(field) in field_mapping:
+                append_if_not_none(parameters, var, field_mapping[snake_to_camel(field)] + "={var}")
+            else:
+                for key, value in field_mapping.items():
+                    if key.lower() == snake_to_camel(field).lower():
+                        append_if_not_none(parameters, var, key + "={var}")
         
     return parameters
```

