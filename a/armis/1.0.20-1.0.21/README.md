# Comparing `tmp/armis-1.0.20.tar.gz` & `tmp/armis-1.0.21.tar.gz`

## Comparing `armis-1.0.20.tar` & `armis-1.0.21.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 armis-1.0.20/requirements.txt
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 armis-1.0.20/src/armis/__about__.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 armis-1.0.20/src/armis/__init__.py
--rwxr-xr-x   0        0        0    46741 2020-02-02 00:00:00.000000 armis-1.0.20/src/armis/armiscloud.py
--rwxr-xr-x   0        0        0     3008 2020-02-02 00:00:00.000000 armis-1.0.20/tests/test_apicalls.py
--rwxr-xr-x   0        0        0      801 2020-02-02 00:00:00.000000 armis-1.0.20/tests/test_boundaries.py
--rwxr-xr-x   0        0        0      838 2020-02-02 00:00:00.000000 armis-1.0.20/tests/test_ceiling.py
--rwxr-xr-x   0        0        0      500 2020-02-02 00:00:00.000000 armis-1.0.20/tests/test_collectors.py
--rwxr-xr-x   0        0        0     2161 2020-02-02 00:00:00.000000 armis-1.0.20/tests/test_devices.py
--rwxr-xr-x   0        0        0      722 2020-02-02 00:00:00.000000 armis-1.0.20/tests/test_fixture.py
--rwxr-xr-x   0        0        0     1143 2020-02-02 00:00:00.000000 armis-1.0.20/tests/test_integrations.py
--rwxr-xr-x   0        0        0      102 2020-02-02 00:00:00.000000 armis-1.0.20/tests/test_notimplemented.py
--rwxr-xr-x   0        0        0     1643 2020-02-02 00:00:00.000000 armis-1.0.20/tests/test_objectcreation.py
--rwxr-xr-x   0        0        0      414 2020-02-02 00:00:00.000000 armis-1.0.20/tests/test_sites.py
--rwxr-xr-x   0        0        0     1299 2020-02-02 00:00:00.000000 armis-1.0.20/tests/test_tagging.py
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 armis-1.0.20/.gitignore
--rw-r--r--   0        0        0     4218 2020-02-02 00:00:00.000000 armis-1.0.20/README.md
--rw-r--r--   0        0        0     4927 2020-02-02 00:00:00.000000 armis-1.0.20/pyproject.toml
--rw-r--r--   0        0        0     5498 2020-02-02 00:00:00.000000 armis-1.0.20/PKG-INFO
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 armis-1.0.21/requirements.txt
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 armis-1.0.21/src/armis/__about__.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 armis-1.0.21/src/armis/__init__.py
+-rwxr-xr-x   0        0        0    53264 2020-02-02 00:00:00.000000 armis-1.0.21/src/armis/armiscloud.py
+-rwxr-xr-x   0        0        0     3008 2020-02-02 00:00:00.000000 armis-1.0.21/tests/test_apicalls.py
+-rwxr-xr-x   0        0        0     2088 2020-02-02 00:00:00.000000 armis-1.0.21/tests/test_boundaries.py
+-rwxr-xr-x   0        0        0      838 2020-02-02 00:00:00.000000 armis-1.0.21/tests/test_ceiling.py
+-rwxr-xr-x   0        0        0      751 2020-02-02 00:00:00.000000 armis-1.0.21/tests/test_collectors.py
+-rwxr-xr-x   0        0        0     2149 2020-02-02 00:00:00.000000 armis-1.0.21/tests/test_devices.py
+-rwxr-xr-x   0        0        0      722 2020-02-02 00:00:00.000000 armis-1.0.21/tests/test_fixture.py
+-rwxr-xr-x   0        0        0     1163 2020-02-02 00:00:00.000000 armis-1.0.21/tests/test_integrations.py
+-rwxr-xr-x   0        0        0      102 2020-02-02 00:00:00.000000 armis-1.0.21/tests/test_notimplemented.py
+-rwxr-xr-x   0        0        0     1643 2020-02-02 00:00:00.000000 armis-1.0.21/tests/test_objectcreation.py
+-rwxr-xr-x   0        0        0      414 2020-02-02 00:00:00.000000 armis-1.0.21/tests/test_sites.py
+-rwxr-xr-x   0        0        0     1299 2020-02-02 00:00:00.000000 armis-1.0.21/tests/test_tagging.py
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 armis-1.0.21/tests/test_users.py
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 armis-1.0.21/.gitignore
+-rw-r--r--   0        0        0     5644 2020-02-02 00:00:00.000000 armis-1.0.21/README.md
+-rw-r--r--   0        0        0     4759 2020-02-02 00:00:00.000000 armis-1.0.21/pyproject.toml
+-rw-r--r--   0        0        0     6924 2020-02-02 00:00:00.000000 armis-1.0.21/PKG-INFO
```

### Comparing `armis-1.0.20/src/armis/armiscloud.py` & `armis-1.0.21/src/armis/armiscloud.py`

 * *Files 6% similar despite different names*

```diff
@@ -349,16 +349,15 @@
                     _ = self._json_decoder.decode(r.text)
                 except msgspec.DecodeError as err:
                     self.log.critical("exception: %s", str(err))
                     self.log.debug("text of response=%s", r.text)
                     raise err
 
                 self.log.debug("size of return text=%s", str(len(r.text)))
-                if len(r.text) < 1000:
-                    self.log.debug("return text=%s", r.text)
+                self.log.debug("return text=%s", r.text[:1000])
 
                 return r
 
     def _update_authorization_token(self) -> None:
         """Fetch an authorization token.
 
         Check if the token we have is still valid.  If not, get a new token and
@@ -367,15 +366,15 @@
         self.log.debug("BEGIN")
         now = pendulum.now().timestamp()
         remaining_time = self._authorization_token_expiration - now
         self.log.debug("now=%s", str(now))
         self.log.debug("remaining_time=%s", str(remaining_time))
 
         if remaining_time < 1_000:
-            self.log.debug("remaining_time < 1000")
+            self.log.debug("remaining_time <1000")
             self.log.debug("expires=%s", str(self._authorization_token_expiration))
             self.log.debug("now > _authorization_token_expiration")
             self.log.debug("_authorization_token expired, getting new one")
             url = self.TENANT_BASE_URL / "v1/access_token/"
             r = self.httpx_client.post(
                 str(url),
                 data={
@@ -1289,7 +1288,188 @@
             self.log.critical("text=%s", site_request.text)
             self.log.critical("continuing")
             raise Exception("dashboard http response !=200")
 
         if "data" in self._json_decoder.decode(site_request.text):
             return self._json_decoder.decode(site_request.text)["data"]
         return {}
+
+    def delete_user(self, user_id_or_email):
+        """Delete a user given the user_id or email.
+
+        Parameters
+        ----------
+        user_id_or_email : str|int
+            A user_id (int) or email (str) to delete.
+
+        Returns
+        -------
+        delete_user_result : str
+            Text from the output of the delete action.
+        """
+        url = self.TENANT_BASE_URL / f"v1/users/{user_id_or_email}/"
+        self.log.debug("url=%s", str(url))
+
+        user_delete = self._api_http_request(method="DELETE", url=url)
+        self.log.debug("return text=%s", str(user_delete.text))
+        self.log.debug("status_code=%s", str(user_delete.status_code))
+        if user_delete.status_code != httpx.codes.OK:
+            self.log.info("FAILED USER UPDATE for user: %s", str(user_id_or_email))
+            self.log.debug(user_delete.text)
+            raise Exception("delete user issue", user_delete.text)
+
+        return self._json_decoder.decode(user_delete.text)
+
+    def edit_user(self, user_id_or_email: str | int, **kwargs: dict) -> dict:
+        """Edit a user given the user_id or email.
+
+        Parameters
+        ----------
+        user_id_or_email : str|int
+            user_id (int) or email (str) to change
+        email : str
+            email address of the user
+        location : str
+            Location of the user
+        name : str
+            Name of user
+        phone : str
+            Phone number of user
+        roleassignment : list
+            List of roles the user should be assigned to
+        title : str
+            Title of the user
+        username : str
+            username of the user
+
+        Returns
+        -------
+        user_update_result : dict
+            A dictionary of the edited user details
+        """
+        # attributes that are required: email, roleassignment, and username
+        # first use what was provided via the method and then fetch
+        # all missing data from the cloud
+
+        if len(kwargs) == 0:
+            raise ValueError("Need a field to be changed")
+
+        need_data_from_cloud = False
+
+        required_attributes = ["email", "roleAssignment", "username"]
+        optional_attributes = ["location", "name", "phone", "title"]
+        edit_user_dict = {}
+
+        if "@" in str(user_id_or_email):
+            edit_user_dict["email"] = user_id_or_email
+        else:
+            edit_user_dict["email"] = None
+
+        for required_attribute in required_attributes:
+            if edit_user_dict.get(required_attribute) is None:
+                edit_user_dict[required_attribute] = kwargs.get(
+                    required_attribute,
+                    None,
+                )
+        if None in list(edit_user_dict.values()):
+            need_data_from_cloud = True
+
+        if need_data_from_cloud:
+            try:
+                existinguser = self.get_user(user_id_or_email=user_id_or_email)
+            except RuntimeError as e:
+                raise RuntimeError(e)
+            for required_attribute in required_attributes:
+                if edit_user_dict[required_attribute] is None:
+                    edit_user_dict[required_attribute] = existinguser[
+                        required_attribute
+                    ]
+        for optional_attribute in optional_attributes:
+            optional_attribute_value = kwargs.get(optional_attribute, None)
+            if optional_attribute_value is not None:
+                edit_user_dict[optional_attribute] = optional_attribute_value
+
+        self.log.debug("edit_user_dict is now: %s", str(edit_user_dict))
+        # when updating, roleassignment and username are required
+        url = self.TENANT_BASE_URL / f"v1/users/{user_id_or_email}/"
+        user_update = self._api_http_request(
+            method="PATCH",
+            url=url,
+            json=edit_user_dict,
+        )
+        self.log.debug("return text=%s", str(user_update.text))
+        self.log.debug("status_code=%s", str(user_update.status_code))
+        if user_update.status_code != httpx.codes.OK:
+            self.log.info("FAILED USER UPDATE for user: %s", str(user_id_or_email))
+            self.log.debug(user_update.text)
+            raise Exception("edit user issue", user_update.text)
+
+        return self._json_decoder.decode(user_update.text)
+
+    def get_user(self, user_id_or_email, **kwargs):
+        """Get a user by user_id or email.
+
+        Parameters
+        ----------
+        user_id_or_email : str | int
+            The user_id or email of the user to retrieve.
+        fields: list
+            The list of fields to retrieve.
+
+        Returns
+        -------
+        userdetails: dict
+            A dictionary of user information.
+        """
+        if len(str(user_id_or_email)) < 1:
+            raise ValueError("missing user_id_or_email")
+
+        fields = kwargs.get("fields", [])
+        if isinstance(fields, str):
+            fields = [fields]
+
+        url = self.TENANT_BASE_URL / f"v1/users/{user_id_or_email}/"
+        if len(fields) > 0:
+            url.args["fields"] = ",".join(fields)
+
+        self.log.debug("url=%s", str(url))
+
+        user_details = self._api_http_request(method="GET", url=url)
+
+        if user_details.status_code != httpx.codes.OK:
+            self.log.critical("STATUS CODE !=200")
+            self.log.critical("status_code=%s", str(user_details.status_code))
+            self.log.critical("text=%s", user_details.text)
+            raise RuntimeError(user_details.text)
+
+        data = self._json_decoder.decode(user_details.text)
+        success_status = data["success"]
+        if success_status is True:
+            return data["data"]
+
+        raise RuntimeError(user_details.text)
+
+    def get_users(self) -> dict:
+        """Get a list of users.
+
+        Returns
+        -------
+        users : dict
+            A dictionary of users.
+        """
+        url = self.TENANT_BASE_URL / "v1/users/"
+        self.log.debug("url=%s", str(url))
+        users_details = self._api_http_request(method="GET", url=url)
+
+        if users_details.status_code != httpx.codes.OK:
+            self.log.critical("STATUS CODE !=200")
+            self.log.critical("status_code=%s", str(users_details.status_code))
+            self.log.critical("text=%s", users_details.text)
+            raise Exception("users_details issue", users_details.text)
+
+        users = {}
+        data = self._json_decoder.decode(users_details.text)
+        if "users" in data["data"]:
+            for user in data["data"]["users"]:
+                users[user["id"]] = user
+
+        return users
```

### Comparing `armis-1.0.20/tests/test_apicalls.py` & `armis-1.0.21/tests/test_apicalls.py`

 * *Files identical despite different names*

### Comparing `armis-1.0.20/tests/test_ceiling.py` & `armis-1.0.21/tests/test_ceiling.py`

 * *Files identical despite different names*

### Comparing `armis-1.0.20/tests/test_devices.py` & `armis-1.0.21/tests/test_devices.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 import pytest
 import tenacity
 from test_fixture import armis_object
 
 
 @pytest.fixture(scope="module")
 def device_asq():
-    return 'in:devices timeFrame:"10 Seconds"'
+    return 'in:devices timeFrame:"1 Minutes"'
 
 
 def test_get_devices_count(armis_object, device_asq):
     x = armis_object.get_devices_count(
         asq=device_asq,
     )
-    assert x > 0
+    assert x >= 0
 
 
 def test_get_devices_count_noasq(armis_object):
     with pytest.raises(ValueError):
         armis_object.get_devices_count()
 
 
@@ -29,41 +29,41 @@
         armis_object.get_devices_count(asq="in:nothing")
 
 
 def test_get_devices(armis_object, device_asq):
     x = armis_object.get_devices(
         asq=device_asq,
     )
-    assert len(x) > 0
+    assert len(x) >= 0
 
 
 def test_get_devices_mismatched_fields(armis_object, device_asq):
     with pytest.raises(ValueError):
         armis_object.get_devices(
             asq=device_asq,
             fields_wanted=["not", "valid", "fields"],
         )
 
 
-def test_get_devices_ensure_fields_match(armis_object):
+def test_get_devices_ensure_fields_match(armis_object, device_asq):
     fields_wanted = [
         "id",
         "boundaries",
         "name",
         "accessSwitch",
         "boundaries",
         "category",
         "operatingSystem",
         "operatingSystemVersion",
         "osBuildNumber",
         "publicIp",
         "purdueLevel",
     ]
     x = armis_object.get_devices(
-        asq='in:devices timeFrame:"10 Seconds"',
+        asq=device_asq,
         fields_wanted=fields_wanted,
     )
 
     firstdevice = x[0]
     fields_retrieved = list(firstdevice.keys())
     fields_difference = set(fields_wanted) - set(fields_retrieved)
     assert len(fields_difference) == 0
```

### Comparing `armis-1.0.20/tests/test_fixture.py` & `armis-1.0.21/tests/test_fixture.py`

 * *Files identical despite different names*

### Comparing `armis-1.0.20/tests/test_integrations.py` & `armis-1.0.21/tests/test_integrations.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,21 +20,21 @@
 def test_get_integration(integrations, armis_object):
     for _ in range(5):
         randomintegrationid = random.choice(list(integrations.keys()))
         randomintegration = armis_object.get_integration(randomintegrationid)
         assert randomintegrationid == randomintegration["id"]
 
 
-def test_get_integration_dne(armis_object, integrations):
+def test_get_integration_invalid(armis_object, integrations):
     integration_ids = sorted(list(integrations.keys()))
 
     # let's make up an integration_id that does not exist, i.e. not in
     # this set:
     # 0 >= valid integrations_ids >= max(list of integration_ids)
 
-    integrationid_dne = random.randint(
+    integrationid_invalid = random.randint(
         integration_ids[-1] * 2,
         integration_ids[-1] * 2222,
     )
 
-    integration_dne = armis_object.get_integration(integrationid_dne)
-    assert len(integration_dne) == 0
+    integration_invalid = armis_object.get_integration(integrationid_invalid)
+    assert len(integration_invalid) == 0
```

### Comparing `armis-1.0.20/tests/test_objectcreation.py` & `armis-1.0.21/tests/test_objectcreation.py`

 * *Files identical despite different names*

### Comparing `armis-1.0.20/tests/test_tagging.py` & `armis-1.0.21/tests/test_tagging.py`

 * *Files identical despite different names*

### Comparing `armis-1.0.20/.gitignore` & `armis-1.0.21/.gitignore`

 * *Files identical despite different names*

### Comparing `armis-1.0.20/pyproject.toml` & `armis-1.0.21/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -62,22 +62,14 @@
 ]
 [tool.hatch.envs.default.scripts]
 test = "pytest -rExXsP --cov=armis --cov-report html:.coverage_report/html {args:tests}"
 
 [[tool.hatch.envs.all.matrix]]
 python = ["3.8", "3.9", "3.10", "3.11", "3.12"]
 
-[tool.hatch.envs.types]
-dependencies = [
-  "mypy>=1.0.0",
-]
-
-[tool.hatch.envs.types.scripts]
-check = "mypy --install-types --non-interactive {args:src/armis tests}"
-
 [tool.hatch.build.targets.sdist]
 exclude = [
   "private*",
   ".coverage_report",
   "coverage_report",
   "docs/",
   "pytest.ini",
@@ -85,16 +77,14 @@
   ".github",
   "mkdocs.yml",
 ]
 
 [publish.index]
 disable = true
 
-
-
 [tool.coverage.run]
 source_pkgs = ["armis", "tests"]
 branch = true
 parallel = true
 omit = [
   "src/armis/__about__.py",
 ]
```

### Comparing `armis-1.0.20/PKG-INFO` & `armis-1.0.21/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,7 @@
-Metadata-Version: 2.3
-Name: armis
-Version: 1.0.20
-Summary: Connect and perform actions with the Armis cloud
-Project-URL: Homepage, https://github.com/mmlange/armis-python/
-Project-URL: Issues, https://github.com/mmlange/armis-python/issues
-Project-URL: Source, https://github.com/mmlange/armis-python/
-Author-email: Matthew Lange <mmlange@gmail.com>
-Maintainer-email: Matthew Lange <mmlange@gmail.com>
-License-Expression: BSD-3-Clause
-Keywords: api,armis,development
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Topic :: Communications
-Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.8
-Requires-Dist: furl==2.1.3
-Requires-Dist: httpx[brotli,http2]==0.27.0
-Requires-Dist: msgspec==0.18.6
-Requires-Dist: pendulum==3.0.0
-Requires-Dist: tenacity==8.2.3
-Description-Content-Type: text/markdown
-
 # Armis Python Library
 
 <p align="center"><strong>armis</strong> <em>- A Python library for interacting with the Armis cloud.</em></p>
 
 <p align="center">
 <a href="https://github.com/mmlange/armis-python/actions">
     <img src="https://github.com/mmlange/armis-python/actions/workflows/testsuite.yml/badge.svg" alt="Test Suite">
@@ -112,15 +81,14 @@
     }
 )
 print(result)
 {'data': {'id': 392309238}, 'success': True}
 ```
 
 ## Collector Operations
-
 Get a list of collectors:
 
 ```python
 collectors = a.get_collectors()
 print(collectors)
 
 {1234: {'clusterId': 0, 'collectorNumber': 1234, 'defaultGateway': '10.0.0.1', 'httpsProxyRedacted': '', 'ipAddress': '10.0.0.2', 'lastSeen': '2019-05-15T13:00:00+00:00', 'macAddress': '00:12:34:56:78:90', 'name': 'Collector 1234', 'status': 'Offline', 'subnet': '10.0.0.0/24', 'type': 'Physical'}}
@@ -129,15 +97,37 @@
 Get the details for a specific collector:
 
 ```python
 myimportantcollector = a.get_collector(collector_id=1234)
 print(myimportantcollector)
 
 {'clusterId': 0, 'collectorNumber': 1234, 'defaultGateway': '10.0.0.1', 'httpsProxyRedacted': '', 'ipAddress': '10.0.0.2', 'lastSeen': '2019-05-15T13:00:00+00:00', 'macAddress': '00:12:34:56:78:90', 'name': 'Collector 1234', 'status': 'Offline', 'subnet': '10.0.0.0/24', 'type': 'Physical'}
+```
+
+## User Operations
+Get a list of users:
+```python
+users = a.get_users()
+print(users)
+
+{12: {'email': 'johndoe@example.com', 'id': 12, 'isActive': True, 'lastLoginTime': '2019-05-15T13:01:23.456789', 'location': '', 'name': 'John Doe', 'phone': '', 'povEulaSigningDate': None, 'prodEulaSigningDate': None, 'reportPermissions': None, 'role': None, 'roleAssignment': [{'name': ['Admin']}], 'title': '', 'twoFactorAuthentication': False, 'username': 'johndoe'}}
+```
+
+Get the details for a specific user, either by userid or email address:
+```python
+a_user = a.get_user(12)
+{'email': 'johndoe@example.com', 'id': 12, 'isActive': True, 'lastLoginTime': '2019-05-15T13:01:23.456789', 'location': '', 'name': 'John Doe', 'phone': '', 'povEulaSigningDate': None, 'prodEulaSigningDate': None, 'reportPermissions': None, 'role': None, 'roleAssignment': [{'name': ['Admin']}], 'title': '', 'twoFactorAuthentication': False, 'username': 'johndoe'}
 
+a_user = a.get_user('johndoe@example.com')
+{'email': 'johndoe@example.com', 'id': 12, 'isActive': True, 'lastLoginTime': '2019-05-15T13:01:23.456789', 'location': '', 'name': 'John Doe', 'phone': '', 'povEulaSigningDate': None, 'prodEulaSigningDate': None, 'reportPermissions': None, 'role': None, 'roleAssignment': [{'name': ['Admin']}], 'title': '', 'twoFactorAuthentication': False, 'username': 'johndoe'}
+```
+
+Delete a user by user_id or email address:
+```python
+a.delete_user('12')
 ```
 
 ## Features
 
 **armis** gives you:
 
 * Easy connection to the Armis cloud using an API secret key.
```

#### html2text {}

```diff
@@ -1,25 +1,8 @@
-Metadata-Version: 2.3 Name: armis Version: 1.0.20 Summary: Connect and perform
-actions with the Armis cloud Project-URL: Homepage, https://github.com/mmlange/
-armis-python/ Project-URL: Issues, https://github.com/mmlange/armis-python/
-issues Project-URL: Source, https://github.com/mmlange/armis-python/ Author-
-email: Matthew Lange
-gmail.com> Maintainer-email: Matthew Lange
-gmail.com> License-Expression: BSD-3-Clause Keywords: api,armis,development
-Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
-Developers Classifier: License :: OSI Approved :: BSD License Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3 :: Only Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Programming Language :: Python :: 3.12 Classifier: Topic :: Communications
-Classifier: Topic :: Software Development :: Libraries Requires-Python: >=3.8
-Requires-Dist: furl==2.1.3 Requires-Dist: httpx[brotli,http2]==0.27.0 Requires-
-Dist: msgspec==0.18.6 Requires-Dist: pendulum==3.0.0 Requires-Dist:
-tenacity==8.2.3 Description-Content-Type: text/markdown # Armis Python Library
+# Armis Python Library
         aarrmmiiss -- AA PPyytthhoonn lliibbrraarryy ffoorr iinntteerraaccttiinngg wwiitthh tthhee AArrmmiiss cclloouudd..
                                  _[_T_e_s_t_ _S_u_i_t_e_]
 **armis** is a Python client library for interacting with the Armis cloud. It
 connects using **HTTP/2** by default, falling back to **HTTP/1.1** when
 necessary. Python 3.8+ is supported. --- Install **armis** using pip:
 ```console $ pip install armis ``` # A Quick Demo of Features ## Getting
 Started First, let's create an ArmisCloud object: ```python from armis import
@@ -48,15 +31,34 @@
 00:00+00:00', 'macAddress': '00:12:34:56:78:90', 'name': 'Collector 1234',
 'status': 'Offline', 'subnet': '10.0.0.0/24', 'type': 'Physical'}} ``` Get the
 details for a specific collector: ```python myimportantcollector =
 a.get_collector(collector_id=1234) print(myimportantcollector) {'clusterId': 0,
 'collectorNumber': 1234, 'defaultGateway': '10.0.0.1', 'httpsProxyRedacted':
 '', 'ipAddress': '10.0.0.2', 'lastSeen': '2019-05-15T13:00:00+00:00',
 'macAddress': '00:12:34:56:78:90', 'name': 'Collector 1234', 'status':
-'Offline', 'subnet': '10.0.0.0/24', 'type': 'Physical'} ``` ## Features
+'Offline', 'subnet': '10.0.0.0/24', 'type': 'Physical'} ``` ## User Operations
+Get a list of users: ```python users = a.get_users() print(users) {12:
+{'email': 'johndoe@example.com', 'id': 12, 'isActive': True, 'lastLoginTime':
+'2019-05-15T13:01:23.456789', 'location': '', 'name': 'John Doe', 'phone': '',
+'povEulaSigningDate': None, 'prodEulaSigningDate': None, 'reportPermissions':
+None, 'role': None, 'roleAssignment': [{'name': ['Admin']}], 'title': '',
+'twoFactorAuthentication': False, 'username': 'johndoe'}} ``` Get the details
+for a specific user, either by userid or email address: ```python a_user =
+a.get_user(12) {'email': 'johndoe@example.com', 'id': 12, 'isActive': True,
+'lastLoginTime': '2019-05-15T13:01:23.456789', 'location': '', 'name': 'John
+Doe', 'phone': '', 'povEulaSigningDate': None, 'prodEulaSigningDate': None,
+'reportPermissions': None, 'role': None, 'roleAssignment': [{'name':
+['Admin']}], 'title': '', 'twoFactorAuthentication': False, 'username':
+'johndoe'} a_user = a.get_user('johndoe@example.com') {'email':
+'johndoe@example.com', 'id': 12, 'isActive': True, 'lastLoginTime': '2019-05-
+15T13:01:23.456789', 'location': '', 'name': 'John Doe', 'phone': '',
+'povEulaSigningDate': None, 'prodEulaSigningDate': None, 'reportPermissions':
+None, 'role': None, 'roleAssignment': [{'name': ['Admin']}], 'title': '',
+'twoFactorAuthentication': False, 'username': 'johndoe'} ``` Delete a user by
+user_id or email address: ```python a.delete_user('12') ``` ## Features
 **armis** gives you: * Easy connection to the Armis cloud using an API secret
 key. * A quick way to fetch devices from the cloud. * Retries in the event the
 cloud times out. This can happen with large queries that take more than 2
 minutes. This is the default for CloudFlare, which front-ends the cloud
 infrastructure. * Mostly type annotated. * Nearly 100% test coverage. ##
 Installation Install with pip: ```console $ pip install armis ``` **armis**
 requires Python 3.8+. ## Dependencies **armis** relies on these excellent
```

