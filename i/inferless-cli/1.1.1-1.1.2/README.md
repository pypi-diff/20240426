# Comparing `tmp/inferless_cli-1.1.1.tar.gz` & `tmp/inferless_cli-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inferless_cli-1.1.1.tar", max compression
+gzip compressed data, was "inferless_cli-1.1.2.tar", max compression
```

## Comparing `inferless_cli-1.1.1.tar` & `inferless_cli-1.1.2.tar`

### file list

```diff
@@ -1,25 +1,27 @@
--rw-r--r--   0        0        0     9036 2024-03-19 05:25:09.615067 inferless_cli-1.1.1/README.md
--rw-r--r--   0        0        0       37 2024-03-20 07:13:33.138070 inferless_cli-1.1.1/inferless_cli/__init__.py
--rw-r--r--   0        0        0       50 2024-03-13 03:52:17.953547 inferless_cli-1.1.1/inferless_cli/__main__.py
--rw-r--r--   0        0        0     4835 2024-03-19 05:25:11.572753 inferless_cli-1.1.1/inferless_cli/main.py
--rw-r--r--   0        0        0        0 2024-03-13 03:51:47.516671 inferless_cli-1.1.1/inferless_cli/prompts/__init__.py
--rw-r--r--   0        0        0    20451 2024-03-13 14:35:01.214374 inferless_cli-1.1.1/inferless_cli/prompts/deploy.py
--rw-r--r--   0        0        0    11391 2024-03-13 14:35:01.214724 inferless_cli-1.1.1/inferless_cli/prompts/init.py
--rw-r--r--   0        0        0     3779 2024-03-13 03:53:05.727048 inferless_cli-1.1.1/inferless_cli/prompts/log.py
--rw-r--r--   0        0        0      854 2024-03-13 03:51:54.338936 inferless_cli-1.1.1/inferless_cli/prompts/login.py
--rw-r--r--   0        0        0    15846 2024-03-20 06:34:09.176617 inferless_cli-1.1.1/inferless_cli/prompts/model.py
--rw-r--r--   0        0        0    18976 2024-03-14 11:57:44.835814 inferless_cli-1.1.1/inferless_cli/prompts/run.py
--rw-r--r--   0        0        0     5984 2024-03-13 03:53:05.727966 inferless_cli-1.1.1/inferless_cli/prompts/runtime.py
--rw-r--r--   0        0        0     2026 2024-03-13 03:53:05.728163 inferless_cli-1.1.1/inferless_cli/prompts/secret.py
--rw-r--r--   0        0        0     4231 2024-03-20 06:19:47.141761 inferless_cli-1.1.1/inferless_cli/prompts/token.py
--rw-r--r--   0        0        0    22032 2024-03-20 07:13:17.066302 inferless_cli-1.1.1/inferless_cli/prompts/volume.py
--rw-r--r--   0        0        0     1699 2024-03-13 03:53:05.729058 inferless_cli-1.1.1/inferless_cli/prompts/workspace.py
--rw-r--r--   0        0        0        0 2024-03-13 03:52:07.884835 inferless_cli-1.1.1/inferless_cli/utils/__init__.py
--rw-r--r--   0        0        0     2870 2024-03-13 03:53:05.729413 inferless_cli-1.1.1/inferless_cli/utils/api.py
--rw-r--r--   0        0        0    14630 2024-03-20 05:15:59.906549 inferless_cli-1.1.1/inferless_cli/utils/constants.py
--rw-r--r--   0        0        0     7174 2024-03-20 05:15:59.907099 inferless_cli-1.1.1/inferless_cli/utils/credentials.py
--rw-r--r--   0        0        0    28470 2024-03-20 05:15:59.907731 inferless_cli-1.1.1/inferless_cli/utils/helpers.py
--rw-r--r--   0        0        0    25570 2024-03-20 07:10:35.982553 inferless_cli-1.1.1/inferless_cli/utils/services.py
--rw-r--r--   0        0        0     7065 2024-03-13 03:52:15.076191 inferless_cli-1.1.1/inferless_cli/utils/validators.py
--rw-r--r--   0        0        0      671 2024-03-20 07:13:43.571004 inferless_cli-1.1.1/pyproject.toml
--rw-r--r--   0        0        0    10049 1970-01-01 00:00:00.000000 inferless_cli-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0    10052 2024-04-22 04:37:30.629340 inferless_cli-1.1.2/README.md
+-rw-r--r--   0        0        0       37 2024-04-26 08:38:38.118679 inferless_cli-1.1.2/inferless_cli/__init__.py
+-rw-r--r--   0        0        0       50 2024-03-13 03:52:17.953547 inferless_cli-1.1.2/inferless_cli/__main__.py
+-rw-r--r--   0        0        0     7282 2024-04-22 04:37:30.630760 inferless_cli-1.1.2/inferless_cli/main.py
+-rw-r--r--   0        0        0        0 2024-03-13 03:51:47.516671 inferless_cli-1.1.2/inferless_cli/prompts/__init__.py
+-rw-r--r--   0        0        0    23068 2024-04-26 09:57:42.716132 inferless_cli-1.1.2/inferless_cli/prompts/deploy.py
+-rw-r--r--   0        0        0     1802 2024-04-08 10:17:33.453829 inferless_cli-1.1.2/inferless_cli/prompts/export.py
+-rw-r--r--   0        0        0    11391 2024-03-13 14:35:01.214724 inferless_cli-1.1.2/inferless_cli/prompts/init.py
+-rw-r--r--   0        0        0     3779 2024-03-13 03:53:05.727048 inferless_cli-1.1.2/inferless_cli/prompts/log.py
+-rw-r--r--   0        0        0      854 2024-03-13 03:51:54.338936 inferless_cli-1.1.2/inferless_cli/prompts/login.py
+-rw-r--r--   0        0        0    15846 2024-03-26 03:45:26.809903 inferless_cli-1.1.2/inferless_cli/prompts/model.py
+-rw-r--r--   0        0        0    18882 2024-04-26 08:39:22.573369 inferless_cli-1.1.2/inferless_cli/prompts/run.py
+-rw-r--r--   0        0        0     5984 2024-03-13 03:53:05.727966 inferless_cli-1.1.2/inferless_cli/prompts/runtime.py
+-rw-r--r--   0        0        0     2026 2024-03-13 03:53:05.728163 inferless_cli-1.1.2/inferless_cli/prompts/secret.py
+-rw-r--r--   0        0        0     4231 2024-03-26 03:45:26.810630 inferless_cli-1.1.2/inferless_cli/prompts/token.py
+-rw-r--r--   0        0        0    22032 2024-03-26 03:45:26.810909 inferless_cli-1.1.2/inferless_cli/prompts/volume.py
+-rw-r--r--   0        0        0     1699 2024-03-13 03:53:05.729058 inferless_cli-1.1.2/inferless_cli/prompts/workspace.py
+-rw-r--r--   0        0        0        0 2024-03-13 03:52:07.884835 inferless_cli-1.1.2/inferless_cli/utils/__init__.py
+-rw-r--r--   0        0        0     2870 2024-03-13 03:53:05.729413 inferless_cli-1.1.2/inferless_cli/utils/api.py
+-rw-r--r--   0        0        0    14752 2024-04-08 10:17:33.455242 inferless_cli-1.1.2/inferless_cli/utils/constants.py
+-rw-r--r--   0        0        0     1068 2024-03-26 03:50:38.927856 inferless_cli-1.1.2/inferless_cli/utils/convertors.py
+-rw-r--r--   0        0        0     7174 2024-03-26 03:45:26.811483 inferless_cli-1.1.2/inferless_cli/utils/credentials.py
+-rw-r--r--   0        0        0    28795 2024-04-26 08:32:53.056800 inferless_cli-1.1.2/inferless_cli/utils/helpers.py
+-rw-r--r--   0        0        0    26839 2024-04-26 09:17:36.749109 inferless_cli-1.1.2/inferless_cli/utils/services.py
+-rw-r--r--   0        0        0     7065 2024-03-13 03:52:15.076191 inferless_cli-1.1.2/inferless_cli/utils/validators.py
+-rw-r--r--   0        0        0      671 2024-04-26 08:38:30.382551 inferless_cli-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0    11065 1970-01-01 00:00:00.000000 inferless_cli-1.1.2/PKG-INFO
```

### Comparing `inferless_cli-1.1.1/README.md` & `inferless_cli-1.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 * `-v, --version`
 * `--help`: Show this message and exit.
 
 **Commands**:
 
 * `deploy`: Deploy a model to Inferless
+* `export`: Export the runtime configuration of...
 * `init`: Initialize a new Inferless model
 * `log`: Inferless models logs (view build logs or...
 * `login`: Login to Inferless
 * `mode`: Change mode
 * `model`: Manage Inferless models (list , delete ,...
 * `run`: Run a model locally
 * `runtime`: Manage Inferless runtimes (can be used to...
@@ -41,14 +42,31 @@
 $ inferless deploy [OPTIONS]
 ```
 
 **Options**:
 
 * `--help`: Show this message and exit.
 
+## `inferless export`
+
+Export the runtime configuration of another provider to Inferless runtime config
+
+**Usage**:
+
+```console
+$ inferless export [OPTIONS]
+```
+
+**Options**:
+
+* `-r, --runtime TEXT`: The runtime configuration file of another provider  [default: cog.yaml]
+* `-d, --destination TEXT`: The destination file for the Inferless runtime configuration  [default: inferless-runtime-config.yaml]
+* `-f, --from TEXT`: The provider from which to export the runtime configuration  [default: replicate]
+* `--help`: Show this message and exit.
+
 ## `inferless init`
 
 Initialize a new Inferless model
 
 **Usage**:
 
 ```console
@@ -233,14 +251,18 @@
 ```console
 $ inferless run [OPTIONS]
 ```
 
 **Options**:
 
 * `-r, --runtime TEXT`: custom runtime config file path to override from inferless-runtime-config.yaml
+* `-t, --type TEXT`: Type of runtime to run [inferless, replicate]
+* `-n, --name TEXT`: Name of the model to deploy on inferless  [default: inferless-model]
+* `-f, --env-file TEXT`: Path to an env file containing environment variables (one per line in KEY=VALUE format)
+* `-e, --env TEXT`: Environment variables to set for the runtime (e.g. 'KEY=VALUE'). If the env variable contains special chars please escape them.
 * `--help`: Show this message and exit.
 
 ## `inferless runtime`
 
 Manage Inferless runtimes (can be used to list runtimes and upload new runtimes)
 
 **Usage**:
```

### Comparing `inferless_cli-1.1.1/inferless_cli/main.py` & `inferless_cli-1.1.2/inferless_cli/main.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 import rich
 import typer
 from inferless_cli.prompts import run
 
-from inferless_cli.utils.constants import DEFAULT_YAML_FILE_NAME
+from typing import Optional, List
+from inferless_cli.utils.constants import (
+    DEFAULT_YAML_FILE_NAME,
+    DEFAULT_RUNTIME_FILE_NAME,
+    PROVIDER_CHOICES,
+)
 from .utils.services import (
     callback_with_auth_validation,
     min_version_required,
 )
 from .utils.helpers import (
     check_import_source,
     sentry_init,
@@ -20,14 +25,15 @@
     token,
     deploy,
     log,
     model,
     secret,
     volume,
     runtime,
+    export,
 )
 from prompt_toolkit import prompt
 import sys
 
 sys.tracebacklimit = 0
 
 sentry_init()
@@ -121,14 +127,42 @@
     runtime.app,
     name="runtime",
     help="Manage Inferless runtimes (can be used to list runtimes and upload new runtimes)",
     callback=callback_with_auth_validation,
 )
 
 
+@app.command(
+    "export",
+    help="Export the runtime configuration of another provider to Inferless runtime config",
+)
+def export_def(
+    source_file: Optional[str] = typer.Option(
+        "cog.yaml",
+        "--runtime",
+        "-r",
+        help="The runtime configuration file of another provider",
+    ),
+    destination_file: Optional[str] = typer.Option(
+        DEFAULT_RUNTIME_FILE_NAME,
+        "--destination",
+        "-d",
+        help="The destination file for the Inferless runtime configuration",
+    ),
+    from_provider: Optional[str] = typer.Option(
+        "replicate",
+        "--from",
+        "-f",
+        help="The provider from which to export the runtime configuration",
+    ),
+):
+    callback_with_auth_validation()
+    export.export_runtime_configuration(source_file, destination_file, from_provider)
+
+
 @app.command("log", help="Inferless models logs (view build logs or call logs)")
 def log_def(
     model_id: str = typer.Argument(None, help="Model id or model import id"),
     import_logs: bool = typer.Option(False, "--import-logs", "-i", help="Import logs"),
     logs_type: str = typer.Option(
         "BUILD", "--type", "-t", help="Logs type [BUILD, CALL]]"
     ),
@@ -164,17 +198,64 @@
 def run_local_def(
     runtime: str = typer.Option(
         None,
         "--runtime",
         "-r",
         help="custom runtime config file path to override from inferless-runtime-config.yaml",
     ),
+    runtime_type: str = typer.Option(
+        None,
+        "--type",
+        "-t",
+        help="Type of runtime to run [inferless, replicate]",
+    ),
+    name: str = typer.Option(
+        "inferless-model",
+        "--name",
+        "-n",
+        help="Name of the model to deploy on inferless",
+    ),
+    env_file: Optional[str] = typer.Option(
+        None,
+        "--env-file",
+        "-f",
+        help="Path to an env file containing environment variables (one per line in KEY=VALUE format)",
+    ),
+    env_vars: List[str] = typer.Option(
+        [],
+        "--env",
+        "-e",
+        help="Environment variables to set for the runtime (e.g. 'KEY=VALUE'). If the env variable contains special chars please escape them.",
+    ),
 ):
     callback_with_auth_validation()
-    run.local_run(runtime)
+    if runtime_type is not None and runtime_type not in PROVIDER_CHOICES:
+        rich.print(
+            f"Error: '--type' must be one of {PROVIDER_CHOICES}, got '{runtime_type}' instead."
+        )
+        raise typer.Exit(code=1)
+
+    if runtime_type is None and runtime is not None:
+        rich.print(
+            "[yellow]Type not given. Assuming type as Inferless.[/yellow]"
+        )
+        runtime_type = "inferless"
+
+    env_dict = {}
+    if env_file:
+        with open(env_file, "r") as f:
+            for line in f:
+                key, value = line.strip().split("=", 1)
+                env_dict[key] = value
+
+    for env_var in env_vars:
+        key, value = env_var.split("=", 1)
+        env_dict[key] = value
+
+    run.local_run(runtime, runtime_type, name, env_dict)
 
 
 @app.command("login", help="Login to Inferless")
 def login_def():
     min_version_required()
     login.login_prompt()
```

### Comparing `inferless_cli-1.1.1/inferless_cli/prompts/deploy.py` & `inferless_cli-1.1.2/inferless_cli/prompts/deploy.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import time
 import os
 import tempfile
 import typer
+
 from inferless_cli.utils.helpers import (
     create_yaml,
     create_zip_file,
     decrypt_tokens,
+    get_current_mode,
     get_default_machine_values,
     is_inferless_yaml_present,
     log_exception,
     read_json,
     read_yaml,
     yaml,
 )
@@ -22,14 +24,15 @@
     set_env_variables,
     update_model_configuration,
     upload_io,
     validate_import_model,
     start_import_model,
     upload_file,
     validate_github_url_permissions,
+    create_presigned_io_upload_url,
 )
 
 from inferless_cli.utils.constants import GITHUB, GIT
 
 
 def deploy_local(config_file_name, redeploy):
     is_yaml_present = is_inferless_yaml_present(config_file_name)
@@ -181,19 +184,44 @@
                 rich.print(e)
                 raise typer.Exit(1)
             io_schema = False
             if "io_schema" in config:
                 io_schema = config["io_schema"]
 
             if not io_schema:
-                inputs = read_json(config["optional"]["input_file_name"])
-                outputs = read_json(config["optional"]["output_file_name"])
+                # inputs = read_json(config["optional"]["input_file_name"])
+                # outputs = read_json(config["optional"]["output_file_name"])
                 try:
+                    input_file_name = f"{model_id}/input.json"
+                    output_file_name = f"{model_id}/output.json"
+                    input_payload = {
+                        "url_for": "INPUT_OUTPUT_JSON_UPLOAD",
+                        "file_name": input_file_name,
+                    }
+                    output_payload = {
+                        "url_for": "INPUT_OUTPUT_JSON_UPLOAD",
+                        "file_name": output_file_name,
+                    }
+                    create_presigned_io_upload_url(
+                        input_payload, config["optional"]["input_file_name"]
+                    )
+                    create_presigned_io_upload_url(
+                        output_payload, config["optional"]["output_file_name"]
+                    )
+                    S3_BUCKET_NAME = "infer-data"
+                    if get_current_mode() == "DEV":
+                        S3_BUCKET_NAME = "infer-data-dev"
+                    s3_input_url = f"s3://{S3_BUCKET_NAME}/{input_file_name}"
+                    s3_output_url = f"s3://{S3_BUCKET_NAME}/{output_file_name}"
                     _ = upload_io(
-                        {"id": model_id, "input_json": inputs, "output_json": outputs}
+                        {
+                            "id": model_id,
+                            "input_json": {"s3_infer_data_url": s3_input_url},
+                            "output_json": {"s3_infer_data_url": s3_output_url},
+                        }
                     )
                 except Exception as e:
                     rich.print(e)
                     raise typer.Exit(1)
             # inputs = read_json(config["optional"]["input_file_name"])
             # outputs = read_json(config["optional"]["output_file_name"])
             # try:
@@ -371,19 +399,44 @@
         if "model_import" in details:
             model_id = details["model_import"]["id"]
             io_schema = False
             if "io_schema" in config:
                 io_schema = config["io_schema"]
 
             if not io_schema:
-                inputs = read_json(config["optional"]["input_file_name"])
-                outputs = read_json(config["optional"]["output_file_name"])
+                # inputs = read_json(config["optional"]["input_file_name"])
+                # outputs = read_json(config["optional"]["output_file_name"])
                 try:
+                    input_file_name = f"{model_id}/input.json"
+                    output_file_name = f"{model_id}/output.json"
+                    input_payload = {
+                        "url_for": "INPUT_OUTPUT_JSON_UPLOAD",
+                        "file_name": input_file_name,
+                    }
+                    output_payload = {
+                        "url_for": "INPUT_OUTPUT_JSON_UPLOAD",
+                        "file_name": output_file_name,
+                    }
+                    create_presigned_io_upload_url(
+                        input_payload, config["optional"]["input_file_name"]
+                    )
+                    create_presigned_io_upload_url(
+                        output_payload, config["optional"]["output_file_name"]
+                    )
+                    S3_BUCKET_NAME = "infer-data"
+                    if get_current_mode() == "DEV":
+                        S3_BUCKET_NAME = "infer-data-dev"
+                    s3_input_url = f"s3://{S3_BUCKET_NAME}/{input_file_name}"
+                    s3_output_url = f"s3://{S3_BUCKET_NAME}/{output_file_name}"
                     _ = upload_io(
-                        {"id": model_id, "input_json": inputs, "output_json": outputs}
+                        {
+                            "id": model_id,
+                            "input_json": {"s3_infer_data_url": s3_input_url},
+                            "output_json": {"s3_infer_data_url": s3_output_url},
+                        }
                     )
                 except Exception as e:
                     rich.print(e)
                     raise typer.Exit(1)
 
             progress.update(task_id, description="Validating the model...")
             try:
```

### Comparing `inferless_cli-1.1.1/inferless_cli/prompts/init.py` & `inferless_cli-1.1.2/inferless_cli/prompts/init.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.1/inferless_cli/prompts/log.py` & `inferless_cli-1.1.2/inferless_cli/prompts/log.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.1/inferless_cli/prompts/login.py` & `inferless_cli-1.1.2/inferless_cli/prompts/login.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.1/inferless_cli/prompts/model.py` & `inferless_cli-1.1.2/inferless_cli/prompts/model.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.1/inferless_cli/prompts/run.py` & `inferless_cli-1.1.2/inferless_cli/prompts/run.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,345 +32,363 @@
 from inferless_cli.utils.services import (
     create_presigned_download_url,
     get_cli_files,
     get_file_download,
     get_templates_list,
     get_volume_info_with_id,
 )
+from inferless_cli.utils.convertors import Convertors
 
 MODEL_DIR_STRING = "##model_dir_path##"
 
 
-def local_run(runtime: str):
+def local_run(runtime: str, runtime_type: str, name: str, env_dict: dict):
     if not is_docker_running():
         rich.print("[red]Docker is not running.[/red]")
         raise typer.Exit(1)
     _, _, _, workspace_id, _ = decrypt_tokens()
-    is_yaml_present = is_inferless_yaml_present(DEFAULT_YAML_FILE_NAME)
     volume_path = None
-    if is_yaml_present:
-        with Progress(
-            SpinnerColumn(),
-            TextColumn("[progress.description]{task.description}"),
-            transient=True,
-        ) as progress:
-            task_id = progress.add_task(description="Setting up things...", total=None)
+    with Progress(
+        SpinnerColumn(),
+        TextColumn("[progress.description]{task.description}"),
+        transient=True,
+    ) as progress:
+        task_id = progress.add_task(description="Setting up things...", total=None)
+        is_yaml_present = is_inferless_yaml_present(DEFAULT_YAML_FILE_NAME)
+        if not is_yaml_present:
+            config = {
+                "name": name,
+                "source_framework_type": "PYTORCH",
+                "io_schema": True,
+                "env": env_dict,
+            }
+        else:
             config = read_yaml(DEFAULT_YAML_FILE_NAME)
-            if (
-                config
-                and "configuration" in config
-                and "custom_volume_id" in config["configuration"]
-                and config["configuration"]["custom_volume_id"]
-            ):
-                progress.update(
-                    task_id, description="Getting your Volume Mount details..."
-                )
-                volume_data = find_volume_by_id(
-                    workspace_id, config["configuration"]["custom_volume_id"]
-                )
-                volume_path = volume_data["path"]
 
-            model_name = config["name"]
+        if runtime and runtime_type == "replicate":
+            Convertors.convert_cog_to_runtime_yaml(runtime, DEFAULT_RUNTIME_FILE_NAME)
 
-            yaml_location = DEFAULT_RUNTIME_FILE_NAME
+        # add a logic to check if inferless.yaml is present. id yes continue else check for name param is present or generate new random name. check for env variables if sent via parmas. check for runtime param and type. if the type is not inferless run inferless export command and generate inferless-runtime-config file. 
+        if (
+            config
+            and "configuration" in config
+            and "custom_volume_id" in config["configuration"]
+            and config["configuration"]["custom_volume_id"]
+        ):
+            progress.update(
+                task_id, description="Getting your Volume Mount details..."
+            )
+            volume_data = find_volume_by_id(
+                workspace_id, config["configuration"]["custom_volume_id"]
+            )
+            volume_path = volume_data["path"]
+
+        model_name = config["name"]
 
-            if runtime:
-                yaml_location = runtime
-            elif "optional" in config and "runtime_file_name" in config["optional"]:
-                yaml_location = config["optional"]["runtime_file_name"]
+        yaml_location = DEFAULT_RUNTIME_FILE_NAME
+
+        if runtime:
+            yaml_location = runtime
+        elif "optional" in config and "runtime_file_name" in config["optional"]:
+            yaml_location = config["optional"]["runtime_file_name"]
+
+        if (
+            "source_framework_type" in config
+            and config["source_framework_type"] == "PYTORCH"
+        ):
+            progress.update(
+                task_id,
+                description="Generating required files for loading model...",
+            )
+            try:
+                config_pbtxt_file_contents = get_cli_files("sample_config.pbtxt")
+                config_pbtxt_file = base64.b64decode(
+                    config_pbtxt_file_contents
+                ).decode("utf-8")
+            except Exception as e:
+                rich.print(e)
+                raise typer.Exit(1)
+            inputs = create_config_from_json(config, config_pbtxt_file)
+
+            io_schema = False
+            if "io_schema" in config:
+                io_schema = config["io_schema"]
+
+            input_schema_path = "input_schema.py"
+            data_dict = None
+            if not io_schema:
+                input_json = read_json(config["optional"]["input_file_name"])
+                output_json = read_json(config["optional"]["output_file_name"])
+
+            if os.path.exists(input_schema_path):
+                data_dict = create_input_from_schema(input_schema_path)
+                input_tensor = copy.deepcopy(data_dict["inputs"])
+                output_tensor = []
+            elif io_schema and not os.path.exists(input_schema_path):
+                rich.print(
+                    "[red]Input Schema not Found[/red]"
+                )
+            # elif io_schema and not os.path.exists(input_schema_path) then typer.exit("input schema not found")
+            elif input_json and "inputs" in input_json:
+                input_tensor = copy.deepcopy(input_json["inputs"])
+                # ! Handle this edge case
+                output_tensor = copy.deepcopy(output_json["outputs"])
+            else:
+                rich.print(
+                    "[red]Both Input Schema and Input Json are not present[/red]"
+                )
+                raise typer.Exit(1)
 
             if (
-                "source_framework_type" in config
-                and config["source_framework_type"] == "PYTORCH"
+                config
+                and "configuration" in config
+                and "is_serverless" in config["configuration"]
+                and config["configuration"]["is_serverless"]
             ):
-                progress.update(
-                    task_id,
-                    description="Generating required files for loading model...",
-                )
                 try:
-                    config_pbtxt_file_contents = get_cli_files("sample_config.pbtxt")
-                    config_pbtxt_file = base64.b64decode(
-                        config_pbtxt_file_contents
-                    ).decode("utf-8")
+                    model_py_file_contents = get_cli_files(
+                        "default_serverless_model.py"
+                    )
+                    model_py_file = base64.b64decode(model_py_file_contents).decode(
+                        "utf-8"
+                    )
                 except Exception as e:
                     rich.print(e)
                     raise typer.Exit(1)
-                inputs = create_config_from_json(config, config_pbtxt_file)
-
-                io_schema = False
-                if "io_schema" in config:
-                    io_schema = config["io_schema"]
-
-                input_schema_path = "input_schema.py"
-                data_dict = None
-                if not io_schema:
-                    input_json = read_json(config["optional"]["input_file_name"])
-                    output_json = read_json(config["optional"]["output_file_name"])
-
-                if os.path.exists(input_schema_path):
-                    data_dict = create_input_from_schema(input_schema_path)
-                    input_tensor = copy.deepcopy(data_dict["inputs"])
-                    output_tensor = []
-                elif input_json and "inputs" in input_json:
-                    input_tensor = copy.deepcopy(input_json["inputs"])
-                    # ! Handle this edge case
-                    output_tensor = copy.deepcopy(output_json["outputs"])
-                else:
-                    rich.print(
-                        "[red]Both Input Schema and Input Json are not present[/red]"
+            elif data_dict and "batch_size" in data_dict:
+                try:
+                    model_py_file_contents = get_cli_files("default_batch_model.py")
+                    model_py_file = base64.b64decode(model_py_file_contents).decode(
+                        "utf-8"
                     )
+                except Exception as e:
+                    rich.print(e)
                     raise typer.Exit(1)
-
-                if (
-                    config
-                    and "configuration" in config
-                    and "is_serverless" in config["configuration"]
-                    and config["configuration"]["is_serverless"]
-                ):
-                    try:
-                        model_py_file_contents = get_cli_files(
-                            "default_serverless_model.py"
-                        )
-                        model_py_file = base64.b64decode(model_py_file_contents).decode(
-                            "utf-8"
-                        )
-                    except Exception as e:
-                        rich.print(e)
-                        raise typer.Exit(1)
-                elif data_dict and "batch_size" in data_dict:
-                    try:
-                        model_py_file_contents = get_cli_files("default_batch_model.py")
-                        model_py_file = base64.b64decode(model_py_file_contents).decode(
-                            "utf-8"
-                        )
-                    except Exception as e:
-                        rich.print(e)
-                        raise typer.Exit(1)
-                else:
-                    try:
-                        model_py_file_contents = get_cli_files("default_model.py")
-                        model_py_file = base64.b64decode(model_py_file_contents).decode(
-                            "utf-8"
-                        )
-                    except Exception as e:
-                        rich.print(e)
-                        raise typer.Exit(1)
-
-                generate_template_model(input_tensor, output_tensor, model_py_file)
             else:
-                inputs = get_inputs_from_input_json(config)
-
-            runtime_id = None
-            runtime_url = None
-            if (
-                "configuration" in config
-                and "custom_runtime_id" in config["configuration"]
-            ):
                 try:
-                    runtimes_list = get_templates_list(workspace_id)
+                    model_py_file_contents = get_cli_files("default_model.py")
+                    model_py_file = base64.b64decode(model_py_file_contents).decode(
+                        "utf-8"
+                    )
                 except Exception as e:
                     rich.print(e)
                     raise typer.Exit(1)
-                runtime_id = config["configuration"]["custom_runtime_id"]
 
-                for item in runtimes_list:
-                    # Use .get() for safer access to dictionary items
-                    item_id = item.get("id")
-                    if item_id == runtime_id:
-                        runtime_url = item.get("template_url")
-                        break  # Exit the loop since we found the matching item
+            generate_template_model(input_tensor, output_tensor, model_py_file)
+        else:
+            inputs = get_inputs_from_input_json(config)
+
+        runtime_id = None
+        runtime_url = None
+        if (
+            runtime is None
+            and "configuration" in config
+            and "custom_runtime_id" in config["configuration"]
+        ):
+            try:
+                runtimes_list = get_templates_list(workspace_id)
+            except Exception as e:
+                rich.print(e)
+                raise typer.Exit(1)
+            runtime_id = config["configuration"]["custom_runtime_id"]
+
+            for item in runtimes_list:
+                # Use .get() for safer access to dictionary items
+                item_id = item.get("id")
+                if item_id == runtime_id:
+                    runtime_url = item.get("template_url")
+                    break  # Exit the loop since we found the matching item
+
+        BUILDING_DOCKER_MSG = (
+            "Building the Docker Image (Might take some time. Please wait...)"
+        )
+        if runtime_id and not runtime_url:
+            rich.print(
+                f"[yellow]runtime with id: {runtime_id}, not found! Please check if the rutime is avaliabe in current workspace"
+            )
 
-            BUILDING_DOCKER_MSG = (
-                "Building the Docker Image (Might take some time. Please wait...)"
+        if os.path.exists(yaml_location):
+            progress.update(
+                task_id,
+                description="Analysing your runtime config...",
             )
-            if runtime_id and not runtime_url:
-                rich.print(
-                    f"[yellow]runtime with id: {runtime_id}, not found! Please check if the rutime is avaliabe in current workspace"
+            try:
+                docker_file_contents = get_cli_files("default_template_dockerfile")
+                default_template_dockerfile = base64.b64decode(
+                    docker_file_contents
+                ).decode("utf-8")
+            except Exception as e:
+                rich.print(e)
+                raise typer.Exit(1)
+            default_template_dockerfile = default_template_dockerfile.replace(
+                MODEL_DIR_STRING, f"/models/{model_name}/1/"
+            )
+            if (
+                "source_framework_type" in config
+                and config["source_framework_type"] == "PYTORCH"
+            ):
+                default_template_dockerfile = default_template_dockerfile.replace(
+                    "##configpbtxt##",
+                    f"COPY config.pbtxt /models/{model_name}/",
+                )
+            with open(yaml_location, "r") as yaml_file:
+                default_template_dockerfile = load_yaml_file(
+                    yaml_file, default_template_dockerfile
                 )
 
-            if os.path.exists(yaml_location):
                 progress.update(
                     task_id,
-                    description="Analysing your runtime config...",
+                    description=BUILDING_DOCKER_MSG,
                 )
+                build_docker_image(default_template_dockerfile)
+        elif runtime_url and runtime_id:
+            progress.update(
+                task_id,
+                description="Analysing your runtime config...",
+            )
+            runtime_url = runtime_url.split("/")
+            filename = (
+                runtime_url[len(runtime_url) - 2]
+                + "/"
+                + runtime_url[len(runtime_url) - 1]
+            )
+            payload = {
+                "url_for": "YAML_FILE_DOWNLOAD",
+                "file_name": filename,
+            }
+            try:
+                res = create_presigned_download_url(payload)
+                response = get_file_download(res)
+            except Exception as e:
+                rich.print(e)
+                raise typer.Exit(1)
+            if response.status_code == 200:
+                yaml_file = response.content
                 try:
-                    docker_file_contents = get_cli_files("default_template_dockerfile")
+                    docker_file_contents = get_cli_files(
+                        "default_template_dockerfile"
+                    )
                     default_template_dockerfile = base64.b64decode(
                         docker_file_contents
                     ).decode("utf-8")
                 except Exception as e:
                     rich.print(e)
                     raise typer.Exit(1)
                 default_template_dockerfile = default_template_dockerfile.replace(
                     MODEL_DIR_STRING, f"/models/{model_name}/1/"
                 )
+                default_template_dockerfile = load_yaml_file(
+                    yaml_file, default_template_dockerfile
+                )
                 if (
                     "source_framework_type" in config
                     and config["source_framework_type"] == "PYTORCH"
                 ):
-                    default_template_dockerfile = default_template_dockerfile.replace(
-                        "##configpbtxt##",
-                        f"COPY config.pbtxt /models/{model_name}/",
-                    )
-
-                with open(yaml_location, "r") as yaml_file:
-                    default_template_dockerfile = load_yaml_file(
-                        yaml_file, default_template_dockerfile
-                    )
-
-                    progress.update(
-                        task_id,
-                        description=BUILDING_DOCKER_MSG,
-                    )
-                    build_docker_image(default_template_dockerfile)
-            elif runtime_url and runtime_id:
-                progress.update(
-                    task_id,
-                    description="Analysing your runtime config...",
-                )
-                runtime_url = runtime_url.split("/")
-                filename = (
-                    runtime_url[len(runtime_url) - 2]
-                    + "/"
-                    + runtime_url[len(runtime_url) - 1]
-                )
-                payload = {
-                    "url_for": "YAML_FILE_DOWNLOAD",
-                    "file_name": filename,
-                }
-                try:
-                    res = create_presigned_download_url(payload)
-                    response = get_file_download(res)
-                except Exception as e:
-                    rich.print(e)
-                    raise typer.Exit(1)
-                if response.status_code == 200:
-                    yaml_file = response.content
-                    try:
-                        docker_file_contents = get_cli_files(
-                            "default_template_dockerfile"
+                    default_template_dockerfile = (
+                        default_template_dockerfile.replace(
+                            "##configpbtxt##",
+                            f"COPY config.pbtxt /models/{model_name}/",
                         )
-                        default_template_dockerfile = base64.b64decode(
-                            docker_file_contents
-                        ).decode("utf-8")
-                    except Exception as e:
-                        rich.print(e)
-                        raise typer.Exit(1)
-                    default_template_dockerfile = default_template_dockerfile.replace(
-                        MODEL_DIR_STRING, f"/models/{model_name}/1/"
                     )
-                    default_template_dockerfile = load_yaml_file(
-                        yaml_file, default_template_dockerfile
-                    )
-                    if (
-                        "source_framework_type" in config
-                        and config["source_framework_type"] == "PYTORCH"
-                    ):
-                        default_template_dockerfile = (
-                            default_template_dockerfile.replace(
-                                "##configpbtxt##",
-                                f"COPY config.pbtxt /models/{model_name}/",
-                            )
-                        )
-
-                    progress.update(
-                        task_id,
-                        description=BUILDING_DOCKER_MSG,
-                    )
-                    build_docker_image(default_template_dockerfile)
-            else:
-                rich.print(
-                    "\n[yellow]No Custom runtime dectected. Using Inferless default runtime [/yellow]\n"
-                )
-                try:
-                    requirements_text_contents = get_cli_files("requirements.txt")
-                    requirements_text = base64.b64decode(
-                        requirements_text_contents
-                    ).decode("utf-8")
-                except Exception as e:
-                    rich.print(e)
-                    raise typer.Exit(1)
 
-                requirements_lines = requirements_text.strip().split("\n")
-                requirements_lines = [
-                    line
-                    for line in requirements_lines
-                    if not line.strip().startswith("#")
-                ]
-                pip_install_commands = "\n".join(
-                    f"RUN pip install --no-cache-dir {line}"
-                    for line in requirements_lines
-                    if line.strip()
-                )
-                try:
-                    docker_file_contents = get_cli_files("default_dockerfile")
-                    default_dockerfile = base64.b64decode(docker_file_contents).decode(
-                        "utf-8"
-                    )
-                except Exception as e:
-                    rich.print(e)
-                    raise typer.Exit(1)
-                default_dockerfile = default_dockerfile.replace(
-                    MODEL_DIR_STRING, f"/models/{model_name}/1/"
-                )
-                default_dockerfile = default_dockerfile.replace(
-                    "##localdependencies##", pip_install_commands
-                )
-                if (
-                    "source_framework_type" in config
-                    and config["source_framework_type"] == "PYTORCH"
-                ):
-                    default_dockerfile = default_dockerfile.replace(
-                        "##configpbtxt##", f"COPY config.pbtxt /models/{model_name}/"
-                    )
                 progress.update(
                     task_id,
                     description=BUILDING_DOCKER_MSG,
                 )
-                build_docker_image(default_dockerfile)
-
-            rich.print("[green]Docker Image Successfully Built.[/green]\n")
-            files_to_delete = ["config.pbtxt", "model.py"]
-            delete_files(files_to_delete)
-            progress.update(
-                task_id,
-                description="Starting the Docker Container...",
+                build_docker_image(default_template_dockerfile)
+        else:
+            rich.print(
+                "\n[yellow]No Custom runtime dectected. Using Inferless default runtime [/yellow]\n"
+            )
+            try:
+                requirements_text_contents = get_cli_files("requirements.txt")
+                requirements_text = base64.b64decode(
+                    requirements_text_contents
+                ).decode("utf-8")
+            except Exception as e:
+                rich.print(e)
+                raise typer.Exit(1)
+
+            requirements_lines = requirements_text.strip().split("\n")
+            requirements_lines = [
+                line
+                for line in requirements_lines
+                if not line.strip().startswith("#")
+            ]
+            pip_install_commands = "\n".join(
+                f"RUN pip install --no-cache-dir {line}"
+                for line in requirements_lines
+                if line.strip()
+            )
+            try:
+                docker_file_contents = get_cli_files("default_dockerfile")
+                default_dockerfile = base64.b64decode(docker_file_contents).decode(
+                    "utf-8"
+                )
+            except Exception as e:
+                rich.print(e)
+                raise typer.Exit(1)
+            default_dockerfile = default_dockerfile.replace(
+                MODEL_DIR_STRING, f"/models/{model_name}/1/"
+            )
+            default_dockerfile = default_dockerfile.replace(
+                "##localdependencies##", pip_install_commands
             )
-            env_vars = {}
-            if "env" in config:
-                env_vars = config["env"]
-
-            # Start Docker container
-            stop_containers_using_port_8000()
             if (
                 "source_framework_type" in config
                 and config["source_framework_type"] == "PYTORCH"
             ):
-                start_docker_container(
-                    volume_path=volume_path, autostart=False, env=env_vars
-                )
-                time.sleep(10)
-                load_model_template(model_name)
-                time.sleep(5)
-                infer_model(model_name, inputs)
-                unload_model_template(model_name)
-                load_model_template(model_name)
-            else:
-                start_docker_container(
-                    volume_path=volume_path, autostart=True, env=env_vars
+                default_dockerfile = default_dockerfile.replace(
+                    "##configpbtxt##", f"COPY config.pbtxt /models/{model_name}/"
                 )
+            progress.update(
+                task_id,
+                description=BUILDING_DOCKER_MSG,
+            )
+            build_docker_image(default_dockerfile)
 
-            progress.remove_task(task_id)
-
-            rich.print("[green]Container started successfully.[/green]\n")
-            rich.print(
-                "\n[bold][yellow]Note: [/yellow][/bold]Container usually takes around 15 to 20 seconds to expose the PORT. cURL command should work after that.\n"
+        rich.print("[green]Docker Image Successfully Built.[/green]\n")
+        files_to_delete = ["config.pbtxt", "model.py"]
+        delete_files(files_to_delete)
+        progress.update(
+            task_id,
+            description="Starting the Docker Container...",
+        )
+        env_vars = {}
+        if "env" in config:
+            env_vars = config["env"]
+
+        # Start Docker container
+        stop_containers_using_port_8000()
+        if (
+            "source_framework_type" in config
+            and config["source_framework_type"] == "PYTORCH"
+        ):
+            start_docker_container(
+                volume_path=volume_path, autostart=False, env=env_vars
+            )
+            time.sleep(10)
+            load_model_template(model_name)
+            time.sleep(5)
+            infer_model(model_name, inputs)
+            unload_model_template(model_name)
+            load_model_template(model_name)
+        else:
+            start_docker_container(
+                volume_path=volume_path, autostart=True, env=env_vars
             )
-            rich.print("\n[bold][underline]CURL COMMAND[/underline][/bold]\n")
-            print_curl_command(model_name, inputs)
+
+        progress.remove_task(task_id)
+
+        rich.print("[green]Container started successfully.[/green]\n")
+        rich.print(
+            "\n[bold][yellow]Note: [/yellow][/bold]Container usually takes around 15 to 20 seconds to expose the PORT. cURL command should work after that.\n"
+        )
+        rich.print("\n[bold][underline]CURL COMMAND[/underline][/bold]\n")
+        print_curl_command(model_name, inputs)
 
 
 def create_requirements_file(requirements_text):
     with open("inferless_requirements.txt", "w") as f:
         f.write(requirements_text)
```

### Comparing `inferless_cli-1.1.1/inferless_cli/prompts/runtime.py` & `inferless_cli-1.1.2/inferless_cli/prompts/runtime.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.1/inferless_cli/prompts/secret.py` & `inferless_cli-1.1.2/inferless_cli/prompts/secret.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.1/inferless_cli/prompts/token.py` & `inferless_cli-1.1.2/inferless_cli/prompts/token.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.1/inferless_cli/prompts/volume.py` & `inferless_cli-1.1.2/inferless_cli/prompts/volume.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.1/inferless_cli/prompts/workspace.py` & `inferless_cli-1.1.2/inferless_cli/prompts/workspace.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.1/inferless_cli/utils/api.py` & `inferless_cli-1.1.2/inferless_cli/utils/api.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.1/inferless_cli/utils/constants.py` & `inferless_cli-1.1.2/inferless_cli/utils/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -465,7 +465,11 @@
     # you can add more python packages here
   system_packages:
     # - "libssl-dev" #example
     # you can add system packages here
 """
 
 GLITCHTIP_DSN = "https://7d9a4e0478da4efaa34b1f5c8191b820@app.glitchtip.com/5058"
+
+
+PROVIDER_CHOICES = ["replicate", "inferless"]
+PROVIDER_EXPORT_CHOICES = list(set(PROVIDER_CHOICES) - set(["inferless"]))
```

### Comparing `inferless_cli-1.1.1/inferless_cli/utils/credentials.py` & `inferless_cli-1.1.2/inferless_cli/utils/credentials.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.1/inferless_cli/utils/helpers.py` & `inferless_cli-1.1.2/inferless_cli/utils/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -262,14 +262,27 @@
     else:
         _, _, token, refresh_token, user_id, workspace_id, workspace_name, _ = (
             load_credentials()
         )
         return (token, refresh_token, user_id, workspace_id, workspace_name)
 
 
+def get_current_mode():
+    if is_keyring_supported():
+        try:
+            mode = KEYRING.get_password("Inferless", "mode")
+            return mode
+        except Exception as e:
+            log_exception(e)
+            return None
+    else:
+        _, _, _, _, _, _, _, mode = load_credentials()
+        return mode
+
+
 def is_inferless_yaml_present(file_path=DEFAULT_YAML_FILE_NAME):
     file_name = file_path
     current_dir = os.getcwd()
     file_path = os.path.join(current_dir, file_name)
 
     return os.path.isfile(file_path)
 
@@ -611,27 +624,28 @@
     try:
         client = docker.from_env()
 
         # Create a temporary tarball for Docker build context using NamedTemporaryFile
         with NamedTemporaryFile(delete=False, suffix=".tar.gz") as temp_tar:
             dockerfile_tar_path = temp_tar.name
             with tarfile.open(name=dockerfile_tar_path, mode="w:gz") as tar:
-                # Add Dockerfile to tarball
-                dockerfile = BytesIO(dockerfile_content.encode("utf-8"))
-                info = tarfile.TarInfo(name="Dockerfile")
-                info.size = len(dockerfile.getvalue())
-                tar.addfile(tarinfo=info, fileobj=dockerfile)
 
                 # Walk through the context_path directory and add all files to the tarball
                 for root, dirs, files in os.walk(context_path):
                     for file in files:
                         file_path = os.path.join(root, file)
                         arcname = os.path.relpath(file_path, start=context_path)
                         tar.add(file_path, arcname=arcname)
 
+                # Add Dockerfile to tarball
+                dockerfile = BytesIO(dockerfile_content.encode("utf-8"))
+                info = tarfile.TarInfo(name="Dockerfile")
+                info.size = len(dockerfile.getvalue())
+                tar.addfile(tarinfo=info, fileobj=dockerfile)
+
         # Build image using the temporary tarball as context
         with open(dockerfile_tar_path, "rb") as fileobj:
             image, _ = client.images.build(
                 fileobj=fileobj,
                 tag="inferless-inference",
                 rm=True,
                 custom_context=True,
```

### Comparing `inferless_cli-1.1.1/inferless_cli/utils/services.py` & `inferless_cli-1.1.2/inferless_cli/utils/services.py`

 * *Files 2% similar despite different names*

```diff
@@ -840,7 +840,48 @@
         if not response.json().get("details"):
             raise Exception(NO_DETAILS_MSG)
 
         return response.json()["details"]
     except Exception as e:
         log_exception(e)
         raise Exception("Failed to get required utils file.")
+
+
+def create_presigned_io_upload_url(payload, path):
+    try:
+        response = make_request(PRESIGNED_URL, method="POST", auth=True, data=payload)
+
+        data = response.json()
+        if data:
+            return upload_io_file(data["details"], path)
+        else:
+            raise Exception(f"Upload failed with status code {response.status_code}")
+    except Exception as e:
+        log_exception(e)
+        raise Exception(FAILED_TO_CREATE_MESSAGE)
+
+
+def upload_io_file(url, path):
+    try:
+        file_size = os.path.getsize(path)
+        with open(path, "rb") as file:
+            response = make_request(
+                url,
+                method="PUT",
+                data="" if file_size == 0 else file,
+                auth=False,
+                convert_json=False,
+                headers={
+                    "Content-Type": "text/json",
+                },
+            )
+            if response.status_code == 200:
+                return {
+                    "status": "success",
+                }
+            else:
+                raise Exception(
+                    f"Upload failed with status code {response.status_code}"
+                )
+    except Exception as e:
+        log_exception(e)
+        raise Exception(FAILED_TO_CREATE_MESSAGE)
```

### Comparing `inferless_cli-1.1.1/inferless_cli/utils/validators.py` & `inferless_cli-1.1.2/inferless_cli/utils/validators.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.1/pyproject.toml` & `inferless_cli-1.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "inferless-cli"
-version = "1.1.1"
+version = "1.1.2"
 description = "Inferless - Deploy Machine Learning Models in Minutes."
 authors = ["Naveen <naveen@inferless.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 inferless = "inferless_cli.main:app"
```

### Comparing `inferless_cli-1.1.1/PKG-INFO` & `inferless_cli-1.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inferless-cli
-Version: 1.1.1
+Version: 1.1.2
 Summary: Inferless - Deploy Machine Learning Models in Minutes.
 Author: Naveen
 Author-email: naveen@inferless.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -41,14 +41,15 @@
 
 * `-v, --version`
 * `--help`: Show this message and exit.
 
 **Commands**:
 
 * `deploy`: Deploy a model to Inferless
+* `export`: Export the runtime configuration of...
 * `init`: Initialize a new Inferless model
 * `log`: Inferless models logs (view build logs or...
 * `login`: Login to Inferless
 * `mode`: Change mode
 * `model`: Manage Inferless models (list , delete ,...
 * `run`: Run a model locally
 * `runtime`: Manage Inferless runtimes (can be used to...
@@ -67,14 +68,31 @@
 $ inferless deploy [OPTIONS]
 ```
 
 **Options**:
 
 * `--help`: Show this message and exit.
 
+## `inferless export`
+
+Export the runtime configuration of another provider to Inferless runtime config
+
+**Usage**:
+
+```console
+$ inferless export [OPTIONS]
+```
+
+**Options**:
+
+* `-r, --runtime TEXT`: The runtime configuration file of another provider  [default: cog.yaml]
+* `-d, --destination TEXT`: The destination file for the Inferless runtime configuration  [default: inferless-runtime-config.yaml]
+* `-f, --from TEXT`: The provider from which to export the runtime configuration  [default: replicate]
+* `--help`: Show this message and exit.
+
 ## `inferless init`
 
 Initialize a new Inferless model
 
 **Usage**:
 
 ```console
@@ -259,14 +277,18 @@
 ```console
 $ inferless run [OPTIONS]
 ```
 
 **Options**:
 
 * `-r, --runtime TEXT`: custom runtime config file path to override from inferless-runtime-config.yaml
+* `-t, --type TEXT`: Type of runtime to run [inferless, replicate]
+* `-n, --name TEXT`: Name of the model to deploy on inferless  [default: inferless-model]
+* `-f, --env-file TEXT`: Path to an env file containing environment variables (one per line in KEY=VALUE format)
+* `-e, --env TEXT`: Environment variables to set for the runtime (e.g. 'KEY=VALUE'). If the env variable contains special chars please escape them.
 * `--help`: Show this message and exit.
 
 ## `inferless runtime`
 
 Manage Inferless runtimes (can be used to list runtimes and upload new runtimes)
 
 **Usage**:
```

