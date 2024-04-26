# Comparing `tmp/ck_apstra_api-0.3.2.tar.gz` & `tmp/ck_apstra_api-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ck_apstra_api-0.3.2.tar", max compression
+gzip compressed data, was "ck_apstra_api-0.3.3.tar", max compression
```

## Comparing `ck_apstra_api-0.3.2.tar` & `ck_apstra_api-0.3.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1068 2023-09-28 00:59:26.688335 ck_apstra_api-0.3.2/LICENSE
--rw-r--r--   0        0        0     1226 2023-11-24 23:30:58.367886 ck_apstra_api-0.3.2/README.md
--rw-r--r--   0        0        0     1159 2024-04-23 22:16:41.771405 ck_apstra_api-0.3.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-09-28 01:27:34.624568 ck_apstra_api-0.3.2/src/ck_apstra_api/__init__.py
--rwxr-xr-x   0        0        0    32668 2024-04-23 19:17:44.299909 ck_apstra_api-0.3.2/src/ck_apstra_api/apstra_blueprint.py
--rwxr-xr-x   0        0        0     8468 2024-04-23 18:59:16.565550 ck_apstra_api-0.3.2/src/ck_apstra_api/apstra_session.py
--rw-r--r--   0        0        0     9265 2023-11-29 15:30:29.638239 ck_apstra_api-0.3.2/src/ck_apstra_api/cli.py
--rw-r--r--   0        0        0    25422 2024-04-23 21:12:17.400215 ck_apstra_api-0.3.2/src/ck_apstra_api/generic_system.py
--rw-r--r--   0        0        0    11866 2023-10-23 01:37:34.339126 ck_apstra_api-0.3.2/src/ck_apstra_api/ip_endpoint.py
--rw-r--r--   0        0        0     2346 2023-11-17 18:23:57.618869 ck_apstra_api-0.3.2/src/ck_apstra_api/pull_device_configuration.py
--rw-r--r--   0        0        0     1861 1970-01-01 00:00:00.000000 ck_apstra_api-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-09-28 00:59:26.688335 ck_apstra_api-0.3.3/LICENSE
+-rw-r--r--   0        0        0     1214 2024-04-26 20:50:38.182562 ck_apstra_api-0.3.3/README.md
+-rw-r--r--   0        0        0     1695 2024-04-26 21:43:33.250610 ck_apstra_api-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-09-28 01:27:34.624568 ck_apstra_api-0.3.3/src/ck_apstra_api/__init__.py
+-rwxr-xr-x   0        0        0    33225 2024-04-26 21:40:34.126716 ck_apstra_api-0.3.3/src/ck_apstra_api/apstra_blueprint.py
+-rwxr-xr-x   0        0        0     8575 2024-04-26 20:40:45.858504 ck_apstra_api-0.3.3/src/ck_apstra_api/apstra_session.py
+-rw-r--r--   0        0        0     9265 2023-11-29 15:30:29.638239 ck_apstra_api-0.3.3/src/ck_apstra_api/cli.py
+-rw-r--r--   0        0        0    27268 2024-04-26 21:40:01.932382 ck_apstra_api-0.3.3/src/ck_apstra_api/generic_system.py
+-rw-r--r--   0        0        0    11866 2023-10-23 01:37:34.339126 ck_apstra_api-0.3.3/src/ck_apstra_api/ip_endpoint.py
+-rw-r--r--   0        0        0     2346 2023-11-17 18:23:57.618869 ck_apstra_api-0.3.3/src/ck_apstra_api/pull_device_configuration.py
+-rw-r--r--   0        0        0     1882 1970-01-01 00:00:00.000000 ck_apstra_api-0.3.3/PKG-INFO
```

### Comparing `ck_apstra_api-0.3.2/LICENSE` & `ck_apstra_api-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ck_apstra_api-0.3.2/README.md` & `ck_apstra_api-0.3.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # ck-apstra-api
 
 
 ## prepare venv
 
 ```
-python3.11 -m venv venv
-source venv/bin/activate
-pip install ck-apstra-api
+uv venv
+source .venv/bin/activate
+uv pip install ck-apstra-api
 ```
 
 
 ## var/.env file example
 
 ```
 apstra_server_host=local-apstra.pslab.link
```

### Comparing `ck_apstra_api-0.3.2/src/ck_apstra_api/apstra_blueprint.py` & `ck_apstra_api-0.3.3/src/ck_apstra_api/apstra_blueprint.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 #!/usr/bin/env python3
 
 import logging
-from typing import List, Optional, Tuple
+from typing import List, Optional
 import uuid
 from enum import StrEnum
 from functools import cache
 
+from result import Err, Result, Ok
+
 from ck_apstra_api.apstra_session import CkApstraSession
 from ck_apstra_api.apstra_session import prep_logging
 
 
 class CkEnum(StrEnum):
     MEMBER_SWITCH = 'member_switch'
     MEMBER_INTERFACE = 'member_interface'
@@ -91,15 +93,15 @@
             'id': "43964eca-9b21-4144-8c44-9f173c224623",
             'source_versions': { "config_blueprint": 6051 }
           }
         """
         return self.session.get_items(f"blueprints/{self.id}")
 
     # def query(self, query_string: str, print_prefix: str = None, multiline: bool = False) -> list:
-    def query(self, query_string: str) -> Tuple[Optional[List], Optional[str]]:
+    def query(self, query_string: str) -> Result[List, str]:
         """
         Query the Apstra API.
 
         Args:
             query: The query string.
             strip: Strip the query string. Required in case of multi-line query.
 
@@ -110,56 +112,59 @@
         query_candidate = query_string.strip().replace("\n", '')        
         url = f"{self.url_prefix}/qe"
         payload = {
             "query": query_candidate
         }
         response = self.session.session.post(url, json=payload)
         if response.status_code != 200:
-            return None, f"status_code is not 200 {response.status_code=} != 200: {payload=}, {response.text=}"
+            return Err(f"status_code is not 200 {response.status_code=} != 200: {payload=}, {response.text=}")
         # the content should have 'items'. otherwise, the query would be invalid
         elif 'items' not in response.json():
-            return None, f"items does not exist: {query_string=}, {response.text=}"
-        return response.json()['items'], None
+            return Err(f"items does not exist: {query_string=}, {response.text=}")
+        return Ok(response.json()['items'])
     
     # TODO: integrate with other functions
     def get_managed_system_nodes(self):
         SYSTEM_NODE_NAME='system'
         system_query = f"node('system', system_type='switch', management_level='full_control', name='{SYSTEM_NODE_NAME}')"
         resp, error = self.query(system_query)
         self.managed_system_nodes = [x[SYSTEM_NODE_NAME] for x in resp]
         return self.managed_system_nodes
 
     
     # return the first entry for the system
     # @cache
-    def get_system_with_im(self, system_label) -> Tuple[Optional[dict], Optional[str]]:
-        system_im, error = self.query(f"node('system', label='{system_label}', name='system').out().node('interface_map', name='im')")
+    def get_system_with_im(self, system_label) -> Result[dict,str]:
+        system_im_result = self.query(f"node('system', label='{system_label}', name='system').out().node('interface_map', name='im')")
         # if system_label not in self.system_label_2_id_cache:
         #     # self.system_label_2_id_cache[system_label] = { 'id': system_im['system']['id'] }
         #     # self.system_id_2_label_cache[system_im['system']['id']] = system_label
         #     if  'interface_map_id' not in self.system_label_2_id_cache[system_label]:
         #         self.system_label_2_id_cache[system_label]['interface_map_id'] = system_im['im']['id']
         #         self.system_label_2_id_cache[system_label]['device_profile_id'] = system_im['im']['device_profile_id']
-        return system_im[0], error
+        if isinstance(system_im_result, Err):
+            error_message = f"Error: {system_label=}\n\tquery() {system_im_result.err_value=}"
+            return Err(error_message)
+        return Ok(system_im_result.ok_value[0])
 
     # can be checked before the system creation - should not be cached in such case
     # @cache
-    def get_system_node_from_label(self, system_label) -> Tuple[Optional[dict], Optional[str]]:
+    def get_system_node_from_label(self, system_label) -> Result[dict, str]:
         """
         Return the system dict from the system label
         called from move_access_switch
         """
         query = f"node('system', label='{system_label}', name='system')"
-        system_query_result, error = self.query(query)
-        if error:
-            return None, f"{system_label} not found for {query}: from query: {error}"
+        system_query_result = self.query(query)
+        if isinstance(system_query_result, Err):
+            return Err(f"{system_label} not found for {query}: from query: {error}")
         # self.logger.warning(f"{system_label=} {system_query_result=}")
-        if len(system_query_result) == 0:
-            return None, None
-        return system_query_result[0]['system'], None
+        if len(system_query_result.ok_value) == 0:
+            return Ok({})
+        return Ok(system_query_result.ok_value[0]['system'])
 
 
     def get_system_label(self, system_id):
         '''
         Get the system label from the system id
         '''
         if system_id not in self.system_id_2_label_cache:
@@ -195,15 +200,15 @@
             optional(
                 node('tag', name='{CkEnum.TAG}').out().node(name='{CkEnum.LINK}')
             )
         )"""
         # self.logger.warning(f"get_server_interface_nodes() {system_label=} {interface_query=}")
         return self.query(interface_query)
 
-    def get_switch_interface_nodes(self, switch_labels=None, intf_name=None) -> str:
+    def get_switch_interface_nodes(self, switch_labels=None, intf_name=None) -> Result[List, str]:
         """
         Return interface nodes of the switches
             switch_labels: list of system labels, a str for the single system label, or None for all switches
             return CkEnum.MEMBER_INTERFACE and CkEnum.MEMBER_SWITCH
                 optionally CkEnum.EVPN_INTERFACE if it is a LAG
             It can be used for VLAN CT association
             TODO: implement intf_name in case of multiple link generic system
@@ -235,16 +240,16 @@
                 node(name='{CkEnum.MEMBER_INTERFACE}')
                     .in_('composed_of').node('interface', name='{CkEnum.AE_INTERFACE}')
             ),
             optional(
                 node('tag', name='{CkEnum.TAG}').out().node(name='{CkEnum.LINK}')
             )
         )"""
-        interface_nodes, error = self.query(interface_query)
-        return interface_nodes
+        interface_nodes_result = self.query(interface_query)
+        return interface_nodes_result
 
     def get_single_vlan_ct_id(self, vn_id: int):
         '''
         Get the single VLAN CT ID
 
         Return tuple of (tagged CT id, untagged CT id)
         '''
@@ -268,78 +273,83 @@
         Get the CT IDs from the CT labels
         '''
         if isinstance(ct_labels, str):
             ct_labels = [ct_labels]
         ct_list_query = f"""
             node('ep_endpoint_policy', policy_type_name='batch', label=is_in({ct_labels}), name='ep')
         """
-        ct_list, error = self.query(ct_list_query)
+        ct_list_result = self.query(ct_list_query)
+        if isinstance(ct_list_result, Err):
+            return Err(f"Error: {ct_list_result.err_value=}")
+        ct_list = ct_list_result.ok_value
         if len(ct_list) == 0:
             self.logger.debug(f"No CTs found for {ct_labels=}")
             return []
         return [x['ep']['id'] for x in ct_list]
     
-    def add_generic_system(self, generic_system_spec: dict) -> Tuple[Optional[List], Optional[str]]:
+    def add_generic_system(self, generic_system_spec: dict) -> Result[List, str]:
         """
         Add a generic system (and access switch pair) to the blueprint.
 
         Args:
             generic_system_spec: The specification of the generic system.
 
         Returns:
             The ID of the switch-system-link ids.
         """
         new_generic_system_label = generic_system_spec['new_systems'][0]['label']
         existing_system_query = f"node('system', label='{new_generic_system_label}', name='system')"
-        existing_system, error = self.query(existing_system_query)
-        if len(existing_system) > 0:
+        existing_system_result = self.query(existing_system_query)
+        if len(existing_system_result.ok_value) > 0:
             # skipping if the system already exists
             # return []
-            return [], None
+            return Ok([])
         url = f"{self.url_prefix}/switch-system-links"
         created_generic_system = self.session.session.post(url, json=generic_system_spec)
         if created_generic_system.status_code >= 400:
             # self.logger.error(f"System not created: {created_generic_system=}, {new_generic_system_label=}, {created_generic_system.text=}")
-            return [], f"System not created: {created_generic_system=}, {new_generic_system_label=}, {created_generic_system.text=}"
+            return Err(f"System not created: {created_generic_system=}, {new_generic_system_label=}, {created_generic_system.text=}")
         # which case?
         if created_generic_system is None or len(created_generic_system.json()) == 0 or 'ids' not in created_generic_system.json():
-            return [], None
-        return created_generic_system.json()['ids'], None
+            return Err("Not created")
+        return Ok(created_generic_system.json()['ids'])
 
-    def get_transformation_id(self, system_label, intf_name, speed) -> Tuple[Optional[int], Optional[str]]:
+    def get_transformation_id(self, system_label, intf_name, speed) -> Result[int, str]:
         '''
         Get the transformation ID for the interface
 
         Args:
             system_label: The label of the system
             intf_name: The name of the interface
             speed: The speed of the interface in the format of '10G'
         '''
         # the unit is in uppercase
         speed = speed.upper()
-        system_im, error = self.get_system_with_im(system_label)
-        if error:
-            return None, f"{system_label=} {intf_name=} {speed=}\n\tError get_system_with_im {error=}"
-        device_profile, error = self.session.get_device_profile(system_im['im']['device_profile_id'])
-        if error:
-            return None, f"{system_label=} {intf_name=} {speed=}\n\tError get_device_profile {error=}"
+        system_im_result = self.get_system_with_im(system_label)
+        if isinstance(system_im_result, Err):
+            return Err(f"{system_label=} {intf_name=} {speed=}\n\tError get_system_with_im {error=}")
+        system_im = system_im_result.ok_value
+        device_profile_result = self.session.get_device_profile(system_im['im']['device_profile_id'])
+        if isinstance(device_profile_result, Err):
+            return Err(f"{system_label=} {intf_name=} {speed=}\n\tError get_device_profile {device_profile_result.err_value=}")
+        device_profile = device_profile_result.ok_value
         if 'ports' not in device_profile:
-            return None, f"{system_label=} {intf_name=} {speed=}\n\tError: no ports in device profile {device_profile=}"
+            return Err(f"{system_label=} {intf_name=} {speed=}\n\tError: no ports in device profile {device_profile=}")
         for port in device_profile['ports']:
             if 'transformations' not in port:
-                return None, f"{system_label=} {intf_name=} {speed=}\n\tError: no transformations in port {port=}"         
+                return Err(f"{system_label=} {intf_name=} {speed=}\n\tError: no transformations in port {port=}")    
             for transformation in port['transformations']:
                 # self.logger.debug(f"{transformation=}")
                 for intf in transformation['interfaces']:
                     # if intf['name'] == intf_name:
                     #     self.logger.debug(f"{intf=}")
                     if intf['name'] == intf_name and intf['speed']['unit'] == speed[-1:] and intf['speed']['value'] == int(speed[:-1]): 
                         # self.logger.warning(f"{intf_name=}, {intf=}")
-                        return transformation['transformation_id'], None
-        return None, f"transformation not found for {system_label=} {intf_name=} {speed=}"
+                        return Ok(transformation['transformation_id'])
+        return Err(f"transformation not found for {system_label=} {intf_name=} {speed=}")
 
     def patch_leaf_server_link(self, link_spec: dict) -> None:
         """
         Patch a leaf-server link.
 
         Args:
             link_spec: The specification of the leaf-server link.
@@ -427,17 +437,17 @@
         if len(the_nodes_list) == 0:
             self.logger.warning(f"{nodes=} is not a list or string")
             return
         # in case of single tags_to_add
         if isinstance(tags_to_add, str):
             tags_to_add = [tags_to_add]
         # no need to check the present of tags in tags_to_add 
-        tag_nodes, error = self.query(f"node(id=is_in({the_nodes_list})).in_().node('tag', label=is_in({tags_to_add}), name='tag')")
-        are_tags_the_same = len(tag_nodes) == (len(tags_to_add) * len(nodes))
-        self.logger.debug(f"{nodes=} {the_nodes_list=} {tags_to_add=}, {tags_to_remove=}, {are_tags_the_same=} {tag_nodes}")
+        tag_nodes_result = self.query(f"node(id=is_in({the_nodes_list})).in_().node('tag', label=is_in({tags_to_add}), name='tag')")
+        are_tags_the_same = len(tag_nodes_result.ok_value) == (len(tags_to_add) * len(nodes))
+        self.logger.debug(f"{nodes=} {the_nodes_list=} {tags_to_add=}, {tags_to_remove=}, {are_tags_the_same=} {tag_nodes_result.ok_value}")
 
         # self.logger.debug(f"{nodes=} {tags_to_add=}, {tags_to_remove=} {are_tags_the_same=}")
         # The tags are the same as the existing tags
         # if are_tags_the_same or (not tags_to_add and not tags_to_remove):
         #     return
         tagging_spec['nodes'] = the_nodes_list
         tagging_spec['add'] = tags_to_add
```

### Comparing `ck_apstra_api-0.3.2/src/ck_apstra_api/apstra_session.py` & `ck_apstra_api-0.3.3/src/ck_apstra_api/apstra_session.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #!/usr/bin/env python3
 from functools import cache
-from typing import Optional, Tuple
+from typing import Optional
 import requests
 import urllib3
 import logging
 import time
 from datetime import datetime
-
+from result import Result, Ok, Err
 
 class CustomFormatter(logging.Formatter):
     grey = "\x1b[38;20m"
     yellow = "\x1b[33;20m"
     red = "\x1b[31;20m"
     bold_red = "\x1b[31;1m"
     reset = "\x1b[0m"
@@ -124,29 +124,31 @@
         Returns:
             True if the Apstra controller is online, False otherwise.
         """
         return self.token is not None
 
 
     @cache
-    def get_device_profile(self, device_profile_name: str = None) -> Tuple[Optional[dict], Optional[str]]:
+    def get_device_profile(self, device_profile_name: str = None) -> Result[dict, str]:
         """
         Get the device profile with the specified name.
 
         Args:
             name: The name of the device profile.
 
         Returns:
             The device profile, or None if the device profile does not exist.
         """
         if device_profile_name is None:
-            return None, f"Error: {device_profile_name=}"
+            return Err(f"Error: {device_profile_name=}")
+            # return None, f"Error: {device_profile_name=}"
         device_profiles = self.get_items('device-profiles')['items']
         the_device_profile = [x for x in device_profiles if x['id'] == device_profile_name][0]
-        return the_device_profile, None
+        return Ok(the_device_profile)
+        # return the_device_profile, None
 
 
     def get_logical_device(self, id: int) -> dict:
         """
         Get the logical device with the specified ID.
 
         Args:
```

### Comparing `ck_apstra_api-0.3.2/src/ck_apstra_api/cli.py` & `ck_apstra_api-0.3.3/src/ck_apstra_api/cli.py`

 * *Files identical despite different names*

### Comparing `ck_apstra_api-0.3.2/src/ck_apstra_api/generic_system.py` & `ck_apstra_api-0.3.3/src/ck_apstra_api/generic_system.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 
 import logging
 from math import isnan
 from pathlib import Path
-from typing import List, Optional, Any, Tuple, TypeVar, Annotated
+from typing import List, Optional, Any, TypeVar, Annotated
 import os
 import uuid
 
+from result import Result, Ok, Err
+
 from ck_apstra_api.apstra_session import CkApstraSession
 from ck_apstra_api.apstra_blueprint import CkApstraBlueprint, CkEnum
 
 
 def form_lacp(apstra_bp, generic_system_label: str, generic_system_links_list: list):
     # bp = job_env.main_bp
     bp = apstra_bp
@@ -42,15 +44,18 @@
             # skip if now switch is defined
             if not sw_label or not sw_ifname:
                 continue
             if sw_ifname[:2] not in ['et', 'xe', 'ge']:
                 # TODO: should fail on input validation
                 logging.warning(f"form_lacp Skipping: Switch for {generic_system_label}, {sw_ifname[:2]} has invalid interface name {sw_ifname}:{sw_ifname}")
                 continue
-            switch_link_nodes = bp.get_switch_interface_nodes([sw_label], sw_ifname)
+            switch_link_nodes_result = bp.get_switch_interface_nodes([sw_label], sw_ifname)
+            if isinstance(switch_link_nodes_result, Err):
+                return Err(f"form_lacp Err: {sw_label}:{sw_ifname} not found in blueprint {bp.label}")
+            switch_link_nodes = switch_link_nodes_result.ok_value
             if switch_link_nodes is None or len(switch_link_nodes) == 0:
                 logging.warning(f"form_lacp Skipping: Generic system {generic_system_label} has invalid interface {sw_label}:{sw_ifname}")
                 continue
             link_node_id = switch_link_nodes[0][CkEnum.LINK]['id']
             sw_if_node_id = switch_link_nodes[0][CkEnum.MEMBER_INTERFACE]['id']
             gs_if_node_id = switch_link_nodes[0][CkEnum.GENERIC_SYSTEM_INTERFACE]['id']
             link_spec = {
@@ -67,23 +72,24 @@
         if lag_updated:
             logging.warning(f"Unexpected return: LACP updated for generic system {generic_system_label} in blueprint {bp_label}: {lag_updated}")
         # logging.debug(f"lag_updated: {lag_updated}")
     
 
 # def add_tags(job_env: CkJobEnv, generic_system_label: str, generic_system_links_list: list):
 #     bp = job_env.main_bp
-def add_tags(apstra_bp, generic_system_label: str, generic_system_links_list: list) -> Tuple[Optional[str], Optional[str]]:
+def add_tags(apstra_bp, generic_system_label: str, generic_system_links_list: list) -> Result[str, str]:
     bp = apstra_bp
     link_id_num = 0
-    generic_system_node, error = bp.get_system_node_from_label(generic_system_label)
-    if error:
-        logging.warning(f"add_tags skipping: {error}")
-        return None, f"add_tags {generic_system_label} not found in blueprint {bp.label}"
+    generic_system_node_result = bp.get_system_node_from_label(generic_system_label)
+    if isinstance(generic_system_node_result, Err):
+        logging.warning(f"add_tags skipping: {generic_system_node_result.err_value}")
+        return Err(f"add_tags {generic_system_label} not found in blueprint {bp.label}")
+    generic_system_node = generic_system_node_result.ok_value
     if not generic_system_node:
-        return None, f"add_tags {generic_system_label} not found in blueprint {bp.label}"
+        return Err(f"add_tags {generic_system_label} not found in blueprint {bp.label}")
     generic_system_id = generic_system_node['id']
     for link in generic_system_links_list:
         link_id_num += 1
         group_label = f"link{link_id_num}"
         gs_tags = link['gs_tags']
         if len(gs_tags) > 0:
             bp.post_tagging(generic_system_id, tags_to_add=gs_tags)            
@@ -98,25 +104,28 @@
             # the switch label and the interface should be defined. If not, skip
             if not sw_label or not sw_ifname:
                 continue
             # the switch interface name should be legit
             if sw_ifname[:2] not in ['et', 'xe', 'ge']:
                 logging.warning(f"Skipping: Generic system {generic_system_label} has invalid interface name {sw_ifname}")
                 continue
-            switch_link_nodes = bp.get_switch_interface_nodes(sw_label, sw_ifname)
+            switch_link_nodes_result = bp.get_switch_interface_nodes(sw_label, sw_ifname)
+            if isinstance(switch_link_nodes_result, Err):
+                return Err(f"add_tags Err: {sw_label}:{sw_ifname} not found in blueprint {bp.label}")
+            switch_link_nodes = switch_link_nodes_result.ok_value
             if switch_link_nodes is None or len(switch_link_nodes) == 0:
                 logging.warning(f"Skipping: Generic system {generic_system_label} has invalid interface {sw_label}:{sw_ifname}")
                 continue
             link_node_id = switch_link_nodes[0][CkEnum.LINK]['id']
             # logging.debug(f"{member_tags=}")
             if len(member_tags) > 0:
                 logging.debug(f"{member_tags=}")
                 bp.post_tagging(link_node_id, tags_to_add=member_tags)
                 
-    return None, None
+    return Ok('done')
 
 # def rename_generic_system_intf(job_env: CkJobEnv, generic_system_label: str, generic_system_links_list: list):
 #     bp = job_env.main_bp
 def rename_generic_system_intf(apstra_bp, generic_system_label: str, generic_system_links_list: list):
     bp = apstra_bp
     bp_label = bp.label
     patch_cable_map_spec = {
@@ -150,18 +159,21 @@
             gs_ifname = link[f"gs_ifname{member_number}"] if f"gs_ifname{member_number}" in link else link[f"server_intf{member_number}"]
             # skip if data is missing
             if not sw_label or not sw_ifname:
                 continue
             if sw_ifname[:2] not in ['et', 'xe', 'ge']:
                 logging.warning(f"Skipping: Generic system {generic_system_label} has invalid interface name {sw_ifname}")
                 continue
-            switch_link_nodes = bp.get_switch_interface_nodes([sw_label], sw_ifname)
+            switch_link_nodes_result = bp.get_switch_interface_nodes([sw_label], sw_ifname)
             # logging.warning(f"{sw_label=}, {sw_ifname=}, {len(switch_link_nodes)=}")
             # logging.debug(f"{label_label=}, {link[label_label]=}")
             # logging.debug(f"{len(switch_link_nodes)=}, {switch_link_nodes=}")
+            if isinstance(switch_link_nodes_result, Err):
+                return Err(f"rename_generic_system_intf Err: {sw_label}:{sw_ifname} not found in blueprint {bp.label}\n\t get_switch_interface_nodes {switch_link_nodes_result.err_value}") 
+            switch_link_nodes = switch_link_nodes_result.ok_value
             if switch_link_nodes is None or len(switch_link_nodes) == 0:
                 logging.warning(f"Skipping: Generic system {generic_system_label} has invalid interface {sw_label}:{sw_ifname}")
                 continue
             link_node_id = switch_link_nodes[0][CkEnum.LINK]['id']
             sw_if_node_id = switch_link_nodes[0][CkEnum.MEMBER_INTERFACE]['id']
             gs_if_node_id = switch_link_nodes[0][CkEnum.GENERIC_SYSTEM_INTERFACE]['id']
             
@@ -251,15 +263,18 @@
         #         ct_ids.append(bp.get_single_vlan_ct_or_create(untagged_vlan, is_tagged=False))
         #         logging.debug(f"{untagged_vlan=}, {ct_ids=}")
         if 'ct_ids' not in locals():
             logging.debug(f"Skipping: Generic system {generic_system_label} has no CTs")
             continue
         logging.debug(f"{link=} {ct_ids=}")
         # intf_nodes = bp.get_switch_interface_nodes([link['label1']], link['ifname1'])
-        intf_nodes = bp.get_switch_interface_nodes([link['switch1']], link['switch_intf1'])
+        intf_nodes_result = bp.get_switch_interface_nodes([link['switch1']], link['switch_intf1'])
+        if isinstance(intf_nodes_result, Err):
+            return Err(f"assign_connectivity_templates Err: {link['switch1']}:{link['switch_intf1']} not found in blueprint {bp.label}")
+        intf_nodes = intf_nodes_result.ok_value
         if len(intf_nodes) == 0:
             logging.warning(f"{len(intf_nodes)=}, {intf_nodes=}")
             # logging.warning(f"Skipping: Generic system {generic_system_label} has invalid interface {link['label1']}:{link['ifname1']}")
             logging.warning(f"Skipping: Generic system {generic_system_label} has invalid interface {link['switch1']}:{link['switch_intf1']}")
             continue
         ap_id = None
         if intf_nodes[0][CkEnum.EVPN_INTERFACE]:
@@ -275,23 +290,23 @@
         # logging.debug(f"{ct_assign_spec=}")
         ct_assign_updated = bp.patch_obj_policy_batch_apply(ct_assign_spec, params={'async': 'full'})
         logging.debug(f"CT assign updated for generic system {generic_system_label} in blueprint {bp_label}: {ct_assign_updated} {ct_assign_spec=}")
         # logging.debug(f"ct_assign_updated: {ct_assign_updated}"
 
 
 
-def add_single_generic_system(bp, gs_label, gs_links_list) -> Tuple[Optional[str], Optional[str]]:
+def add_single_generic_system(bp, gs_label, gs_links_list) -> Result[str, str]:
     # gs_count += 1
     gs_link_total = len(gs_links_list)
     # logging.info(f"add_generic_system Adding generic system {gs_count}/{gs_total}: {gs_label} with {gs_link_total} links")
-    existing_gs, _ = bp.get_system_node_from_label(gs_label)
-    if existing_gs:
-        logging.warning(f"add_single_generic_system Skipping: Generic system {gs_label} already exists in blueprint {bp.label}")
+    existing_gs_result = bp.get_system_node_from_label(gs_label)
+    if isinstance(existing_gs_result, Ok) and existing_gs_result.ok_value:
+        error_message = f"add_single_generic_system Skipping: Generic system {gs_label} already exists in blueprint {bp.label}"
         # TODO: verify the content
-        return None, None
+        return Err(error_message)
     # if gs_link_total > 1:
     #     logging.warning(f"Adding generic system {gs_label} with {gs_link_total} links\n{gs_links_list}")
     #     return
     generic_system_spec = {
         'links': [],
         'new_systems': [],
     }
@@ -310,29 +325,31 @@
             this_ifname = link[f"switch_intf{link_id_num}"]
             # skip if data is missing
             if not switch_label:
                 continue
             if this_ifname[:2] not in ['et', 'xe', 'ge']:
                 error_message = f"Error: wrong interface for {gs_label} - {switch_label}:{this_ifname}"
                 # logging.warning(f"add_single_generic_system Error : {error_message}")
-                return None, error_message
+                return Err(error_message)
             logging.debug(f"{switch_label=}")
-            switch_node, error = bp.get_system_node_from_label(switch_label)
-            if error:
+            switch_node_result = bp.get_system_node_from_label(switch_label)
+            if isinstance(switch_node_result, Err):
                 error_message = f"Error: generic system {gs_label} has absent switch {switch_label}\n\tFrom get_system_node_from_label {error}"
                 # logging.warning(f"add_single_generic_system {error_message}")
-                return None, error_message
+                return Err(error_message)
+            switch_node = switch_node_result.ok_value
             if not switch_node:
                 return None, f"Error: {switch_label} not found in blueprint {bp.label}"
             switch_id = switch_node['id']
-            transformation_id, error = bp.get_transformation_id(switch_label, this_ifname , link_speed)
-            if error:
-                error_message = f"Error: generic system {gs_label} has absent transformation {switch_label}:{this_ifname}\n\tFrom get_transformation_id {error}"
+            transformation_id_result = bp.get_transformation_id(switch_label, this_ifname , link_speed)
+            if isinstance(transformation_id_result, Err):
+                error_message = f"Error: generic system {gs_label} has absent transformation {switch_label}:{this_ifname}\n\tFrom get_transformation_id {transformation_id_result.err_value}"
                 logging.warning(f"add_single_generic_system {error_message}")
-                return None, error_message
+                return Err(error_message)
+            transformation_id = transformation_id_result.ok_value
             link_spec = {
                 'switch': {
                     'system_id': switch_id,
                     # 'transformation_id': bp.get_transformation_id(link[f"switch{link_id_num}"], this_ifname , link_speed),
                     'transformation_id': transformation_id,
                     'if_name': link[f"switch_intf{link_id_num}"],
                 },
@@ -399,24 +416,24 @@
         new_system['logical_device']['panels'][0]['port_groups'].append(port_group)
         display_name = f"{display_name}-{count}x{speed}"
     new_system['logical_device']['display_name'] = display_name
     new_system['logical_device']['id'] = display_name
     generic_system_spec['new_systems'].append(new_system)
     logging.debug(f"add_single_generic_system {generic_system_spec=}, {speed_count=}")
 
-    generic_system_created, error = bp.add_generic_system(generic_system_spec)
-    if error:
-        error_message = f"Error: generic system {gs_label} not created\n\tFrom add_generic_system {error}"
+    generic_system_created_result = bp.add_generic_system(generic_system_spec)
+    if isinstance(generic_system_created_result, Err):
+        error_message = f"Error: generic system {gs_label} not created\n\tFrom add_generic_system {generic_system_created_result.err_value}"
         # logging.warning(error_message)
-        return None, error_message
+        return Err(error_message)
 
-    return None, None
+    return Ok('done')
                                                                              
 
-def add_generic_system(apstra_session, generic_systems: dict) -> Tuple[Optional[str], Optional[str]]:
+def add_generic_system(apstra_session, generic_systems: dict) -> Result[str, str]:
     """
     Add a single generic system to the Apstra server from the given generic systems data.
     Revised from add_generic_systems.
 
     Generic systems data:
     {
         <blueprint_label>: {
@@ -447,51 +464,52 @@
 
                     "comment": null
                 }
             ]
         }
     }
     """
+    func_name = "add_generic_system"
 
     ## create the generic systems
     bp_total = len(generic_systems)  # total number of blueprints
     bp_count = 0
-    logging.info(f"add_generic_system Adding generic systems to {bp_total} blueprints")
+    logging.info(f"{func_name} Adding generic systems to {bp_total} blueprints")
     for bp_label, bp_data in generic_systems.items():
         bp_count += 1
-        logging.info(f"add_generic_system Adding generic systems to blueprint {bp_count}/{bp_total}: {bp_label}")
+        logging.info(f"{func_name} Adding generic systems to blueprint {bp_count}/{bp_total}: {bp_label}")
         bp = CkApstraBlueprint(apstra_session, bp_label)
         # logging.debug(f"{bp=}, {bp.id=}")
         gs_total = len(bp_data)
         gs_count = 0
-        logging.info(f"add_generic_system Adding {gs_total} generic systems to blueprint {bp_label}")
+        logging.info(f"{func_name} Adding {gs_total} generic systems to blueprint {bp_label}")
         for gs_label, gs_links_list in bp_data.items():
             gs_count += 1
             gs_link_total = len(gs_links_list)
-            logging.info(f"add_generic_system Adding generic system {gs_count}/{gs_total}: {gs_label} with {gs_link_total} links")
-            _, error = add_single_generic_system(bp, gs_label, gs_links_list)
-            if error:
-                logging.warning(f"add_generic_system Error for {gs_label=}:\n\tFrom add_single_generic_system: {error}")
-                # return None, f"add_generic_system {error}"
+            logging.info(f"{func_name} Adding generic system {gs_count}/{gs_total}: {gs_label} with {gs_link_total} links")
+            add_single_gs_result = add_single_generic_system(bp, gs_label, gs_links_list)
+            if isinstance(add_single_gs_result, Err):
+                logging.warning(f"{func_name} Error for {gs_label=}:\n\tFrom add_single_generic_system: {add_single_gs_result.err_value}")
+                # return None, f"{func_name} {error}"
 
         ## form LACP in the BP iterating over the generic systems
         for gs_label, gs_links_list in bp_data.items():
             form_lacp(bp, gs_label, gs_links_list)
-            _, error = add_tags(bp, gs_label, gs_links_list)
-            if error:
-                logging.warning(f"add_generic_system Error for {gs_label=}:\n\tFrom add_tags: {error}")
+            add_tags_result = add_tags(bp, gs_label, gs_links_list)
+            if isinstance(add_tags_result, Err):
+                logging.warning(f"{func_name} Error for {gs_label=}:\n\tFrom add_tags: {add_tags_result.err_value}")
                 # return None, f"add_generic_system {error}"
                 continue
             rename_generic_system_intf(bp, gs_label, gs_links_list)
 
             # # update connectivity templates - this should be run after lag update
             # assign_connectivity_templates(job_env, gs_label, gs_links_list)
             assign_connectivity_templates(bp, gs_label, gs_links_list)
 
-        return None, None    
+    return Ok(f"{func_name}: {bp_total} blueprints, {gs_total} generic systems added")
 
 
 
 if __name__ == "__main__":
     # click_add_generic_systems()
     apstra_server_host = '10.85.192.45'
     apstra_server_port = '443'
@@ -549,9 +567,14 @@
                     "switch4": None,
                     "switch_intf4": None,
                     "comment": None
                 }
             ]
         }
     }
-    add_generic_system(apstra, generic_systems)
+    add_gs_result = add_generic_system(apstra, generic_systems)
+    logging.info(f"{add_gs_result=}")
+    if isinstance(add_gs_result, Ok):
+        logging.warning(add_gs_result.ok_value)
+    else:
+        logging.warning(add_gs_result.err_value)
```

### Comparing `ck_apstra_api-0.3.2/src/ck_apstra_api/ip_endpoint.py` & `ck_apstra_api-0.3.3/src/ck_apstra_api/ip_endpoint.py`

 * *Files identical despite different names*

### Comparing `ck_apstra_api-0.3.2/src/ck_apstra_api/pull_device_configuration.py` & `ck_apstra_api-0.3.3/src/ck_apstra_api/pull_device_configuration.py`

 * *Files identical despite different names*

### Comparing `ck_apstra_api-0.3.2/PKG-INFO` & `ck_apstra_api-0.3.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 Metadata-Version: 2.1
 Name: ck-apstra-api
-Version: 0.3.2
+Version: 0.3.3
 Summary: An implementation to use Apstra API
 License: MIT
 Author: Charlie Kim
 Author-email: ckim@juniper.net
 Requires-Python: >=3.11,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: pandas (>=2.1.1,<3.0.0)
 Requires-Dist: pydantic (>=2.4.2,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: result (==0.16.1)
 Description-Content-Type: text/markdown
 
 # ck-apstra-api
 
 
 ## prepare venv
 
 ```
-python3.11 -m venv venv
-source venv/bin/activate
-pip install ck-apstra-api
+uv venv
+source .venv/bin/activate
+uv pip install ck-apstra-api
 ```
 
 
 ## var/.env file example
 
 ```
 apstra_server_host=local-apstra.pslab.link
```

