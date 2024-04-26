# Comparing `tmp/aaz-dev-2.6.1.tar.gz` & `tmp/aaz_dev-2.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aaz-dev-2.6.1.tar", last modified: Fri Mar 15 08:49:20 2024, max compression
+gzip compressed data, was "aaz_dev-2.6.2.tar", last modified: Fri Apr 26 07:25:41 2024, max compression
```

## Comparing `aaz-dev-2.6.1.tar` & `aaz_dev-2.6.2.tar`

### file list

```diff
@@ -1,248 +1,248 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 08:49:20.935454 aaz-dev-2.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11698 2024-03-15 08:48:51.000000 aaz-dev-2.6.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-03-15 08:48:51.000000 aaz-dev-2.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-03-15 08:48:51.000000 aaz-dev-2.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9137 2024-03-15 08:49:20.935454 aaz-dev-2.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7897 2024-03-15 08:48:51.000000 aaz-dev-2.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-15 08:49:20.935454 aaz-dev-2.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 08:49:20.891455 aaz-dev-2.6.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 08:49:20.899455 aaz-dev-2.6.1/src/aaz_dev/
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 08:49:20.899455 aaz-dev-2.6.1/src/aaz_dev/app/
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/app/app.py
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/app/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     5784 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/app/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/app/url_converters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 08:49:20.899455 aaz-dev-2.6.1/src/aaz_dev/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 08:49:20.899455 aaz-dev-2.6.1/src/aaz_dev/cli/api/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/cli/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9728 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/cli/api/_cmds.py
--rw-r--r--   0 runner    (1001) docker     (127)     7277 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/cli/api/az.py
--rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/cli/api/portal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 08:49:20.903455 aaz-dev-2.6.1/src/aaz_dev/cli/controller/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/cli/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18546 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/cli/controller/az_arg_group_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    14917 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/cli/controller/az_atomic_profile_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/cli/controller/az_client_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/cli/controller/az_command_ctx.py
--rw-r--r--   0 runner    (1001) docker     (127)    15508 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/cli/controller/az_command_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    27670 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/cli/controller/az_module_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    39660 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/cli/controller/az_operation_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/cli/controller/az_output_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9401 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/cli/controller/az_profile_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8924 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/cli/controller/az_selector_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    19027 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/cli/controller/portal_cli_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 08:49:20.903455 aaz-dev-2.6.1/src/aaz_dev/cli/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/cli/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 08:49:20.903455 aaz-dev-2.6.1/src/aaz_dev/cli/model/atomic/
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/cli/model/atomic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/cli/model/atomic/_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/cli/model/atomic/_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/cli/model/atomic/_command_group.py
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/cli/model/atomic/_example.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/cli/model/atomic/_help.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/cli/model/atomic/_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/cli/model/atomic/_resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 08:49:20.903455 aaz-dev-2.6.1/src/aaz_dev/cli/model/common/
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/cli/model/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/cli/model/common/_fields.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 08:49:20.907455 aaz-dev-2.6.1/src/aaz_dev/cli/model/view/
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/cli/model/view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/cli/model/view/_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/cli/model/view/_command_group.py
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/cli/model/view/_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/cli/model/view/_profile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 08:49:20.907455 aaz-dev-2.6.1/src/aaz_dev/cli/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/cli/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/cli/templates/_filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 08:49:20.907455 aaz-dev-2.6.1/src/aaz_dev/cli/templates/aaz/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/cli/templates/aaz/__init__.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 08:49:20.907455 aaz-dev-2.6.1/src/aaz_dev/cli/templates/aaz/command/
--rw-r--r--   0 runner    (1001) docker     (127)    31956 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/cli/templates/aaz/command/_cmd.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 08:49:20.907455 aaz-dev-2.6.1/src/aaz_dev/cli/templates/aaz/group/
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/cli/templates/aaz/group/__cmd_group.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/cli/templates/aaz/group/__init__.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 08:49:20.907455 aaz-dev-2.6.1/src/aaz_dev/cli/templates/aaz/profile/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/cli/templates/aaz/profile/__init__.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/cli/templates/aaz/profile/_clients.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 08:49:20.907455 aaz-dev-2.6.1/src/aaz_dev/cli/templates/extension/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/cli/templates/extension/HISTORY.rst.j2
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/cli/templates/extension/README.md.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 08:49:20.907455 aaz-dev-2.6.1/src/aaz_dev/cli/templates/extension/azext_/
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/cli/templates/extension/azext_/__init__.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/cli/templates/extension/azext_/_help.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/cli/templates/extension/azext_/_params.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/cli/templates/extension/azext_/commands.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/cli/templates/extension/azext_/custom.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 08:49:20.907455 aaz-dev-2.6.1/src/aaz_dev/cli/templates/extension/azext_/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/cli/templates/extension/azext_/tests/__init__.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 08:49:20.907455 aaz-dev-2.6.1/src/aaz_dev/cli/templates/extension/azext_/tests/profile/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/cli/templates/extension/azext_/tests/profile/__init__.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/cli/templates/extension/azext_/tests/profile/test_.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/cli/templates/extension/setup.cfg.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/cli/templates/extension/setup.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)    18306 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/cli/templates/macros.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 08:49:20.911455 aaz-dev-2.6.1/src/aaz_dev/cli/templates/main/
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/cli/templates/main/__init__.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/cli/templates/main/_help.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/cli/templates/main/_params.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/cli/templates/main/commands.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/cli/templates/main/custom.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 08:49:20.911455 aaz-dev-2.6.1/src/aaz_dev/cli/templates/main/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/cli/templates/main/tests/__init__.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 08:49:20.911455 aaz-dev-2.6.1/src/aaz_dev/cli/templates/main/tests/profile/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/cli/templates/main/tests/profile/__init__.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/cli/templates/main/tests/profile/test_.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/cli/templates/python.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 08:49:20.911455 aaz-dev-2.6.1/src/aaz_dev/command/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/command/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 08:49:20.911455 aaz-dev-2.6.1/src/aaz_dev/command/api/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/command/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10167 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/command/api/_cmds.py
--rw-r--r--   0 runner    (1001) docker     (127)    28013 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/command/api/editor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/command/api/specs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 08:49:20.911455 aaz-dev-2.6.1/src/aaz_dev/command/controller/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/command/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42226 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/command/controller/cfg_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/command/controller/cfg_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/command/controller/client_cfg_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    25715 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/command/controller/specs_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    68895 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/command/controller/workspace_cfg_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/command/controller/workspace_client_cfg_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/command/controller/workspace_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    48777 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/command/controller/workspace_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 08:49:20.915454 aaz-dev-2.6.1/src/aaz_dev/command/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/command/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 08:49:20.919454 aaz-dev-2.6.1/src/aaz_dev/command/model/configuration/
--rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/command/model/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26834 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/command/model/configuration/_arg.py
--rw-r--r--   0 runner    (1001) docker     (127)    16496 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/command/model/configuration/_arg_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/command/model/configuration/_arg_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    17525 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/command/model/configuration/_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    16144 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/command/model/configuration/_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/command/model/configuration/_command_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/command/model/configuration/_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/command/model/configuration/_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     7024 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/command/model/configuration/_content.py
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/command/model/configuration/_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     4989 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/command/model/configuration/_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)    10501 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/command/model/configuration/_format.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/command/model/configuration/_help.py
--rw-r--r--   0 runner    (1001) docker     (127)    16687 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/command/model/configuration/_http.py
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/command/model/configuration/_http_request_body.py
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/command/model/configuration/_http_response_body.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/command/model/configuration/_instance_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/command/model/configuration/_instance_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/command/model/configuration/_instance_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     6195 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/command/model/configuration/_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/command/model/configuration/_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/command/model/configuration/_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    37141 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/command/model/configuration/_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    13845 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/command/model/configuration/_selector_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/command/model/configuration/_subresource_selector.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/command/model/configuration/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/command/model/configuration/_xml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 08:49:20.919454 aaz-dev-2.6.1/src/aaz_dev/command/model/editor/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/command/model/editor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/command/model/editor/_workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 08:49:20.919454 aaz-dev-2.6.1/src/aaz_dev/command/model/specs/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/command/model/specs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/command/model/specs/_command_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/command/model/specs/_resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 08:49:20.919454 aaz-dev-2.6.1/src/aaz_dev/command/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/command/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/command/templates/_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/command/templates/command.md.j2
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/command/templates/group.md.j2
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/command/templates/resource_ref.md.j2
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/command/templates/tree.md.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 08:49:20.919454 aaz-dev-2.6.1/src/aaz_dev/swagger/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/swagger/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 08:49:20.919454 aaz-dev-2.6.1/src/aaz_dev/swagger/api/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/swagger/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/swagger/api/_cmds.py
--rw-r--r--   0 runner    (1001) docker     (127)     9280 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/swagger/api/specs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 08:49:20.923454 aaz-dev-2.6.1/src/aaz_dev/swagger/controller/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/swagger/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25776 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/swagger/controller/command_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6898 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/swagger/controller/specs_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 08:49:20.923454 aaz-dev-2.6.1/src/aaz_dev/swagger/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/swagger/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 08:49:20.927454 aaz-dev-2.6.1/src/aaz_dev/swagger/model/schema/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/swagger/model/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27067 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/swagger/model/schema/cmd_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/swagger/model/schema/contact.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/swagger/model/schema/external_documentation.py
--rw-r--r--   0 runner    (1001) docker     (127)    18059 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/swagger/model/schema/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/swagger/model/schema/header.py
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/swagger/model/schema/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/swagger/model/schema/items.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/swagger/model/schema/license.py
--rw-r--r--   0 runner    (1001) docker     (127)    12934 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/swagger/model/schema/operation.py
--rw-r--r--   0 runner    (1001) docker     (127)    11427 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/swagger/model/schema/parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5063 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/swagger/model/schema/path_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/swagger/model/schema/reference.py
--rw-r--r--   0 runner    (1001) docker     (127)     5486 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/swagger/model/schema/response.py
--rw-r--r--   0 runner    (1001) docker     (127)    28837 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/swagger/model/schema/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/swagger/model/schema/security_scheme.py
--rw-r--r--   0 runner    (1001) docker     (127)     5933 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/swagger/model/schema/swagger.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/swagger/model/schema/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/swagger/model/schema/x_ms_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/swagger/model/schema/x_ms_long_running_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/swagger/model/schema/x_ms_odata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/swagger/model/schema/x_ms_pageable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/swagger/model/schema/x_ms_parameter_grouping.py
--rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/swagger/model/schema/x_ms_parameterized_host.py
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/swagger/model/schema/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 08:49:20.927454 aaz-dev-2.6.1/src/aaz_dev/swagger/model/specs/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/swagger/model/specs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7003 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/swagger/model/specs/_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     9618 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/swagger/model/specs/_resource_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/swagger/model/specs/_swagger_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/swagger/model/specs/_swagger_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/swagger/model/specs/_swagger_specs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/swagger/model/specs/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 08:49:20.927454 aaz-dev-2.6.1/src/aaz_dev/swagger/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/swagger/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/swagger/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/swagger/utils/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 08:49:20.927454 aaz-dev-2.6.1/src/aaz_dev/ui/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-03-15 08:49:20.000000 aaz-dev-2.6.1/src/aaz_dev/ui/asset-manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-03-15 08:49:05.000000 aaz-dev-2.6.1/src/aaz_dev/ui/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-03-15 08:49:20.000000 aaz-dev-2.6.1/src/aaz_dev/ui/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     5347 2024-03-15 08:49:05.000000 aaz-dev-2.6.1/src/aaz_dev/ui/logo192.png
--rw-r--r--   0 runner    (1001) docker     (127)     9664 2024-03-15 08:49:05.000000 aaz-dev-2.6.1/src/aaz_dev/ui/logo512.png
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-03-15 08:49:05.000000 aaz-dev-2.6.1/src/aaz_dev/ui/manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-15 08:49:05.000000 aaz-dev-2.6.1/src/aaz_dev/ui/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 08:49:20.895455 aaz-dev-2.6.1/src/aaz_dev/ui/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 08:49:20.931454 aaz-dev-2.6.1/src/aaz_dev/ui/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-03-15 08:49:20.000000 aaz-dev-2.6.1/src/aaz_dev/ui/static/css/main.e6c13ad2.css
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-15 08:49:20.000000 aaz-dev-2.6.1/src/aaz_dev/ui/static/css/main.e6c13ad2.css.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 08:49:20.931454 aaz-dev-2.6.1/src/aaz_dev/ui/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)   659880 2024-03-15 08:49:20.000000 aaz-dev-2.6.1/src/aaz_dev/ui/static/js/main.aa1f209d.js
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-03-15 08:49:20.000000 aaz-dev-2.6.1/src/aaz_dev/ui/static/js/main.aa1f209d.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)  2745937 2024-03-15 08:49:20.000000 aaz-dev-2.6.1/src/aaz_dev/ui/static/js/main.aa1f209d.js.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 08:49:20.935454 aaz-dev-2.6.1/src/aaz_dev/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/utils/base64.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/utils/case.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/utils/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4403 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/utils/error_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/utils/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/utils/plane.py
--rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/utils/portal_file_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/src/aaz_dev/utils/stage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 08:49:20.935454 aaz-dev-2.6.1/src/aaz_dev.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9137 2024-03-15 08:49:20.000000 aaz-dev-2.6.1/src/aaz_dev.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8751 2024-03-15 08:49:20.000000 aaz-dev-2.6.1/src/aaz_dev.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 08:49:20.000000 aaz-dev-2.6.1/src/aaz_dev.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-15 08:49:20.000000 aaz-dev-2.6.1/src/aaz_dev.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-03-15 08:49:20.000000 aaz-dev-2.6.1/src/aaz_dev.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-15 08:49:20.000000 aaz-dev-2.6.1/src/aaz_dev.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-03-15 08:48:52.000000 aaz-dev-2.6.1/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.322156 aaz_dev-2.6.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11947 2024-04-26 07:25:05.000000 aaz_dev-2.6.2/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-26 07:25:05.000000 aaz_dev-2.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-26 07:25:05.000000 aaz_dev-2.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9306 2024-04-26 07:25:41.322156 aaz_dev-2.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8066 2024-04-26 07:25:05.000000 aaz_dev-2.6.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 07:25:41.322156 aaz_dev-2.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.282156 aaz_dev-2.6.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.286156 aaz_dev-2.6.2/src/aaz_dev/
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.290156 aaz_dev-2.6.2/src/aaz_dev/app/
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/app/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/app/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5784 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/app/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/app/url_converters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.290156 aaz_dev-2.6.2/src/aaz_dev/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.290156 aaz_dev-2.6.2/src/aaz_dev/cli/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9728 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/api/_cmds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7277 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/api/az.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/api/portal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.290156 aaz_dev-2.6.2/src/aaz_dev/cli/controller/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18546 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/controller/az_arg_group_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14917 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/controller/az_atomic_profile_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/controller/az_client_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/controller/az_command_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15508 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/controller/az_command_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27670 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/controller/az_module_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39660 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/controller/az_operation_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/controller/az_output_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9401 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/controller/az_profile_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8924 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/controller/az_selector_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19027 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/controller/portal_cli_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.290156 aaz_dev-2.6.2/src/aaz_dev/cli/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.294156 aaz_dev-2.6.2/src/aaz_dev/cli/model/atomic/
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/model/atomic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/model/atomic/_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/model/atomic/_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/model/atomic/_command_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/model/atomic/_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/model/atomic/_help.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/model/atomic/_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/model/atomic/_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.294156 aaz_dev-2.6.2/src/aaz_dev/cli/model/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/model/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/model/common/_fields.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.294156 aaz_dev-2.6.2/src/aaz_dev/cli/model/view/
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/model/view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/model/view/_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/model/view/_command_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/model/view/_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/model/view/_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.294156 aaz_dev-2.6.2/src/aaz_dev/cli/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/templates/_filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.294156 aaz_dev-2.6.2/src/aaz_dev/cli/templates/aaz/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/templates/aaz/__init__.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.294156 aaz_dev-2.6.2/src/aaz_dev/cli/templates/aaz/command/
+-rw-r--r--   0 runner    (1001) docker     (127)    31956 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/templates/aaz/command/_cmd.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.294156 aaz_dev-2.6.2/src/aaz_dev/cli/templates/aaz/group/
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/templates/aaz/group/__cmd_group.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/templates/aaz/group/__init__.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.294156 aaz_dev-2.6.2/src/aaz_dev/cli/templates/aaz/profile/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/templates/aaz/profile/__init__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/templates/aaz/profile/_clients.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.298156 aaz_dev-2.6.2/src/aaz_dev/cli/templates/extension/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/templates/extension/HISTORY.rst.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/templates/extension/README.md.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.298156 aaz_dev-2.6.2/src/aaz_dev/cli/templates/extension/azext_/
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/templates/extension/azext_/__init__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/templates/extension/azext_/_help.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/templates/extension/azext_/_params.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/templates/extension/azext_/commands.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/templates/extension/azext_/custom.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.298156 aaz_dev-2.6.2/src/aaz_dev/cli/templates/extension/azext_/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/templates/extension/azext_/tests/__init__.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.298156 aaz_dev-2.6.2/src/aaz_dev/cli/templates/extension/azext_/tests/profile/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/templates/extension/azext_/tests/profile/__init__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/templates/extension/azext_/tests/profile/test_.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/templates/extension/setup.cfg.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/templates/extension/setup.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)    18306 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/templates/macros.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.298156 aaz_dev-2.6.2/src/aaz_dev/cli/templates/main/
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/templates/main/__init__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/templates/main/_help.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/templates/main/_params.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/templates/main/commands.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/templates/main/custom.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.298156 aaz_dev-2.6.2/src/aaz_dev/cli/templates/main/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/templates/main/tests/__init__.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.298156 aaz_dev-2.6.2/src/aaz_dev/cli/templates/main/tests/profile/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/templates/main/tests/profile/__init__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/templates/main/tests/profile/test_.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/templates/python.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.298156 aaz_dev-2.6.2/src/aaz_dev/command/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.298156 aaz_dev-2.6.2/src/aaz_dev/command/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10167 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/api/_cmds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28013 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/api/editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/api/specs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.302156 aaz_dev-2.6.2/src/aaz_dev/command/controller/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42226 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/controller/cfg_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/controller/cfg_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/controller/client_cfg_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25715 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/controller/specs_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68895 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/controller/workspace_cfg_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/controller/workspace_client_cfg_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/controller/workspace_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48777 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/controller/workspace_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.302156 aaz_dev-2.6.2/src/aaz_dev/command/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.306156 aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26834 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_arg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16496 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_arg_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_arg_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17525 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16144 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_command_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7024 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4989 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10501 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_help.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16687 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_http_request_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_http_response_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_instance_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_instance_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_instance_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6195 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37141 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13845 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_selector_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_subresource_selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_xml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.306156 aaz_dev-2.6.2/src/aaz_dev/command/model/editor/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/editor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/editor/_workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.306156 aaz_dev-2.6.2/src/aaz_dev/command/model/specs/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/specs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/specs/_command_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/specs/_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.306156 aaz_dev-2.6.2/src/aaz_dev/command/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/templates/_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/templates/command.md.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/templates/group.md.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/templates/resource_ref.md.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/templates/tree.md.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.306156 aaz_dev-2.6.2/src/aaz_dev/swagger/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.310156 aaz_dev-2.6.2/src/aaz_dev/swagger/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/api/_cmds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9280 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/api/specs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.310156 aaz_dev-2.6.2/src/aaz_dev/swagger/controller/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25776 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/controller/command_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6898 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/controller/specs_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.310156 aaz_dev-2.6.2/src/aaz_dev/swagger/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.314156 aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27739 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/cmd_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/contact.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/external_documentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18059 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/items.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/license.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12934 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11427 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5063 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/path_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5486 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29035 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/security_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5933 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/swagger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/x_ms_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/x_ms_long_running_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/x_ms_odata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/x_ms_pageable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/x_ms_parameter_grouping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/x_ms_parameterized_host.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.314156 aaz_dev-2.6.2/src/aaz_dev/swagger/model/specs/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/model/specs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7003 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/model/specs/_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9796 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/model/specs/_resource_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/model/specs/_swagger_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/model/specs/_swagger_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/model/specs/_swagger_specs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/model/specs/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.314156 aaz_dev-2.6.2/src/aaz_dev/swagger/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/utils/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.314156 aaz_dev-2.6.2/src/aaz_dev/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-26 07:25:40.000000 aaz_dev-2.6.2/src/aaz_dev/ui/asset-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-04-26 07:25:24.000000 aaz_dev-2.6.2/src/aaz_dev/ui/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-26 07:25:40.000000 aaz_dev-2.6.2/src/aaz_dev/ui/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5347 2024-04-26 07:25:24.000000 aaz_dev-2.6.2/src/aaz_dev/ui/logo192.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9664 2024-04-26 07:25:24.000000 aaz_dev-2.6.2/src/aaz_dev/ui/logo512.png
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-26 07:25:24.000000 aaz_dev-2.6.2/src/aaz_dev/ui/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-26 07:25:24.000000 aaz_dev-2.6.2/src/aaz_dev/ui/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.286156 aaz_dev-2.6.2/src/aaz_dev/ui/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.314156 aaz_dev-2.6.2/src/aaz_dev/ui/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-26 07:25:40.000000 aaz_dev-2.6.2/src/aaz_dev/ui/static/css/main.e6c13ad2.css
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-26 07:25:40.000000 aaz_dev-2.6.2/src/aaz_dev/ui/static/css/main.e6c13ad2.css.map
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.318156 aaz_dev-2.6.2/src/aaz_dev/ui/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)   659880 2024-04-26 07:25:40.000000 aaz_dev-2.6.2/src/aaz_dev/ui/static/js/main.aa1f209d.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-26 07:25:40.000000 aaz_dev-2.6.2/src/aaz_dev/ui/static/js/main.aa1f209d.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  2745937 2024-04-26 07:25:40.000000 aaz_dev-2.6.2/src/aaz_dev/ui/static/js/main.aa1f209d.js.map
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.322156 aaz_dev-2.6.2/src/aaz_dev/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/utils/base64.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/utils/case.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/utils/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4403 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/utils/error_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/utils/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/utils/plane.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/utils/portal_file_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/utils/stage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.322156 aaz_dev-2.6.2/src/aaz_dev.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9306 2024-04-26 07:25:40.000000 aaz_dev-2.6.2/src/aaz_dev.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8751 2024-04-26 07:25:40.000000 aaz_dev-2.6.2/src/aaz_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 07:25:40.000000 aaz_dev-2.6.2/src/aaz_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-26 07:25:40.000000 aaz_dev-2.6.2/src/aaz_dev.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-26 07:25:40.000000 aaz_dev-2.6.2/src/aaz_dev.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-26 07:25:40.000000 aaz_dev-2.6.2/src/aaz_dev.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/version.py
```

### Comparing `aaz-dev-2.6.1/HISTORY.rst` & `aaz_dev-2.6.2/HISTORY.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 .. :changelog:
 
 Release History
 ===============
 
+2.6.2
+++++++
+* Refine documentation (#345, #349, #355, #356)
+* Add response schema for lro delete operation (#350)
+* Support empty free-form object (#348)
+* Display ParseJsonFailed error logs (#347)
+* Fix readOnly parsing problem in Swagger (#346)
+
 2.6.1
 ++++++
 * Adapt new polices for LRO operation (#333)
 
 2.6.0
 ++++++
 * Fix invalid URL in the document (#327)
```

### Comparing `aaz-dev-2.6.1/LICENSE` & `aaz_dev-2.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/PKG-INFO` & `aaz_dev-2.6.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aaz-dev
-Version: 2.6.1
+Version: 2.6.2
 Summary: Microsoft Atomic Azure CLI Commands Developer Tools
 Home-page: https://github.com/Azure/aaz-dev-tools
 Author: Microsoft Corporation
 Author-email: azpycli@microsoft.com
 License: MIT
 Keywords: azure
 Classifier: Development Status :: 5 - Production/Stable
@@ -33,15 +33,15 @@
 Requires-Dist: Jinja2~=3.0.3
 Requires-Dist: MarkupSafe~=2.0.1
 Requires-Dist: jsonschema~=4.17.1
 Requires-Dist: click~=8.1.2
 
 # Microsoft Atomic Azure CLI Dev Tools
 
-The *aaz-dev* tool is designed to generate atomic Azure CLI commands from OpenAPI specifications. For more information, please refer to [document](https://azure.github.io/aaz-dev-tools/) and [video](https://msit.microsoftstream.com/video/d8c50840-98dc-a27a-806a-f1ed2daa33a9).
+The *aaz-dev* tool is designed to generate atomic Azure CLI commands from OpenAPI specifications. For more information, please refer to [document](https://azure.github.io/aaz-dev-tools/) and [video](https://microsoft.sharepoint.com/teams/AzureCLITools237/_layouts/15/embed.aspx?UniqueId=97905452-69c2-4f7c-8c6b-b411c7fd0013&embed=%7B%22ust%22%3Atrue%2C%22hv%22%3A%22CopyEmbedCode%22%7D&referrer=StreamWebApp&referrerScenario=EmbedDialog.Create).
 
 ## Installation
 Currently, we can install it with a [.whl file](https://github.com/Azure/aaz-dev-tools/releases). Later on, we'll publish it to PyPI to support *pip install* way of installation.
 
 ## Setting up your development environment
 
 ### 1 Code repos
```

### Comparing `aaz-dev-2.6.1/README.md` & `aaz_dev-2.6.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Microsoft Atomic Azure CLI Dev Tools
 
-The *aaz-dev* tool is designed to generate atomic Azure CLI commands from OpenAPI specifications. For more information, please refer to [document](https://azure.github.io/aaz-dev-tools/) and [video](https://msit.microsoftstream.com/video/d8c50840-98dc-a27a-806a-f1ed2daa33a9).
+The *aaz-dev* tool is designed to generate atomic Azure CLI commands from OpenAPI specifications. For more information, please refer to [document](https://azure.github.io/aaz-dev-tools/) and [video](https://microsoft.sharepoint.com/teams/AzureCLITools237/_layouts/15/embed.aspx?UniqueId=97905452-69c2-4f7c-8c6b-b411c7fd0013&embed=%7B%22ust%22%3Atrue%2C%22hv%22%3A%22CopyEmbedCode%22%7D&referrer=StreamWebApp&referrerScenario=EmbedDialog.Create).
 
 ## Installation
 Currently, we can install it with a [.whl file](https://github.com/Azure/aaz-dev-tools/releases). Later on, we'll publish it to PyPI to support *pip install* way of installation.
 
 ## Setting up your development environment
 
 ### 1 Code repos
```

### Comparing `aaz-dev-2.6.1/setup.py` & `aaz_dev-2.6.2/setup.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/app/app.py` & `aaz_dev-2.6.2/src/aaz_dev/app/app.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/app/run.py` & `aaz_dev-2.6.2/src/aaz_dev/app/run.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/app/url_converters.py` & `aaz_dev-2.6.2/src/aaz_dev/app/url_converters.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/cli/api/_cmds.py` & `aaz_dev-2.6.2/src/aaz_dev/cli/api/_cmds.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/cli/api/az.py` & `aaz_dev-2.6.2/src/aaz_dev/cli/api/az.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/cli/api/portal.py` & `aaz_dev-2.6.2/src/aaz_dev/cli/api/portal.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/cli/controller/az_arg_group_generator.py` & `aaz_dev-2.6.2/src/aaz_dev/cli/controller/az_arg_group_generator.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/cli/controller/az_atomic_profile_builder.py` & `aaz_dev-2.6.2/src/aaz_dev/cli/controller/az_atomic_profile_builder.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/cli/controller/az_client_generator.py` & `aaz_dev-2.6.2/src/aaz_dev/cli/controller/az_client_generator.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/cli/controller/az_command_ctx.py` & `aaz_dev-2.6.2/src/aaz_dev/cli/controller/az_command_ctx.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/cli/controller/az_command_generator.py` & `aaz_dev-2.6.2/src/aaz_dev/cli/controller/az_command_generator.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/cli/controller/az_module_manager.py` & `aaz_dev-2.6.2/src/aaz_dev/cli/controller/az_module_manager.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/cli/controller/az_operation_generator.py` & `aaz_dev-2.6.2/src/aaz_dev/cli/controller/az_operation_generator.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/cli/controller/az_output_generator.py` & `aaz_dev-2.6.2/src/aaz_dev/cli/controller/az_output_generator.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/cli/controller/az_profile_generator.py` & `aaz_dev-2.6.2/src/aaz_dev/cli/controller/az_profile_generator.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/cli/controller/az_selector_generator.py` & `aaz_dev-2.6.2/src/aaz_dev/cli/controller/az_selector_generator.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/cli/controller/portal_cli_generator.py` & `aaz_dev-2.6.2/src/aaz_dev/cli/controller/portal_cli_generator.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/cli/model/atomic/_client.py` & `aaz_dev-2.6.2/src/aaz_dev/cli/model/atomic/_client.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/cli/model/atomic/_command.py` & `aaz_dev-2.6.2/src/aaz_dev/cli/model/atomic/_command.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/cli/model/atomic/_command_group.py` & `aaz_dev-2.6.2/src/aaz_dev/cli/model/atomic/_command_group.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/cli/model/atomic/_help.py` & `aaz_dev-2.6.2/src/aaz_dev/cli/model/atomic/_help.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/cli/model/atomic/_profile.py` & `aaz_dev-2.6.2/src/aaz_dev/cli/model/atomic/_profile.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/cli/model/common/_fields.py` & `aaz_dev-2.6.2/src/aaz_dev/cli/model/common/_fields.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/cli/model/view/_command.py` & `aaz_dev-2.6.2/src/aaz_dev/cli/model/view/_command.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/cli/model/view/_command_group.py` & `aaz_dev-2.6.2/src/aaz_dev/cli/model/view/_command_group.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/cli/model/view/_module.py` & `aaz_dev-2.6.2/src/aaz_dev/cli/model/view/_module.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/cli/model/view/_profile.py` & `aaz_dev-2.6.2/src/aaz_dev/cli/model/view/_profile.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/cli/templates/__init__.py` & `aaz_dev-2.6.2/src/aaz_dev/cli/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/cli/templates/_filters.py` & `aaz_dev-2.6.2/src/aaz_dev/cli/templates/_filters.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/cli/templates/aaz/command/_cmd.py.j2` & `aaz_dev-2.6.2/src/aaz_dev/cli/templates/aaz/command/_cmd.py.j2`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/cli/templates/aaz/group/__cmd_group.py.j2` & `aaz_dev-2.6.2/src/aaz_dev/cli/templates/aaz/group/__cmd_group.py.j2`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/cli/templates/aaz/profile/_clients.py.j2` & `aaz_dev-2.6.2/src/aaz_dev/cli/templates/aaz/profile/_clients.py.j2`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/cli/templates/extension/azext_/__init__.py.j2` & `aaz_dev-2.6.2/src/aaz_dev/cli/templates/extension/azext_/__init__.py.j2`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/cli/templates/extension/setup.py.j2` & `aaz_dev-2.6.2/src/aaz_dev/cli/templates/extension/setup.py.j2`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/cli/templates/macros.j2` & `aaz_dev-2.6.2/src/aaz_dev/cli/templates/macros.j2`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/cli/templates/main/__init__.py.j2` & `aaz_dev-2.6.2/src/aaz_dev/cli/templates/main/__init__.py.j2`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/command/api/_cmds.py` & `aaz_dev-2.6.2/src/aaz_dev/command/api/_cmds.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/command/api/editor.py` & `aaz_dev-2.6.2/src/aaz_dev/command/api/editor.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/command/api/specs.py` & `aaz_dev-2.6.2/src/aaz_dev/command/api/specs.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/command/controller/cfg_reader.py` & `aaz_dev-2.6.2/src/aaz_dev/command/controller/cfg_reader.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/command/controller/client_cfg_reader.py` & `aaz_dev-2.6.2/src/aaz_dev/command/controller/client_cfg_reader.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/command/controller/specs_manager.py` & `aaz_dev-2.6.2/src/aaz_dev/command/controller/specs_manager.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/command/controller/workspace_cfg_editor.py` & `aaz_dev-2.6.2/src/aaz_dev/command/controller/workspace_cfg_editor.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/command/controller/workspace_client_cfg_editor.py` & `aaz_dev-2.6.2/src/aaz_dev/command/controller/workspace_client_cfg_editor.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/command/controller/workspace_helper.py` & `aaz_dev-2.6.2/src/aaz_dev/command/controller/workspace_helper.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/command/controller/workspace_manager.py` & `aaz_dev-2.6.2/src/aaz_dev/command/controller/workspace_manager.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/command/model/configuration/__init__.py` & `aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/command/model/configuration/_arg.py` & `aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_arg.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/command/model/configuration/_arg_builder.py` & `aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_arg_builder.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/command/model/configuration/_arg_group.py` & `aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_arg_group.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/command/model/configuration/_client.py` & `aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_client.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/command/model/configuration/_command.py` & `aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_command.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/command/model/configuration/_command_group.py` & `aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_command_group.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/command/model/configuration/_condition.py` & `aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_condition.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/command/model/configuration/_configuration.py` & `aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_configuration.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/command/model/configuration/_content.py` & `aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_content.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/command/model/configuration/_fields.py` & `aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_fields.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/command/model/configuration/_format.py` & `aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_format.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/command/model/configuration/_help.py` & `aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_help.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/command/model/configuration/_http.py` & `aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_http.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/command/model/configuration/_http_request_body.py` & `aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_http_request_body.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/command/model/configuration/_http_response_body.py` & `aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_http_response_body.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/command/model/configuration/_instance_create.py` & `aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_instance_create.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/command/model/configuration/_instance_delete.py` & `aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_instance_delete.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/command/model/configuration/_instance_update.py` & `aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_instance_update.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/command/model/configuration/_operation.py` & `aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_operation.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/command/model/configuration/_output.py` & `aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_output.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/command/model/configuration/_resource.py` & `aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_resource.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/command/model/configuration/_schema.py` & `aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_schema.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/command/model/configuration/_selector_index.py` & `aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_selector_index.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/command/model/configuration/_subresource_selector.py` & `aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_subresource_selector.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/command/model/configuration/_utils.py` & `aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_utils.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/command/model/configuration/_xml.py` & `aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_xml.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/command/model/editor/_workspace.py` & `aaz_dev-2.6.2/src/aaz_dev/command/model/editor/_workspace.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/command/model/specs/_command_tree.py` & `aaz_dev-2.6.2/src/aaz_dev/command/model/specs/_command_tree.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/command/templates/__init__.py` & `aaz_dev-2.6.2/src/aaz_dev/command/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/command/templates/_filters.py` & `aaz_dev-2.6.2/src/aaz_dev/command/templates/_filters.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/command/templates/command.md.j2` & `aaz_dev-2.6.2/src/aaz_dev/command/templates/command.md.j2`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/command/templates/group.md.j2` & `aaz_dev-2.6.2/src/aaz_dev/command/templates/group.md.j2`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/swagger/api/_cmds.py` & `aaz_dev-2.6.2/src/aaz_dev/swagger/api/_cmds.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/swagger/api/specs.py` & `aaz_dev-2.6.2/src/aaz_dev/swagger/api/specs.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/swagger/controller/command_generator.py` & `aaz_dev-2.6.2/src/aaz_dev/swagger/controller/command_generator.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/swagger/controller/specs_manager.py` & `aaz_dev-2.6.2/src/aaz_dev/swagger/controller/specs_manager.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/swagger/model/schema/cmd_builder.py` & `aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/cmd_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     CMDFloat32Schema, CMDFloat32SchemaBase, \
     CMDFloat64Schema, CMDFloat64SchemaBase, \
     CMDObjectSchema, CMDObjectSchemaBase, \
     CMDArraySchema, CMDArraySchemaBase, \
     CMDClsSchema, CMDClsSchemaBase, \
     CMDHttpResponseJsonBody
 
+from swagger.model.specs._utils import operation_id_separate
 from swagger.utils import exceptions
 from .fields import MutabilityEnum
 from .response import Response
 from .schema import ReferenceSchema
 from .x_ms_pageable import XmsPageable
 from functools import reduce
 from utils.case import to_camel_case
@@ -247,29 +248,32 @@
                 else:
                     model = CMDClsSchema()
                 model.read_only = self.read_only
                 model.frozen = self.frozen
                 model._type = f"@{name}"
             else:
                 model = self(schema.ref_instance, **kwargs)
+                model.read_only = self.read_only
             return model
 
         if name not in self.cls_definitions:
             if support_cls_schema:
                 # register in cls_definitions first in case of loop reference below
                 self.cls_definitions[name] = {"count": 1}
                 model = self(schema.ref_instance, **kwargs)
+                model.read_only = self.read_only
                 if isinstance(model, (CMDObjectSchemaBase, CMDArraySchemaBase)):
                     # Important: only support object and array schema to defined as cls
                     # when self.cls_definitions[name]['count'] > 1, the loop reference exist
                     self.cls_definitions[name]['model'] = model
                 else:
                     del self.cls_definitions[name]
             else:
                 model = self(schema.ref_instance, **kwargs)
+                model.read_only = self.read_only
         else:
             if support_cls_schema:
                 self.cls_definitions[name]['count'] += 1
                 if self.in_base:
                     model = CMDClsSchemaBase()
                 else:
                     model = CMDClsSchema()
@@ -287,14 +291,15 @@
                 if 'model' not in self.cls_definitions[name]:
                     raise exceptions.InvalidSwaggerValueError(
                         msg="Find invalid reference loop",
                         key=schema.traces,
                         value=name
                     )
                 model = self(schema.ref_instance, **kwargs)
+                model.read_only = self.read_only
         return model
 
     def get_cls_definition_model(self, model):
         assert isinstance(model, CMDClsSchemaBase)
         name = model.type[1:]
         return self.cls_definitions[name]['model']
 
@@ -580,21 +585,27 @@
             success_responses.append(success_202_response)
         if success_204_response is not None:
             # append 204 No Content response at the end of success response
             success_responses.append(success_204_response)
 
         success_codes = reduce(lambda x, y: x | y, [codes for codes, _ in success_responses])
         if schema.x_ms_long_running_operation and not success_codes & {200, 201}:
-            lro_response = Response()
-            lro_response.description = "Response schema for long-running operation."
-
             if lro_schema := schema.x_ms_lro_final_state_schema:
-                lro_response.schema = lro_schema  # use `final-state-schema` as response
-
-            success_responses.append(({200, 201}, lro_response))
+                lro_response = Response()
+                lro_response.description = "Response schema for long-running operation."
+                lro_response.schema = lro_schema
+
+                success_responses.append(({200, 201}, lro_response))  # use `final-state-schema` as response
+
+            elif operation_id_separate(schema.operation_id)[-1][0] == "delete":
+                lro_response = Response()
+                lro_response.description = "Response schema for long-running operation."
+                success_responses.append(({200, 201}, lro_response))
+            else:
+                logger.warning(f"No response schema for long-running-operation: {schema.operation_id}.")
 
         # # default response
         # if 'default' not in error_responses and len(error_responses) == 1:
         #     p_resp, p_model = [*error_responses.values()][0]
         #     if p_model.body is not None:
         #         # use the current error response as default
         #         p_model.status_codes = None
```

### Comparing `aaz-dev-2.6.1/src/aaz_dev/swagger/model/schema/contact.py` & `aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/contact.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/swagger/model/schema/fields.py` & `aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/fields.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/swagger/model/schema/info.py` & `aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/info.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/swagger/model/schema/items.py` & `aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/items.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/swagger/model/schema/operation.py` & `aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/operation.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/swagger/model/schema/parameter.py` & `aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/parameter.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/swagger/model/schema/path_item.py` & `aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/path_item.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/swagger/model/schema/reference.py` & `aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/reference.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/swagger/model/schema/response.py` & `aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/response.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/swagger/model/schema/schema.py` & `aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,14 +86,17 @@
         super().link(swagger_loader, *traces)
 
         self.ref_instance, instance_traces = swagger_loader.load_ref(self.ref, *self.traces, 'ref')
         if isinstance(self.ref_instance, Linkable):
             self.ref_instance.link(swagger_loader, *instance_traces)
         if self.ref_instance.x_ms_azure_resource:
             self.x_ms_azure_resource = True
+        if self.ref_instance.read_only:
+            # inherit read only from $ref
+            self.read_only = True
 
     def to_cmd(self, builder, support_cls_schema=False, **kwargs):
         model = builder.register_cls_definition(self, support_cls_schema=support_cls_schema, **kwargs)
         if isinstance(model, CMDSchema):
             builder.setup_description(model, self)
             if self.x_ms_client_flatten:
                 model.client_flatten = True
@@ -291,14 +294,16 @@
 
         if self.ref is not None:
             self.ref_instance, instance_traces = swagger_loader.load_ref(self.ref, *self.traces, 'ref')
             if isinstance(self.ref_instance, Linkable):
                 self.ref_instance.link(swagger_loader, *instance_traces)
             if self.ref_instance.x_ms_azure_resource:
                 self.x_ms_azure_resource = True
+            if self.ref_instance.read_only:
+                self.read_only = True
 
         if self.items is not None:
             if isinstance(self.items, list):
                 for idx, item in enumerate(self.items):
                     item.link(swagger_loader, *self.traces, 'items', idx)
             else:
                 self.items.link(swagger_loader, *self.traces, 'items')
```

### Comparing `aaz-dev-2.6.1/src/aaz_dev/swagger/model/schema/security_scheme.py` & `aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/security_scheme.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/swagger/model/schema/swagger.py` & `aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/swagger.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/swagger/model/schema/tag.py` & `aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/tag.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/swagger/model/schema/x_ms_enum.py` & `aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/x_ms_enum.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/swagger/model/schema/x_ms_long_running_operation.py` & `aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/x_ms_long_running_operation.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/swagger/model/schema/x_ms_odata.py` & `aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/x_ms_odata.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/swagger/model/schema/x_ms_pageable.py` & `aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/x_ms_pageable.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/swagger/model/schema/x_ms_parameter_grouping.py` & `aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/x_ms_parameter_grouping.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/swagger/model/schema/x_ms_parameterized_host.py` & `aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/x_ms_parameterized_host.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/swagger/model/schema/xml.py` & `aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/xml.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/swagger/model/specs/_resource.py` & `aaz_dev-2.6.2/src/aaz_dev/swagger/model/specs/_resource.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/swagger/model/specs/_resource_provider.py` & `aaz_dev-2.6.2/src/aaz_dev/swagger/model/specs/_resource_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,16 +179,20 @@
                        f'\tFile: {map_path_2_repo(curr_resource.file_path)} Path: {curr_resource.path}\n'
                        f'\tFile: {map_path_2_repo(resource.file_path)} Path: {resource.path}')
         return False
 
     def _parse_resources_in_file(self, file_path):
         resources = []
 
-        with open(file_path, 'r', encoding='utf-8') as f:
-            body = json.load(f)
+        try:
+            with open(file_path, 'r', encoding='utf-8') as f:
+                body = json.load(f)
+        except Exception as err:
+            logger.error(f'InvalidSwaggerFile: {self} : ParseJsonFailed: {file_path} : {err}')
+            return resources
 
         # check swagger version
         swagger_version = body.get('swagger', None)
         if swagger_version != '2.0':
             logger.error(f'InvalidSwaggerFile: {self} : invalid swagger version {swagger_version} in file {file_path}')
             return resources
```

### Comparing `aaz-dev-2.6.1/src/aaz_dev/swagger/model/specs/_swagger_loader.py` & `aaz_dev-2.6.2/src/aaz_dev/swagger/model/specs/_swagger_loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,16 +17,20 @@
 
     def load_file(self, file_path):
         from swagger.model.schema.swagger import Swagger
         loaded = self.get_loaded(file_path)
         if loaded is not None:
             return loaded
 
-        with open(file_path, 'r', encoding='utf-8') as f:
-            body = json.load(f)
+        try:
+            with open(file_path, 'r', encoding='utf-8') as f:
+                body = json.load(f)
+        except Exception as err:
+            logger.error(f'InvalidSwaggerFile: ParseJsonFailed: {file_path} : {err}')
+            raise
 
         if 'example' in file_path.lower():
             loaded = body
         else:
             self.patch_swagger(body)
             loaded = Swagger(body)
             self.loaded_swaggers[file_path] = loaded
@@ -38,14 +42,19 @@
         """Current will patch `additionalProperties: {}` expression"""
         def _patch_list(lst):
             for item in lst:
                 if isinstance(item, dict):
                     _patch_dict(item)
 
         def _patch_dict(dct):
+            # add `additionalProperties: true` to empty object
+            if "type" in dct and dct["type"] == "object":
+                if not {*dct.keys()} - {"type", "description"}:
+                    dct["additionalProperties"] = True
+
             for key in [*dct.keys()]:
                 if key == "additionalProperties" and dct[key] == {}:
                     # replace `additionalProperties: {}` by `additionalProperties: true`
                     dct[key] = True
                 _patch(dct[key])
 
         def _patch(data):
```

### Comparing `aaz-dev-2.6.1/src/aaz_dev/swagger/model/specs/_swagger_module.py` & `aaz_dev-2.6.2/src/aaz_dev/swagger/model/specs/_swagger_module.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/swagger/model/specs/_swagger_specs.py` & `aaz_dev-2.6.2/src/aaz_dev/swagger/model/specs/_swagger_specs.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/swagger/model/specs/_utils.py` & `aaz_dev-2.6.2/src/aaz_dev/swagger/model/specs/_utils.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/swagger/utils/tools.py` & `aaz_dev-2.6.2/src/aaz_dev/swagger/utils/tools.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/ui/favicon.ico` & `aaz_dev-2.6.2/src/aaz_dev/ui/favicon.ico`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/ui/index.html` & `aaz_dev-2.6.2/src/aaz_dev/ui/index.html`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/ui/logo192.png` & `aaz_dev-2.6.2/src/aaz_dev/ui/logo192.png`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/ui/logo512.png` & `aaz_dev-2.6.2/src/aaz_dev/ui/logo512.png`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/ui/static/css/main.e6c13ad2.css.map` & `aaz_dev-2.6.2/src/aaz_dev/ui/static/css/main.e6c13ad2.css.map`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/ui/static/js/main.aa1f209d.js` & `aaz_dev-2.6.2/src/aaz_dev/ui/static/js/main.aa1f209d.js`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/ui/static/js/main.aa1f209d.js.LICENSE.txt` & `aaz_dev-2.6.2/src/aaz_dev/ui/static/js/main.aa1f209d.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/ui/static/js/main.aa1f209d.js.map` & `aaz_dev-2.6.2/src/aaz_dev/ui/static/js/main.aa1f209d.js.map`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/utils/config.py` & `aaz_dev-2.6.2/src/aaz_dev/utils/config.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/utils/error_format.py` & `aaz_dev-2.6.2/src/aaz_dev/utils/error_format.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/utils/exceptions.py` & `aaz_dev-2.6.2/src/aaz_dev/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/utils/fields.py` & `aaz_dev-2.6.2/src/aaz_dev/utils/fields.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/utils/plane.py` & `aaz_dev-2.6.2/src/aaz_dev/utils/plane.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/utils/portal_file_schema.py` & `aaz_dev-2.6.2/src/aaz_dev/utils/portal_file_schema.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev/utils/stage.py` & `aaz_dev-2.6.2/src/aaz_dev/utils/stage.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-2.6.1/src/aaz_dev.egg-info/PKG-INFO` & `aaz_dev-2.6.2/src/aaz_dev.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aaz-dev
-Version: 2.6.1
+Version: 2.6.2
 Summary: Microsoft Atomic Azure CLI Commands Developer Tools
 Home-page: https://github.com/Azure/aaz-dev-tools
 Author: Microsoft Corporation
 Author-email: azpycli@microsoft.com
 License: MIT
 Keywords: azure
 Classifier: Development Status :: 5 - Production/Stable
@@ -33,15 +33,15 @@
 Requires-Dist: Jinja2~=3.0.3
 Requires-Dist: MarkupSafe~=2.0.1
 Requires-Dist: jsonschema~=4.17.1
 Requires-Dist: click~=8.1.2
 
 # Microsoft Atomic Azure CLI Dev Tools
 
-The *aaz-dev* tool is designed to generate atomic Azure CLI commands from OpenAPI specifications. For more information, please refer to [document](https://azure.github.io/aaz-dev-tools/) and [video](https://msit.microsoftstream.com/video/d8c50840-98dc-a27a-806a-f1ed2daa33a9).
+The *aaz-dev* tool is designed to generate atomic Azure CLI commands from OpenAPI specifications. For more information, please refer to [document](https://azure.github.io/aaz-dev-tools/) and [video](https://microsoft.sharepoint.com/teams/AzureCLITools237/_layouts/15/embed.aspx?UniqueId=97905452-69c2-4f7c-8c6b-b411c7fd0013&embed=%7B%22ust%22%3Atrue%2C%22hv%22%3A%22CopyEmbedCode%22%7D&referrer=StreamWebApp&referrerScenario=EmbedDialog.Create).
 
 ## Installation
 Currently, we can install it with a [.whl file](https://github.com/Azure/aaz-dev-tools/releases). Later on, we'll publish it to PyPI to support *pip install* way of installation.
 
 ## Setting up your development environment
 
 ### 1 Code repos
```

### Comparing `aaz-dev-2.6.1/src/aaz_dev.egg-info/SOURCES.txt` & `aaz_dev-2.6.2/src/aaz_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

