# Comparing `tmp/pulumi_splunk-1.3.0a1713904842.tar.gz` & `tmp/pulumi_splunk-1.3.0a1714113247.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_splunk-1.3.0a1713904842.tar", last modified: Tue Apr 23 20:46:38 2024, max compression
+gzip compressed data, was "pulumi_splunk-1.3.0a1714113247.tar", last modified: Fri Apr 26 06:42:45 2024, max compression
```

## Comparing `pulumi_splunk-1.3.0a1713904842.tar` & `pulumi_splunk-1.3.0a1714113247.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:46:38.097815 pulumi_splunk-1.3.0a1713904842/
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-23 20:46:38.097815 pulumi_splunk-1.3.0a1713904842/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:46:38.097815 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/
--rw-r--r--   0 runner    (1001) docker     (127)     5441 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   148655 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/admin_saml_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    38750 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/apps_local.py
--rw-r--r--   0 runner    (1001) docker     (127)    21899 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/authentication_users.py
--rw-r--r--   0 runner    (1001) docker     (127)    45836 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/authorization_roles.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:46:38.097815 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    10038 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/configs_conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    14395 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/data_ui_views.py
--rw-r--r--   0 runner    (1001) docker     (127)    12228 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/generic_acl.py
--rw-r--r--   0 runner    (1001) docker     (127)    24990 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/global_http_event_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)   154850 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/indexes.py
--rw-r--r--   0 runner    (1001) docker     (127)    23782 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/inputs_http_event_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)    42116 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/inputs_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)    29975 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/inputs_script.py
--rw-r--r--   0 runner    (1001) docker     (127)    18917 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/inputs_tcp_cooked.py
--rw-r--r--   0 runner    (1001) docker     (127)    36618 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/inputs_tcp_raw.py
--rw-r--r--   0 runner    (1001) docker     (127)    10593 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/inputs_tcp_splunk_tcp_token.py
--rw-r--r--   0 runner    (1001) docker     (127)    13939 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/inputs_tcp_ssl.py
--rw-r--r--   0 runner    (1001) docker     (127)    34245 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/inputs_udp.py
--rw-r--r--   0 runner    (1001) docker     (127)   127784 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    44031 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/outputs_tcp_default.py
--rw-r--r--   0 runner    (1001) docker     (127)    43483 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/outputs_tcp_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    31965 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/outputs_tcp_server.py
--rw-r--r--   0 runner    (1001) docker     (127)    27871 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/outputs_tcp_syslog.py
--rw-r--r--   0 runner    (1001) docker     (127)     9916 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   514483 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/saved_searches.py
--rw-r--r--   0 runner    (1001) docker     (127)    17022 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/sh_indexes_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:46:38.097815 pulumi_splunk-1.3.0a1713904842/pulumi_splunk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-23 20:46:38.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-23 20:46:38.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 20:46:38.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-23 20:46:38.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-23 20:46:38.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 20:46:38.097815 pulumi_splunk-1.3.0a1713904842/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:42:45.454488 pulumi_splunk-1.3.0a1714113247/
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-26 06:42:45.450488 pulumi_splunk-1.3.0a1714113247/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-04-26 06:42:38.000000 pulumi_splunk-1.3.0a1714113247/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:42:45.450488 pulumi_splunk-1.3.0a1714113247/pulumi_splunk/
+-rw-r--r--   0 runner    (1001) docker     (127)     5441 2024-04-26 06:42:38.000000 pulumi_splunk-1.3.0a1714113247/pulumi_splunk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   148655 2024-04-26 06:42:38.000000 pulumi_splunk-1.3.0a1714113247/pulumi_splunk/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-26 06:42:38.000000 pulumi_splunk-1.3.0a1714113247/pulumi_splunk/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-04-26 06:42:38.000000 pulumi_splunk-1.3.0a1714113247/pulumi_splunk/admin_saml_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38750 2024-04-26 06:42:38.000000 pulumi_splunk-1.3.0a1714113247/pulumi_splunk/apps_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21899 2024-04-26 06:42:38.000000 pulumi_splunk-1.3.0a1714113247/pulumi_splunk/authentication_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45836 2024-04-26 06:42:38.000000 pulumi_splunk-1.3.0a1714113247/pulumi_splunk/authorization_roles.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:42:45.450488 pulumi_splunk-1.3.0a1714113247/pulumi_splunk/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-26 06:42:38.000000 pulumi_splunk-1.3.0a1714113247/pulumi_splunk/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-26 06:42:38.000000 pulumi_splunk-1.3.0a1714113247/pulumi_splunk/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-26 06:42:38.000000 pulumi_splunk-1.3.0a1714113247/pulumi_splunk/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10038 2024-04-26 06:42:38.000000 pulumi_splunk-1.3.0a1714113247/pulumi_splunk/configs_conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14395 2024-04-26 06:42:38.000000 pulumi_splunk-1.3.0a1714113247/pulumi_splunk/data_ui_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12228 2024-04-26 06:42:38.000000 pulumi_splunk-1.3.0a1714113247/pulumi_splunk/generic_acl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24990 2024-04-26 06:42:38.000000 pulumi_splunk-1.3.0a1714113247/pulumi_splunk/global_http_event_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)   154850 2024-04-26 06:42:38.000000 pulumi_splunk-1.3.0a1714113247/pulumi_splunk/indexes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23782 2024-04-26 06:42:38.000000 pulumi_splunk-1.3.0a1714113247/pulumi_splunk/inputs_http_event_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42116 2024-04-26 06:42:38.000000 pulumi_splunk-1.3.0a1714113247/pulumi_splunk/inputs_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29975 2024-04-26 06:42:38.000000 pulumi_splunk-1.3.0a1714113247/pulumi_splunk/inputs_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18917 2024-04-26 06:42:38.000000 pulumi_splunk-1.3.0a1714113247/pulumi_splunk/inputs_tcp_cooked.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36618 2024-04-26 06:42:38.000000 pulumi_splunk-1.3.0a1714113247/pulumi_splunk/inputs_tcp_raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10593 2024-04-26 06:42:38.000000 pulumi_splunk-1.3.0a1714113247/pulumi_splunk/inputs_tcp_splunk_tcp_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13939 2024-04-26 06:42:38.000000 pulumi_splunk-1.3.0a1714113247/pulumi_splunk/inputs_tcp_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34245 2024-04-26 06:42:38.000000 pulumi_splunk-1.3.0a1714113247/pulumi_splunk/inputs_udp.py
+-rw-r--r--   0 runner    (1001) docker     (127)   127784 2024-04-26 06:42:38.000000 pulumi_splunk-1.3.0a1714113247/pulumi_splunk/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44031 2024-04-26 06:42:38.000000 pulumi_splunk-1.3.0a1714113247/pulumi_splunk/outputs_tcp_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43483 2024-04-26 06:42:38.000000 pulumi_splunk-1.3.0a1714113247/pulumi_splunk/outputs_tcp_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31965 2024-04-26 06:42:38.000000 pulumi_splunk-1.3.0a1714113247/pulumi_splunk/outputs_tcp_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27871 2024-04-26 06:42:38.000000 pulumi_splunk-1.3.0a1714113247/pulumi_splunk/outputs_tcp_syslog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9916 2024-04-26 06:42:38.000000 pulumi_splunk-1.3.0a1714113247/pulumi_splunk/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-26 06:42:38.000000 pulumi_splunk-1.3.0a1714113247/pulumi_splunk/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 06:42:38.000000 pulumi_splunk-1.3.0a1714113247/pulumi_splunk/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   514483 2024-04-26 06:42:38.000000 pulumi_splunk-1.3.0a1714113247/pulumi_splunk/saved_searches.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17022 2024-04-26 06:42:38.000000 pulumi_splunk-1.3.0a1714113247/pulumi_splunk/sh_indexes_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:42:45.450488 pulumi_splunk-1.3.0a1714113247/pulumi_splunk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-26 06:42:45.000000 pulumi_splunk-1.3.0a1714113247/pulumi_splunk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-26 06:42:45.000000 pulumi_splunk-1.3.0a1714113247/pulumi_splunk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 06:42:45.000000 pulumi_splunk-1.3.0a1714113247/pulumi_splunk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-26 06:42:45.000000 pulumi_splunk-1.3.0a1714113247/pulumi_splunk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-26 06:42:45.000000 pulumi_splunk-1.3.0a1714113247/pulumi_splunk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-26 06:42:38.000000 pulumi_splunk-1.3.0a1714113247/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 06:42:45.454488 pulumi_splunk-1.3.0a1714113247/setup.cfg
```

### Comparing `pulumi_splunk-1.3.0a1713904842/PKG-INFO` & `pulumi_splunk-1.3.0a1714113247/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_splunk
-Version: 1.3.0a1713904842
+Version: 1.3.0a1714113247
 Summary: A Pulumi package for creating and managing splunk cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-splunk
 Keywords: pulumi,splunk
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_splunk-1.3.0a1713904842/README.md` & `pulumi_splunk-1.3.0a1714113247/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1713904842/pulumi_splunk/__init__.py` & `pulumi_splunk-1.3.0a1714113247/pulumi_splunk/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1713904842/pulumi_splunk/_inputs.py` & `pulumi_splunk-1.3.0a1714113247/pulumi_splunk/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1713904842/pulumi_splunk/_utilities.py` & `pulumi_splunk-1.3.0a1714113247/pulumi_splunk/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1713904842/pulumi_splunk/admin_saml_groups.py` & `pulumi_splunk-1.3.0a1714113247/pulumi_splunk/admin_saml_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1713904842/pulumi_splunk/apps_local.py` & `pulumi_splunk-1.3.0a1714113247/pulumi_splunk/apps_local.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1713904842/pulumi_splunk/authentication_users.py` & `pulumi_splunk-1.3.0a1714113247/pulumi_splunk/authentication_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1713904842/pulumi_splunk/authorization_roles.py` & `pulumi_splunk-1.3.0a1714113247/pulumi_splunk/authorization_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1713904842/pulumi_splunk/config/__init__.pyi` & `pulumi_splunk-1.3.0a1714113247/pulumi_splunk/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1713904842/pulumi_splunk/config/vars.py` & `pulumi_splunk-1.3.0a1714113247/pulumi_splunk/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1713904842/pulumi_splunk/configs_conf.py` & `pulumi_splunk-1.3.0a1714113247/pulumi_splunk/configs_conf.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1713904842/pulumi_splunk/data_ui_views.py` & `pulumi_splunk-1.3.0a1714113247/pulumi_splunk/data_ui_views.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1713904842/pulumi_splunk/generic_acl.py` & `pulumi_splunk-1.3.0a1714113247/pulumi_splunk/generic_acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1713904842/pulumi_splunk/global_http_event_collector.py` & `pulumi_splunk-1.3.0a1714113247/pulumi_splunk/global_http_event_collector.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1713904842/pulumi_splunk/indexes.py` & `pulumi_splunk-1.3.0a1714113247/pulumi_splunk/indexes.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1713904842/pulumi_splunk/inputs_http_event_collector.py` & `pulumi_splunk-1.3.0a1714113247/pulumi_splunk/inputs_http_event_collector.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1713904842/pulumi_splunk/inputs_monitor.py` & `pulumi_splunk-1.3.0a1714113247/pulumi_splunk/inputs_monitor.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1713904842/pulumi_splunk/inputs_script.py` & `pulumi_splunk-1.3.0a1714113247/pulumi_splunk/inputs_script.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1713904842/pulumi_splunk/inputs_tcp_cooked.py` & `pulumi_splunk-1.3.0a1714113247/pulumi_splunk/inputs_tcp_cooked.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1713904842/pulumi_splunk/inputs_tcp_raw.py` & `pulumi_splunk-1.3.0a1714113247/pulumi_splunk/inputs_tcp_raw.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1713904842/pulumi_splunk/inputs_tcp_splunk_tcp_token.py` & `pulumi_splunk-1.3.0a1714113247/pulumi_splunk/inputs_tcp_splunk_tcp_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1713904842/pulumi_splunk/inputs_tcp_ssl.py` & `pulumi_splunk-1.3.0a1714113247/pulumi_splunk/inputs_tcp_ssl.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1713904842/pulumi_splunk/inputs_udp.py` & `pulumi_splunk-1.3.0a1714113247/pulumi_splunk/inputs_udp.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1713904842/pulumi_splunk/outputs.py` & `pulumi_splunk-1.3.0a1714113247/pulumi_splunk/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1713904842/pulumi_splunk/outputs_tcp_default.py` & `pulumi_splunk-1.3.0a1714113247/pulumi_splunk/outputs_tcp_default.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1713904842/pulumi_splunk/outputs_tcp_group.py` & `pulumi_splunk-1.3.0a1714113247/pulumi_splunk/outputs_tcp_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1713904842/pulumi_splunk/outputs_tcp_server.py` & `pulumi_splunk-1.3.0a1714113247/pulumi_splunk/outputs_tcp_server.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1713904842/pulumi_splunk/outputs_tcp_syslog.py` & `pulumi_splunk-1.3.0a1714113247/pulumi_splunk/outputs_tcp_syslog.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1713904842/pulumi_splunk/provider.py` & `pulumi_splunk-1.3.0a1714113247/pulumi_splunk/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1713904842/pulumi_splunk/saved_searches.py` & `pulumi_splunk-1.3.0a1714113247/pulumi_splunk/saved_searches.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1713904842/pulumi_splunk/sh_indexes_manager.py` & `pulumi_splunk-1.3.0a1714113247/pulumi_splunk/sh_indexes_manager.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1713904842/pulumi_splunk.egg-info/PKG-INFO` & `pulumi_splunk-1.3.0a1714113247/pulumi_splunk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_splunk
-Version: 1.3.0a1713904842
+Version: 1.3.0a1714113247
 Summary: A Pulumi package for creating and managing splunk cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-splunk
 Keywords: pulumi,splunk
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_splunk-1.3.0a1713904842/pulumi_splunk.egg-info/SOURCES.txt` & `pulumi_splunk-1.3.0a1714113247/pulumi_splunk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1713904842/pyproject.toml` & `pulumi_splunk-1.3.0a1714113247/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_splunk"
   description = "A Pulumi package for creating and managing splunk cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0a1,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "splunk"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "1.3.0a1713904842"
+  version = "1.3.0a1714113247"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-splunk"
 
 [build-system]
```
