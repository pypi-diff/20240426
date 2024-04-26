# Comparing `tmp/pingen2sdk-0.3.1.tar.gz` & `tmp/pingen2sdk-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pingen2sdk-0.3.1.tar", last modified: Tue Apr 23 08:12:50 2024, max compression
+gzip compressed data, was "pingen2sdk-0.4.0.tar", last modified: Fri Apr 26 09:42:33 2024, max compression
```

## Comparing `pingen2sdk-0.3.1.tar` & `pingen2sdk-0.4.0.tar`

### file list

```diff
@@ -1,44 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:12:50.095928 pingen2sdk-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-23 08:12:44.000000 pingen2sdk-0.3.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-23 08:12:44.000000 pingen2sdk-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-23 08:12:44.000000 pingen2sdk-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-04-23 08:12:50.095928 pingen2sdk-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-04-23 08:12:44.000000 pingen2sdk-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:12:50.091928 pingen2sdk-0.3.1/pingen2sdk/
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-23 08:12:44.000000 pingen2sdk-0.3.1/pingen2sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4308 2024-04-23 08:12:44.000000 pingen2sdk-0.3.1/pingen2sdk/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:12:50.095928 pingen2sdk-0.3.1/pingen2sdk/api_resources/
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-23 08:12:44.000000 pingen2sdk-0.3.1/pingen2sdk/api_resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-23 08:12:44.000000 pingen2sdk-0.3.1/pingen2sdk/api_resources/batch_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     7039 2024-04-23 08:12:44.000000 pingen2sdk-0.3.1/pingen2sdk/api_resources/batches.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-23 08:12:44.000000 pingen2sdk-0.3.1/pingen2sdk/api_resources/file_upload.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-23 08:12:44.000000 pingen2sdk-0.3.1/pingen2sdk/api_resources/letter_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     6583 2024-04-23 08:12:44.000000 pingen2sdk-0.3.1/pingen2sdk/api_resources/letters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-23 08:12:44.000000 pingen2sdk-0.3.1/pingen2sdk/api_resources/organisations.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-23 08:12:44.000000 pingen2sdk-0.3.1/pingen2sdk/api_resources/user_associations.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-23 08:12:44.000000 pingen2sdk-0.3.1/pingen2sdk/api_resources/users.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-23 08:12:44.000000 pingen2sdk-0.3.1/pingen2sdk/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-23 08:12:44.000000 pingen2sdk-0.3.1/pingen2sdk/oauth.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-23 08:12:44.000000 pingen2sdk-0.3.1/pingen2sdk/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:12:50.095928 pingen2sdk-0.3.1/pingen2sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-04-23 08:12:50.000000 pingen2sdk-0.3.1/pingen2sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-23 08:12:50.000000 pingen2sdk-0.3.1/pingen2sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 08:12:50.000000 pingen2sdk-0.3.1/pingen2sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-23 08:12:50.000000 pingen2sdk-0.3.1/pingen2sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-23 08:12:50.000000 pingen2sdk-0.3.1/pingen2sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-23 08:12:44.000000 pingen2sdk-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 08:12:50.095928 pingen2sdk-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:12:50.095928 pingen2sdk-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 08:12:44.000000 pingen2sdk-0.3.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:12:50.095928 pingen2sdk-0.3.1/tests/api_resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 08:12:44.000000 pingen2sdk-0.3.1/tests/api_resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-23 08:12:44.000000 pingen2sdk-0.3.1/tests/api_resources/test_batch_events.py
--rw-r--r--   0 runner    (1001) docker     (127)    15184 2024-04-23 08:12:44.000000 pingen2sdk-0.3.1/tests/api_resources/test_batches.py
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-23 08:12:44.000000 pingen2sdk-0.3.1/tests/api_resources/test_file_upload.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-23 08:12:44.000000 pingen2sdk-0.3.1/tests/api_resources/test_letter_events.py
--rw-r--r--   0 runner    (1001) docker     (127)    18780 2024-04-23 08:12:44.000000 pingen2sdk-0.3.1/tests/api_resources/test_letters.py
--rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-04-23 08:12:44.000000 pingen2sdk-0.3.1/tests/api_resources/test_organisations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-04-23 08:12:44.000000 pingen2sdk-0.3.1/tests/api_resources/test_user_accociations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-23 08:12:44.000000 pingen2sdk-0.3.1/tests/api_resources/test_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-04-23 08:12:44.000000 pingen2sdk-0.3.1/tests/test_oauth.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-23 08:12:44.000000 pingen2sdk-0.3.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:42:33.676478 pingen2sdk-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-26 09:42:27.000000 pingen2sdk-0.4.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-26 09:42:27.000000 pingen2sdk-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-26 09:42:27.000000 pingen2sdk-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-04-26 09:42:33.676478 pingen2sdk-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-04-26 09:42:27.000000 pingen2sdk-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:42:33.672478 pingen2sdk-0.4.0/pingen2sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-26 09:42:27.000000 pingen2sdk-0.4.0/pingen2sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4308 2024-04-26 09:42:27.000000 pingen2sdk-0.4.0/pingen2sdk/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:42:33.676478 pingen2sdk-0.4.0/pingen2sdk/api_resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-26 09:42:27.000000 pingen2sdk-0.4.0/pingen2sdk/api_resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-26 09:42:27.000000 pingen2sdk-0.4.0/pingen2sdk/api_resources/batch_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7001 2024-04-26 09:42:27.000000 pingen2sdk-0.4.0/pingen2sdk/api_resources/batches.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-26 09:42:27.000000 pingen2sdk-0.4.0/pingen2sdk/api_resources/file_upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-26 09:42:27.000000 pingen2sdk-0.4.0/pingen2sdk/api_resources/letter_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6527 2024-04-26 09:42:27.000000 pingen2sdk-0.4.0/pingen2sdk/api_resources/letters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-26 09:42:27.000000 pingen2sdk-0.4.0/pingen2sdk/api_resources/organisations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-26 09:42:27.000000 pingen2sdk-0.4.0/pingen2sdk/api_resources/user_associations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-26 09:42:27.000000 pingen2sdk-0.4.0/pingen2sdk/api_resources/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-26 09:42:27.000000 pingen2sdk-0.4.0/pingen2sdk/api_resources/webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-26 09:42:27.000000 pingen2sdk-0.4.0/pingen2sdk/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-26 09:42:27.000000 pingen2sdk-0.4.0/pingen2sdk/incoming_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-26 09:42:27.000000 pingen2sdk-0.4.0/pingen2sdk/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-26 09:42:27.000000 pingen2sdk-0.4.0/pingen2sdk/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-26 09:42:27.000000 pingen2sdk-0.4.0/pingen2sdk/webhook_event.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:42:33.676478 pingen2sdk-0.4.0/pingen2sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-04-26 09:42:33.000000 pingen2sdk-0.4.0/pingen2sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-04-26 09:42:33.000000 pingen2sdk-0.4.0/pingen2sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 09:42:33.000000 pingen2sdk-0.4.0/pingen2sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-26 09:42:33.000000 pingen2sdk-0.4.0/pingen2sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-26 09:42:33.000000 pingen2sdk-0.4.0/pingen2sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-26 09:42:27.000000 pingen2sdk-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 09:42:33.676478 pingen2sdk-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:42:33.676478 pingen2sdk-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 09:42:27.000000 pingen2sdk-0.4.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:42:33.676478 pingen2sdk-0.4.0/tests/api_resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 09:42:27.000000 pingen2sdk-0.4.0/tests/api_resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-26 09:42:27.000000 pingen2sdk-0.4.0/tests/api_resources/test_batch_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15148 2024-04-26 09:42:27.000000 pingen2sdk-0.4.0/tests/api_resources/test_batches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-26 09:42:27.000000 pingen2sdk-0.4.0/tests/api_resources/test_file_upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-26 09:42:27.000000 pingen2sdk-0.4.0/tests/api_resources/test_letter_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18724 2024-04-26 09:42:27.000000 pingen2sdk-0.4.0/tests/api_resources/test_letters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-04-26 09:42:27.000000 pingen2sdk-0.4.0/tests/api_resources/test_organisations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-04-26 09:42:27.000000 pingen2sdk-0.4.0/tests/api_resources/test_user_accociations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-26 09:42:27.000000 pingen2sdk-0.4.0/tests/api_resources/test_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7088 2024-04-26 09:42:27.000000 pingen2sdk-0.4.0/tests/api_resources/test_webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8967 2024-04-26 09:42:27.000000 pingen2sdk-0.4.0/tests/test_incoming_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-04-26 09:42:27.000000 pingen2sdk-0.4.0/tests/test_oauth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-26 09:42:27.000000 pingen2sdk-0.4.0/tox.ini
```

### Comparing `pingen2sdk-0.3.1/LICENSE` & `pingen2sdk-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pingen2sdk-0.3.1/PKG-INFO` & `pingen2sdk-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pingen2sdk
-Version: 0.3.1
+Version: 0.4.0
 Summary: Official Python Pingen SDK for API V2
 Author-email: Pingen GmbH <info@pingen.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/pingencom/pingen2-sdk-python
 Project-URL: Bug Tracker, https://github.com/pingencom/pingen2-sdk-python/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -67,15 +67,15 @@
 
 organisationList = pingen2sdk.Organisations(access_token, True).get_collection()
 
 organisation_id = organisationList.data["data"][0]["id"]
 
 LettersEndpoint = pingen2sdk.Letters(organisation_id, access_token, True)
 
-response = LettersEndpoint.upload_and_create_letter(
+response = LettersEndpoint.upload_and_create(
     "./letter.pdf",
     "sdk.pdf",
     "left",
     False,
     "fast",
     "simplex",
     "color",
```

### Comparing `pingen2sdk-0.3.1/README.md` & `pingen2sdk-0.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 organisationList = pingen2sdk.Organisations(access_token, True).get_collection()
 
 organisation_id = organisationList.data["data"][0]["id"]
 
 LettersEndpoint = pingen2sdk.Letters(organisation_id, access_token, True)
 
-response = LettersEndpoint.upload_and_create_letter(
+response = LettersEndpoint.upload_and_create(
     "./letter.pdf",
     "sdk.pdf",
     "left",
     False,
     "fast",
     "simplex",
     "color",
```

### Comparing `pingen2sdk-0.3.1/pingen2sdk/api.py` & `pingen2sdk-0.4.0/pingen2sdk/api.py`

 * *Files identical despite different names*

### Comparing `pingen2sdk-0.3.1/pingen2sdk/api_resources/__init__.py` & `pingen2sdk-0.4.0/pingen2sdk/api_resources/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,7 +5,8 @@
 from pingen2sdk.api_resources.users import Users as Users
 from pingen2sdk.api_resources.user_associations import (
     UserAssociations as UserAssociations,
 )
 from pingen2sdk.api_resources.organisations import Organisations as Organisations
 from pingen2sdk.api_resources.batches import Batches as Batches
 from pingen2sdk.api_resources.batch_events import BatchEvents as BatchEvents
+from pingen2sdk.api_resources.webhooks import Webhooks as Webhooks
```

### Comparing `pingen2sdk-0.3.1/pingen2sdk/api_resources/batch_events.py` & `pingen2sdk-0.4.0/pingen2sdk/api_resources/batch_events.py`

 * *Files identical despite different names*

### Comparing `pingen2sdk-0.3.1/pingen2sdk/api_resources/batches.py` & `pingen2sdk-0.4.0/pingen2sdk/api_resources/batches.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     ) -> pingen2sdk.PingenResponse:
         return self.api_requestor.perform_get_request(
             "/organisations/%s/batches" % self.organisation_id,
             params,
             supplied_headers,
         )
 
-    def upload_and_create_batch(
+    def upload_and_create(
         self,
         path_to_file: str,
         name: str,
         icon: Literal[
             "campaign",
             "megaphone",
             "wave-hand",
@@ -70,29 +70,29 @@
             Literal["first_page", "last_page"]
         ] = None,
     ) -> pingen2sdk.PingenResponse:
         file_upload = pingen2sdk.FileUpload(self.api_requestor)
         file_url, file_url_signature = file_upload.request_file_upload()
         file_upload.put_file(path_to_file, file_url)
 
-        return self.create_batch(
+        return self.create(
             file_url,
             file_url_signature,
             name,
             icon,
             file_original_name,
             address_position,
             grouping_type,
             grouping_options_split_type,
             grouping_options_split_size,
             grouping_options_split_separator,
             grouping_options_split_position,
         )
 
-    def create_batch(
+    def create(
         self,
         file_url: str,
         file_url_signature: str,
         name: str,
         icon: Literal[
             "campaign",
             "megaphone",
@@ -132,29 +132,29 @@
             "grouping_options_split_type": grouping_options_split_type,
         }
 
         if grouping_options_split_size is not None:
             attributes["grouping_options_split_size"] = grouping_options_split_size
 
         if grouping_options_split_separator is not None:
-            attributes[
-                "grouping_options_split_separator"
-            ] = grouping_options_split_separator
+            attributes["grouping_options_split_separator"] = (
+                grouping_options_split_separator
+            )
 
         if grouping_options_split_position is not None:
-            attributes[
-                "grouping_options_split_position"
-            ] = grouping_options_split_position
+            attributes["grouping_options_split_position"] = (
+                grouping_options_split_position
+            )
 
         return self.api_requestor.perform_post_request(
             "/organisations/%s/batches" % self.organisation_id,
             json.dumps({"data": {"type": "batches", "attributes": attributes}}),
         )
 
-    def send_batch(
+    def send(
         self,
         batch_id: str,
         delivery_product: Mapping[str, str],
         print_mode: str,
         print_spectrum: str,
     ) -> pingen2sdk.PingenResponse:
         return self.api_requestor.perform_patch_request(
@@ -170,31 +170,31 @@
                             "print_spectrum": print_spectrum,
                         },
                     }
                 }
             ),
         )
 
-    def cancel_batch(
+    def cancel(
         self,
         batch_id: str,
     ) -> pingen2sdk.PingenResponse:
         return self.api_requestor.perform_cancel_request(
             "/organisations/%s/batches/%s/cancel" % (self.organisation_id, batch_id),
         )
 
-    def delete_batch(
+    def delete(
         self,
         batch_id: str,
     ) -> pingen2sdk.PingenResponse:
         return self.api_requestor.perform_delete_request(
             "/organisations/%s/batches/%s" % (self.organisation_id, batch_id),
         )
 
-    def edit_batch(
+    def edit(
         self,
         batch_id: str,
         paper_types: List[str],
     ) -> pingen2sdk.PingenResponse:
         return self.api_requestor.perform_patch_request(
             "/organisations/%s/batches/%s" % (self.organisation_id, batch_id),
             json.dumps(
```

### Comparing `pingen2sdk-0.3.1/pingen2sdk/api_resources/file_upload.py` & `pingen2sdk-0.4.0/pingen2sdk/api_resources/file_upload.py`

 * *Files identical despite different names*

### Comparing `pingen2sdk-0.3.1/pingen2sdk/api_resources/letter_events.py` & `pingen2sdk-0.4.0/pingen2sdk/api_resources/letter_events.py`

 * *Files identical despite different names*

### Comparing `pingen2sdk-0.3.1/pingen2sdk/api_resources/letters.py` & `pingen2sdk-0.4.0/pingen2sdk/api_resources/letters.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     ) -> pingen2sdk.PingenResponse:
         return self.api_requestor.perform_get_request(
             "/organisations/%s/letters" % self.organisation_id,
             params,
             supplied_headers,
         )
 
-    def upload_and_create_letter(
+    def upload_and_create(
         self,
         path_to_file: str,
         file_original_name: str,
         address_position: Literal["left", "right"],
         auto_send: False,
         delivery_product: Optional[str] = None,
         print_mode: Optional[str] = None,
@@ -51,28 +51,28 @@
         sender_address: Optional[str] = None,
         meta_data: Optional[Dict] = None,
     ) -> pingen2sdk.PingenResponse:
         file_upload = pingen2sdk.FileUpload(self.api_requestor)
         file_url, file_signature = file_upload.request_file_upload()
         file_upload.put_file(path_to_file, file_url)
 
-        return self.create_letter(
+        return self.create(
             file_url,
             file_signature,
             file_original_name,
             address_position,
             auto_send,
             delivery_product,
             print_mode,
             print_spectrum,
             sender_address,
             meta_data,
         )
 
-    def create_letter(
+    def create(
         self,
         file_url: str,
         file_signature: str,
         file_original_name: str,
         address_position: Literal["left", "right"],
         auto_send: False,
         delivery_product: Optional[str] = None,
@@ -105,15 +105,15 @@
             attributes["meta_data"] = meta_data
 
         return self.api_requestor.perform_post_request(
             "/organisations/%s/letters" % self.organisation_id,
             json.dumps({"data": {"type": "letters", "attributes": attributes}}),
         )
 
-    def send_letter(
+    def send(
         self,
         letter_id: str,
         delivery_product: str,
         print_mode: str,
         print_spectrum: str,
     ) -> pingen2sdk.PingenResponse:
         return self.api_requestor.perform_patch_request(
@@ -129,31 +129,31 @@
                             "print_spectrum": print_spectrum,
                         },
                     }
                 }
             ),
         )
 
-    def cancel_letter(
+    def cancel(
         self,
         letter_id: str,
     ) -> pingen2sdk.PingenResponse:
         return self.api_requestor.perform_cancel_request(
             "/organisations/%s/letters/%s/cancel" % (self.organisation_id, letter_id),
         )
 
-    def delete_letter(
+    def delete(
         self,
         letter_id: str,
     ) -> pingen2sdk.PingenResponse:
         return self.api_requestor.perform_delete_request(
             "/organisations/%s/letters/%s" % (self.organisation_id, letter_id),
         )
 
-    def edit_letter(
+    def edit(
         self,
         letter_id: str,
         paper_types: List[str],
     ) -> pingen2sdk.PingenResponse:
         return self.api_requestor.perform_patch_request(
             "/organisations/%s/letters/%s" % (self.organisation_id, letter_id),
             json.dumps(
@@ -165,15 +165,15 @@
                             "paper_types": paper_types,
                         },
                     }
                 }
             ),
         )
 
-    def get_letter_file(
+    def get_file(
         self,
         letter_id: str,
     ) -> IOBase:
         return self.api_requestor.perform_stream_request(
             "/organisations/%s/letters/%s/file" % (self.organisation_id, letter_id),
         )
```

### Comparing `pingen2sdk-0.3.1/pingen2sdk/api_resources/organisations.py` & `pingen2sdk-0.4.0/pingen2sdk/api_resources/organisations.py`

 * *Files identical despite different names*

### Comparing `pingen2sdk-0.3.1/pingen2sdk/api_resources/user_associations.py` & `pingen2sdk-0.4.0/pingen2sdk/api_resources/user_associations.py`

 * *Files identical despite different names*

### Comparing `pingen2sdk-0.3.1/pingen2sdk/api_resources/users.py` & `pingen2sdk-0.4.0/pingen2sdk/api_resources/users.py`

 * *Files identical despite different names*

### Comparing `pingen2sdk-0.3.1/pingen2sdk/error.py` & `pingen2sdk-0.4.0/pingen2sdk/error.py`

 * *Files 24% similar despite different names*

```diff
@@ -27,7 +27,15 @@
         self.headers = headers or {}
         self.status_code = status_code
         self.request_id = self.headers.get("x-request-id", None)
 
 
 class AuthenticationError(PingenError):
     pass
+
+
+class WebhookSignatureException(Exception):
+    _message: Optional[str]
+
+    def __init__(self, message=""):
+        self.message = message
+        super().__init__(self.message)
```

### Comparing `pingen2sdk-0.3.1/pingen2sdk/oauth.py` & `pingen2sdk-0.4.0/pingen2sdk/oauth.py`

 * *Files identical despite different names*

### Comparing `pingen2sdk-0.3.1/pingen2sdk/response.py` & `pingen2sdk-0.4.0/pingen2sdk/response.py`

 * *Files identical despite different names*

### Comparing `pingen2sdk-0.3.1/pingen2sdk.egg-info/PKG-INFO` & `pingen2sdk-0.4.0/pingen2sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pingen2sdk
-Version: 0.3.1
+Version: 0.4.0
 Summary: Official Python Pingen SDK for API V2
 Author-email: Pingen GmbH <info@pingen.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/pingencom/pingen2-sdk-python
 Project-URL: Bug Tracker, https://github.com/pingencom/pingen2-sdk-python/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -67,15 +67,15 @@
 
 organisationList = pingen2sdk.Organisations(access_token, True).get_collection()
 
 organisation_id = organisationList.data["data"][0]["id"]
 
 LettersEndpoint = pingen2sdk.Letters(organisation_id, access_token, True)
 
-response = LettersEndpoint.upload_and_create_letter(
+response = LettersEndpoint.upload_and_create(
     "./letter.pdf",
     "sdk.pdf",
     "left",
     False,
     "fast",
     "simplex",
     "color",
```

### Comparing `pingen2sdk-0.3.1/pingen2sdk.egg-info/SOURCES.txt` & `pingen2sdk-0.4.0/pingen2sdk.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -3,34 +3,39 @@
 MANIFEST.in
 README.md
 pyproject.toml
 tox.ini
 pingen2sdk/__init__.py
 pingen2sdk/api.py
 pingen2sdk/error.py
+pingen2sdk/incoming_webhook.py
 pingen2sdk/oauth.py
 pingen2sdk/response.py
+pingen2sdk/webhook_event.py
 pingen2sdk.egg-info/PKG-INFO
 pingen2sdk.egg-info/SOURCES.txt
 pingen2sdk.egg-info/dependency_links.txt
 pingen2sdk.egg-info/requires.txt
 pingen2sdk.egg-info/top_level.txt
 pingen2sdk/api_resources/__init__.py
 pingen2sdk/api_resources/batch_events.py
 pingen2sdk/api_resources/batches.py
 pingen2sdk/api_resources/file_upload.py
 pingen2sdk/api_resources/letter_events.py
 pingen2sdk/api_resources/letters.py
 pingen2sdk/api_resources/organisations.py
 pingen2sdk/api_resources/user_associations.py
 pingen2sdk/api_resources/users.py
+pingen2sdk/api_resources/webhooks.py
 tests/__init__.py
+tests/test_incoming_webhook.py
 tests/test_oauth.py
 tests/api_resources/__init__.py
 tests/api_resources/test_batch_events.py
 tests/api_resources/test_batches.py
 tests/api_resources/test_file_upload.py
 tests/api_resources/test_letter_events.py
 tests/api_resources/test_letters.py
 tests/api_resources/test_organisations.py
 tests/api_resources/test_user_accociations.py
-tests/api_resources/test_users.py
+tests/api_resources/test_users.py
+tests/api_resources/test_webhooks.py
```

### Comparing `pingen2sdk-0.3.1/pyproject.toml` & `pingen2sdk-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pingen2sdk"
-version = "0.3.1"
+version = "0.4.0"
 authors = [
   { name="Pingen GmbH", email="info@pingen.com" },
 ]
 description = "Official Python Pingen SDK for API V2"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `pingen2sdk-0.3.1/tests/api_resources/test_batch_events.py` & `pingen2sdk-0.4.0/tests/api_resources/test_batch_events.py`

 * *Files identical despite different names*

### Comparing `pingen2sdk-0.3.1/tests/api_resources/test_batches.py` & `pingen2sdk-0.4.0/tests/api_resources/test_batches.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,15 +221,15 @@
                 "Content-Type": "application/vnd.api+json",
                 "X-Request-Id": "requestx-xxxx-xxxx-xxxx-xxxxxxxxxxx2",
             },
             json=self._get_expected_payload("xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxx11"),
             status=201,
         )
 
-        response = batches.create_batch(
+        response = batches.create(
             "https://s3.example/bucket/filename?signer=url",
             "$2y$10$BLOzVbYTXrh4LZbSYNVf7eEDrc58vvQ9PRVZABqV/9WS1eqIcm3M",
             "lorem.pdf",
             "flash",
             "lorem.pdf",
             "left",
             "merge",
@@ -261,15 +261,15 @@
                 "Content-Type": "application/vnd.api+json",
                 "X-Request-Id": "requestx-xxxx-xxxx-xxxx-xxxxxxxxxxx3",
             },
             json=self._get_expected_payload("xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxx111"),
             status=201,
         )
 
-        response = batches.upload_and_create_batch(
+        response = batches.upload_and_create(
             "tests/api_resources/files/lorem.pdf",
             "testing",
             "flash",
             "lorem.pdf",
             "left",
             "merge",
             "file",
@@ -298,15 +298,15 @@
                 "Content-Type": "application/vnd.api+json",
                 "X-Request-Id": "requestx-xxxx-xxxx-xxxx-xxxxxxxxx332",
             },
             json=self._get_expected_payload(batch_id),
             status=200,
         )
 
-        response = batches.send_batch(
+        response = batches.send(
             batch_id,
             [
                 {"country": "CH", "delivery_product": "postag_a"},
                 {"country": "DE", "delivery_product": "fast"},
             ],
             "simplex",
             "color",
@@ -331,15 +331,15 @@
         batches = self._construct_resource()
 
         responses.patch(
             url,
             status=202,
         )
 
-        response = batches.cancel_batch(
+        response = batches.cancel(
             batch_id,
         )
 
         assert response.status_code == 202
 
     @responses.activate
     def test_delete_batch(self):
@@ -352,15 +352,15 @@
         batches = self._construct_resource()
 
         responses.delete(
             url,
             status=204,
         )
 
-        response = batches.delete_batch(
+        response = batches.delete(
             batch_id,
         )
 
         assert response.status_code == 204
 
     @responses.activate
     def test_edit_batch(self):
@@ -378,15 +378,15 @@
                 "Content-Type": "application/vnd.api+json",
                 "X-Request-Id": "requestx-xxxx-xxxx-xxxx-xxxxxxxxx552",
             },
             json=self._get_expected_payload(batch_id),
             status=200,
         )
 
-        response = batches.edit_batch(
+        response = batches.edit(
             batch_id,
             list({"normal", "qr"}),
         )
 
         assert response.data["data"]["id"] == batch_id
         assert response.status_code == 200
         assert response.headers == {
```

### Comparing `pingen2sdk-0.3.1/tests/api_resources/test_file_upload.py` & `pingen2sdk-0.4.0/tests/api_resources/test_file_upload.py`

 * *Files identical despite different names*

### Comparing `pingen2sdk-0.3.1/tests/api_resources/test_letter_events.py` & `pingen2sdk-0.4.0/tests/api_resources/test_letter_events.py`

 * *Files identical despite different names*

### Comparing `pingen2sdk-0.3.1/tests/api_resources/test_letters.py` & `pingen2sdk-0.4.0/tests/api_resources/test_letters.py`

 * *Files 7% similar despite different names*

```diff
@@ -258,15 +258,15 @@
                 "Content-Type": "application/vnd.api+json",
                 "X-Request-Id": "requestx-xxxx-xxxx-xxxx-xxxxxxxxxxx2",
             },
             json=self._get_expected_payload("xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxx11"),
             status=201,
         )
 
-        response = letters.create_letter(
+        response = letters.create(
             "https://s3.example/bucket/filename?signer=url",
             "$2y$10$BLOzVbYTXrh4LZbSYNVf7eEDrc58vvQ9PRVZABqV/9WS1eqIcm3M",
             "lorem.pdf",
             "left",
             True,
             "fast",
             "simplex",
@@ -314,15 +314,15 @@
                 "Content-Type": "application/vnd.api+json",
                 "X-Request-Id": "requestx-xxxx-xxxx-xxxx-xxxxxxxxxxx3",
             },
             json=self._get_expected_payload("xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxx111"),
             status=201,
         )
 
-        response = letters.upload_and_create_letter(
+        response = letters.upload_and_create(
             "tests/api_resources/files/lorem.pdf",
             "lorem.pdf",
             "left",
             False,
         )
 
         assert response.data["data"]["id"] == "xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxx111"
@@ -348,15 +348,15 @@
                 "Content-Type": "application/vnd.api+json",
                 "X-Request-Id": "requestx-xxxx-xxxx-xxxx-xxxxxxxxx332",
             },
             json=self._get_expected_payload(letter_id),
             status=200,
         )
 
-        response = letters.send_letter(
+        response = letters.send(
             letter_id,
             "fast",
             "simplex",
             "color",
         )
 
         assert response.data["data"]["id"] == letter_id
@@ -378,15 +378,15 @@
         letters = self._construct_resource()
 
         responses.patch(
             url,
             status=202,
         )
 
-        response = letters.cancel_letter(
+        response = letters.cancel(
             letter_id,
         )
 
         assert response.status_code == 202
 
     @responses.activate
     def test_delete_letter(self):
@@ -399,15 +399,15 @@
         letters = self._construct_resource()
 
         responses.delete(
             url,
             status=204,
         )
 
-        response = letters.delete_letter(
+        response = letters.delete(
             letter_id,
         )
 
         assert response.status_code == 204
 
     @responses.activate
     def test_delete_letter_unauthorize(self):
@@ -429,15 +429,15 @@
                         "detail": "The JWT string must have two dots",
                         "source": {"pointer": None, "parameter": None},
                     }
                 },
                 status=401,
             )
 
-            letters.delete_letter(
+            letters.delete(
                 letter_id,
             )
 
     @responses.activate
     def test_edit_letter(self):
         letter_id = "testedit-xxxx-xxxx-xxxx-xxxxxxxxx551"
         url = "%s/organisations/testxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxx1/letters/%s" % (
@@ -453,15 +453,15 @@
                 "Content-Type": "application/vnd.api+json",
                 "X-Request-Id": "requestx-xxxx-xxxx-xxxx-xxxxxxxxx552",
             },
             json=self._get_expected_payload(letter_id),
             status=200,
         )
 
-        response = letters.edit_letter(
+        response = letters.edit(
             letter_id,
             list({"normal", "qr"}),
         )
 
         assert response.data["data"]["id"] == letter_id
         assert response.status_code == 200
         assert response.headers == {
@@ -483,15 +483,15 @@
         letters = pingen2sdk.Letters(organisation_id, access_token, True)
 
         responses.get(
             url,
             match=[responses.matchers.request_kwargs_matcher({"stream": True})],
         )
 
-        letters.get_letter_file(
+        letters.get_file(
             letter_id,
         )
 
     @responses.activate
     def test_calculate_price(self):
         url = (
             "%s/organisations/testxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxx1/letters/price-calculator"
```

### Comparing `pingen2sdk-0.3.1/tests/api_resources/test_organisations.py` & `pingen2sdk-0.4.0/tests/api_resources/test_organisations.py`

 * *Files identical despite different names*

### Comparing `pingen2sdk-0.3.1/tests/api_resources/test_user_accociations.py` & `pingen2sdk-0.4.0/tests/api_resources/test_user_accociations.py`

 * *Files identical despite different names*

### Comparing `pingen2sdk-0.3.1/tests/api_resources/test_users.py` & `pingen2sdk-0.4.0/tests/api_resources/test_users.py`

 * *Files identical despite different names*

### Comparing `pingen2sdk-0.3.1/tests/test_oauth.py` & `pingen2sdk-0.4.0/tests/test_oauth.py`

 * *Files identical despite different names*

### Comparing `pingen2sdk-0.3.1/tox.ini` & `pingen2sdk-0.4.0/tox.ini`

 * *Files identical despite different names*

