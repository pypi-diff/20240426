# Comparing `tmp/prelude_sdk-1.7.2.tar.gz` & `tmp/prelude_sdk-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prelude_sdk-1.7.2.tar", last modified: Wed Apr 17 18:50:02 2024, max compression
+gzip compressed data, was "prelude_sdk-1.7.3.tar", last modified: Thu Apr 25 22:31:47 2024, max compression
```

## Comparing `prelude_sdk-1.7.2.tar` & `prelude_sdk-1.7.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-17 18:50:02.366851 prelude_sdk-1.7.2/
--rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude_sdk-1.7.2/LICENSE
--rw-r--r--   0 pack       (501) staff       (20)     1163 2024-04-17 18:50:02.366769 prelude_sdk-1.7.2/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      697 2023-04-11 22:16:02.000000 prelude_sdk-1.7.2/README.md
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-17 18:50:02.359145 prelude_sdk-1.7.2/prelude_sdk/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude_sdk-1.7.2/prelude_sdk/__init__.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-17 18:50:02.362801 prelude_sdk-1.7.2/prelude_sdk/controllers/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude_sdk-1.7.2/prelude_sdk/controllers/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     6020 2024-04-17 18:29:22.000000 prelude_sdk-1.7.2/prelude_sdk/controllers/build_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     6626 2024-04-17 18:29:22.000000 prelude_sdk-1.7.2/prelude_sdk/controllers/detect_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     1080 2024-04-17 18:29:22.000000 prelude_sdk-1.7.2/prelude_sdk/controllers/generate_controller.py
--rw-r--r--   0 pack       (501) staff       (20)      580 2024-04-17 18:29:22.000000 prelude_sdk-1.7.2/prelude_sdk/controllers/http_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     8288 2024-04-17 18:29:22.000000 prelude_sdk-1.7.2/prelude_sdk/controllers/iam_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     3727 2024-04-17 18:29:22.000000 prelude_sdk-1.7.2/prelude_sdk/controllers/partner_controller.py
--rw-r--r--   0 pack       (501) staff       (20)      559 2024-04-17 18:29:22.000000 prelude_sdk-1.7.2/prelude_sdk/controllers/probe_controller.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-17 18:50:02.363653 prelude_sdk-1.7.2/prelude_sdk/models/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude_sdk-1.7.2/prelude_sdk/models/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     2816 2023-07-11 13:50:29.000000 prelude_sdk-1.7.2/prelude_sdk/models/account.py
--rw-r--r--   0 pack       (501) staff       (20)     4642 2024-04-11 16:14:14.000000 prelude_sdk-1.7.2/prelude_sdk/models/codes.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-17 18:50:02.366496 prelude_sdk-1.7.2/prelude_sdk.egg-info/
--rw-r--r--   0 pack       (501) staff       (20)     1163 2024-04-17 18:50:02.000000 prelude_sdk-1.7.2/prelude_sdk.egg-info/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      865 2024-04-17 18:50:02.000000 prelude_sdk-1.7.2/prelude_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 pack       (501) staff       (20)        1 2024-04-17 18:50:02.000000 prelude_sdk-1.7.2/prelude_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 pack       (501) staff       (20)        9 2024-04-17 18:50:02.000000 prelude_sdk-1.7.2/prelude_sdk.egg-info/requires.txt
--rw-r--r--   0 pack       (501) staff       (20)       12 2024-04-17 18:50:02.000000 prelude_sdk-1.7.2/prelude_sdk.egg-info/top_level.txt
--rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude_sdk-1.7.2/pyproject.toml
--rw-r--r--   0 pack       (501) staff       (20)      532 2024-04-17 18:50:02.367107 prelude_sdk-1.7.2/setup.cfg
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-17 18:50:02.365904 prelude_sdk-1.7.2/tests/
--rw-r--r--   0 pack       (501) staff       (20)     5494 2024-04-17 18:29:22.000000 prelude_sdk-1.7.2/tests/conftest.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-17 18:50:02.366074 prelude_sdk-1.7.2/tests/templates/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-04-07 19:23:14.000000 prelude_sdk-1.7.2/tests/templates/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)    10423 2024-04-17 18:29:22.000000 prelude_sdk-1.7.2/tests/test_build.py
--rw-r--r--   0 pack       (501) staff       (20)     5991 2024-04-17 18:29:22.000000 prelude_sdk-1.7.2/tests/test_detect.py
--rw-r--r--   0 pack       (501) staff       (20)     1936 2024-04-17 18:29:22.000000 prelude_sdk-1.7.2/tests/test_generate.py
--rw-r--r--   0 pack       (501) staff       (20)     8372 2024-04-17 18:29:22.000000 prelude_sdk-1.7.2/tests/test_iam.py
--rw-r--r--   0 pack       (501) staff       (20)    12997 2024-04-17 18:29:22.000000 prelude_sdk-1.7.2/tests/test_partner.py
--rw-r--r--   0 pack       (501) staff       (20)     4587 2024-04-17 18:29:22.000000 prelude_sdk-1.7.2/tests/test_probe.py
--rw-r--r--   0 pack       (501) staff       (20)     2073 2024-04-17 18:29:22.000000 prelude_sdk-1.7.2/tests/testutils.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-25 22:31:47.276436 prelude_sdk-1.7.3/
+-rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude_sdk-1.7.3/LICENSE
+-rw-r--r--   0 pack       (501) staff       (20)     1163 2024-04-25 22:31:47.276377 prelude_sdk-1.7.3/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      697 2023-04-11 22:16:02.000000 prelude_sdk-1.7.3/README.md
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-25 22:31:47.269545 prelude_sdk-1.7.3/prelude_sdk/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude_sdk-1.7.3/prelude_sdk/__init__.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-25 22:31:47.272638 prelude_sdk-1.7.3/prelude_sdk/controllers/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude_sdk-1.7.3/prelude_sdk/controllers/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     6020 2024-04-17 18:29:22.000000 prelude_sdk-1.7.3/prelude_sdk/controllers/build_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     6626 2024-04-17 18:29:22.000000 prelude_sdk-1.7.3/prelude_sdk/controllers/detect_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     1080 2024-04-17 18:29:22.000000 prelude_sdk-1.7.3/prelude_sdk/controllers/generate_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)      580 2024-04-17 18:29:22.000000 prelude_sdk-1.7.3/prelude_sdk/controllers/http_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     8288 2024-04-17 18:29:22.000000 prelude_sdk-1.7.3/prelude_sdk/controllers/iam_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     3727 2024-04-17 18:29:22.000000 prelude_sdk-1.7.3/prelude_sdk/controllers/partner_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)      559 2024-04-17 18:29:22.000000 prelude_sdk-1.7.3/prelude_sdk/controllers/probe_controller.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-25 22:31:47.273334 prelude_sdk-1.7.3/prelude_sdk/models/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude_sdk-1.7.3/prelude_sdk/models/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     2816 2023-07-11 13:50:29.000000 prelude_sdk-1.7.3/prelude_sdk/models/account.py
+-rw-r--r--   0 pack       (501) staff       (20)     4564 2024-04-25 18:56:47.000000 prelude_sdk-1.7.3/prelude_sdk/models/codes.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-25 22:31:47.276036 prelude_sdk-1.7.3/prelude_sdk.egg-info/
+-rw-r--r--   0 pack       (501) staff       (20)     1163 2024-04-25 22:31:47.000000 prelude_sdk-1.7.3/prelude_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      865 2024-04-25 22:31:47.000000 prelude_sdk-1.7.3/prelude_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 pack       (501) staff       (20)        1 2024-04-25 22:31:47.000000 prelude_sdk-1.7.3/prelude_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 pack       (501) staff       (20)        9 2024-04-25 22:31:47.000000 prelude_sdk-1.7.3/prelude_sdk.egg-info/requires.txt
+-rw-r--r--   0 pack       (501) staff       (20)       12 2024-04-25 22:31:47.000000 prelude_sdk-1.7.3/prelude_sdk.egg-info/top_level.txt
+-rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude_sdk-1.7.3/pyproject.toml
+-rw-r--r--   0 pack       (501) staff       (20)      532 2024-04-25 22:31:47.276652 prelude_sdk-1.7.3/setup.cfg
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-25 22:31:47.275728 prelude_sdk-1.7.3/tests/
+-rw-r--r--   0 pack       (501) staff       (20)     5494 2024-04-17 18:29:22.000000 prelude_sdk-1.7.3/tests/conftest.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-25 22:31:47.275880 prelude_sdk-1.7.3/tests/templates/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-04-07 19:23:14.000000 prelude_sdk-1.7.3/tests/templates/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)    10423 2024-04-17 18:29:22.000000 prelude_sdk-1.7.3/tests/test_build.py
+-rw-r--r--   0 pack       (501) staff       (20)     6295 2024-04-25 18:56:47.000000 prelude_sdk-1.7.3/tests/test_detect.py
+-rw-r--r--   0 pack       (501) staff       (20)     1936 2024-04-17 18:29:22.000000 prelude_sdk-1.7.3/tests/test_generate.py
+-rw-r--r--   0 pack       (501) staff       (20)     8372 2024-04-17 18:29:22.000000 prelude_sdk-1.7.3/tests/test_iam.py
+-rw-r--r--   0 pack       (501) staff       (20)    13032 2024-04-25 18:56:47.000000 prelude_sdk-1.7.3/tests/test_partner.py
+-rw-r--r--   0 pack       (501) staff       (20)     4587 2024-04-17 18:29:22.000000 prelude_sdk-1.7.3/tests/test_probe.py
+-rw-r--r--   0 pack       (501) staff       (20)     2073 2024-04-17 18:29:22.000000 prelude_sdk-1.7.3/tests/testutils.py
```

### Comparing `prelude_sdk-1.7.2/LICENSE` & `prelude_sdk-1.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `prelude_sdk-1.7.2/PKG-INFO` & `prelude_sdk-1.7.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-sdk
-Version: 1.7.2
+Version: 1.7.3
 Summary: For interacting with the Prelude API
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `prelude_sdk-1.7.2/README.md` & `prelude_sdk-1.7.3/README.md`

 * *Files identical despite different names*

### Comparing `prelude_sdk-1.7.2/prelude_sdk/controllers/build_controller.py` & `prelude_sdk-1.7.3/prelude_sdk/controllers/build_controller.py`

 * *Files identical despite different names*

### Comparing `prelude_sdk-1.7.2/prelude_sdk/controllers/detect_controller.py` & `prelude_sdk-1.7.3/prelude_sdk/controllers/detect_controller.py`

 * *Files identical despite different names*

### Comparing `prelude_sdk-1.7.2/prelude_sdk/controllers/generate_controller.py` & `prelude_sdk-1.7.3/prelude_sdk/controllers/generate_controller.py`

 * *Files identical despite different names*

### Comparing `prelude_sdk-1.7.2/prelude_sdk/controllers/http_controller.py` & `prelude_sdk-1.7.3/prelude_sdk/controllers/http_controller.py`

 * *Files identical despite different names*

### Comparing `prelude_sdk-1.7.2/prelude_sdk/controllers/iam_controller.py` & `prelude_sdk-1.7.3/prelude_sdk/controllers/iam_controller.py`

 * *Files identical despite different names*

### Comparing `prelude_sdk-1.7.2/prelude_sdk/controllers/partner_controller.py` & `prelude_sdk-1.7.3/prelude_sdk/controllers/partner_controller.py`

 * *Files identical despite different names*

### Comparing `prelude_sdk-1.7.2/prelude_sdk/controllers/probe_controller.py` & `prelude_sdk-1.7.3/prelude_sdk/controllers/probe_controller.py`

 * *Files identical despite different names*

### Comparing `prelude_sdk-1.7.2/prelude_sdk/models/account.py` & `prelude_sdk-1.7.3/prelude_sdk/models/account.py`

 * *Files identical despite different names*

### Comparing `prelude_sdk-1.7.2/prelude_sdk/models/codes.py` & `prelude_sdk-1.7.3/prelude_sdk/models/codes.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     TIMED_OUT = 102
     FAILED_CLEANUP = 103
     TEST_NOT_RELEVANT = 104
     DYNAMIC_QUARANTINE = 105
     BLOCKED_AT_PERIMETER = 106
     EXPLOIT_PREVENTED = 107
     ENDPOINT_NOT_RELEVANT = 108
-    TEST_DISALLOWED = 126
+    OS_PREVENTED_EXECUTION = 126
     STATIC_QUARANTINE = 127
     BLOCKED = 137
     UNEXPECTED_ERROR = 256
 
     @classmethod
     def _missing_(cls, value):
         if value and not isinstance(value, int):
@@ -118,22 +118,20 @@
                 ExitCode.ENDPOINT_NOT_RELEVANT,
                 ExitCode.TEST_NOT_RELEVANT,
             ],
             State.PROTECTED: [
                 ExitCode.BLOCKED,
                 ExitCode.BLOCKED_AT_PERIMETER,
                 ExitCode.DYNAMIC_QUARANTINE,
-                ExitCode.ENDPOINT_NOT_RELEVANT,
                 ExitCode.EXPLOIT_PREVENTED,
+                ExitCode.OS_PREVENTED_EXECUTION,
                 ExitCode.PROCESS_BLOCKED,
                 ExitCode.PROCESS_BLOCKED_GRACEFULLY,
                 ExitCode.PROTECTED,
                 ExitCode.STATIC_QUARANTINE,
-                ExitCode.TEST_DISALLOWED,
-                ExitCode.TEST_NOT_RELEVANT,
             ],
             State.UNPROTECTED: [
                 ExitCode.UNPROTECTED,
             ],
         }
```

### Comparing `prelude_sdk-1.7.2/prelude_sdk.egg-info/PKG-INFO` & `prelude_sdk-1.7.3/prelude_sdk.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-sdk
-Version: 1.7.2
+Version: 1.7.3
 Summary: For interacting with the Prelude API
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `prelude_sdk-1.7.2/prelude_sdk.egg-info/SOURCES.txt` & `prelude_sdk-1.7.3/prelude_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prelude_sdk-1.7.2/setup.cfg` & `prelude_sdk-1.7.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = prelude-sdk
-version = 1.7.2
+version = 1.7.3
 author = Prelude Research
 author_email = support@preludesecurity.com
 description = For interacting with the Prelude API
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/preludeorg
 classifiers =
```

### Comparing `prelude_sdk-1.7.2/tests/conftest.py` & `prelude_sdk-1.7.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `prelude_sdk-1.7.2/tests/test_build.py` & `prelude_sdk-1.7.3/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `prelude_sdk-1.7.2/tests/test_detect.py` & `prelude_sdk-1.7.3/tests/test_detect.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,23 +47,24 @@
         assert 1 <= len(res)
         ep = [r for r in res if r['serial_num'] == self.serial][0]
         pytest.expected_endpoint['endpoint_id'] = ep['endpoint_id']
         pytest.endpoint_id = ep['endpoint_id']
 
         diffs = check_dict_items(pytest.expected_endpoint, ep)
         assert not diffs, json.dumps(diffs, indent=2)
-        assert parse(ep['last_seen']).date() == parse(ep['created']).date()
+        assert ep['last_seen'] is None
 
     def test_update_endpoint(self, unwrap):
         res = unwrap(self.detect.update_endpoint)(self.detect, endpoint_id=pytest.endpoint_id, tags=self.updated_tags)
         assert res['id'] == pytest.endpoint_id
         pytest.expected_endpoint['tags'] = [self.updated_tags]
 
         res = unwrap(self.detect.list_endpoints)(self.detect)
-        diffs = check_dict_items(pytest.expected_endpoint, res[0])
+        ep = [r for r in res if r['endpoint_id'] == pytest.endpoint_id][0]
+        diffs = check_dict_items(pytest.expected_endpoint, ep)
         assert not diffs, json.dumps(diffs, indent=2)
 
     def test_schedule_threat(self, unwrap):
         queue_length = len(pytest.expected_account['queue'])
 
         res = unwrap(self.detect.schedule)(self.detect, [dict(threat_id=pytest.threat_id, run_code=RunCode.DAILY.name)])
         pytest.expected_account['queue'].append(res[0])
@@ -118,18 +119,24 @@
     def test_describe_activity(self, unwrap, api):
         res = requests.get(api, headers=dict(token=pytest.token, dos=f'darwin-x86_64', dat=f'{pytest.test_id}:100',
                                              version='2.1'))
         assert res.status_code in [200, 302]
         filters = dict(
             start=datetime.now(timezone.utc) - timedelta(days=1),
             finish=datetime.now(timezone.utc) + timedelta(days=1),
-            endpoints=pytest.endpoint_id
+            endpoints=pytest.endpoint_id,
+            tests=pytest.test_id,
         )
         res = unwrap(self.detect.describe_activity)(self.detect, view='logs', filters=filters)
         assert 1 == len(res), json.dumps(res, indent=2)
 
+        res = unwrap(self.detect.list_endpoints)(self.detect)
+        assert 1 <= len(res)
+        ep = [r for r in res if r['serial_num'] == self.serial][0]
+        assert parse(ep['last_seen']).date() == parse(ep['created']).date()
+
     def test_delete_endpoint(self, unwrap):
         unwrap(self.detect.delete_endpoint)(self.detect, ident=pytest.endpoint_id)
         res = unwrap(self.detect.list_endpoints)(self.detect)
         ep = [r for r in res if r['serial_num'] == self.serial]
         assert 0 == len(ep), json.dumps(ep, indent=2)
```

### Comparing `prelude_sdk-1.7.2/tests/test_generate.py` & `prelude_sdk-1.7.3/tests/test_generate.py`

 * *Files identical despite different names*

### Comparing `prelude_sdk-1.7.2/tests/test_iam.py` & `prelude_sdk-1.7.3/tests/test_iam.py`

 * *Files identical despite different names*

### Comparing `prelude_sdk-1.7.2/tests/test_partner.py` & `prelude_sdk-1.7.3/tests/test_partner.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,17 +131,18 @@
     def test_activity_logs(self, unwrap, api, host, edr_id, control, os, platform, policy, policy_name, partner_api, user, secret, webhook_keys):
         res = requests.get(api, headers=dict(token=pytest.token, dos=f'{platform}-x86_64', dat=f'{pytest.test_id}:100',
                                              version='2.1'))
         assert res.status_code in [200, 302]
         pytest.endpoint_1['dos'] = f'{platform}-x86_64'
 
         filters = dict(
-            start=datetime.now(timezone.utc) - timedelta(days=7),
+            start=datetime.now(timezone.utc) - timedelta(days=1),
             finish=datetime.now(timezone.utc) + timedelta(days=1),
-            endpoints=pytest.endpoint_1['endpoint_id']
+            endpoints=pytest.endpoint_1['endpoint_id'],
+            tests=pytest.test_id,
         )
         res = unwrap(self.detect.describe_activity)(self.detect, view='logs', filters=filters)
         assert len(res) == 1, json.dumps(res, indent=2)
         expected = dict(
             test=pytest.test_id,
             endpoint_id=pytest.endpoint_1['endpoint_id'],
             status=100,
@@ -166,15 +167,15 @@
         if control == Control.CROWDSTRIKE:
             assert 1 == len(res)
             assert pytest.expected_detection['rule']['logsource']['product'] == res[0]['platform']
             assert 1 == len(res[0]['rules'])
             assert f'{pytest.expected_detection["rule"]["title"]} ({pytest.detection_id[:8]}) (0)' == res[0]['rules'][0]['name']
             assert res[0]['rules'][0]['status'] in ['ALREADY_EXISTS', 'CREATED']
         else:
-            assert len(res) == 5
+            assert 5 == len(res)
             assert {'file', 'ioc_id'} == res[0].keys()
             assert res[0]['file'].startswith(pytest.test_id)
 
     def test_detach(self, unwrap, host, edr_id, control, os, platform, policy, policy_name, partner_api, user, secret, webhook_keys):
         try:
             unwrap(self.partner.detach)(self.partner, partner=control)
             res = unwrap(self.iam.get_account)(self.iam)
```

### Comparing `prelude_sdk-1.7.2/tests/test_probe.py` & `prelude_sdk-1.7.3/tests/test_probe.py`

 * *Files identical despite different names*

### Comparing `prelude_sdk-1.7.2/tests/testutils.py` & `prelude_sdk-1.7.3/tests/testutils.py`

 * *Files identical despite different names*

