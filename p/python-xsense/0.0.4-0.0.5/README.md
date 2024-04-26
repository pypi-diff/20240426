# Comparing `tmp/python-xsense-0.0.4.tar.gz` & `tmp/python-xsense-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-xsense-0.0.4.tar", last modified: Mon Apr 22 18:57:35 2024, max compression
+gzip compressed data, was "python-xsense-0.0.5.tar", last modified: Fri Apr 26 20:22:32 2024, max compression
```

## Comparing `python-xsense-0.0.4.tar` & `python-xsense-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2024-04-22 18:57:35.867764 python-xsense-0.0.4/
--rw-r--r--   0 theo       (501) staff       (20)     1859 2024-04-22 18:57:35.865311 python-xsense-0.0.4/PKG-INFO
--rw-r--r--   0 theo       (501) staff       (20)     1226 2024-04-18 18:45:42.000000 python-xsense-0.0.4/README.rst
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2024-04-22 18:57:35.863410 python-xsense-0.0.4/python_xsense.egg-info/
--rw-r--r--   0 theo       (501) staff       (20)     1859 2024-04-22 18:57:35.000000 python-xsense-0.0.4/python_xsense.egg-info/PKG-INFO
--rw-r--r--   0 theo       (501) staff       (20)      400 2024-04-22 18:57:35.000000 python-xsense-0.0.4/python_xsense.egg-info/SOURCES.txt
--rw-r--r--   0 theo       (501) staff       (20)        1 2024-04-22 18:57:35.000000 python-xsense-0.0.4/python_xsense.egg-info/dependency_links.txt
--rw-r--r--   0 theo       (501) staff       (20)       51 2024-04-22 18:57:35.000000 python-xsense-0.0.4/python_xsense.egg-info/requires.txt
--rw-r--r--   0 theo       (501) staff       (20)        7 2024-04-22 18:57:35.000000 python-xsense-0.0.4/python_xsense.egg-info/top_level.txt
--rw-r--r--   0 theo       (501) staff       (20)       38 2024-04-22 18:57:35.867987 python-xsense-0.0.4/setup.cfg
--rw-r--r--   0 theo       (501) staff       (20)      911 2024-04-22 18:57:15.000000 python-xsense-0.0.4/setup.py
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2024-04-22 18:57:35.861041 python-xsense-0.0.4/xsense/
--rw-r--r--   0 theo       (501) staff       (20)      147 2024-02-20 08:37:03.000000 python-xsense-0.0.4/xsense/__init__.py
--rw-r--r--   0 theo       (501) staff       (20)     4814 2024-04-22 18:57:07.000000 python-xsense-0.0.4/xsense/async_xsense.py
--rw-r--r--   0 theo       (501) staff       (20)     3745 2024-04-18 16:47:49.000000 python-xsense-0.0.4/xsense/aws_signer.py
--rw-r--r--   0 theo       (501) staff       (20)     6106 2024-04-22 18:57:07.000000 python-xsense-0.0.4/xsense/base.py
--rw-r--r--   0 theo       (501) staff       (20)      387 2024-04-14 15:45:02.000000 python-xsense-0.0.4/xsense/device.py
--rw-r--r--   0 theo       (501) staff       (20)      539 2024-04-14 15:46:07.000000 python-xsense-0.0.4/xsense/entity.py
--rw-r--r--   0 theo       (501) staff       (20)     1019 2024-04-14 14:39:29.000000 python-xsense-0.0.4/xsense/house.py
--rw-r--r--   0 theo       (501) staff       (20)      566 2024-04-12 18:42:45.000000 python-xsense-0.0.4/xsense/mapping.py
--rw-r--r--   0 theo       (501) staff       (20)     1198 2024-04-14 16:07:00.000000 python-xsense-0.0.4/xsense/station.py
--rw-r--r--   0 theo       (501) staff       (20)     1411 2024-04-14 18:51:33.000000 python-xsense-0.0.4/xsense/utils.py
--rw-r--r--   0 theo       (501) staff       (20)     4051 2024-04-22 18:57:07.000000 python-xsense-0.0.4/xsense/xsense.py
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2024-04-26 20:22:32.158665 python-xsense-0.0.5/
+-rw-r--r--   0 theo       (501) staff       (20)     1859 2024-04-26 20:22:32.157964 python-xsense-0.0.5/PKG-INFO
+-rw-r--r--   0 theo       (501) staff       (20)     1226 2024-04-18 18:45:42.000000 python-xsense-0.0.5/README.rst
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2024-04-26 20:22:32.157256 python-xsense-0.0.5/python_xsense.egg-info/
+-rw-r--r--   0 theo       (501) staff       (20)     1859 2024-04-26 20:22:31.000000 python-xsense-0.0.5/python_xsense.egg-info/PKG-INFO
+-rw-r--r--   0 theo       (501) staff       (20)      421 2024-04-26 20:22:31.000000 python-xsense-0.0.5/python_xsense.egg-info/SOURCES.txt
+-rw-r--r--   0 theo       (501) staff       (20)        1 2024-04-26 20:22:31.000000 python-xsense-0.0.5/python_xsense.egg-info/dependency_links.txt
+-rw-r--r--   0 theo       (501) staff       (20)       51 2024-04-26 20:22:31.000000 python-xsense-0.0.5/python_xsense.egg-info/requires.txt
+-rw-r--r--   0 theo       (501) staff       (20)        7 2024-04-26 20:22:31.000000 python-xsense-0.0.5/python_xsense.egg-info/top_level.txt
+-rw-r--r--   0 theo       (501) staff       (20)       38 2024-04-26 20:22:32.158741 python-xsense-0.0.5/setup.cfg
+-rw-r--r--   0 theo       (501) staff       (20)      911 2024-04-26 20:21:56.000000 python-xsense-0.0.5/setup.py
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2024-04-26 20:22:32.156345 python-xsense-0.0.5/xsense/
+-rw-r--r--   0 theo       (501) staff       (20)      147 2024-02-20 08:37:03.000000 python-xsense-0.0.5/xsense/__init__.py
+-rw-r--r--   0 theo       (501) staff       (20)     5906 2024-04-26 20:21:49.000000 python-xsense-0.0.5/xsense/async_xsense.py
+-rw-r--r--   0 theo       (501) staff       (20)     3745 2024-04-18 16:47:49.000000 python-xsense-0.0.5/xsense/aws_signer.py
+-rw-r--r--   0 theo       (501) staff       (20)     6437 2024-04-26 20:21:49.000000 python-xsense-0.0.5/xsense/base.py
+-rw-r--r--   0 theo       (501) staff       (20)      387 2024-04-25 20:57:22.000000 python-xsense-0.0.5/xsense/device.py
+-rw-r--r--   0 theo       (501) staff       (20)      546 2024-04-26 20:21:49.000000 python-xsense-0.0.5/xsense/entity.py
+-rw-r--r--   0 theo       (501) staff       (20)      169 2024-04-26 20:21:49.000000 python-xsense-0.0.5/xsense/exceptions.py
+-rw-r--r--   0 theo       (501) staff       (20)     1019 2024-04-14 14:39:29.000000 python-xsense-0.0.5/xsense/house.py
+-rw-r--r--   0 theo       (501) staff       (20)     1016 2024-04-26 20:21:49.000000 python-xsense-0.0.5/xsense/mapping.py
+-rw-r--r--   0 theo       (501) staff       (20)     1198 2024-04-14 16:07:00.000000 python-xsense-0.0.5/xsense/station.py
+-rw-r--r--   0 theo       (501) staff       (20)     1411 2024-04-14 18:51:33.000000 python-xsense-0.0.5/xsense/utils.py
+-rw-r--r--   0 theo       (501) staff       (20)     5023 2024-04-26 20:21:49.000000 python-xsense-0.0.5/xsense/xsense.py
```

### Comparing `python-xsense-0.0.4/PKG-INFO` & `python-xsense-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-xsense
-Version: 0.0.4
+Version: 0.0.5
 Summary: XSense Python Module
 Home-page: https://github.com/theosnel/python-xsense
 Author: Theo Snelleman
 Author-email: <python@theo.snelleman.net>
 License: MIT
 Keywords: python,xsense
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `python-xsense-0.0.4/README.rst` & `python-xsense-0.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `python-xsense-0.0.4/python_xsense.egg-info/PKG-INFO` & `python-xsense-0.0.5/python_xsense.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-xsense
-Version: 0.0.4
+Version: 0.0.5
 Summary: XSense Python Module
 Home-page: https://github.com/theosnel/python-xsense
 Author: Theo Snelleman
 Author-email: <python@theo.snelleman.net>
 License: MIT
 Keywords: python,xsense
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `python-xsense-0.0.4/setup.py` & `python-xsense-0.0.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 DESCRIPTION = 'XSense Python Module'
 
 with open('README.rst', 'r') as fd:
     LONG_DESCRIPTION = fd.read()
 
 setup(
     name='python-xsense',
```

### Comparing `python-xsense-0.0.4/xsense/async_xsense.py` & `python-xsense-0.0.5/xsense/async_xsense.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from datetime import datetime
 import json
 
 import aiohttp
 
 from xsense.aws_signer import AWSSigner
 from xsense.base import XSenseBase
+from xsense.exceptions import SessionExpired, APIFailure
 from xsense.house import House
 from xsense.station import Station
 
 
 class AsyncXSense(XSenseBase):
     async def api_call(self, code, unauth=False, **kwargs):
         data = {
@@ -37,16 +38,29 @@
                     "appCode": self.APPCODE,
                 },
                 headers=headers
             ) as response:
                 self._lastres = response
 
                 data = await response.json()
+
+                if response.status >= 400:
+                    message = data.get('message') or 'unknown error'
+                    raise APIFailure(f'API failure: {response.status}/{message}')
+
+                if 'reCode' not in data:
+                    raise APIFailure('API failure: Cannot understand response')
+
                 if data['reCode'] != 200:
-                    raise RuntimeError(f"Request for code {code} failed with error {data['reCode']} {data.get('reMsg')}")
+                    errCode = data.get('errCode', 0)
+                    if errCode in ('10000008', '10000020'):
+                        raise SessionExpired(data.get('reMsg'))
+                    raise APIFailure(
+                        f"Request for code {code} failed with error {errCode}/{data['reCode']} {data.get('reMsg')}"
+                    )
                 return data['reData']
 
     async def get_thing(self, station: Station, page: str):
         if self._aws_token_expiring():
             await self.load_aws()
 
         url, headers = self._thing_request(station, page)
@@ -68,14 +82,18 @@
         async with aiohttp.ClientSession() as session:
             async with session.post(
                 url, json=data, headers=headers
             ) as response:
                 self._lastres = response
                 text = await response.text()
                 data = json.loads(text)
+
+                if response.status == 400:
+                    raise SessionExpired(data.get('message', 'token refresh failed'))
+
                 self._parse_refresh_result(data.get('AuthenticationResult', {}))
 
     async def init(self):
         await self.get_client_info()
 
     async def load_aws(self):
         await self.get_aws_tokens()
@@ -133,12 +151,19 @@
             'utctimestamp': "0"
         }
         return await self.api_call("103007", **params)
 
     async def get_station_state(self, station: Station):
         res = await self.get_thing(station, f'2nd_info_{station.sn}')
 
-        station.set_data(res['state']['reported'])
+        if 'reported' in res.get('state', {}):
+            station.set_data(res['state']['reported'])
+        else:
+            raise APIFailure(f'Unable to retrieve station data: {self._lastres.status}/{self._lastres.text()}')
 
     async def get_state(self, station: Station):
         res = await self.get_thing(station, '2nd_mainpage')
-        self._parse_get_state(station, res['state']['reported'])
+
+        if 'reported' in res.get('state', {}):
+            self._parse_get_state(station, res['state']['reported'])
+        else:
+            raise APIFailure(f'Unable to retrieve station data: {self._lastres.status}/{self._lastres.text()}')
```

### Comparing `python-xsense-0.0.4/xsense/aws_signer.py` & `python-xsense-0.0.5/xsense/aws_signer.py`

 * *Files identical despite different names*

### Comparing `python-xsense-0.0.4/xsense/base.py` & `python-xsense-0.0.5/xsense/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from datetime import datetime, timedelta, timezone
 from typing import Dict
 
 import boto3
 from botocore.exceptions import ClientError
 from pycognito import AWSSRP
 
+from .exceptions import AuthFailed
 from .station import Station
 from .house import House
 
 
 class XSenseBase:
     API = 'https://api.x-sense-iot.com'
     VERSION = "v1.18.0_20240311"
@@ -38,14 +39,17 @@
     signer = None
 
     _lastres = None
 
     def __init__(self):
         self.houses: Dict[str, House] = {}
 
+    def _parse_client_error(self, e: ClientError):
+        return e.response.get('Error', {}).get('Message') or str(e)
+
     def sync_login(self, username, password):
         self.username = username
         session = boto3.Session()
         cognito = session.client('cognito-idp', region_name=self.region)
 
         aws_srp = AWSSRP(
             username=username,
@@ -61,15 +65,15 @@
         try:
             response = cognito.initiate_auth(
                 ClientId=self.clientid,
                 AuthFlow='USER_SRP_AUTH',
                 AuthParameters=auth_params
             )
         except ClientError as e:
-            raise RuntimeError(f'Cannot login, initiate_auth failed: {e}') from e
+            raise AuthFailed(self._parse_client_error(e)) from e
 
         userid = response['ChallengeParameters']['USERNAME']
 
         challenge_response = aws_srp.process_challenge(response["ChallengeParameters"], auth_params)
 
         challenge_response['SECRET_HASH'] = self.generate_hash(userid + self.clientid)
 
@@ -83,21 +87,23 @@
             auth_result = response['AuthenticationResult']
             self.access_token = auth_result['AccessToken']
             self.id_token = auth_result['IdToken']
             self.refresh_token =auth_result['RefreshToken']
             self.access_token_expiry = datetime.now(timezone.utc) + timedelta(seconds=auth_result['ExpiresIn'])
 
         except ClientError as e:
-            raise RuntimeError(f'Cannot login, respond_to_auth failed: {e}') from e
+            raise AuthFailed(self._parse_client_error(e)) from e
 
     def restore_session(self, username, access_token, refresh_token, id_token):
         self.username = username
         self.access_token = access_token
         self.refresh_token = refresh_token
         self.id_token = id_token
+        self.access_token_expiry = datetime.now(timezone.utc)
+        self.aws_access_expiry = datetime.now(timezone.utc)
 
     def _access_token_expiring(self):
         return datetime.now(timezone.utc) > self.access_token_expiry - timedelta(seconds=60)
 
     def _aws_token_expiring(self):
         return datetime.now(timezone.utc) > self.aws_access_expiry - timedelta(seconds=60)
 
@@ -167,20 +173,22 @@
 
         signed = self.signer.sign_headers('GET', url, station.house.mqtt_region, headers, None)
         headers |= signed
 
         return url, headers
 
     def _parse_refresh_result(self, data: Dict):
+        if 'RefreshToken' in data:
+            self.refresh_token = data['RefreshToken']
         if 'AccessToken' in data:
             self.access_token = data['AccessToken']
         if 'IdToken' in data:
             self.id_token = data['IdToken']
         if 'ExpiresIn' in data:
             self.access_token_expiry = datetime.now(timezone.utc) + timedelta(seconds=data['ExpiresIn'])
 
     def _parse_get_state(self, station: Station, data: Dict):
         if 'wifiRSSI' in data:
             station.data['wifiRSSI'] = data['wifiRSSI']
         for sn, i in data['devs'].items():
             dev = station.get_device_by_sn(sn)
-            dev.set_data(i)
+            dev.set_data(i)
```

### Comparing `python-xsense-0.0.4/xsense/entity.py` & `python-xsense-0.0.5/xsense/entity.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,14 +12,14 @@
     ):
         self.room_id = kwargs.get('roomId')
         self._data = {}
 
     def set_data(self, values: dict):
         data = values.copy()
         if 'online' in values:
-            self.online = values.pop('online')
+            self.online = values.pop('online') != '0'
         data |= data.pop('status', {})
         self._data.update(map_values(self.type, data))
 
     @property
     def data(self):
         return self._data
```

### Comparing `python-xsense-0.0.4/xsense/house.py` & `python-xsense-0.0.5/xsense/house.py`

 * *Files identical despite different names*

### Comparing `python-xsense-0.0.4/xsense/mapping.py` & `python-xsense-0.0.5/xsense/mapping.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,42 @@
-from typing import Dict
+import typing
 
 property_mapper = {
     'STH51': {
-        'a': 'alarm_status',
+        'a': 'alarmStatus',
         'b': 'temperature',
         'c': 'humidity',
-        'd': 'temperature_unit',
-        'e': 'temperature_range',
-        'f': 'humidity_range',
-        'g': 'alarm_enabled',
-        'h': 'continued_alarm',
+        'd': 'temperatureUnit',
+        'e': 'temperatureRange',
+        'f': 'humidityRange',
+        'g': 'alarmEnabled',
+        'h': 'continuedAlarm',
         't': 'time'
     }
 }
 
+type_mapping = {
+    'batInfo': int,
+    'rfLevel': int,
+    'alarmStatus': lambda x: x == '1',
+    'alarmEnabled': lambda x: x == '1',
+    'muteStatus': lambda x: x == '1',
+    'continuedAlarm': lambda x: x == '1',
+    'coPpm': int,
+    'coLevel': int,
+    'isLifeEnd': lambda x: x == '1',
+    'temperature': float,
+    'humidity': float
+}
+
+
+def map_type(k: str, value: typing.Any):
+    return type_mapping[k](value) if k in type_mapping else value
+
 
-def map_values(device_type: str, data: Dict):
-    if device_type not in property_mapper:
-        return data
+def map_values(device_type: str, data: typing.Dict):
+    mapping = property_mapper[device_type] if device_type in property_mapper else {}
 
-    mapping = property_mapper[device_type]
     return {
-        mapping.get(k, k): v
+        mapping.get(k, k): map_type(mapping.get(k, k), v)
         for k, v in data.items()
     }
```

### Comparing `python-xsense-0.0.4/xsense/station.py` & `python-xsense-0.0.5/xsense/station.py`

 * *Files identical despite different names*

### Comparing `python-xsense-0.0.4/xsense/utils.py` & `python-xsense-0.0.5/xsense/utils.py`

 * *Files identical despite different names*

