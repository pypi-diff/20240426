# Comparing `tmp/cybereason-0.5.1.tar.gz` & `tmp/cybereason-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cybereason-0.5.1.tar", last modified: Sat Apr 13 11:44:25 2024, max compression
+gzip compressed data, was "cybereason-0.6.0.tar", last modified: Fri Apr 26 16:34:15 2024, max compression
```

## Comparing `cybereason-0.5.1.tar` & `cybereason-0.6.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 nuno      (1000) nuno      (1000)        0 2024-04-13 11:44:25.824684 cybereason-0.5.1/
--rwxrwxrwx   0 nuno      (1000) nuno      (1000)     1481 2023-07-28 13:38:20.000000 cybereason-0.5.1/LICENSE
--rw-rw-r--   0 nuno      (1000) nuno      (1000)     2935 2024-04-13 11:44:25.824684 cybereason-0.5.1/PKG-INFO
--rw-rw-r--   0 nuno      (1000) nuno      (1000)     1329 2024-03-09 11:12:55.000000 cybereason-0.5.1/pyproject.toml
--rwxrwxrwx   0 nuno      (1000) nuno      (1000)     1668 2024-04-13 11:44:25.824684 cybereason-0.5.1/setup.cfg
--rwxrwxrwx   0 nuno      (1000) nuno      (1000)       60 2023-07-28 13:38:20.000000 cybereason-0.5.1/setup.py
-drwxrwxr-x   0 nuno      (1000) nuno      (1000)        0 2024-04-13 11:44:25.820683 cybereason-0.5.1/src/
-drwxrwxr-x   0 nuno      (1000) nuno      (1000)        0 2024-04-13 11:44:25.820683 cybereason-0.5.1/src/cybereason/
--rwxrwxrwx   0 nuno      (1000) nuno      (1000)      177 2024-04-13 11:42:52.000000 cybereason-0.5.1/src/cybereason/__init__.py
--rwxrwxrwx   0 nuno      (1000) nuno      (1000)     2019 2024-04-13 10:35:59.000000 cybereason-0.5.1/src/cybereason/_typing.py
--rwxrwxrwx   0 nuno      (1000) nuno      (1000)    16340 2024-04-13 11:40:40.000000 cybereason-0.5.1/src/cybereason/client.py
--rwxrwxrwx   0 nuno      (1000) nuno      (1000)     4620 2024-03-14 15:31:06.000000 cybereason-0.5.1/src/cybereason/exceptions.py
--rwxrwxrwx   0 nuno      (1000) nuno      (1000)     3531 2023-11-26 16:25:11.000000 cybereason-0.5.1/src/cybereason/incident_response.py
--rwxrwxrwx   0 nuno      (1000) nuno      (1000)     6528 2024-03-14 15:18:27.000000 cybereason-0.5.1/src/cybereason/malops.py
-drwxrwxr-x   0 nuno      (1000) nuno      (1000)        0 2024-04-13 11:44:25.820683 cybereason-0.5.1/src/cybereason/parse/
--rwxrwxrwx   0 nuno      (1000) nuno      (1000)      147 2023-07-28 13:38:20.000000 cybereason-0.5.1/src/cybereason/parse/__init__.py
--rwxrwxrwx   0 nuno      (1000) nuno      (1000)     2472 2023-07-28 13:38:20.000000 cybereason-0.5.1/src/cybereason/parse/cef.py
--rwxrwxrwx   0 nuno      (1000) nuno      (1000)     2846 2023-07-28 13:38:20.000000 cybereason-0.5.1/src/cybereason/parse/server.py
--rwxrwxrwx   0 nuno      (1000) nuno      (1000)        0 2023-07-28 13:38:20.000000 cybereason-0.5.1/src/cybereason/py.typed
--rwxrwxrwx   0 nuno      (1000) nuno      (1000)     5175 2023-07-28 13:38:20.000000 cybereason-0.5.1/src/cybereason/rules.py
--rwxrwxrwx   0 nuno      (1000) nuno      (1000)    16945 2024-03-14 15:31:28.000000 cybereason-0.5.1/src/cybereason/sensors.py
--rwxrwxrwx   0 nuno      (1000) nuno      (1000)     4774 2024-03-30 02:49:47.000000 cybereason-0.5.1/src/cybereason/system.py
--rwxrwxrwx   0 nuno      (1000) nuno      (1000)     7678 2024-03-08 13:36:46.000000 cybereason-0.5.1/src/cybereason/threat_intel.py
-drwxrwxr-x   0 nuno      (1000) nuno      (1000)        0 2024-04-13 11:44:25.820683 cybereason-0.5.1/src/cybereason/utils/
--rwxrwxrwx   0 nuno      (1000) nuno      (1000)     4515 2023-07-28 13:38:20.000000 cybereason-0.5.1/src/cybereason/utils/__init__.py
--rwxrwxrwx   0 nuno      (1000) nuno      (1000)      796 2023-07-28 13:38:20.000000 cybereason-0.5.1/src/cybereason/utils/guid.py
-drwxrwxr-x   0 nuno      (1000) nuno      (1000)        0 2024-04-13 11:44:25.820683 cybereason-0.5.1/src/cybereason.egg-info/
--rw-rw-r--   0 nuno      (1000) nuno      (1000)     2935 2024-04-13 11:44:25.000000 cybereason-0.5.1/src/cybereason.egg-info/PKG-INFO
--rw-rw-r--   0 nuno      (1000) nuno      (1000)      719 2024-04-13 11:44:25.000000 cybereason-0.5.1/src/cybereason.egg-info/SOURCES.txt
--rw-rw-r--   0 nuno      (1000) nuno      (1000)        1 2024-04-13 11:44:25.000000 cybereason-0.5.1/src/cybereason.egg-info/dependency_links.txt
--rw-rw-r--   0 nuno      (1000) nuno      (1000)        1 2023-11-26 15:59:18.000000 cybereason-0.5.1/src/cybereason.egg-info/not-zip-safe
--rw-rw-r--   0 nuno      (1000) nuno      (1000)      229 2024-04-13 11:44:25.000000 cybereason-0.5.1/src/cybereason.egg-info/requires.txt
--rw-rw-r--   0 nuno      (1000) nuno      (1000)       11 2024-04-13 11:44:25.000000 cybereason-0.5.1/src/cybereason.egg-info/top_level.txt
+drwxrwxr-x   0 nuno      (1000) nuno      (1000)        0 2024-04-26 16:34:15.475464 cybereason-0.6.0/
+-rwxrwxrwx   0 nuno      (1000) nuno      (1000)     1481 2023-07-28 13:38:20.000000 cybereason-0.6.0/LICENSE
+-rw-rw-r--   0 nuno      (1000) nuno      (1000)     2935 2024-04-26 16:34:15.475464 cybereason-0.6.0/PKG-INFO
+-rw-rw-r--   0 nuno      (1000) nuno      (1000)     1329 2024-03-09 11:12:55.000000 cybereason-0.6.0/pyproject.toml
+-rwxrwxrwx   0 nuno      (1000) nuno      (1000)     1668 2024-04-26 16:34:15.475464 cybereason-0.6.0/setup.cfg
+-rwxrwxrwx   0 nuno      (1000) nuno      (1000)       60 2023-07-28 13:38:20.000000 cybereason-0.6.0/setup.py
+drwxrwxr-x   0 nuno      (1000) nuno      (1000)        0 2024-04-26 16:34:15.467464 cybereason-0.6.0/src/
+drwxrwxr-x   0 nuno      (1000) nuno      (1000)        0 2024-04-26 16:34:15.471464 cybereason-0.6.0/src/cybereason/
+-rwxrwxrwx   0 nuno      (1000) nuno      (1000)      177 2024-04-25 23:15:52.000000 cybereason-0.6.0/src/cybereason/__init__.py
+-rwxrwxrwx   0 nuno      (1000) nuno      (1000)     2019 2024-04-13 10:35:59.000000 cybereason-0.6.0/src/cybereason/_typing.py
+-rwxrwxrwx   0 nuno      (1000) nuno      (1000)    16380 2024-04-25 22:13:22.000000 cybereason-0.6.0/src/cybereason/client.py
+-rwxrwxrwx   0 nuno      (1000) nuno      (1000)     4620 2024-03-14 15:31:06.000000 cybereason-0.6.0/src/cybereason/exceptions.py
+-rwxrwxrwx   0 nuno      (1000) nuno      (1000)     3531 2023-11-26 16:25:11.000000 cybereason-0.6.0/src/cybereason/incident_response.py
+-rwxrwxrwx   0 nuno      (1000) nuno      (1000)     6759 2024-04-25 18:21:24.000000 cybereason-0.6.0/src/cybereason/malops.py
+drwxrwxr-x   0 nuno      (1000) nuno      (1000)        0 2024-04-26 16:34:15.471464 cybereason-0.6.0/src/cybereason/parse/
+-rwxrwxrwx   0 nuno      (1000) nuno      (1000)      147 2023-07-28 13:38:20.000000 cybereason-0.6.0/src/cybereason/parse/__init__.py
+-rwxrwxrwx   0 nuno      (1000) nuno      (1000)     2472 2023-07-28 13:38:20.000000 cybereason-0.6.0/src/cybereason/parse/cef.py
+-rwxrwxrwx   0 nuno      (1000) nuno      (1000)     2846 2023-07-28 13:38:20.000000 cybereason-0.6.0/src/cybereason/parse/server.py
+-rwxrwxrwx   0 nuno      (1000) nuno      (1000)        0 2023-07-28 13:38:20.000000 cybereason-0.6.0/src/cybereason/py.typed
+-rwxrwxrwx   0 nuno      (1000) nuno      (1000)     5175 2023-07-28 13:38:20.000000 cybereason-0.6.0/src/cybereason/rules.py
+-rwxrwxrwx   0 nuno      (1000) nuno      (1000)    16945 2024-03-14 15:31:28.000000 cybereason-0.6.0/src/cybereason/sensors.py
+-rwxrwxrwx   0 nuno      (1000) nuno      (1000)     4774 2024-03-30 02:49:47.000000 cybereason-0.6.0/src/cybereason/system.py
+-rwxrwxrwx   0 nuno      (1000) nuno      (1000)     7678 2024-03-08 13:36:46.000000 cybereason-0.6.0/src/cybereason/threat_intel.py
+drwxrwxr-x   0 nuno      (1000) nuno      (1000)        0 2024-04-26 16:34:15.475464 cybereason-0.6.0/src/cybereason/utils/
+-rwxrwxrwx   0 nuno      (1000) nuno      (1000)     4515 2023-07-28 13:38:20.000000 cybereason-0.6.0/src/cybereason/utils/__init__.py
+-rwxrwxrwx   0 nuno      (1000) nuno      (1000)      796 2023-07-28 13:38:20.000000 cybereason-0.6.0/src/cybereason/utils/guid.py
+drwxrwxr-x   0 nuno      (1000) nuno      (1000)        0 2024-04-26 16:34:15.471464 cybereason-0.6.0/src/cybereason.egg-info/
+-rw-rw-r--   0 nuno      (1000) nuno      (1000)     2935 2024-04-26 16:34:15.000000 cybereason-0.6.0/src/cybereason.egg-info/PKG-INFO
+-rw-rw-r--   0 nuno      (1000) nuno      (1000)      719 2024-04-26 16:34:15.000000 cybereason-0.6.0/src/cybereason.egg-info/SOURCES.txt
+-rw-rw-r--   0 nuno      (1000) nuno      (1000)        1 2024-04-26 16:34:15.000000 cybereason-0.6.0/src/cybereason.egg-info/dependency_links.txt
+-rw-rw-r--   0 nuno      (1000) nuno      (1000)        1 2023-11-26 15:59:18.000000 cybereason-0.6.0/src/cybereason.egg-info/not-zip-safe
+-rw-rw-r--   0 nuno      (1000) nuno      (1000)      229 2024-04-26 16:34:15.000000 cybereason-0.6.0/src/cybereason.egg-info/requires.txt
+-rw-rw-r--   0 nuno      (1000) nuno      (1000)       11 2024-04-26 16:34:15.000000 cybereason-0.6.0/src/cybereason.egg-info/top_level.txt
```

### Comparing `cybereason-0.5.1/LICENSE` & `cybereason-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cybereason-0.5.1/PKG-INFO` & `cybereason-0.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybereason
-Version: 0.5.1
+Version: 0.6.0
 Summary: Async Cybereason API client
 Home-page: https://github.com/forensic-security/cybereason#readme
 Author: Nuno André
 Author-email: mail@nunoand.re
 License: BSD-3-Clause
 Project-URL: Source, https://github.com/forensic-security/cybereason
 Project-URL: Bug Tracker, https://github.com/forensic-security/cybereason/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cybereason Version: 0.5.1 Summary: Async Cybereason
+Metadata-Version: 2.1 Name: cybereason Version: 0.6.0 Summary: Async Cybereason
 API client Home-page: https://github.com/forensic-security/cybereason#readme
 Author: Nuno AndrÃ© Author-email: mail@nunoand.re License: BSD-3-Clause
 Project-URL: Source, https://github.com/forensic-security/cybereason Project-
 URL: Bug Tracker, https://github.com/forensic-security/cybereason/issues
 Keywords: cybereason,cybersecurity,security,edr Platform: any Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators Classifier: Framework ::
```

### Comparing `cybereason-0.5.1/pyproject.toml` & `cybereason-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cybereason-0.5.1/setup.cfg` & `cybereason-0.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `cybereason-0.5.1/src/cybereason/_typing.py` & `cybereason-0.6.0/src/cybereason/_typing.py`

 * *Files identical despite different names*

### Comparing `cybereason-0.5.1/src/cybereason/client.py` & `cybereason-0.6.0/src/cybereason/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,15 +132,15 @@
                 log.warning('Renewing expired password.')
                 data = {
                     'oldPassword':        self.password,
                     'newPassword':        self.new_password,
                     'confirmNewPassword': self.new_password,
                     'submit':             'Login',
                 }
-                await self.session.post('?originalurl=/current?', data=data, **options)
+                await self.session.post('?originalurl=/current?', data=data, **options)  # type: ignore
                 self.password = self.new_password
 
         if 'Two factor authentication' in resp.text:
             if not self.totp_code:
                 await self.session.aclose()
                 raise AuthenticationError('TOTP code (2FA) is required')
 
@@ -367,15 +367,16 @@
         sort:         'Literal["ASC", "DESC"]' = 'ASC',
     ) -> 'AsyncIterator[Dict[str, Any]]':
         '''
         Args:
             check_resp: ``True`` if the response returns either a
                 {status, data} or a {outcome, data} schema.
         '''
-        data = {**data, 'limit': page_size, 'offset': 0, 'sortDirection': sort}
+        data = {**data, 'limit': page_size, 'offset': 0}
+        data.setdefault('sortDirection', sort)
 
         while True:
             resp = await self.post(path, data)
             if check_resp is True:
                 resp = self.check_resp(resp)
 
             for item in resp[key]:
```

### Comparing `cybereason-0.5.1/src/cybereason/exceptions.py` & `cybereason-0.6.0/src/cybereason/exceptions.py`

 * *Files identical despite different names*

### Comparing `cybereason-0.5.1/src/cybereason/incident_response.py` & `cybereason-0.6.0/src/cybereason/incident_response.py`

 * *Files identical despite different names*

### Comparing `cybereason-0.5.1/src/cybereason/malops.py` & `cybereason-0.6.0/src/cybereason/malops.py`

 * *Files 9% similar despite different names*

```diff
@@ -118,16 +118,25 @@
         resp = await self.post('crimes/get-comments', malop_id, raw_data=True)
         for msg in resp:
             msg['message'] = unescape(msg['message'])
         return resp
 
     @min_version(17, 5)
     @authz('Analyst L1')
-    async def get_malware_alerts(self, filters=None) -> 'AsyncIterator[Any]':
-        data = {'filters': filters or [], 'sortingFieldName': 'timestamp'}
+    async def get_malware_alerts(
+        self,
+        filters:       'Optional[List[Dict]]' = None,
+        sort_fieldname: str = 'timestamp',
+        sort_direction: str = 'DESC',
+    ) -> 'AsyncIterator[Any]':
+        data = {
+            'filters':          filters or [],
+            'sortingFieldName': sort_fieldname,
+            'sortDirection':    sort_direction,
+        }
         async for alert in self.aiter_pages('malware/query', data, 'malwares', check_resp=True):
             yield alert
 
 # region LABELS
     @min_version(20, 1, 43)
     async def get_malops_labels(
         self, malops_ids: 'Optional[List[MalopId]]' = None
```

### Comparing `cybereason-0.5.1/src/cybereason/parse/cef.py` & `cybereason-0.6.0/src/cybereason/parse/cef.py`

 * *Files identical despite different names*

### Comparing `cybereason-0.5.1/src/cybereason/parse/server.py` & `cybereason-0.6.0/src/cybereason/parse/server.py`

 * *Files identical despite different names*

### Comparing `cybereason-0.5.1/src/cybereason/rules.py` & `cybereason-0.6.0/src/cybereason/rules.py`

 * *Files identical despite different names*

### Comparing `cybereason-0.5.1/src/cybereason/sensors.py` & `cybereason-0.6.0/src/cybereason/sensors.py`

 * *Files identical despite different names*

### Comparing `cybereason-0.5.1/src/cybereason/system.py` & `cybereason-0.6.0/src/cybereason/system.py`

 * *Files identical despite different names*

### Comparing `cybereason-0.5.1/src/cybereason/threat_intel.py` & `cybereason-0.6.0/src/cybereason/threat_intel.py`

 * *Files identical despite different names*

### Comparing `cybereason-0.5.1/src/cybereason/utils/__init__.py` & `cybereason-0.6.0/src/cybereason/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cybereason-0.5.1/src/cybereason/utils/guid.py` & `cybereason-0.6.0/src/cybereason/utils/guid.py`

 * *Files identical despite different names*

### Comparing `cybereason-0.5.1/src/cybereason.egg-info/PKG-INFO` & `cybereason-0.6.0/src/cybereason.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybereason
-Version: 0.5.1
+Version: 0.6.0
 Summary: Async Cybereason API client
 Home-page: https://github.com/forensic-security/cybereason#readme
 Author: Nuno André
 Author-email: mail@nunoand.re
 License: BSD-3-Clause
 Project-URL: Source, https://github.com/forensic-security/cybereason
 Project-URL: Bug Tracker, https://github.com/forensic-security/cybereason/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cybereason Version: 0.5.1 Summary: Async Cybereason
+Metadata-Version: 2.1 Name: cybereason Version: 0.6.0 Summary: Async Cybereason
 API client Home-page: https://github.com/forensic-security/cybereason#readme
 Author: Nuno AndrÃ© Author-email: mail@nunoand.re License: BSD-3-Clause
 Project-URL: Source, https://github.com/forensic-security/cybereason Project-
 URL: Bug Tracker, https://github.com/forensic-security/cybereason/issues
 Keywords: cybereason,cybersecurity,security,edr Platform: any Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators Classifier: Framework ::
```

### Comparing `cybereason-0.5.1/src/cybereason.egg-info/SOURCES.txt` & `cybereason-0.6.0/src/cybereason.egg-info/SOURCES.txt`

 * *Files identical despite different names*

