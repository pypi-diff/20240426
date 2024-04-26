# Comparing `tmp/close_dot_io-0.0.912.tar.gz` & `tmp/close_dot_io-0.0.913.tar.gz`

## Comparing `close_dot_io-0.0.912.tar` & `close_dot_io-0.0.913.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 close_dot_io-0.0.912/.pre-commit-config.yaml
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 close_dot_io-0.0.912/requirements-dev.txt
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 close_dot_io-0.0.912/src/close_dot_io/__about__.py
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 close_dot_io-0.0.912/src/close_dot_io/__init__.py
--rw-r--r--   0        0        0    13491 2020-02-02 00:00:00.000000 close_dot_io-0.0.912/src/close_dot_io/client.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 close_dot_io-0.0.912/src/close_dot_io/dict_util.py
--rw-r--r--   0        0        0     3593 2020-02-02 00:00:00.000000 close_dot_io-0.0.912/src/close_dot_io/enums.py
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 close_dot_io-0.0.912/src/close_dot_io/security.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 close_dot_io-0.0.912/src/close_dot_io/resources/__init__.py
--rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 close_dot_io-0.0.912/src/close_dot_io/resources/activity.py
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 close_dot_io-0.0.912/src/close_dot_io/resources/base.py
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 close_dot_io-0.0.912/src/close_dot_io/resources/connected_account.py
--rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 close_dot_io-0.0.912/src/close_dot_io/resources/contact.py
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 close_dot_io-0.0.912/src/close_dot_io/resources/event.py
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 close_dot_io-0.0.912/src/close_dot_io/resources/lead.py
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 close_dot_io-0.0.912/src/close_dot_io/resources/opportunity.py
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 close_dot_io-0.0.912/src/close_dot_io/resources/sequence.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 close_dot_io-0.0.912/src/close_dot_io/resources/smart_view.py
--rw-r--r--   0        0        0     8550 2020-02-02 00:00:00.000000 close_dot_io-0.0.912/src/close_dot_io/resources/webhook.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 close_dot_io-0.0.912/tests/__init__.py
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 close_dot_io-0.0.912/.gitignore
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 close_dot_io-0.0.912/LICENSE.txt
--rw-r--r--   0        0        0    16966 2020-02-02 00:00:00.000000 close_dot_io-0.0.912/README.md
--rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 close_dot_io-0.0.912/pyproject.toml
--rw-r--r--   0        0        0    18047 2020-02-02 00:00:00.000000 close_dot_io-0.0.912/PKG-INFO
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 close_dot_io-0.0.913/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 close_dot_io-0.0.913/requirements-dev.txt
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 close_dot_io-0.0.913/src/close_dot_io/__about__.py
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 close_dot_io-0.0.913/src/close_dot_io/__init__.py
+-rw-r--r--   0        0        0    13491 2020-02-02 00:00:00.000000 close_dot_io-0.0.913/src/close_dot_io/client.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 close_dot_io-0.0.913/src/close_dot_io/dict_util.py
+-rw-r--r--   0        0        0     3593 2020-02-02 00:00:00.000000 close_dot_io-0.0.913/src/close_dot_io/enums.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 close_dot_io-0.0.913/src/close_dot_io/security.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 close_dot_io-0.0.913/src/close_dot_io/resources/__init__.py
+-rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 close_dot_io-0.0.913/src/close_dot_io/resources/activity.py
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 close_dot_io-0.0.913/src/close_dot_io/resources/base.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 close_dot_io-0.0.913/src/close_dot_io/resources/connected_account.py
+-rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 close_dot_io-0.0.913/src/close_dot_io/resources/contact.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 close_dot_io-0.0.913/src/close_dot_io/resources/event.py
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 close_dot_io-0.0.913/src/close_dot_io/resources/lead.py
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 close_dot_io-0.0.913/src/close_dot_io/resources/opportunity.py
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 close_dot_io-0.0.913/src/close_dot_io/resources/sequence.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 close_dot_io-0.0.913/src/close_dot_io/resources/smart_view.py
+-rw-r--r--   0        0        0     8550 2020-02-02 00:00:00.000000 close_dot_io-0.0.913/src/close_dot_io/resources/webhook.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 close_dot_io-0.0.913/tests/__init__.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 close_dot_io-0.0.913/.gitignore
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 close_dot_io-0.0.913/LICENSE.txt
+-rw-r--r--   0        0        0    16966 2020-02-02 00:00:00.000000 close_dot_io-0.0.913/README.md
+-rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 close_dot_io-0.0.913/pyproject.toml
+-rw-r--r--   0        0        0    18047 2020-02-02 00:00:00.000000 close_dot_io-0.0.913/PKG-INFO
```

### Comparing `close_dot_io-0.0.912/.pre-commit-config.yaml` & `close_dot_io-0.0.913/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `close_dot_io-0.0.912/src/close_dot_io/client.py` & `close_dot_io-0.0.913/src/close_dot_io/client.py`

 * *Files identical despite different names*

### Comparing `close_dot_io-0.0.912/src/close_dot_io/enums.py` & `close_dot_io-0.0.913/src/close_dot_io/enums.py`

 * *Files identical despite different names*

### Comparing `close_dot_io-0.0.912/src/close_dot_io/resources/__init__.py` & `close_dot_io-0.0.913/src/close_dot_io/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `close_dot_io-0.0.912/src/close_dot_io/resources/activity.py` & `close_dot_io-0.0.913/src/close_dot_io/resources/activity.py`

 * *Files identical despite different names*

### Comparing `close_dot_io-0.0.912/src/close_dot_io/resources/base.py` & `close_dot_io-0.0.913/src/close_dot_io/resources/base.py`

 * *Files identical despite different names*

### Comparing `close_dot_io-0.0.912/src/close_dot_io/resources/contact.py` & `close_dot_io-0.0.913/src/close_dot_io/resources/contact.py`

 * *Files identical despite different names*

### Comparing `close_dot_io-0.0.912/src/close_dot_io/resources/event.py` & `close_dot_io-0.0.913/src/close_dot_io/resources/event.py`

 * *Files identical despite different names*

### Comparing `close_dot_io-0.0.912/src/close_dot_io/resources/lead.py` & `close_dot_io-0.0.913/src/close_dot_io/resources/lead.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     @classmethod
     def create_from_contact(cls, contact: T, **other_lead_data):
         other_lead_data.pop("contacts", None)
         return cls(contacts=[contact], **other_lead_data)
 
     def model_post_init(self, __context: Any) -> None:
         if not self.opportunities:
+            self._opp_ids_on_init = set()
             return
         self._opp_ids_on_init = {opp.id for opp in self.opportunities if opp.id}
 
     @computed_field
     @property
     def display_name(self) -> str | None:
         return self.name
```

### Comparing `close_dot_io-0.0.912/src/close_dot_io/resources/opportunity.py` & `close_dot_io-0.0.913/src/close_dot_io/resources/opportunity.py`

 * *Files identical despite different names*

### Comparing `close_dot_io-0.0.912/src/close_dot_io/resources/sequence.py` & `close_dot_io-0.0.913/src/close_dot_io/resources/sequence.py`

 * *Files identical despite different names*

### Comparing `close_dot_io-0.0.912/src/close_dot_io/resources/smart_view.py` & `close_dot_io-0.0.913/src/close_dot_io/resources/smart_view.py`

 * *Files identical despite different names*

### Comparing `close_dot_io-0.0.912/src/close_dot_io/resources/webhook.py` & `close_dot_io-0.0.913/src/close_dot_io/resources/webhook.py`

 * *Files identical despite different names*

### Comparing `close_dot_io-0.0.912/LICENSE.txt` & `close_dot_io-0.0.913/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `close_dot_io-0.0.912/README.md` & `close_dot_io-0.0.913/README.md`

 * *Files identical despite different names*

### Comparing `close_dot_io-0.0.912/pyproject.toml` & `close_dot_io-0.0.913/pyproject.toml`

 * *Files identical despite different names*

### Comparing `close_dot_io-0.0.912/PKG-INFO` & `close_dot_io-0.0.913/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: close-dot-io
-Version: 0.0.912
+Version: 0.0.913
 Summary: Easy interface to work with the Close.io API.
 Project-URL: Documentation, https://github.com/unknown/close_dot_io#readme
 Project-URL: Issues, https://github.com/unknown/close_dot_io/issues
 Project-URL: Source, https://github.com/unknown/close_dot_io
 Author-email: Copyfactory <dev@copyfactory.io>
 License-Expression: MIT
 License-File: LICENSE.txt
```

