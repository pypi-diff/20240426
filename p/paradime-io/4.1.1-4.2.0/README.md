# Comparing `tmp/paradime_io-4.1.1.tar.gz` & `tmp/paradime_io-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paradime_io-4.1.1.tar", max compression
+gzip compressed data, was "paradime_io-4.2.0.tar", max compression
```

## Comparing `paradime_io-4.1.1.tar` & `paradime_io-4.2.0.tar`

### file list

```diff
@@ -1,36 +1,37 @@
--rw-r--r--   0        0        0     1074 2024-04-09 16:14:06.041028 paradime_io-4.1.1/LICENSE
--rw-r--r--   0        0        0     1060 2024-04-09 16:14:06.041028 paradime_io-4.1.1/README.md
--rw-r--r--   0        0        0       84 2024-04-09 16:14:06.045028 paradime_io-4.1.1/paradime/__init__.py
--rw-r--r--   0        0        0        0 2024-04-09 16:14:06.045028 paradime_io-4.1.1/paradime/apis/__init__.py
--rw-r--r--   0        0        0        0 2024-04-09 16:14:06.045028 paradime_io-4.1.1/paradime/apis/audit_log/__init__.py
--rw-r--r--   0        0        0     1901 2024-04-09 16:14:06.045028 paradime_io-4.1.1/paradime/apis/audit_log/client.py
--rw-r--r--   0        0        0      423 2024-04-09 16:14:06.045028 paradime_io-4.1.1/paradime/apis/audit_log/types.py
--rw-r--r--   0        0        0        0 2024-04-09 16:14:06.045028 paradime_io-4.1.1/paradime/apis/bolt/__init__.py
--rw-r--r--   0        0        0    14252 2024-04-09 16:14:06.045028 paradime_io-4.1.1/paradime/apis/bolt/client.py
--rw-r--r--   0        0        0      387 2024-04-09 16:14:06.045028 paradime_io-4.1.1/paradime/apis/bolt/exception.py
--rw-r--r--   0        0        0     1609 2024-04-09 16:14:06.045028 paradime_io-4.1.1/paradime/apis/bolt/types.py
--rw-r--r--   0        0        0        0 2024-04-09 16:14:06.045028 paradime_io-4.1.1/paradime/apis/custom_integration/__init__.py
--rw-r--r--   0        0        0    12369 2024-04-09 16:14:06.045028 paradime_io-4.1.1/paradime/apis/custom_integration/client.py
--rw-r--r--   0        0        0    17115 2024-04-09 16:14:06.045028 paradime_io-4.1.1/paradime/apis/custom_integration/types.py
--rw-r--r--   0        0        0      321 2024-04-09 16:14:06.045028 paradime_io-4.1.1/paradime/apis/custom_integration/utils.py
--rw-r--r--   0        0        0        0 2024-04-09 16:14:06.045028 paradime_io-4.1.1/paradime/apis/users/__init__.py
--rw-r--r--   0        0        0     4052 2024-04-09 16:14:06.045028 paradime_io-4.1.1/paradime/apis/users/client.py
--rw-r--r--   0        0        0      656 2024-04-09 16:14:06.045028 paradime_io-4.1.1/paradime/apis/users/types.py
--rw-r--r--   0        0        0        0 2024-04-09 16:14:06.045028 paradime_io-4.1.1/paradime/apis/workspaces/__init__.py
--rw-r--r--   0        0        0      823 2024-04-09 16:14:06.045028 paradime_io-4.1.1/paradime/apis/workspaces/client.py
--rw-r--r--   0        0        0       88 2024-04-09 16:14:06.045028 paradime_io-4.1.1/paradime/apis/workspaces/types.py
--rw-r--r--   0        0        0        0 2024-04-09 16:14:06.045028 paradime_io-4.1.1/paradime/cli/__init__.py
--rw-r--r--   0        0        0     3122 2024-04-09 16:14:06.045028 paradime_io-4.1.1/paradime/cli/bolt.py
--rw-r--r--   0        0        0      538 2024-04-09 16:14:06.045028 paradime_io-4.1.1/paradime/cli/cli.py
--rw-r--r--   0        0        0      963 2024-04-09 16:14:06.045028 paradime_io-4.1.1/paradime/cli/login.py
--rw-r--r--   0        0        0      192 2024-04-09 16:14:06.045028 paradime_io-4.1.1/paradime/cli/version.py
--rw-r--r--   0        0        0     3437 2024-04-09 16:14:06.045028 paradime_io-4.1.1/paradime/client/api_client.py
--rw-r--r--   0        0        0      231 2024-04-09 16:14:06.045028 paradime_io-4.1.1/paradime/client/api_exception.py
--rw-r--r--   0        0        0      974 2024-04-09 16:14:06.045028 paradime_io-4.1.1/paradime/client/paradime_cli_client.py
--rw-r--r--   0        0        0     1692 2024-04-09 16:14:06.045028 paradime_io-4.1.1/paradime/client/paradime_client.py
--rw-r--r--   0        0        0        0 2024-04-09 16:14:06.045028 paradime_io-4.1.1/paradime/core/__init__.py
--rw-r--r--   0        0        0        0 2024-04-09 16:14:06.045028 paradime_io-4.1.1/paradime/core/bolt/__init__.py
--rw-r--r--   0        0        0     5615 2024-04-09 16:14:06.045028 paradime_io-4.1.1/paradime/core/bolt/schedule.py
--rw-r--r--   0        0        0      376 2024-04-09 16:14:06.045028 paradime_io-4.1.1/paradime/version.py
--rw-r--r--   0        0        0     1138 2024-04-09 16:14:06.045028 paradime_io-4.1.1/pyproject.toml
--rw-r--r--   0        0        0     1815 1970-01-01 00:00:00.000000 paradime_io-4.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-04-26 14:03:32.017141 paradime_io-4.2.0/LICENSE
+-rw-r--r--   0        0        0     1060 2024-04-26 14:03:32.017141 paradime_io-4.2.0/README.md
+-rw-r--r--   0        0        0       84 2024-04-26 14:03:32.017141 paradime_io-4.2.0/paradime/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 14:03:32.021141 paradime_io-4.2.0/paradime/apis/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 14:03:32.021141 paradime_io-4.2.0/paradime/apis/audit_log/__init__.py
+-rw-r--r--   0        0        0     1901 2024-04-26 14:03:32.021141 paradime_io-4.2.0/paradime/apis/audit_log/client.py
+-rw-r--r--   0        0        0      423 2024-04-26 14:03:32.021141 paradime_io-4.2.0/paradime/apis/audit_log/types.py
+-rw-r--r--   0        0        0        0 2024-04-26 14:03:32.021141 paradime_io-4.2.0/paradime/apis/bolt/__init__.py
+-rw-r--r--   0        0        0    14252 2024-04-26 14:03:32.021141 paradime_io-4.2.0/paradime/apis/bolt/client.py
+-rw-r--r--   0        0        0      387 2024-04-26 14:03:32.021141 paradime_io-4.2.0/paradime/apis/bolt/exception.py
+-rw-r--r--   0        0        0     1609 2024-04-26 14:03:32.021141 paradime_io-4.2.0/paradime/apis/bolt/types.py
+-rw-r--r--   0        0        0        0 2024-04-26 14:03:32.021141 paradime_io-4.2.0/paradime/apis/custom_integration/__init__.py
+-rw-r--r--   0        0        0    12369 2024-04-26 14:03:32.021141 paradime_io-4.2.0/paradime/apis/custom_integration/client.py
+-rw-r--r--   0        0        0    17115 2024-04-26 14:03:32.021141 paradime_io-4.2.0/paradime/apis/custom_integration/types.py
+-rw-r--r--   0        0        0      321 2024-04-26 14:03:32.021141 paradime_io-4.2.0/paradime/apis/custom_integration/utils.py
+-rw-r--r--   0        0        0        0 2024-04-26 14:03:32.021141 paradime_io-4.2.0/paradime/apis/users/__init__.py
+-rw-r--r--   0        0        0     4052 2024-04-26 14:03:32.021141 paradime_io-4.2.0/paradime/apis/users/client.py
+-rw-r--r--   0        0        0      656 2024-04-26 14:03:32.021141 paradime_io-4.2.0/paradime/apis/users/types.py
+-rw-r--r--   0        0        0        0 2024-04-26 14:03:32.021141 paradime_io-4.2.0/paradime/apis/workspaces/__init__.py
+-rw-r--r--   0        0        0      823 2024-04-26 14:03:32.021141 paradime_io-4.2.0/paradime/apis/workspaces/client.py
+-rw-r--r--   0        0        0       88 2024-04-26 14:03:32.021141 paradime_io-4.2.0/paradime/apis/workspaces/types.py
+-rw-r--r--   0        0        0        0 2024-04-26 14:03:32.021141 paradime_io-4.2.0/paradime/cli/__init__.py
+-rw-r--r--   0        0        0     2885 2024-04-26 14:03:32.021141 paradime_io-4.2.0/paradime/cli/bolt.py
+-rw-r--r--   0        0        0      538 2024-04-26 14:03:32.021141 paradime_io-4.2.0/paradime/cli/cli.py
+-rw-r--r--   0        0        0     1002 2024-04-26 14:03:32.021141 paradime_io-4.2.0/paradime/cli/login.py
+-rw-r--r--   0        0        0     1966 2024-04-26 14:03:32.021141 paradime_io-4.2.0/paradime/cli/rich_text_output.py
+-rw-r--r--   0        0        0      351 2024-04-26 14:03:32.021141 paradime_io-4.2.0/paradime/cli/version.py
+-rw-r--r--   0        0        0     3719 2024-04-26 14:03:32.021141 paradime_io-4.2.0/paradime/client/api_client.py
+-rw-r--r--   0        0        0      231 2024-04-26 14:03:32.021141 paradime_io-4.2.0/paradime/client/api_exception.py
+-rw-r--r--   0        0        0      974 2024-04-26 14:03:32.021141 paradime_io-4.2.0/paradime/client/paradime_cli_client.py
+-rw-r--r--   0        0        0     1692 2024-04-26 14:03:32.021141 paradime_io-4.2.0/paradime/client/paradime_client.py
+-rw-r--r--   0        0        0        0 2024-04-26 14:03:32.021141 paradime_io-4.2.0/paradime/core/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 14:03:32.021141 paradime_io-4.2.0/paradime/core/bolt/__init__.py
+-rw-r--r--   0        0        0     5615 2024-04-26 14:03:32.021141 paradime_io-4.2.0/paradime/core/bolt/schedule.py
+-rw-r--r--   0        0        0      376 2024-04-26 14:03:32.021141 paradime_io-4.2.0/paradime/version.py
+-rw-r--r--   0        0        0     1156 2024-04-26 14:03:32.021141 paradime_io-4.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1849 1970-01-01 00:00:00.000000 paradime_io-4.2.0/PKG-INFO
```

### Comparing `paradime_io-4.1.1/LICENSE` & `paradime_io-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `paradime_io-4.1.1/README.md` & `paradime_io-4.2.0/README.md`

 * *Files identical despite different names*

### Comparing `paradime_io-4.1.1/paradime/apis/audit_log/client.py` & `paradime_io-4.2.0/paradime/apis/audit_log/client.py`

 * *Files identical despite different names*

### Comparing `paradime_io-4.1.1/paradime/apis/bolt/client.py` & `paradime_io-4.2.0/paradime/apis/bolt/client.py`

 * *Files identical despite different names*

### Comparing `paradime_io-4.1.1/paradime/apis/bolt/types.py` & `paradime_io-4.2.0/paradime/apis/bolt/types.py`

 * *Files identical despite different names*

### Comparing `paradime_io-4.1.1/paradime/apis/custom_integration/client.py` & `paradime_io-4.2.0/paradime/apis/custom_integration/client.py`

 * *Files identical despite different names*

### Comparing `paradime_io-4.1.1/paradime/apis/custom_integration/types.py` & `paradime_io-4.2.0/paradime/apis/custom_integration/types.py`

 * *Files identical despite different names*

### Comparing `paradime_io-4.1.1/paradime/apis/users/client.py` & `paradime_io-4.2.0/paradime/apis/users/client.py`

 * *Files identical despite different names*

### Comparing `paradime_io-4.1.1/paradime/apis/users/types.py` & `paradime_io-4.2.0/paradime/apis/users/types.py`

 * *Files identical despite different names*

### Comparing `paradime_io-4.1.1/paradime/apis/workspaces/client.py` & `paradime_io-4.2.0/paradime/apis/workspaces/client.py`

 * *Files identical despite different names*

### Comparing `paradime_io-4.1.1/paradime/cli/bolt.py` & `paradime_io-4.2.0/paradime/cli/bolt.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 import time
 from pathlib import Path
 from typing import Final, List
 
 import click
 
 from paradime.apis.bolt.types import BoltRunState
+from paradime.cli.rich_text_output import print_error_table, print_run_started, print_run_status
+from paradime.cli.version import print_version
 from paradime.client.api_exception import ParadimeAPIException
 from paradime.client.paradime_cli_client import get_cli_client_or_exit
 from paradime.core.bolt.schedule import (
     SCHEDULE_FILE_NAME,
     is_allowed_command,
     is_valid_schedule_at_path,
     parse_command,
@@ -35,60 +37,46 @@
     wait: bool,
     json: bool,
     schedule_name: str,
 ) -> None:
     """
     Trigger a Paradime Bolt run.
     """
+    if not json:
+        print_version()
+
     # verify
     if command:
         for _command in command:
             if not is_allowed_command(parse_command(_command)):
-                click.echo(
-                    f"Command {_command!r} is not allowed."
-                    if not json
-                    else {"error": f"Command {_command!r} is not allowed."}
-                )
+                print_error_table(f"Command {_command!r} is not allowed.", is_json=json)
                 sys.exit(1)
 
     # trigger run
     client = get_cli_client_or_exit()
     try:
         run_id = client.bolt.trigger_run(
             schedule_name,
             branch=branch,
             commands=list(command) if command else None,
         )
     except ParadimeAPIException as e:
-        click.echo(
-            f"Failed to trigger run: {e}" if not json else {"error": f"Failed to trigger run: {e}"}
-        )
+        print_error_table(f"Failed to trigger run: {e}", is_json=json)
         sys.exit(1)
 
-    click.echo(
-        {
-            "run_id": run_id,
-            "url": f"https://app.paradime.io/bolt/run_id/{run_id}",
-        }
-        if json
-        else run_id
-    )
+    print_run_started(run_id, json)
 
     if wait:
         while True:
             status = client.bolt.get_run_status(run_id)
             if not status:
-                click.echo(
-                    "Unable to fetch status from bolt."
-                    if not json
-                    else {"error": "Unable to fetch status from bolt."}
-                )
+                print_error_table("Unable to fetch status from bolt.", is_json=json)
                 sys.exit(1)
 
-            click.echo({"status": status.value} if json else status)
+            print_run_status(status.value, json)
             if status is not BoltRunState.RUNNING:
                 break
             time.sleep(WAIT_SLEEP)
 
         if status is not BoltRunState.SUCCESS:
             sys.exit(1)
 
@@ -100,17 +88,18 @@
     show_default=True,
     default=SCHEDULE_FILE_NAME,
 )
 def verify(path: str) -> None:
     """
     Verify the paradime_schedules.yml file.
     """
+    print_version()
     error_string = is_valid_schedule_at_path(Path(path))
     if error_string:
-        click.echo(error_string)
+        print_error_table(error_string, is_json=False)
         sys.exit(1)
 
 
 @click.group()
 def bolt() -> None:
     """
     Work with Paradime Bolt from the CLI.
```

### Comparing `paradime_io-4.1.1/paradime/cli/cli.py` & `paradime_io-4.2.0/paradime/cli/cli.py`

 * *Files identical despite different names*

### Comparing `paradime_io-4.1.1/paradime/cli/login.py` & `paradime_io-4.2.0/paradime/cli/login.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 import click
 
+from paradime.cli.version import print_version
 from paradime.client.paradime_cli_client import get_credentials_path
 
 
 @click.command()
 def login() -> None:
     """
     Set the API credentials for the Paradime CLI.
     """
+    print_version()
     credentials_path = get_credentials_path()
     if credentials_path.exists():
         click.confirm(
             "Do you want to overwrite existing credentials?",
             abort=True,
         )
 
-    click.echo("Generate new credentials here: https://app.paradime.io/account-settings/workspace")
+    click.echo("Generate API credentials here: https://app.paradime.io/account-settings/workspace")
 
-    api_key = click.prompt("Please enter the API Key")
-    api_secret = click.prompt("Please enter the API Secret", hide_input=True)
-    api_endpoint = click.prompt("Please enter the API Endpoint")
+    api_key = click.prompt("Enter API Key")
+    api_secret = click.prompt("Enter API Secret", hide_input=True)
+    api_endpoint = click.prompt("Enter API Endpoint")
 
     # write to env file
     credentials_path.parent.mkdir(parents=True, exist_ok=True)
     credentials_path.write_text(
         f"API_ENDPOINT={api_endpoint}\nAPI_KEY={api_key}\nAPI_SECRET={api_secret}\n"
     )
-    click.echo(f"Writen credentials to '{credentials_path}'!")
+    click.echo(f"✨ Credentials written to '{credentials_path}'!")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `paradime_io-4.1.1/paradime/client/api_client.py` & `paradime_io-4.2.0/paradime/client/api_client.py`

 * *Files 11% similar despite different names*

```diff
@@ -54,15 +54,22 @@
 
         Raises:
             ParadimeAPIException: If there are errors in the response body.
         """
 
         response_json = response.json()
         if "errors" in response_json:
-            raise ParadimeAPIException(f"{response_json['errors']}")
+            error_message = self._get_error_message_from_response(response_json)
+            raise ParadimeAPIException(error_message)
+
+    def _get_error_message_from_response(self, response: Dict[str, Any]) -> str:
+        try:
+            return response["errors"][0]["message"]
+        except Exception:
+            return str(response["errors"])
 
     def _raise_for_response_status_errors(self, response: requests.Response) -> None:
         """
         Raise an exception for response status errors.
 
         Args:
             response (requests.Response): The API response.
```

### Comparing `paradime_io-4.1.1/paradime/client/paradime_cli_client.py` & `paradime_io-4.2.0/paradime/client/paradime_cli_client.py`

 * *Files identical despite different names*

### Comparing `paradime_io-4.1.1/paradime/client/paradime_client.py` & `paradime_io-4.2.0/paradime/client/paradime_client.py`

 * *Files identical despite different names*

### Comparing `paradime_io-4.1.1/paradime/core/bolt/schedule.py` & `paradime_io-4.2.0/paradime/core/bolt/schedule.py`

 * *Files identical despite different names*

### Comparing `paradime_io-4.1.1/pyproject.toml` & `paradime_io-4.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 [tool.poetry]
 name = "paradime-io"
-version = "4.1.1"
+version = "4.2.0"
 description = "Paradime - Python SDK"
 authors = ["Bhuvan Singla <bhuvan@paradime.io>", "Maximilian Mitchell <max@paradime.io>"]
 readme = "README.md"
 packages = [
 	{ include = "paradime", from = "." },
 ]
 
 [tool.poetry.scripts]
 paradime = 'paradime.cli.cli:cli'
 
 [tool.poetry.dependencies]
 python = ">=3.8"
-pydantic = "^1.10.0"
+pydantic = "1.10.14"
 requests = "^2.31.0"
-click = "^8.1.0"
+click = "^8.1.7"
 croniter = "^2.0.2"
 pyyaml = "^6.0.1"
-python-dotenv = "^1.0.0"
+python-dotenv = "^1.0.1"
+typer = "^0.12.1"
 
 
 [tool.poetry.group.dev.dependencies]
 types-requests = "^2.31.0.20240125"
 mypy = "^1.8.0"
 black = "^24.2.0"
 isort = "^5.13.2"
```

### Comparing `paradime_io-4.1.1/PKG-INFO` & `paradime_io-4.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: paradime-io
-Version: 4.1.1
+Version: 4.2.0
 Summary: Paradime - Python SDK
 Author: Bhuvan Singla
 Author-email: bhuvan@paradime.io
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: click (>=8.1.0,<9.0.0)
+Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: croniter (>=2.0.2,<3.0.0)
-Requires-Dist: pydantic (>=1.10.0,<2.0.0)
-Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
+Requires-Dist: pydantic (==1.10.14)
+Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: typer (>=0.12.1,<0.13.0)
 Description-Content-Type: text/markdown
 
 <p align="center">
   <a href="https://www.paradime.io">
         <img alt="Paradime" src="https://app.paradime.io/logo192.png" width="60" />
     </a>
 </p>
```

#### html2text {}

```diff
@@ -1,17 +1,18 @@
-Metadata-Version: 2.1 Name: paradime-io Version: 4.1.1 Summary: Paradime -
+Metadata-Version: 2.1 Name: paradime-io Version: 4.2.0 Summary: Paradime -
 Python SDK Author: Bhuvan Singla Author-email: bhuvan@paradime.io Requires-
 Python: >=3.8 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: 3.12 Requires-Dist: click (>=8.1.0,<9.0.0) Requires-Dist: croniter
-(>=2.0.2,<3.0.0) Requires-Dist: pydantic (>=1.10.0,<2.0.0) Requires-Dist:
-python-dotenv (>=1.0.0,<2.0.0) Requires-Dist: pyyaml (>=6.0.1,<7.0.0) Requires-
-Dist: requests (>=2.31.0,<3.0.0) Description-Content-Type: text/markdown
+Python :: 3.12 Requires-Dist: click (>=8.1.7,<9.0.0) Requires-Dist: croniter
+(>=2.0.2,<3.0.0) Requires-Dist: pydantic (==1.10.14) Requires-Dist: python-
+dotenv (>=1.0.1,<2.0.0) Requires-Dist: pyyaml (>=6.0.1,<7.0.0) Requires-Dist:
+requests (>=2.31.0,<3.0.0) Requires-Dist: typer (>=0.12.1,<0.13.0) Description-
+Content-Type: text/markdown
                                   _[_P_a_r_a_d_i_m_e_]
                       ************ PPaarraaddiimmee -- PPyytthhoonn SSDDKK ************
 ## Installation ```sh pip install paradime-io ``` ## SDK Usage Generate your
 API key, secret and endpoint from Paradime workspace settings. ```python from
 paradime import Paradime paradime = Paradime( api_endpoint="API_ENDPOINT",
 api_key="API_KEY", api_secret="API_SECRET", ) # Use the paradime client to
 interact with the API ``` ## CLI Usage For the full specification of the CLI,
```

