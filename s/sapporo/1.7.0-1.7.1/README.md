# Comparing `tmp/sapporo-1.7.0.tar.gz` & `tmp/sapporo-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sapporo-1.7.0.tar", last modified: Mon Apr  8 05:40:48 2024, max compression
+gzip compressed data, was "sapporo-1.7.1.tar", last modified: Fri Apr 26 09:06:02 2024, max compression
```

## Comparing `sapporo-1.7.0.tar` & `sapporo-1.7.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:40:47.998450 sapporo-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11388 2024-04-08 05:40:40.000000 sapporo-1.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-08 05:40:40.000000 sapporo-1.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    19474 2024-04-08 05:40:47.998450 sapporo-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17459 2024-04-08 05:40:40.000000 sapporo-1.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:40:47.994450 sapporo-1.7.0/sapporo/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-08 05:40:40.000000 sapporo-1.7.0/sapporo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-04-08 05:40:40.000000 sapporo-1.7.0/sapporo/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-08 05:40:40.000000 sapporo-1.7.0/sapporo/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-08 05:40:40.000000 sapporo-1.7.0/sapporo/auth_config.json
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-08 05:40:40.000000 sapporo-1.7.0/sapporo/auth_config.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     7483 2024-04-08 05:40:40.000000 sapporo-1.7.0/sapporo/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-08 05:40:40.000000 sapporo-1.7.0/sapporo/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     6579 2024-04-08 05:40:40.000000 sapporo-1.7.0/sapporo/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-08 05:40:40.000000 sapporo-1.7.0/sapporo/executable_workflows.json
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-08 05:40:40.000000 sapporo-1.7.0/sapporo/executable_workflows.schema.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:40:47.994450 sapporo-1.7.0/sapporo/model/
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-08 05:40:40.000000 sapporo-1.7.0/sapporo/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-04-08 05:40:40.000000 sapporo-1.7.0/sapporo/model/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-08 05:40:40.000000 sapporo-1.7.0/sapporo/model/sapporo_wes_1_0_1.py
--rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-04-08 05:40:40.000000 sapporo-1.7.0/sapporo/model/sapporo_wes_1_1_0.py
--rw-r--r--   0 runner    (1001) docker     (127)     6135 2024-04-08 05:40:40.000000 sapporo-1.7.0/sapporo/parser.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    23577 2024-04-08 05:40:40.000000 sapporo-1.7.0/sapporo/ro_crate.py
--rw-r--r--   0 runner    (1001) docker     (127)    12627 2024-04-08 05:40:40.000000 sapporo-1.7.0/sapporo/run.py
--rw-r--r--   0 runner    (1001) docker     (127)    11354 2024-04-08 05:40:40.000000 sapporo-1.7.0/sapporo/run.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-08 05:40:40.000000 sapporo-1.7.0/sapporo/service-info.json
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-04-08 05:40:40.000000 sapporo-1.7.0/sapporo/service-info.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-04-08 05:40:40.000000 sapporo-1.7.0/sapporo/trs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11012 2024-04-08 05:40:40.000000 sapporo-1.7.0/sapporo/validator.py
--rw-r--r--   0 runner    (1001) docker     (127)    36137 2024-04-08 05:40:40.000000 sapporo-1.7.0/sapporo-wes-1-1-0-openapi-spec.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:40:47.998450 sapporo-1.7.0/sapporo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19474 2024-04-08 05:40:47.000000 sapporo-1.7.0/sapporo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-08 05:40:47.000000 sapporo-1.7.0/sapporo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 05:40:47.000000 sapporo-1.7.0/sapporo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-08 05:40:47.000000 sapporo-1.7.0/sapporo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-08 05:40:47.000000 sapporo-1.7.0/sapporo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-08 05:40:47.000000 sapporo-1.7.0/sapporo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 05:40:47.998450 sapporo-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-04-08 05:40:40.000000 sapporo-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:06:02.618016 sapporo-1.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11388 2024-04-26 09:05:51.000000 sapporo-1.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-26 09:05:51.000000 sapporo-1.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    18479 2024-04-26 09:06:02.614016 sapporo-1.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16436 2024-04-26 09:05:51.000000 sapporo-1.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:06:02.614016 sapporo-1.7.1/sapporo/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-26 09:05:51.000000 sapporo-1.7.1/sapporo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-04-26 09:05:51.000000 sapporo-1.7.1/sapporo/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-04-26 09:05:51.000000 sapporo-1.7.1/sapporo/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-26 09:05:51.000000 sapporo-1.7.1/sapporo/auth_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-04-26 09:05:51.000000 sapporo-1.7.1/sapporo/auth_config.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7515 2024-04-26 09:05:51.000000 sapporo-1.7.1/sapporo/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-26 09:05:51.000000 sapporo-1.7.1/sapporo/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6535 2024-04-26 09:05:51.000000 sapporo-1.7.1/sapporo/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-26 09:05:51.000000 sapporo-1.7.1/sapporo/executable_workflows.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-26 09:05:51.000000 sapporo-1.7.1/sapporo/executable_workflows.schema.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:06:02.614016 sapporo-1.7.1/sapporo/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-26 09:05:51.000000 sapporo-1.7.1/sapporo/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-04-26 09:05:51.000000 sapporo-1.7.1/sapporo/model/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-26 09:05:51.000000 sapporo-1.7.1/sapporo/model/sapporo_wes_1_0_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-04-26 09:05:51.000000 sapporo-1.7.1/sapporo/model/sapporo_wes_1_1_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6135 2024-04-26 09:05:51.000000 sapporo-1.7.1/sapporo/parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23577 2024-04-26 09:05:51.000000 sapporo-1.7.1/sapporo/ro_crate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12627 2024-04-26 09:05:51.000000 sapporo-1.7.1/sapporo/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11354 2024-04-26 09:05:51.000000 sapporo-1.7.1/sapporo/run.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-26 09:05:51.000000 sapporo-1.7.1/sapporo/service-info.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-04-26 09:05:51.000000 sapporo-1.7.1/sapporo/service-info.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-04-26 09:05:51.000000 sapporo-1.7.1/sapporo/trs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11012 2024-04-26 09:05:51.000000 sapporo-1.7.1/sapporo/validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36137 2024-04-26 09:05:51.000000 sapporo-1.7.1/sapporo-wes-1-1-0-openapi-spec.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:06:02.614016 sapporo-1.7.1/sapporo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18479 2024-04-26 09:06:02.000000 sapporo-1.7.1/sapporo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-26 09:06:02.000000 sapporo-1.7.1/sapporo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 09:06:02.000000 sapporo-1.7.1/sapporo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-26 09:06:02.000000 sapporo-1.7.1/sapporo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-26 09:06:02.000000 sapporo-1.7.1/sapporo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-26 09:06:02.000000 sapporo-1.7.1/sapporo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 09:06:02.618016 sapporo-1.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-04-26 09:05:51.000000 sapporo-1.7.1/setup.py
```

### Comparing `sapporo-1.7.0/LICENSE` & `sapporo-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sapporo-1.7.0/PKG-INFO` & `sapporo-1.7.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sapporo
-Version: 1.7.0
+Version: 1.7.1
 Summary: The sapporo-service is a standard implementation conforming to the Global Alliance for Genomics and Health (GA4GH) Workflow Execution Service (WES) API specification.
 Home-page: https://github.com/sapporo-wes/sapporo-service
 Author: DDBJ(Bioinformatics and DDBJ Center)
 Author-email: tazro.ohta@chiba-u.jp
 License: Apache2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,14 +20,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: cryptography
 Requires-Dist: cwl-inputs-parser>=1.0.2
 Requires-Dist: flask_jwt_extended
 Requires-Dist: flask-cors
 Requires-Dist: flask
 Requires-Dist: jsonschema
 Requires-Dist: multiqc
 Requires-Dist: psutil
@@ -265,164 +266,126 @@
 $ docker run --rm -v /var/run/docker.sock:/var/run/docker.sock -v $PWD:$PWD -w $PWD ghcr.io/sapporo-wes/sapporo-service:latest python3 /app/sapporo/ro_crate.py $PWD
 ```
 
 For more information on RO-Crate, please also refer to [`./tests/ro-crate`](./tests/ro-crate).
 
 ### Authentication
 
-The sapporo-service supports authentication using JWT.
-The configuration for this authentication is managed through [`./sapporo/auth_config.json`](./sapporo/auth_config.json) file.
-By default, the file is set up as follows:
+The sapporo-service supports authentication, configurable via the [`./sapporo/auth_config.json`](./sapporo/auth_config.json).
+By default, this configuration is as follows:
 
 ```json
 {
   "auth_enabled": false,
-  "jwt_secret_key": "spr_secret_key_please_change_this",
-  "users": [
-    {
-      "username": "spr_test_user",
-      "password": "spr_test_password"
-    }
-  ]
+  "auth_provider": "local",
+  "local_auth": {
+    "jwt_secret_key": "spr_secret_key_please_change_this",
+    "users": [
+      {
+        "username": "spr_test_user",
+        "password": "spr_test_password"
+      }
+    ]
+  },
+  "oidc_auth": {
+    "realm_url": "http://localhost:8080/realms/sapporo-dev",
+    "username_claim": "sub"
+  }
 }
 ```
 
-You can edit this file directly, or, you can change its location using the startup argument `--auth-config` or the environment variable `SAPPORO_AUTH_CONFIG`.
+This configuration file can be directly edited or relocated using the `--auth-config` startup argument or the `SAPPORO_AUTH_CONFIG` environment variable.
 
-The file contains the following fields:
+#### Configuration Fields
 
-- `auth_enabled`: Determines whether JWT authentication is enabled. If set to `true`, JWT authentication is activated.
-- `jwt_secret_key`: The secret key used for signing the JWT. It is strongly recommended to change this value.
-- `users`: A list of users who will perform JWT authentication. Specify `username` and `password`.
+- `auth_enabled`: Determines if JWT authentication is activated. If set to `true`, JWT authentication is enabled.
+- `auth_provider`: Specifies the type of authentication provider, supporting:
+  - `local`: Uses a locally managed list of users for authentication.
+    - Tokens are issued by Sapporo.
+    - Usernames and passwords are referenced from the `auth_config.json`.
+  - `oidc`: Uses an OpenID Connect (OIDC) provider like [Keycloak](https://www.keycloak.org).
+    - Tokens are issued by the OIDC provider.
+    - User information is managed by the OIDC provider.
+- `local_auth`: Configuration for local authentication includes:
+  - `jwt_secret_key`: Secret key for signing JWTs. Changing this key is highly recommended.
+  - `users`: List of users eligible for JWT authentication, specifying username and password.
+- `oidc_auth`: Configuration for OIDC authentication includes:
+  - `realm_url`: URL of the OIDC realm.
+  - `username_claim`: JWT claim used as the username.
 
-When JWT authentication is enabled, the following endpoints require authentication:
+#### Authentication Endpoints
+
+When JWT authentication is enabled, endpoints requiring authentication include:
 
 - `GET /runs`
 - `POST /runs`
 - `GET /runs/{run_id}`
 - `POST /runs/{run_id}/cancel`
 - `GET /runs/{run_id}/status`
 - `GET /runs/{run_id}/data`
 
-Additionally, each run is associated with a `username`, so that, for example, only the user who created the run can access `GET /runs/{run_id}`.
+Each run is associated with a `username`, ensuring that only the user who created a run can access details like `GET /runs/{run_id}`.
+
+#### Local Authentication
 
-Let's take a look at how to use JWT authentication.
-First, edit the `auth-config.json` as follows:
+For local JWT authentication, configure `auth_config.json` as shown:
 
 ```json
 {
   "auth_enabled": true,
-  "jwt_secret_key": "spr_secret_key_please_change_this",
-  "users": [
-    {
-      "username": "spr_test_user1",
-      "password": "spr_test_password1"
-    },
-    {
-      "username": "spr_test_user2",
-      "password": "spr_test_password2"
-    }
-  ]
+  "auth_provider": "local",
+  "local_auth": {
+    "jwt_secret_key": "new_secret_key",
+    "users": [
+      {
+        "username": "user1",
+        "password": "password1"
+      },
+      {
+        "username": "user2",
+        "password": "password2"
+      }
+    ]
+  },
+  "oidc_auth": {
+    "realm_url": "http://localhost:8080/realms/sapporo-dev",
+    "username_claim": "sub"
+  }
 }
 ```
 
-With this configuration, if you start the sapporo-service, `GET /service-info` will return a result, but `GET /runs` will require authentication.
+Starting sapporo-service with this configuration allows access to the `GET /service-info` endpoint, while `GET /runs` will require authentication:
 
 ```bash
 # Start sapporo-service
 $ sapporo
 
 # GET /service-info
 $ curl -X GET localhost:1122/service-info
 {
   "auth_instructions_url": "https://github.com/sapporo-wes/sapporo-service",
   "contact_info_url": "https://github.com/sapporo-wes/sapporo-service",
 ...
 
-# GET /runs
-$ curl -X GET localhost:1122/runs
-{
-  "msg": "Missing Authorization Header",
-  "status": 401
-}
-```
-
-Here, you can generate a JWT required for authentication by sending a `POST /auth` request with `username` and `password` as follows:
-
-```bash
-$ curl -X POST \
+# Generate JWT for authentication
+$ TOKEN=$(curl -s -X POST \
     -H "Content-Type: application/json" \
-    -d '{"username":"spr_test_user1", "password":"spr_test_password1"}' \
-    localhost:1122/auth
-{
-  "access_token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJmcmVzaCI6ZmFsc2UsImlhdCI6MTcwNjQyODY2MCwianRpIjoiY2I5ZTU1MDgtN2RlNy00Y2EzLWE4NjYtN2ZlYmRmYTg4YWQ0IiwidHlwZSI6ImFjY2VzcyIsInN1YiI6InNwcl90ZXN0X3VzZXIxIiwibmJmIjoxNzA2NDI4NjYwLCJjc3JmIjoiZjdlZjNhZmYtMTVlZS00OTc2LTkxYzYtOTU2ZDZjZTVjYmQ5IiwiZXhwIjoxNzA2NDI5NTYwfQ.zyD7Ru72eD_9mJj548DS-qDk8Y5yan-rNbklWmfvcEs"
-}
-```
-
-If you attach this generated JWT to the Authorization header and send it to `GET /runs`, the authentication will pass.
-
-```bash
-$ TOKEN1=$(curl -s -X POST \
-    -H "Content-Type: application/json" \
-    -d '{"username":"spr_test_user1", "password":"spr_test_password1"}' \
+    -d '{"username":"user1", "password":"password1"}' \
     localhost:1122/auth | jq -r '.access_token')
 
-$ curl -X GET -H "Authorization: Bearer $TOKEN1" localhost:1122/runs
+# Authenticate and access runs
+$ curl -X GET -H "Authorization: Bearer $TOKEN" localhost:1122/runs
 {
   "runs": []
 }
 ```
 
-Let's also confirm that User2 cannot access the run executed by User1.
-
-```bash
-$ TOKEN1=$(curl -s -X POST \
-    -H "Content-Type: application/json" \
-    -d '{"username":"spr_test_user1", "password":"spr_test_password1"}' \
-    localhost:1122/auth | jq -r '.access_token')
-$ TOKEN2=$(curl -s -X POST \
-    -H "Content-Type: application/json" \
-    -d '{"username":"spr_test_user2", "password":"spr_test_password2"}' \
-    localhost:1122/auth | jq -r '.access_token')
-
-# Execute a run with User1
-# Please refer to ./tests/curl_example/cwltool_remote_workflow.sh for example
-# Run ID: af95fd09-8406-4f2c-9280-bca900e07289
+#### OpenID Connect (OIDC) Authentication
 
-# GET /runs with User1
-$ curl -X GET -H "Authorization: Bearer $TOKEN1" localhost:1122/runs
-{
-  "runs": [
-    {
-      "run_id": "af95fd09-8406-4f2c-9280-bca900e07289",
-      "state": "COMPLETE"
-    }
-  ]
-}
-
-# GET /runs/{run_id} with User1
-$ curl -X GET -H "Authorization: Bearer $TOKEN1" localhost:1122/runs/af95fd09-8406-4f2c-9280-bca900e07289
-{
-  "outputs": [
-    {
-      ...
-
-# GET /runs with User2
-$ curl -X GET -H "Authorization: Bearer $TOKEN2" localhost:1122/runs
-{
-  "runs": []
-}
-
-# GET /runs/{run_id} with User2
-$ curl -X GET -H "Authorization: Bearer $TOKEN2" localhost:1122/runs/af95fd09-8406-4f2c-9280-bca900e07289
-{
-  "msg": "You don't have permission to access this run.",
-  "status_code": 403
-}
-```
+For OIDC authentication, ensure the `auth_provider` is set to `oidc` and appropriate configurations are specified under `oidc_auth`. Users must obtain a token from the OIDC provider and attach it to the Authorization header for authentication.
 
 ## Development
 
 To start the development environment, follow these steps:
 
 ```bash
 $ docker compose -f compose.dev.yml up -d --build
```

### Comparing `sapporo-1.7.0/README.md` & `sapporo-1.7.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -215,164 +215,126 @@
 $ docker run --rm -v /var/run/docker.sock:/var/run/docker.sock -v $PWD:$PWD -w $PWD ghcr.io/sapporo-wes/sapporo-service:latest python3 /app/sapporo/ro_crate.py $PWD
 ```
 
 For more information on RO-Crate, please also refer to [`./tests/ro-crate`](./tests/ro-crate).
 
 ### Authentication
 
-The sapporo-service supports authentication using JWT.
-The configuration for this authentication is managed through [`./sapporo/auth_config.json`](./sapporo/auth_config.json) file.
-By default, the file is set up as follows:
+The sapporo-service supports authentication, configurable via the [`./sapporo/auth_config.json`](./sapporo/auth_config.json).
+By default, this configuration is as follows:
 
 ```json
 {
   "auth_enabled": false,
-  "jwt_secret_key": "spr_secret_key_please_change_this",
-  "users": [
-    {
-      "username": "spr_test_user",
-      "password": "spr_test_password"
-    }
-  ]
+  "auth_provider": "local",
+  "local_auth": {
+    "jwt_secret_key": "spr_secret_key_please_change_this",
+    "users": [
+      {
+        "username": "spr_test_user",
+        "password": "spr_test_password"
+      }
+    ]
+  },
+  "oidc_auth": {
+    "realm_url": "http://localhost:8080/realms/sapporo-dev",
+    "username_claim": "sub"
+  }
 }
 ```
 
-You can edit this file directly, or, you can change its location using the startup argument `--auth-config` or the environment variable `SAPPORO_AUTH_CONFIG`.
+This configuration file can be directly edited or relocated using the `--auth-config` startup argument or the `SAPPORO_AUTH_CONFIG` environment variable.
+
+#### Configuration Fields
+
+- `auth_enabled`: Determines if JWT authentication is activated. If set to `true`, JWT authentication is enabled.
+- `auth_provider`: Specifies the type of authentication provider, supporting:
+  - `local`: Uses a locally managed list of users for authentication.
+    - Tokens are issued by Sapporo.
+    - Usernames and passwords are referenced from the `auth_config.json`.
+  - `oidc`: Uses an OpenID Connect (OIDC) provider like [Keycloak](https://www.keycloak.org).
+    - Tokens are issued by the OIDC provider.
+    - User information is managed by the OIDC provider.
+- `local_auth`: Configuration for local authentication includes:
+  - `jwt_secret_key`: Secret key for signing JWTs. Changing this key is highly recommended.
+  - `users`: List of users eligible for JWT authentication, specifying username and password.
+- `oidc_auth`: Configuration for OIDC authentication includes:
+  - `realm_url`: URL of the OIDC realm.
+  - `username_claim`: JWT claim used as the username.
 
-The file contains the following fields:
+#### Authentication Endpoints
 
-- `auth_enabled`: Determines whether JWT authentication is enabled. If set to `true`, JWT authentication is activated.
-- `jwt_secret_key`: The secret key used for signing the JWT. It is strongly recommended to change this value.
-- `users`: A list of users who will perform JWT authentication. Specify `username` and `password`.
-
-When JWT authentication is enabled, the following endpoints require authentication:
+When JWT authentication is enabled, endpoints requiring authentication include:
 
 - `GET /runs`
 - `POST /runs`
 - `GET /runs/{run_id}`
 - `POST /runs/{run_id}/cancel`
 - `GET /runs/{run_id}/status`
 - `GET /runs/{run_id}/data`
 
-Additionally, each run is associated with a `username`, so that, for example, only the user who created the run can access `GET /runs/{run_id}`.
+Each run is associated with a `username`, ensuring that only the user who created a run can access details like `GET /runs/{run_id}`.
+
+#### Local Authentication
 
-Let's take a look at how to use JWT authentication.
-First, edit the `auth-config.json` as follows:
+For local JWT authentication, configure `auth_config.json` as shown:
 
 ```json
 {
   "auth_enabled": true,
-  "jwt_secret_key": "spr_secret_key_please_change_this",
-  "users": [
-    {
-      "username": "spr_test_user1",
-      "password": "spr_test_password1"
-    },
-    {
-      "username": "spr_test_user2",
-      "password": "spr_test_password2"
-    }
-  ]
+  "auth_provider": "local",
+  "local_auth": {
+    "jwt_secret_key": "new_secret_key",
+    "users": [
+      {
+        "username": "user1",
+        "password": "password1"
+      },
+      {
+        "username": "user2",
+        "password": "password2"
+      }
+    ]
+  },
+  "oidc_auth": {
+    "realm_url": "http://localhost:8080/realms/sapporo-dev",
+    "username_claim": "sub"
+  }
 }
 ```
 
-With this configuration, if you start the sapporo-service, `GET /service-info` will return a result, but `GET /runs` will require authentication.
+Starting sapporo-service with this configuration allows access to the `GET /service-info` endpoint, while `GET /runs` will require authentication:
 
 ```bash
 # Start sapporo-service
 $ sapporo
 
 # GET /service-info
 $ curl -X GET localhost:1122/service-info
 {
   "auth_instructions_url": "https://github.com/sapporo-wes/sapporo-service",
   "contact_info_url": "https://github.com/sapporo-wes/sapporo-service",
 ...
 
-# GET /runs
-$ curl -X GET localhost:1122/runs
-{
-  "msg": "Missing Authorization Header",
-  "status": 401
-}
-```
-
-Here, you can generate a JWT required for authentication by sending a `POST /auth` request with `username` and `password` as follows:
-
-```bash
-$ curl -X POST \
+# Generate JWT for authentication
+$ TOKEN=$(curl -s -X POST \
     -H "Content-Type: application/json" \
-    -d '{"username":"spr_test_user1", "password":"spr_test_password1"}' \
-    localhost:1122/auth
-{
-  "access_token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJmcmVzaCI6ZmFsc2UsImlhdCI6MTcwNjQyODY2MCwianRpIjoiY2I5ZTU1MDgtN2RlNy00Y2EzLWE4NjYtN2ZlYmRmYTg4YWQ0IiwidHlwZSI6ImFjY2VzcyIsInN1YiI6InNwcl90ZXN0X3VzZXIxIiwibmJmIjoxNzA2NDI4NjYwLCJjc3JmIjoiZjdlZjNhZmYtMTVlZS00OTc2LTkxYzYtOTU2ZDZjZTVjYmQ5IiwiZXhwIjoxNzA2NDI5NTYwfQ.zyD7Ru72eD_9mJj548DS-qDk8Y5yan-rNbklWmfvcEs"
-}
-```
-
-If you attach this generated JWT to the Authorization header and send it to `GET /runs`, the authentication will pass.
-
-```bash
-$ TOKEN1=$(curl -s -X POST \
-    -H "Content-Type: application/json" \
-    -d '{"username":"spr_test_user1", "password":"spr_test_password1"}' \
+    -d '{"username":"user1", "password":"password1"}' \
     localhost:1122/auth | jq -r '.access_token')
 
-$ curl -X GET -H "Authorization: Bearer $TOKEN1" localhost:1122/runs
+# Authenticate and access runs
+$ curl -X GET -H "Authorization: Bearer $TOKEN" localhost:1122/runs
 {
   "runs": []
 }
 ```
 
-Let's also confirm that User2 cannot access the run executed by User1.
-
-```bash
-$ TOKEN1=$(curl -s -X POST \
-    -H "Content-Type: application/json" \
-    -d '{"username":"spr_test_user1", "password":"spr_test_password1"}' \
-    localhost:1122/auth | jq -r '.access_token')
-$ TOKEN2=$(curl -s -X POST \
-    -H "Content-Type: application/json" \
-    -d '{"username":"spr_test_user2", "password":"spr_test_password2"}' \
-    localhost:1122/auth | jq -r '.access_token')
-
-# Execute a run with User1
-# Please refer to ./tests/curl_example/cwltool_remote_workflow.sh for example
-# Run ID: af95fd09-8406-4f2c-9280-bca900e07289
+#### OpenID Connect (OIDC) Authentication
 
-# GET /runs with User1
-$ curl -X GET -H "Authorization: Bearer $TOKEN1" localhost:1122/runs
-{
-  "runs": [
-    {
-      "run_id": "af95fd09-8406-4f2c-9280-bca900e07289",
-      "state": "COMPLETE"
-    }
-  ]
-}
-
-# GET /runs/{run_id} with User1
-$ curl -X GET -H "Authorization: Bearer $TOKEN1" localhost:1122/runs/af95fd09-8406-4f2c-9280-bca900e07289
-{
-  "outputs": [
-    {
-      ...
-
-# GET /runs with User2
-$ curl -X GET -H "Authorization: Bearer $TOKEN2" localhost:1122/runs
-{
-  "runs": []
-}
-
-# GET /runs/{run_id} with User2
-$ curl -X GET -H "Authorization: Bearer $TOKEN2" localhost:1122/runs/af95fd09-8406-4f2c-9280-bca900e07289
-{
-  "msg": "You don't have permission to access this run.",
-  "status_code": 403
-}
-```
+For OIDC authentication, ensure the `auth_provider` is set to `oidc` and appropriate configurations are specified under `oidc_auth`. Users must obtain a token from the OIDC provider and attach it to the Authorization header for authentication.
 
 ## Development
 
 To start the development environment, follow these steps:
 
 ```bash
 $ docker compose -f compose.dev.yml up -d --build
```

### Comparing `sapporo-1.7.0/sapporo/app.py` & `sapporo-1.7.1/sapporo/app.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import sys
 from traceback import format_exc
 
 from flask import Flask, Response, current_app, jsonify
 from flask_cors import CORS
 from werkzeug.exceptions import HTTPException
 
-from sapporo.auth import apply_jwt_manager
+from sapporo.auth import apply_jwt_manager, generate_jwt_public_key
 from sapporo.config import Config, get_config, parse_args, validate_config
 from sapporo.controller import app_bp
 from sapporo.model import ErrorResponse
 
 
 def fix_errorhandler(app: Flask) -> Flask:
     @app.errorhandler(HTTPException)
@@ -47,32 +47,43 @@
     app = Flask(__name__)
     app.register_blueprint(app_bp, url_prefix=config["url_prefix"])
     fix_errorhandler(app)
     CORS(app, resources={r"/*": {"origins": config["access_control_allow_origin"]}})
     with config["auth_config"].open(mode="r", encoding="utf-8") as f:
         auth_config = json.load(f)
         auth_enabled = auth_config["auth_enabled"]
-        jwt_secret_key = auth_config["jwt_secret_key"]
-        auth_users = auth_config["users"]
+        auth_provider = auth_config["auth_provider"]
+
     if auth_enabled:
+        if auth_provider == "local":
+            app.config.update({
+                "JWT_SECRET_KEY": auth_config["local_auth"]["jwt_secret_key"],
+                "AUTH_USERS": auth_config["local_auth"]["users"],
+            })
+        elif auth_provider == "oidc":
+            JWT_ALGORITHM = "RS256"
+            jwt_public_key = generate_jwt_public_key(auth_config["oidc_auth"]["realm_url"], JWT_ALGORITHM)
+            app.config.update({
+                "JWT_ALGORITHM": JWT_ALGORITHM,
+                "JWT_PUBLIC_KEY": jwt_public_key,
+                "JWT_IDENTITY_CLAIM": auth_config["oidc_auth"]["username_claim"],
+            })
         apply_jwt_manager(app)
 
     app.config.update({
         "RUN_DIR": config["run_dir"],
         "SAPPORO_VERSION": config["sapporo_version"],
         "GET_RUNS": config["get_runs"],
         "WORKFLOW_ATTACHMENT": config["workflow_attachment"],
         "REGISTERED_ONLY_MODE": config["registered_only_mode"],
         "SERVICE_INFO": config["service_info"],
         "EXECUTABLE_WORKFLOWS": config["executable_workflows"],
         "RUN_SH": config["run_sh"],
         "URL_PREFIX": config["url_prefix"],
         "AUTH_ENABLED": auth_enabled,
-        "JWT_SECRET_KEY": jwt_secret_key,
-        "AUTH_USERS": auth_users,
         "FLASK_ENV": "development" if config["debug"] else "production",
         "DEBUG": config["debug"],
         "TESTING": config["debug"],
     })
     if config["debug"]:
         app.logger.debug("config: %s", config)
```

### Comparing `sapporo-1.7.0/sapporo/config.py` & `sapporo-1.7.1/sapporo/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     disable_get_runs: bool
     disable_workflow_attachment: bool
     run_only_registered_workflows: bool
     service_info: Optional[Path]
     executable_workflows: Optional[Path]
     run_sh: Optional[Path]
     url_prefix: Optional[str]
+    auth_config: Optional[Path]
 
 
 def parse_args(args: Optional[List[str]] = None) -> TypedNamespace:
     parser: ArgumentParser = argparse.ArgumentParser(
         description="This is an implementation of a GA4GH workflow execution service that can easily support various workflow runners.")
 
     parser.add_argument(
```

### Comparing `sapporo-1.7.0/sapporo/const.py` & `sapporo-1.7.1/sapporo/const.py`

 * *Files identical despite different names*

### Comparing `sapporo-1.7.0/sapporo/controller.py` & `sapporo-1.7.1/sapporo/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 def post_auth() -> Response:
     username = request.json.get("username", None)
     password = request.json.get("password", None)
     if username is None or password is None:
         abort(401, "username and password are required.")
 
     auth = False
-    print(current_app.config["AUTH_USERS"])
     for user in current_app.config["AUTH_USERS"]:
         if user["username"] == username and user["password"] == password:
             auth = True
             break
     if not auth:
         abort(401, "username or password is invalid.")
```

### Comparing `sapporo-1.7.0/sapporo/executable_workflows.json` & `sapporo-1.7.1/sapporo/executable_workflows.json`

 * *Files identical despite different names*

### Comparing `sapporo-1.7.0/sapporo/executable_workflows.schema.json` & `sapporo-1.7.1/sapporo/executable_workflows.schema.json`

 * *Files identical despite different names*

### Comparing `sapporo-1.7.0/sapporo/model/__init__.py` & `sapporo-1.7.1/sapporo/model/__init__.py`

 * *Files identical despite different names*

### Comparing `sapporo-1.7.0/sapporo/model/factory.py` & `sapporo-1.7.1/sapporo/model/factory.py`

 * *Files identical despite different names*

### Comparing `sapporo-1.7.0/sapporo/model/sapporo_wes_1_0_1.py` & `sapporo-1.7.1/sapporo/model/sapporo_wes_1_0_1.py`

 * *Files identical despite different names*

### Comparing `sapporo-1.7.0/sapporo/model/sapporo_wes_1_1_0.py` & `sapporo-1.7.1/sapporo/model/sapporo_wes_1_1_0.py`

 * *Files identical despite different names*

### Comparing `sapporo-1.7.0/sapporo/parser.py` & `sapporo-1.7.1/sapporo/parser.py`

 * *Files identical despite different names*

### Comparing `sapporo-1.7.0/sapporo/ro_crate.py` & `sapporo-1.7.1/sapporo/ro_crate.py`

 * *Files identical despite different names*

### Comparing `sapporo-1.7.0/sapporo/run.py` & `sapporo-1.7.1/sapporo/run.py`

 * *Files identical despite different names*

### Comparing `sapporo-1.7.0/sapporo/run.sh` & `sapporo-1.7.1/sapporo/run.sh`

 * *Files identical despite different names*

### Comparing `sapporo-1.7.0/sapporo/service-info.json` & `sapporo-1.7.1/sapporo/service-info.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9880952380952381%*

 * *Differences: {"'tags'": "{'sapporo-version': '1.7.1'}"}*

```diff
@@ -26,15 +26,15 @@
         "http",
         "https",
         "file",
         "s3"
     ],
     "tags": {
         "news_content": "",
-        "sapporo-version": "1.7.0",
+        "sapporo-version": "1.7.1",
         "wes-name": "sapporo"
     },
     "workflow_engine_versions": {
         "cromwell": "80",
         "cwltool": "3.1.20240112164112",
         "ep3 (experimental)": "v1.7.0",
         "nextflow": "22.04.4",
```

### Comparing `sapporo-1.7.0/sapporo/service-info.schema.json` & `sapporo-1.7.1/sapporo/service-info.schema.json`

 * *Files identical despite different names*

### Comparing `sapporo-1.7.0/sapporo/trs.py` & `sapporo-1.7.1/sapporo/trs.py`

 * *Files identical despite different names*

### Comparing `sapporo-1.7.0/sapporo/validator.py` & `sapporo-1.7.1/sapporo/validator.py`

 * *Files identical despite different names*

### Comparing `sapporo-1.7.0/sapporo-wes-1-1-0-openapi-spec.yml` & `sapporo-1.7.1/sapporo-wes-1-1-0-openapi-spec.yml`

 * *Files identical despite different names*

### Comparing `sapporo-1.7.0/sapporo.egg-info/PKG-INFO` & `sapporo-1.7.1/sapporo.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sapporo
-Version: 1.7.0
+Version: 1.7.1
 Summary: The sapporo-service is a standard implementation conforming to the Global Alliance for Genomics and Health (GA4GH) Workflow Execution Service (WES) API specification.
 Home-page: https://github.com/sapporo-wes/sapporo-service
 Author: DDBJ(Bioinformatics and DDBJ Center)
 Author-email: tazro.ohta@chiba-u.jp
 License: Apache2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,14 +20,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: cryptography
 Requires-Dist: cwl-inputs-parser>=1.0.2
 Requires-Dist: flask_jwt_extended
 Requires-Dist: flask-cors
 Requires-Dist: flask
 Requires-Dist: jsonschema
 Requires-Dist: multiqc
 Requires-Dist: psutil
@@ -265,164 +266,126 @@
 $ docker run --rm -v /var/run/docker.sock:/var/run/docker.sock -v $PWD:$PWD -w $PWD ghcr.io/sapporo-wes/sapporo-service:latest python3 /app/sapporo/ro_crate.py $PWD
 ```
 
 For more information on RO-Crate, please also refer to [`./tests/ro-crate`](./tests/ro-crate).
 
 ### Authentication
 
-The sapporo-service supports authentication using JWT.
-The configuration for this authentication is managed through [`./sapporo/auth_config.json`](./sapporo/auth_config.json) file.
-By default, the file is set up as follows:
+The sapporo-service supports authentication, configurable via the [`./sapporo/auth_config.json`](./sapporo/auth_config.json).
+By default, this configuration is as follows:
 
 ```json
 {
   "auth_enabled": false,
-  "jwt_secret_key": "spr_secret_key_please_change_this",
-  "users": [
-    {
-      "username": "spr_test_user",
-      "password": "spr_test_password"
-    }
-  ]
+  "auth_provider": "local",
+  "local_auth": {
+    "jwt_secret_key": "spr_secret_key_please_change_this",
+    "users": [
+      {
+        "username": "spr_test_user",
+        "password": "spr_test_password"
+      }
+    ]
+  },
+  "oidc_auth": {
+    "realm_url": "http://localhost:8080/realms/sapporo-dev",
+    "username_claim": "sub"
+  }
 }
 ```
 
-You can edit this file directly, or, you can change its location using the startup argument `--auth-config` or the environment variable `SAPPORO_AUTH_CONFIG`.
+This configuration file can be directly edited or relocated using the `--auth-config` startup argument or the `SAPPORO_AUTH_CONFIG` environment variable.
 
-The file contains the following fields:
+#### Configuration Fields
 
-- `auth_enabled`: Determines whether JWT authentication is enabled. If set to `true`, JWT authentication is activated.
-- `jwt_secret_key`: The secret key used for signing the JWT. It is strongly recommended to change this value.
-- `users`: A list of users who will perform JWT authentication. Specify `username` and `password`.
+- `auth_enabled`: Determines if JWT authentication is activated. If set to `true`, JWT authentication is enabled.
+- `auth_provider`: Specifies the type of authentication provider, supporting:
+  - `local`: Uses a locally managed list of users for authentication.
+    - Tokens are issued by Sapporo.
+    - Usernames and passwords are referenced from the `auth_config.json`.
+  - `oidc`: Uses an OpenID Connect (OIDC) provider like [Keycloak](https://www.keycloak.org).
+    - Tokens are issued by the OIDC provider.
+    - User information is managed by the OIDC provider.
+- `local_auth`: Configuration for local authentication includes:
+  - `jwt_secret_key`: Secret key for signing JWTs. Changing this key is highly recommended.
+  - `users`: List of users eligible for JWT authentication, specifying username and password.
+- `oidc_auth`: Configuration for OIDC authentication includes:
+  - `realm_url`: URL of the OIDC realm.
+  - `username_claim`: JWT claim used as the username.
 
-When JWT authentication is enabled, the following endpoints require authentication:
+#### Authentication Endpoints
+
+When JWT authentication is enabled, endpoints requiring authentication include:
 
 - `GET /runs`
 - `POST /runs`
 - `GET /runs/{run_id}`
 - `POST /runs/{run_id}/cancel`
 - `GET /runs/{run_id}/status`
 - `GET /runs/{run_id}/data`
 
-Additionally, each run is associated with a `username`, so that, for example, only the user who created the run can access `GET /runs/{run_id}`.
+Each run is associated with a `username`, ensuring that only the user who created a run can access details like `GET /runs/{run_id}`.
+
+#### Local Authentication
 
-Let's take a look at how to use JWT authentication.
-First, edit the `auth-config.json` as follows:
+For local JWT authentication, configure `auth_config.json` as shown:
 
 ```json
 {
   "auth_enabled": true,
-  "jwt_secret_key": "spr_secret_key_please_change_this",
-  "users": [
-    {
-      "username": "spr_test_user1",
-      "password": "spr_test_password1"
-    },
-    {
-      "username": "spr_test_user2",
-      "password": "spr_test_password2"
-    }
-  ]
+  "auth_provider": "local",
+  "local_auth": {
+    "jwt_secret_key": "new_secret_key",
+    "users": [
+      {
+        "username": "user1",
+        "password": "password1"
+      },
+      {
+        "username": "user2",
+        "password": "password2"
+      }
+    ]
+  },
+  "oidc_auth": {
+    "realm_url": "http://localhost:8080/realms/sapporo-dev",
+    "username_claim": "sub"
+  }
 }
 ```
 
-With this configuration, if you start the sapporo-service, `GET /service-info` will return a result, but `GET /runs` will require authentication.
+Starting sapporo-service with this configuration allows access to the `GET /service-info` endpoint, while `GET /runs` will require authentication:
 
 ```bash
 # Start sapporo-service
 $ sapporo
 
 # GET /service-info
 $ curl -X GET localhost:1122/service-info
 {
   "auth_instructions_url": "https://github.com/sapporo-wes/sapporo-service",
   "contact_info_url": "https://github.com/sapporo-wes/sapporo-service",
 ...
 
-# GET /runs
-$ curl -X GET localhost:1122/runs
-{
-  "msg": "Missing Authorization Header",
-  "status": 401
-}
-```
-
-Here, you can generate a JWT required for authentication by sending a `POST /auth` request with `username` and `password` as follows:
-
-```bash
-$ curl -X POST \
+# Generate JWT for authentication
+$ TOKEN=$(curl -s -X POST \
     -H "Content-Type: application/json" \
-    -d '{"username":"spr_test_user1", "password":"spr_test_password1"}' \
-    localhost:1122/auth
-{
-  "access_token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJmcmVzaCI6ZmFsc2UsImlhdCI6MTcwNjQyODY2MCwianRpIjoiY2I5ZTU1MDgtN2RlNy00Y2EzLWE4NjYtN2ZlYmRmYTg4YWQ0IiwidHlwZSI6ImFjY2VzcyIsInN1YiI6InNwcl90ZXN0X3VzZXIxIiwibmJmIjoxNzA2NDI4NjYwLCJjc3JmIjoiZjdlZjNhZmYtMTVlZS00OTc2LTkxYzYtOTU2ZDZjZTVjYmQ5IiwiZXhwIjoxNzA2NDI5NTYwfQ.zyD7Ru72eD_9mJj548DS-qDk8Y5yan-rNbklWmfvcEs"
-}
-```
-
-If you attach this generated JWT to the Authorization header and send it to `GET /runs`, the authentication will pass.
-
-```bash
-$ TOKEN1=$(curl -s -X POST \
-    -H "Content-Type: application/json" \
-    -d '{"username":"spr_test_user1", "password":"spr_test_password1"}' \
+    -d '{"username":"user1", "password":"password1"}' \
     localhost:1122/auth | jq -r '.access_token')
 
-$ curl -X GET -H "Authorization: Bearer $TOKEN1" localhost:1122/runs
+# Authenticate and access runs
+$ curl -X GET -H "Authorization: Bearer $TOKEN" localhost:1122/runs
 {
   "runs": []
 }
 ```
 
-Let's also confirm that User2 cannot access the run executed by User1.
-
-```bash
-$ TOKEN1=$(curl -s -X POST \
-    -H "Content-Type: application/json" \
-    -d '{"username":"spr_test_user1", "password":"spr_test_password1"}' \
-    localhost:1122/auth | jq -r '.access_token')
-$ TOKEN2=$(curl -s -X POST \
-    -H "Content-Type: application/json" \
-    -d '{"username":"spr_test_user2", "password":"spr_test_password2"}' \
-    localhost:1122/auth | jq -r '.access_token')
-
-# Execute a run with User1
-# Please refer to ./tests/curl_example/cwltool_remote_workflow.sh for example
-# Run ID: af95fd09-8406-4f2c-9280-bca900e07289
+#### OpenID Connect (OIDC) Authentication
 
-# GET /runs with User1
-$ curl -X GET -H "Authorization: Bearer $TOKEN1" localhost:1122/runs
-{
-  "runs": [
-    {
-      "run_id": "af95fd09-8406-4f2c-9280-bca900e07289",
-      "state": "COMPLETE"
-    }
-  ]
-}
-
-# GET /runs/{run_id} with User1
-$ curl -X GET -H "Authorization: Bearer $TOKEN1" localhost:1122/runs/af95fd09-8406-4f2c-9280-bca900e07289
-{
-  "outputs": [
-    {
-      ...
-
-# GET /runs with User2
-$ curl -X GET -H "Authorization: Bearer $TOKEN2" localhost:1122/runs
-{
-  "runs": []
-}
-
-# GET /runs/{run_id} with User2
-$ curl -X GET -H "Authorization: Bearer $TOKEN2" localhost:1122/runs/af95fd09-8406-4f2c-9280-bca900e07289
-{
-  "msg": "You don't have permission to access this run.",
-  "status_code": 403
-}
-```
+For OIDC authentication, ensure the `auth_provider` is set to `oidc` and appropriate configurations are specified under `oidc_auth`. Users must obtain a token from the OIDC provider and attach it to the Authorization header for authentication.
 
 ## Development
 
 To start the development environment, follow these steps:
 
 ```bash
 $ docker compose -f compose.dev.yml up -d --build
```

### Comparing `sapporo-1.7.0/sapporo.egg-info/SOURCES.txt` & `sapporo-1.7.1/sapporo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sapporo-1.7.0/setup.py` & `sapporo-1.7.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,15 @@
             "sapporo/run.sh",
             "sapporo/service-info.json",
             "sapporo/service-info.schema.json",
         ]
     },
     include_package_data=True,
     install_requires=[
+        "cryptography",
         "cwl-inputs-parser>=1.0.2",
         "flask_jwt_extended",
         "flask-cors",
         "flask",
         "jsonschema",
         "multiqc",
         "psutil",
```

