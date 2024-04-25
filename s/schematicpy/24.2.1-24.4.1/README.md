# Comparing `tmp/schematicpy-24.2.1.tar.gz` & `tmp/schematicpy-24.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schematicpy-24.2.1.tar", max compression
+gzip compressed data, was "schematicpy-24.4.1.tar", max compression
```

## Comparing `schematicpy-24.2.1.tar` & `schematicpy-24.4.1.tar`

### file list

```diff
@@ -1,59 +1,58 @@
--rw-r--r--   0        0        0     1073 2024-02-22 22:30:26.223071 schematicpy-24.2.1/LICENSE
--rw-r--r--   0        0        0    17325 2024-02-22 22:30:26.223071 schematicpy-24.2.1/README.md
--rw-r--r--   0        0        0     4064 2024-02-22 22:31:39.504377 schematicpy-24.2.1/pyproject.toml
--rw-r--r--   0        0        0     1424 2024-02-22 22:30:26.227072 schematicpy-24.2.1/schematic/__init__.py
--rw-r--r--   0        0        0     1421 2024-02-22 22:30:26.227072 schematicpy-24.2.1/schematic/__main__.py
--rw-r--r--   0        0        0        0 2024-02-22 22:30:26.227072 schematicpy-24.2.1/schematic/configuration/__init__.py
--rw-r--r--   0        0        0     7438 2024-02-22 22:30:26.227072 schematicpy-24.2.1/schematic/configuration/configuration.py
--rw-r--r--   0        0        0     5034 2024-02-22 22:30:26.227072 schematicpy-24.2.1/schematic/configuration/dataclasses.py
--rw-r--r--   0        0        0      663 2024-02-22 22:30:26.227072 schematicpy-24.2.1/schematic/etc/README.md
--rw-r--r--   0        0        0    76063 2024-02-22 22:30:26.227072 schematicpy-24.2.1/schematic/etc/data_models/biothings.model.jsonld
--rw-r--r--   0        0        0  1387510 2024-02-22 22:30:26.231072 schematicpy-24.2.1/schematic/etc/data_models/schema_org.model.jsonld
--rw-r--r--   0        0        0     4414 2024-02-22 22:30:26.231072 schematicpy-24.2.1/schematic/etc/validation_schemas/class.schema.json
--rw-r--r--   0        0        0     9914 2024-02-22 22:30:26.231072 schematicpy-24.2.1/schematic/etc/validation_schemas/model.schema.json
--rw-r--r--   0        0        0     5021 2024-02-22 22:30:26.231072 schematicpy-24.2.1/schematic/etc/validation_schemas/property.schema.json
--rw-r--r--   0        0        0     3193 2024-02-22 22:30:26.231072 schematicpy-24.2.1/schematic/exceptions.py
--rw-r--r--   0        0        0    13233 2024-02-22 22:30:26.231072 schematicpy-24.2.1/schematic/help.py
--rw-r--r--   0        0        0     3415 2024-02-22 22:30:26.231072 schematicpy-24.2.1/schematic/loader.py
--rw-r--r--   0        0        0       59 2024-02-22 22:30:26.231072 schematicpy-24.2.1/schematic/manifest/__init__.py
--rw-r--r--   0        0        0    10466 2024-02-22 22:30:26.231072 schematicpy-24.2.1/schematic/manifest/commands.py
--rw-r--r--   0        0        0    89190 2024-02-22 22:30:26.231072 schematicpy-24.2.1/schematic/manifest/generator.py
--rw-r--r--   0        0        0    22966 2024-02-22 22:30:26.231072 schematicpy-24.2.1/schematic/models/GE_Helpers.py
--rw-r--r--   0        0        0       52 2024-02-22 22:30:26.231072 schematicpy-24.2.1/schematic/models/__init__.py
--rw-r--r--   0        0        0     7693 2024-02-22 22:30:26.231072 schematicpy-24.2.1/schematic/models/commands.py
--rw-r--r--   0        0        0    18010 2024-02-22 22:30:26.231072 schematicpy-24.2.1/schematic/models/metadata.py
--rw-r--r--   0        0        0    45258 2024-02-22 22:30:26.231072 schematicpy-24.2.1/schematic/models/validate_attribute.py
--rw-r--r--   0        0        0    12730 2024-02-22 22:30:26.231072 schematicpy-24.2.1/schematic/models/validate_manifest.py
--rw-r--r--   0        0        0      495 2024-02-22 22:30:26.231072 schematicpy-24.2.1/schematic/schemas/__init__.py
--rw-r--r--   0        0        0     4660 2024-02-22 22:30:26.231072 schematicpy-24.2.1/schematic/schemas/commands.py
--rw-r--r--   0        0        0     4291 2024-02-22 22:30:26.231072 schematicpy-24.2.1/schematic/schemas/curie.py
--rw-r--r--   0        0        0     6081 2024-02-22 22:30:26.231072 schematicpy-24.2.1/schematic/schemas/data_model_edges.py
--rw-r--r--   0        0        0    30011 2024-02-22 22:30:26.231072 schematicpy-24.2.1/schematic/schemas/data_model_graph.py
--rw-r--r--   0        0        0    17905 2024-02-22 22:30:26.231072 schematicpy-24.2.1/schematic/schemas/data_model_json_schema.py
--rw-r--r--   0        0        0    22193 2024-02-22 22:30:26.235072 schematicpy-24.2.1/schematic/schemas/data_model_jsonld.py
--rw-r--r--   0        0        0    12819 2024-02-22 22:30:26.235072 schematicpy-24.2.1/schematic/schemas/data_model_nodes.py
--rw-r--r--   0        0        0    22874 2024-02-22 22:30:26.235072 schematicpy-24.2.1/schematic/schemas/data_model_parser.py
--rw-r--r--   0        0        0     9561 2024-02-22 22:30:26.235072 schematicpy-24.2.1/schematic/schemas/data_model_relationships.py
--rw-r--r--   0        0        0     6924 2024-02-22 22:30:26.235072 schematicpy-24.2.1/schematic/schemas/data_model_validator.py
--rw-r--r--   0        0        0     7070 2024-02-22 22:30:26.235072 schematicpy-24.2.1/schematic/schemas/json_schema_validator.py
--rw-r--r--   0        0        0       96 2024-02-22 22:30:26.235072 schematicpy-24.2.1/schematic/store/__init__.py
--rw-r--r--   0        0        0      218 2024-02-22 22:30:26.235072 schematicpy-24.2.1/schematic/store/base.py
--rw-r--r--   0        0        0   120688 2024-02-22 22:30:26.235072 schematicpy-24.2.1/schematic/store/synapse.py
--rw-r--r--   0        0        0        0 2024-02-22 22:30:26.235072 schematicpy-24.2.1/schematic/utils/__init__.py
--rw-r--r--   0        0        0     2920 2024-02-22 22:30:26.235072 schematicpy-24.2.1/schematic/utils/cli_utils.py
--rw-r--r--   0        0        0     2870 2024-02-22 22:30:26.235072 schematicpy-24.2.1/schematic/utils/curie_utils.py
--rw-r--r--   0        0        0     9915 2024-02-22 22:30:26.235072 schematicpy-24.2.1/schematic/utils/df_utils.py
--rw-r--r--   0        0        0    10386 2024-02-22 22:30:26.235072 schematicpy-24.2.1/schematic/utils/general.py
--rw-r--r--   0        0        0     5769 2024-02-22 22:30:26.235072 schematicpy-24.2.1/schematic/utils/google_api_utils.py
--rw-r--r--   0        0        0     1221 2024-02-22 22:30:26.235072 schematicpy-24.2.1/schematic/utils/io_utils.py
--rw-r--r--   0        0        0    17546 2024-02-22 22:30:26.235072 schematicpy-24.2.1/schematic/utils/schema_utils.py
--rw-r--r--   0        0        0    10288 2024-02-22 22:30:26.235072 schematicpy-24.2.1/schematic/utils/validate_rules_utils.py
--rw-r--r--   0        0        0     3334 2024-02-22 22:30:26.235072 schematicpy-24.2.1/schematic/utils/validate_utils.py
--rw-r--r--   0        0        0      563 2024-02-22 22:30:26.235072 schematicpy-24.2.1/schematic/utils/viz_utils.py
--rw-r--r--   0        0        0      119 2024-02-22 22:30:26.235072 schematicpy-24.2.1/schematic/version.py
--rw-r--r--   0        0        0      164 2024-02-22 22:30:26.235072 schematicpy-24.2.1/schematic/visualization/__init__.py
--rw-r--r--   0        0        0    12312 2024-02-22 22:30:26.235072 schematicpy-24.2.1/schematic/visualization/attributes_explorer.py
--rw-r--r--   0        0        0     4928 2024-02-22 22:30:26.235072 schematicpy-24.2.1/schematic/visualization/commands.py
--rw-r--r--   0        0        0    40250 2024-02-22 22:30:26.235072 schematicpy-24.2.1/schematic/visualization/tangled_tree.py
--rw-r--r--   0        0        0    19958 1970-01-01 00:00:00.000000 schematicpy-24.2.1/setup.py
--rw-r--r--   0        0        0    19961 1970-01-01 00:00:00.000000 schematicpy-24.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-25 22:42:45.634479 schematicpy-24.4.1/LICENSE
+-rw-r--r--   0        0        0    18039 2024-04-25 22:42:45.634479 schematicpy-24.4.1/README.md
+-rw-r--r--   0        0        0     4129 2024-04-25 22:44:14.830276 schematicpy-24.4.1/pyproject.toml
+-rw-r--r--   0        0        0       93 2024-04-25 22:42:45.638479 schematicpy-24.4.1/schematic/__init__.py
+-rw-r--r--   0        0        0     1296 2024-04-25 22:42:45.638479 schematicpy-24.4.1/schematic/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-25 22:42:45.638479 schematicpy-24.4.1/schematic/configuration/__init__.py
+-rw-r--r--   0        0        0     7438 2024-04-25 22:42:45.638479 schematicpy-24.4.1/schematic/configuration/configuration.py
+-rw-r--r--   0        0        0     5034 2024-04-25 22:42:45.638479 schematicpy-24.4.1/schematic/configuration/dataclasses.py
+-rw-r--r--   0        0        0      663 2024-04-25 22:42:45.638479 schematicpy-24.4.1/schematic/etc/README.md
+-rw-r--r--   0        0        0    76063 2024-04-25 22:42:45.638479 schematicpy-24.4.1/schematic/etc/data_models/biothings.model.jsonld
+-rw-r--r--   0        0        0  1387510 2024-04-25 22:42:45.642479 schematicpy-24.4.1/schematic/etc/data_models/schema_org.model.jsonld
+-rw-r--r--   0        0        0     4414 2024-04-25 22:42:45.642479 schematicpy-24.4.1/schematic/etc/validation_schemas/class.schema.json
+-rw-r--r--   0        0        0     9914 2024-04-25 22:42:45.642479 schematicpy-24.4.1/schematic/etc/validation_schemas/model.schema.json
+-rw-r--r--   0        0        0     5021 2024-04-25 22:42:45.642479 schematicpy-24.4.1/schematic/etc/validation_schemas/property.schema.json
+-rw-r--r--   0        0        0     3193 2024-04-25 22:42:45.642479 schematicpy-24.4.1/schematic/exceptions.py
+-rw-r--r--   0        0        0    12587 2024-04-25 22:42:45.642479 schematicpy-24.4.1/schematic/help.py
+-rw-r--r--   0        0        0     3415 2024-04-25 22:42:45.642479 schematicpy-24.4.1/schematic/loader.py
+-rw-r--r--   0        0        0       59 2024-04-25 22:42:45.642479 schematicpy-24.4.1/schematic/manifest/__init__.py
+-rw-r--r--   0        0        0    11844 2024-04-25 22:42:45.642479 schematicpy-24.4.1/schematic/manifest/commands.py
+-rw-r--r--   0        0        0    89173 2024-04-25 22:42:45.642479 schematicpy-24.4.1/schematic/manifest/generator.py
+-rw-r--r--   0        0        0    23370 2024-04-25 22:42:45.642479 schematicpy-24.4.1/schematic/models/GE_Helpers.py
+-rw-r--r--   0        0        0       52 2024-04-25 22:42:45.642479 schematicpy-24.4.1/schematic/models/__init__.py
+-rw-r--r--   0        0        0     8057 2024-04-25 22:42:45.642479 schematicpy-24.4.1/schematic/models/commands.py
+-rw-r--r--   0        0        0    19316 2024-04-25 22:42:45.642479 schematicpy-24.4.1/schematic/models/metadata.py
+-rw-r--r--   0        0        0    83344 2024-04-25 22:42:45.642479 schematicpy-24.4.1/schematic/models/validate_attribute.py
+-rw-r--r--   0        0        0    14384 2024-04-25 22:42:45.642479 schematicpy-24.4.1/schematic/models/validate_manifest.py
+-rw-r--r--   0        0        0      515 2024-04-25 22:42:45.642479 schematicpy-24.4.1/schematic/schemas/__init__.py
+-rw-r--r--   0        0        0     5037 2024-04-25 22:42:45.646479 schematicpy-24.4.1/schematic/schemas/commands.py
+-rw-r--r--   0        0        0     6100 2024-04-25 22:42:45.646479 schematicpy-24.4.1/schematic/schemas/data_model_edges.py
+-rw-r--r--   0        0        0    36064 2024-04-25 22:42:45.646479 schematicpy-24.4.1/schematic/schemas/data_model_graph.py
+-rw-r--r--   0        0        0    18286 2024-04-25 22:42:45.646479 schematicpy-24.4.1/schematic/schemas/data_model_json_schema.py
+-rw-r--r--   0        0        0    22845 2024-04-25 22:42:45.646479 schematicpy-24.4.1/schematic/schemas/data_model_jsonld.py
+-rw-r--r--   0        0        0    13333 2024-04-25 22:42:45.646479 schematicpy-24.4.1/schematic/schemas/data_model_nodes.py
+-rw-r--r--   0        0        0    24666 2024-04-25 22:42:45.646479 schematicpy-24.4.1/schematic/schemas/data_model_parser.py
+-rw-r--r--   0        0        0     9597 2024-04-25 22:42:45.646479 schematicpy-24.4.1/schematic/schemas/data_model_relationships.py
+-rw-r--r--   0        0        0     7617 2024-04-25 22:42:45.646479 schematicpy-24.4.1/schematic/schemas/data_model_validator.py
+-rw-r--r--   0        0        0     6974 2024-04-25 22:42:45.646479 schematicpy-24.4.1/schematic/schemas/json_schema_validator.py
+-rw-r--r--   0        0        0       96 2024-04-25 22:42:45.646479 schematicpy-24.4.1/schematic/store/__init__.py
+-rw-r--r--   0        0        0      218 2024-04-25 22:42:45.646479 schematicpy-24.4.1/schematic/store/base.py
+-rw-r--r--   0        0        0   122222 2024-04-25 22:42:45.646479 schematicpy-24.4.1/schematic/store/synapse.py
+-rw-r--r--   0        0        0        0 2024-04-25 22:42:45.646479 schematicpy-24.4.1/schematic/utils/__init__.py
+-rw-r--r--   0        0        0     2936 2024-04-25 22:42:45.646479 schematicpy-24.4.1/schematic/utils/cli_utils.py
+-rw-r--r--   0        0        0     3027 2024-04-25 22:42:45.646479 schematicpy-24.4.1/schematic/utils/curie_utils.py
+-rw-r--r--   0        0        0    10358 2024-04-25 22:42:45.646479 schematicpy-24.4.1/schematic/utils/df_utils.py
+-rw-r--r--   0        0        0    10288 2024-04-25 22:42:45.646479 schematicpy-24.4.1/schematic/utils/general.py
+-rw-r--r--   0        0        0     6086 2024-04-25 22:42:45.646479 schematicpy-24.4.1/schematic/utils/google_api_utils.py
+-rw-r--r--   0        0        0     1221 2024-04-25 22:42:45.646479 schematicpy-24.4.1/schematic/utils/io_utils.py
+-rw-r--r--   0        0        0    18045 2024-04-25 22:42:45.646479 schematicpy-24.4.1/schematic/utils/schema_utils.py
+-rw-r--r--   0        0        0    11265 2024-04-25 22:42:45.646479 schematicpy-24.4.1/schematic/utils/validate_rules_utils.py
+-rw-r--r--   0        0        0     6299 2024-04-25 22:42:45.646479 schematicpy-24.4.1/schematic/utils/validate_utils.py
+-rw-r--r--   0        0        0      724 2024-04-25 22:42:45.646479 schematicpy-24.4.1/schematic/utils/viz_utils.py
+-rw-r--r--   0        0        0      119 2024-04-25 22:42:45.646479 schematicpy-24.4.1/schematic/version.py
+-rw-r--r--   0        0        0      164 2024-04-25 22:42:45.646479 schematicpy-24.4.1/schematic/visualization/__init__.py
+-rw-r--r--   0        0        0    12584 2024-04-25 22:42:45.646479 schematicpy-24.4.1/schematic/visualization/attributes_explorer.py
+-rw-r--r--   0        0        0     5809 2024-04-25 22:42:45.646479 schematicpy-24.4.1/schematic/visualization/commands.py
+-rw-r--r--   0        0        0    41350 2024-04-25 22:42:45.646479 schematicpy-24.4.1/schematic/visualization/tangled_tree.py
+-rw-r--r--   0        0        0    20658 1970-01-01 00:00:00.000000 schematicpy-24.4.1/setup.py
+-rw-r--r--   0        0        0    20649 1970-01-01 00:00:00.000000 schematicpy-24.4.1/PKG-INFO
```

### Comparing `schematicpy-24.2.1/LICENSE` & `schematicpy-24.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `schematicpy-24.2.1/README.md` & `schematicpy-24.4.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -16,17 +16,18 @@
 - [Contributors](#contributors)
 
 # Introduction
 SCHEMATIC is an acronym for _Schema Engine for Manifest Ingress and Curation_. The Python based infrastructure provides a _novel_ schema-based, metadata ingress ecosystem, that is meant to streamline the process of biomedical dataset annotation, metadata validation and submission to a data repository for various data contributors.
 
 # Installation
 ## Installation Requirements
-* Python version 3.9.0≤x<3.11.0 
+* Python version 3.9.0≤x<3.11.0
+* You need to be a registered and certified user on [`synapse.org`](https://www.synapse.org/)
 
-Note: You need to be a registered and certified user on [`synapse.org`](https://www.synapse.org/), and also have the right permissions to download the Google credentials files from Synapse.
+Note: Our credential policy for Google credentials in order to create Google sheet files from Schematic, see tutorial ['HERE'](https://scribehow.com/shared/Get_Credentials_for_Google_Drive_and_Google_Sheets_APIs_to_use_with_schematicpy__yqfcJz_rQVeyTcg0KQCINA). If you plan to use `config.yml`, please ensure that the path of `schematic_service_account_creds.json` is indicated there (see `google_sheets > service_account_creds` section)
 
 
 ## Installation guide for data curator app
 
 Create and activate a virtual environment within which you can install the package:
 
 ```
@@ -165,34 +166,38 @@
 _Note_: Paths can be specified relative to the `config.yml` file or as absolute paths.
 
 6. Login to Synapse by using the command line
 On the CLI in your virtual environment, run the following command: 
 ```
 synapse login -u <synapse username> -p <synapse password> --rememberMe
 ```
-Please make sure that you run the command before running `schematic init` below
 
 7. Obtain Google credential Files
-To obtain  ``schematic_service_account_creds.json``, please run: 
-```
-schematic init --config ~/path/to/config.yml
-```
+Running `schematic init` is no longer supported due to security concerns. To obtain  `schematic_service_account_creds.json`, please follow the instructions [here](https://scribehow.com/shared/Enable_Google_Drive_and_Google_Sheets_APIs_for_project__yqfcJz_rQVeyTcg0KQCINA). 
+
 > As v22.12.1 version of schematic, using `token` mode of authentication (in other words, using `token.pickle` and `credentials.json`) is no longer supported due to Google's decision to move away from using OAuth out-of-band (OOB) flow. Click [here](https://developers.google.com/identity/protocols/oauth2/resources/oob-migration) to learn more. 
 
 *Notes*: Use the ``schematic_service_account_creds.json`` file for the service
 account mode of authentication (*for Google services/APIs*). Service accounts 
 are special Google accounts that can be used by applications to access Google APIs 
 programmatically via OAuth2.0, with the advantage being that they do not require 
 human authorization. 
 
 *Background*: schematic uses Google’s API to generate google sheet templates that users fill in to provide (meta)data.
 Most Google sheet functionality could be authenticated with service account. However, more complex Google sheet functionality
 requires token-based authentication. As browser support that requires the token-based authentication diminishes, we are hoping to deprecate
 token-based authentication and keep only service account authentication in the future. 
 
+8. Set up pre-commit hooks
+
+This repository is configured to utilize pre-commit hooks as part of the development process. To enable these hooks, please run the following command and look for the following success message:
+```
+$ pre-commit install
+pre-commit installed at .git/hooks/pre-commit
+```
 
 ### Development process instruction
 
 For new features, bugs, enhancements
 
 1. Pull the latest code from [develop branch in the upstream repo](https://github.com/Sage-Bionetworks/schematic)
 2. Checkout a new branch develop-<feature/fix-name> from the develop branch
```

### Comparing `schematicpy-24.2.1/pyproject.toml` & `schematicpy-24.4.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core>=1.0.0",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "schematicpy"
-version = "v24.2.1"
+version = "v24.4.1"
 description = "Package for biomedical data model and metadata ingress management"
 authors = [ "Milen Nikolov <milen.nikolov@sagebase.org>", "Lingling Peng <lingling.peng@sagebase.org>", "Mialy Defelice <mialy.defelice@sagebase.org>", "Gianna Jordan <gianna.jordan@sagebase.org>", "Bruno Grande <bruno.grande@sagebase.org>", "Robert Allaway <robert.allaway@sagebionetworks.org>",]
 readme = "README.md"
 homepage = "https://github.com/Sage-Bionetworks/schematic"
 repository = "https://github.com/Sage-Bionetworks/schematic"
 documentation = "https://github.com/Sage-Bionetworks/schematic"
 keywords = [ "schema", "metadata", "validation", "data model", "linked data",]
@@ -38,55 +38,57 @@
 numpy = "^1.21.1"
 oauth2client = "^4.1.0"
 pandas = "^2.0.0"
 pygsheets = "^2.0.4"
 PyYAML = "^6.0.0"
 rdflib = "^6.0.0"
 setuptools = "^66.0.0"
-synapseclient = "^3.2.0"
+synapseclient = "^4.1.0"
 tenacity = "^8.0.1"
 toml = "^0.10.2"
 great-expectations = "^0.15.0"
 sphinx-click = "^4.0.0"
-MarkupSafe = "2.1.0"
 itsdangerous = "^2.0.0"
 openpyxl = "^3.0.9"
 pdoc = "^12.2.0"
 dateparser = "^1.1.4"
 pandarallel = "^1.6.4"
-pyopenssl = "^23.0.0"
 typing-extensions = "<4.6.0"
 dataclasses-json = "^0.6.1"
 
 [tool.poetry.extras]
-api = [ "connexion", "Flask", "Flask-Cors", "Jinja2",]
+api = [ "connexion", "Flask", "Flask-Cors", "Jinja2", "pyopenssl",]
 aws = [ "uWSGI",]
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = "--verbose"
 testpaths = [ "tests",]
 filterwarnings = [ "ignore::DeprecationWarning",]
 markers = [ "google_credentials_needed: marks tests requiring Google credentials (skipped on GitHub CI) ", "submission: tests that involve submitting manifests\n    ", "not_windows: tests that don't work on on windows machine\n    ", "schematic_api: marks tests covering API functionality (skipped on regular GitHub CI test suite)\n    ", "rule_combos: marks tests covering combinations of rules that aren't always necessary and can add significantly to CI runtime (skipped on GitHub CI unless prompted to run in commit message)\n    ", "table_operations: marks tests covering table operations that pass locally but fail on CI due to interactions with Synapse (skipped on GitHub CI)\n    ", "rule_benchmark: marks tests covering validation rule benchmarking\n    ", "synapse_credentials_needed: marks api tests that require synapse credentials to run\n    ", "empty_token: marks api tests that send empty credentials in the request\n    ",]
 
 [tool.poetry.dependencies."backports.zoneinfo"]
 markers = "python_version < \"3.9\""
 version = "^0.2.1"
 
 [tool.poetry.dependencies.schematic-db]
-version = "0.0.34"
+version = "0.0.41"
 extras = [ "synapse",]
 
+[tool.poetry.dependencies.pyopenssl]
+version = "^23.0.0"
+optional = true
+
 [tool.poetry.dependencies.connexion]
 extras = [ "swagger-ui",]
 version = "^2.8.0"
 optional = true
 
 [tool.poetry.dependencies.Flask]
-version = "^2.0.0"
+version = "2.1.3"
 optional = true
 
 [tool.poetry.dependencies.Flask-Cors]
 version = "^3.0.10"
 optional = true
 
 [tool.poetry.dependencies.uWSGI]
@@ -107,9 +109,10 @@
 pytest-rerunfailures = "^12.0"
 flake8 = "^6.0.0"
 python-dotenv = "^0.21.0"
 black = "^23.7.0"
 mypy = "^1.4.1"
 pylint = "^2.16.1"
 pytest-xdist = "^3.5.0"
+pre-commit = "^3.6.2"
 
 [tool.poetry.group.aws.dependencies]
```

### Comparing `schematicpy-24.2.1/schematic/__main__.py` & `schematicpy-24.4.1/schematic/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 #!/usr/bin/env python
-
 import logging
 import click
 import click_log
 
 from schematic.manifest.commands import (
     manifest as manifest_cli,
 )  # get manifest commands
 from schematic.models.commands import model as model_cli  # submit manifest commands
 from schematic.schemas.commands import (
     schema as schema_cli,
 )  # schema conversion commands
 from schematic.visualization.commands import (
     viz as viz_cli,
 )  # viz generation commands
-from schematic import init as init_cli  # schematic initialization commands
 
 logger = logging.getLogger()
 click_log.basic_config(logger)
 
 # dict() -> new empty dictionary
 CONTEXT_SETTINGS = dict(help_option_names=["--help", "-h"])  # help options
 
@@ -30,15 +28,14 @@
     """
     Command line interface to the `schematic` backend services.
     """
     logger.info("Starting schematic...")
     logger.debug("Existing sub-commands need to be used with schematic.")
 
 
-main.add_command(init_cli)  # add init commands
 main.add_command(manifest_cli)  # add manifest commands
 main.add_command(model_cli)  # add model commands
 main.add_command(schema_cli)  # add schema commands
 main.add_command(viz_cli)  # add viz commands
 
 
 if __name__ == "__main__":
```

### Comparing `schematicpy-24.2.1/schematic/configuration/configuration.py` & `schematicpy-24.4.1/schematic/configuration/configuration.py`

 * *Files identical despite different names*

### Comparing `schematicpy-24.2.1/schematic/configuration/dataclasses.py` & `schematicpy-24.4.1/schematic/configuration/dataclasses.py`

 * *Files identical despite different names*

### Comparing `schematicpy-24.2.1/schematic/etc/README.md` & `schematicpy-24.4.1/schematic/etc/README.md`

 * *Files identical despite different names*

### Comparing `schematicpy-24.2.1/schematic/etc/data_models/biothings.model.jsonld` & `schematicpy-24.4.1/schematic/etc/data_models/biothings.model.jsonld`

 * *Files identical despite different names*

### Comparing `schematicpy-24.2.1/schematic/etc/data_models/schema_org.model.jsonld` & `schematicpy-24.4.1/schematic/etc/data_models/schema_org.model.jsonld`

 * *Files identical despite different names*

### Comparing `schematicpy-24.2.1/schematic/etc/validation_schemas/class.schema.json` & `schematicpy-24.4.1/schematic/etc/validation_schemas/class.schema.json`

 * *Files identical despite different names*

### Comparing `schematicpy-24.2.1/schematic/etc/validation_schemas/model.schema.json` & `schematicpy-24.4.1/schematic/etc/validation_schemas/model.schema.json`

 * *Files identical despite different names*

### Comparing `schematicpy-24.2.1/schematic/etc/validation_schemas/property.schema.json` & `schematicpy-24.4.1/schematic/etc/validation_schemas/property.schema.json`

 * *Files identical despite different names*

### Comparing `schematicpy-24.2.1/schematic/exceptions.py` & `schematicpy-24.4.1/schematic/exceptions.py`

 * *Files identical despite different names*

### Comparing `schematicpy-24.2.1/schematic/help.py` & `schematicpy-24.4.1/schematic/help.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,38 @@
 """Help messages for CLI commands"""
 # pylint: disable=line-too-long
 #!/usr/bin/env python3
 
+from typing import get_args
+from schematic.utils.schema_utils import DisplayLabelType
+from schematic.visualization.tangled_tree import FigureType, TextType
+
+
+DATA_MODEL_LABELS_DICT = {
+    "display_label": "use the display name as a label, if it is valid (contains no blacklisted characters) otherwise will default to class_label.",
+    "class_label": "default, use standard class or property label.",
+}
+# Ensure that all DisplayLabelTypes have a description
+assert sorted(DATA_MODEL_LABELS_DICT.keys()) == sorted(get_args(DisplayLabelType))
+
+# Combine each label and its description into one string
+DATA_MODEL_LABELS_LIST = [
+    f"{label}, {description}" for label, description in DATA_MODEL_LABELS_DICT.items()
+]
+
+DATA_MODEL_LABELS_HELP = (
+    "Choose how to set the label in the data model. "
+    f"{' '.join(DATA_MODEL_LABELS_LIST)} "
+    "Do not change from default unless there is a real need, using 'display_label' can have consequences if not used properly."
+)
+
+
+FIGURE_TYPES = " or ".join([f"'{item}'" for item in get_args(FigureType)])
+TEXT_TYPES = " or ".join([f"'{item}'" for item in get_args(TextType)])
+
 # `schematic manifest` related sub-commands description
 manifest_commands = {
     "manifest": {
         "config": (
             "Specify the path to the `config.yml` using this option. This is a required argument."
         ),
         "get": {
@@ -50,20 +77,15 @@
                 "You can either explicitly pass the `.json` file here or provide it in the `config.yml` file "
                 "as a value for the `(model > location)` key."
             ),
             "alphabetize_valid_values": (
                 "Specify to alphabetize valid attribute values either ascending (a) or descending (d)."
                 "Optional"
             ),
-            "data_model_labels": (
-                "Choose how to set the label in the data model. "
-                "display_label, use the display name as a label, if it is valid (contains no blacklisted characters) otherwise will default to class_label. "
-                "class_label, default, use standard class or property label. "
-                "Do not change from default unless there is a real need, using 'display_label' can have consequences if not used properly."
-            ),
+            "data_model_labels": DATA_MODEL_LABELS_HELP,
         },
         "migrate": {
             "short_help": (
                 "Specify the path to the `config.yml` using this option. "
                 "This is a required argument."
             ),
             "project_scope": (
@@ -79,14 +101,24 @@
             "dry_run": (
                 "This is a boolean flag. If flag is provided when command line utility is executed, "
                 "a dry run will be performed. No manifests will be re-uploaded and no entities will be migrated, "
                 "but archival folders will still be created. "
                 "Migration information for testing purposes will be logged to the INFO level."
             ),
         },
+        "download": {
+            "short_help": ("Function to download manifest from asset store (Synapse)."),
+            "dataset_id": (
+                "Specify the synID of a dataset folder on Synapse. If there is an exisiting manifest already present "
+                "in that folder, then it will be pulled with the existing annotations for further annotation/modification. "
+            ),
+            "new_manifest_name": (
+                "Specify the new name to download the manifest file as."
+            ),
+        },
     }
 }
 
 
 # `schematic model` related sub-commands description
 model_commands = {
     "model": {
@@ -135,20 +167,18 @@
                 "Attribute display names in the schema must not only include characters that are "
                 "not accepted by Synapse. Annotation names may only contain: letters, numbers, '_' and '.'"
             ),
             "table_column_names": (
                 "class_label, display_label, display_name, default, class_label. When true annotations and table columns will be uploaded with the display name formatting with blacklisted characters removed. "
                 "To use for tables, use in conjunction with the use_schema_label flag."
             ),
-            "data_model_labels": (
-                "Choose how to set the label in the data model. "
-                "display_label, use the display name as a label, if it is valid (contains no blacklisted characters) otherwise will default to class_label. "
-                "class_label, default, use standard class or property label. "
-                "Do not change from default unless there is a real need, using 'display_label' can have consequences if not used properly."
+            "file_annotations_upload": (
+                "This is a boolean flag. Default to True. If False, annotations will not be added to files during submission."
             ),
+            "data_model_labels": DATA_MODEL_LABELS_HELP,
         },
         "validate": {
             "short_help": ("Validation of manifest files."),
             "manifest_path": (
                 "Specify the path to the metadata manifest file that you want to submit to a dataset on Synapse. "
                 "This is a required argument."
             ),
@@ -166,20 +196,15 @@
                 "This is a boolean flag. If flag is provided when command line utility is executed, validation suite will only run with in-house validation rules, "
                 "and Great Expectations rules and suite will not be utilized."
                 "If not, the Great Expectations suite will be utilized and all rules will be available."
             ),
             "project_scope": (
                 "Specify a comma-separated list of projects to search through for cross manifest validation."
             ),
-            "data_model_labels": (
-                "Choose how to set the label in the data model. "
-                "display_label, use the display name as a label, if it is valid (contains no blacklisted characters) otherwise will default to class_label. "
-                "class_label, default, use standard class or property label. "
-                "Do not change from default unless there is a real need, using 'display_label' can have consequences if not used properly."
-            ),
+            "data_model_labels": DATA_MODEL_LABELS_HELP,
         },
     }
 }
 
 
 # `schematic schema` related sub-commands description
 schema_commands = {
@@ -187,49 +212,28 @@
         "convert": {
             "short_help": (
                 "Convert specification from CSV data model to JSON-LD data model."
             ),
             "output_jsonld": (
                 "Path to where the generated JSON-LD file needs to be outputted."
             ),
-            "data_model_labels": (
-                "Choose how to set the label in the data model. "
-                "display_label, use the display name as a label, if it is valid (contains no blacklisted characters) otherwise will default to class_label. "
-                "class_label, default, use standard class or property label. "
-                "Do not change from default unless there is a real need, using 'display_label' can have consequences if not used properly."
-            ),
+            "data_model_labels": DATA_MODEL_LABELS_HELP,
         }
     }
 }
 
-
-# `schematic init` command description
-init_command = {
-    "init": {
-        "short_help": ("Initialize authentication for schematic."),
-        "config": (
-            "Specify the path to the `config.yml` using this option. This is a required argument."
-        ),
-    }
-}
-
 viz_commands = {
     "visualization": {
         "config": (
             "Specify the path to the `config.yml` using this option. This is a required argument."
         ),
         "tangled_tree": {
             "figure_type": (
-                "Specify the type of schema visualization to make. Either 'dependency' or 'component'."
+                f"Specify the type of schema visualization to make. Either {FIGURE_TYPES}."
             ),
             "text_format": (
-                "Specify the type of text to gather for tangled tree visualization, either 'plain' or 'highlighted'."
-            ),
-            "data_model_labels": (
-                "Choose how to set the label in the data model. "
-                "display_label, use the display name as a label, if it is valid (contains no blacklisted characters) otherwise will default to class_label. "
-                "class_label, default, use standard class or property label. "
-                "Do not change from default unless there is a real need, using 'display_label' can have consequences if not used properly."
+                f"Specify the type of text to gather for tangled tree visualization, either {TEXT_TYPES}."
             ),
+            "data_model_labels": DATA_MODEL_LABELS_HELP,
         },
     }
 }
```

### Comparing `schematicpy-24.2.1/schematic/loader.py` & `schematicpy-24.4.1/schematic/loader.py`

 * *Files identical despite different names*

### Comparing `schematicpy-24.2.1/schematic/manifest/commands.py` & `schematicpy-24.4.1/schematic/manifest/commands.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,25 @@
+import json
 import os
+import pandas as pd
 import logging
 from pathlib import Path
 import sys
-from typing import List
+from typing import get_args, List
 import click
 import click_log
 
 from schematic.schemas.data_model_parser import DataModelParser
 from schematic.schemas.data_model_graph import DataModelGraph, DataModelGraphExplorer
 from schematic.manifest.generator import ManifestGenerator
 
+from schematic.utils.schema_utils import DisplayLabelType
 from schematic.utils.cli_utils import log_value_from_config, query_dict, parse_syn_ids
 from schematic.utils.google_api_utils import export_manifest_csv
+
 from schematic.help import manifest_commands
 
 from schematic.store.synapse import SynapseStorage
 from schematic.configuration.configuration import CONFIG
 
 logger = logging.getLogger("schematic")
 click_log.basic_config(logger)
@@ -105,15 +109,15 @@
     default="ascending",
     help=query_dict(manifest_commands, ("manifest", "get", "alphabetize_valid_values")),
 )
 @click.option(
     "--data_model_labels",
     "-dml",
     default="class_label",
-    type=click.Choice(["display_label", "class_label"], case_sensitive=True),
+    type=click.Choice(list(get_args(DisplayLabelType)), case_sensitive=True),
     help=query_dict(manifest_commands, ("manifest", "get", "data_model_labels")),
 )
 @click.pass_obj
 def get_manifest(
     ctx,
     title,
     data_type,
@@ -149,15 +153,15 @@
     parsed_data_model = data_model_parser.parse_model()
 
     # Instantiate DataModelGraph
     data_model_grapher = DataModelGraph(parsed_data_model, data_model_labels)
 
     # Generate graph
     logger.info("Generating data model graph.")
-    graph_data_model = data_model_grapher.generate_data_model_graph()
+    graph_data_model = data_model_grapher.graph
 
     def create_single_manifest(data_type, output_csv=None, output_xlsx=None):
         # create object of type ManifestGenerator
         manifest_generator = ManifestGenerator(
             path_to_data_model=path_to_data_model,
             graph=graph_data_model,
             title=t,
@@ -313,9 +317,51 @@
                 project, jsonld, dry_run
             )
         if archive_project:
             logging.info("Migrating entitites")
             synStore.move_entities_to_new_project(
                 project, archive_project, return_entities, dry_run
             )
-
     return
+
+
+@manifest.command(
+    "download",
+    short_help=query_dict(manifest_commands, ("manifest", "download", "short_help")),
+)
+@click_log.simple_verbosity_option(logger)
+# define the optional arguments
+@click.option(
+    "-d",
+    "--dataset_id",
+    help=query_dict(manifest_commands, ("manifest", "download", "dataset_id")),
+)
+@click.option(
+    "-nmn",
+    "--new_manifest_name",
+    default="",
+    help=query_dict(manifest_commands, ("manifest", "download", "new_manifest_name")),
+)
+@click.pass_obj
+def download_manifest(ctx, dataset_id, new_manifest_name):
+    master_fileview = CONFIG["synapse"]["master_fileview"]
+
+    # use Synapse Storage
+    store = SynapseStorage()
+
+    # download existing file
+    manifest_data = store.getDatasetManifest(
+        datasetId=dataset_id, downloadFile=True, newManifestName=new_manifest_name
+    )
+
+    if not manifest_data:
+        logger.error(
+            "'Dataset_id provided is not able to return a manifest, please check that the id is the parent folder containing the manifest."
+        )
+        sys.exit(1)
+
+    # return local file path
+    manifest_local_file_path = manifest_data["path"]
+    logger.info(
+        f"The manifest has been downloaded to the following location: {manifest_local_file_path}"
+    )
+    return manifest_local_file_path
```

### Comparing `schematicpy-24.2.1/schematic/manifest/generator.py` & `schematicpy-24.4.1/schematic/manifest/generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1136,15 +1136,15 @@
         for i, req in enumerate(ordered_metadata_fields[0]):
             # Gather validation rules and valid values for attribute.
             validation_rules = self.dmge.get_node_validation_rules(
                 node_display_name=req
             )
             if isinstance(validation_rules, dict):
                 validation_rules = extract_component_validation_rules(
-                    validation_rules=validation_rules, manifest_component=self.root
+                    validation_rules_dict=validation_rules, manifest_component=self.root
                 )
 
             # Add regex match validaiton rule to Google Sheets.
             if validation_rules and sheet_url:
                 requests_body = self._request_regex_match_vr_formatting(
                     validation_rules, i, spreadsheet_id, requests_body, strict
                 )
@@ -1673,15 +1673,15 @@
         # Parse Model
         parsed_data_model = data_model_parser.parse_model()
 
         # Instantiate DataModelGraph
         data_model_grapher = DataModelGraph(parsed_data_model, data_model_labels)
 
         # Generate graph
-        graph_data_model = data_model_grapher.generate_data_model_graph()
+        graph_data_model = data_model_grapher.graph
 
         # Gather all returned result urls
         all_results = []
         if data_types[0] == "all manifests":
             dmge = DataModelGraphExplorer(graph_data_model)
             component_digraph = dmge.get_digraph_by_edge_type("requiresComponent")
             components = component_digraph.nodes()
```

### Comparing `schematicpy-24.2.1/schematic/models/GE_Helpers.py` & `schematicpy-24.4.1/schematic/models/GE_Helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,19 +34,45 @@
 
 from schematic.utils.schema_utils import extract_component_validation_rules
 
 from schematic.utils.validate_utils import (
     rule_in_rule_list,
     np_array_to_str_list,
     iterable_to_str_list,
+    required_is_only_rule,
 )
 
 logger = logging.getLogger(__name__)
 
 
+# List of modifiers that users can add to a rule, that arent rules themselves.
+# as additional modifiers are added will need to update this list
+
+RULE_MODIFIERS = ["error", "warning", "strict", "like", "set", "value"]
+VALIDATION_EXPECTATION = {
+    "int": "expect_column_values_to_be_in_type_list",
+    "float": "expect_column_values_to_be_in_type_list",
+    "str": "expect_column_values_to_be_of_type",
+    "num": "expect_column_values_to_be_in_type_list",
+    "date": "expect_column_values_to_be_dateutil_parseable",
+    "recommended": "expect_column_values_to_not_be_null",
+    "protectAges": "expect_column_values_to_be_between",
+    "unique": "expect_column_values_to_be_unique",
+    "inRange": "expect_column_values_to_be_between",
+    "IsNA": "expect_column_values_to_match_regex_list",
+    # To be implemented rules with possible expectations
+    # "list": "expect_column_values_to_not_match_regex_list",
+    # "regex": "expect_column_values_to_match_regex",
+    # "url": "expect_column_values_to_be_valid_urls",
+    # "matchAtLeastOne": "expect_foreign_keys_in_column_a_to_exist_in_column_b",
+    # "matchExactlyOne": "expect_foreign_keys_in_column_a_to_exist_in_column_b",
+    # "matchNone": "expect_compound_columns_to_be_unique",
+}
+
+
 class GreatExpectationsHelpers(object):
     """
     Great Expectations helper class
 
     Provides basic utilities to:
         1) Create GE workflow specific to manifest according to validation rules
         2) Parse results dict to generate appropriate errors
@@ -130,32 +156,14 @@
             Add suite to object
         Input:
 
         Returns:
             saves expectation suite and identifier to self
 
         """
-        validation_expectation = {
-            "int": "expect_column_values_to_be_in_type_list",
-            "float": "expect_column_values_to_be_in_type_list",
-            "str": "expect_column_values_to_be_of_type",
-            "num": "expect_column_values_to_be_in_type_list",
-            "date": "expect_column_values_to_be_dateutil_parseable",
-            "recommended": "expect_column_values_to_not_match_regex_list",
-            "protectAges": "expect_column_values_to_be_between",
-            "unique": "expect_column_values_to_be_unique",
-            "inRange": "expect_column_values_to_be_between",
-            "IsNA": "expect_column_values_to_match_regex_list",
-            # To be implemented rules with possible expectations
-            # "list": "expect_column_values_to_not_match_regex_list",
-            # "regex": "expect_column_values_to_match_regex",
-            # "url": "expect_column_values_to_be_valid_urls",
-            # "matchAtLeastOne": "expect_foreign_keys_in_column_a_to_exist_in_column_b",
-            # "matchExactlyOne": "expect_foreign_keys_in_column_a_to_exist_in_column_b",
-        }
 
         # create blank expectation suite
         self.expectation_suite_name = "Manifest_test_suite"
         self.suite = self.context.add_expectation_suite(
             expectation_suite_name=self.expectation_suite_name,
         )
 
@@ -173,22 +181,29 @@
 
             # check if attribute has any rules associated with it
             if validation_rules:
                 # Check if the validation rule applies to this manifest
                 if isinstance(validation_rules, dict):
                     validation_rules = extract_component_validation_rules(
                         manifest_component=self.manifest["Component"][0],
-                        validation_rules=validation_rules,
+                        validation_rules_dict=validation_rules,
                     )
                 # iterate through all validation rules for an attribute
                 for rule in validation_rules:
                     base_rule = rule.split(" ")[0]
 
                     # check if rule has an implemented expectation
-                    if rule_in_rule_list(rule, self.unimplemented_expectations):
+                    if rule_in_rule_list(
+                        rule, self.unimplemented_expectations
+                    ) or required_is_only_rule(
+                        rule=rule,
+                        attribute=col,
+                        rule_modifiers=RULE_MODIFIERS,
+                        validation_expectation=VALIDATION_EXPECTATION,
+                    ):
                         continue
 
                     args["column"] = col
                     args["result_format"] = "COMPLETE"
 
                     # Validate num
                     if base_rule == "num":
@@ -250,15 +265,14 @@
                                 ),
                             },
                             "validation_rule": rule,
                         }
 
                     elif base_rule == ("recommended"):
                         args["mostly"] = 0.0000000001
-                        args["regex_list"] = ["^$"]
                         meta = {
                             "notes": {
                                 "format": "markdown",
                                 "content": "Expect column to not be empty. **Markdown** `Supported`",
                             },
                             "validation_rule": rule,
                         }
@@ -324,15 +338,15 @@
                         }
 
                     # add expectation for attribute to suite
                     self.add_expectation(
                         rule=rule,
                         args=args,
                         meta=meta,
-                        validation_expectation=validation_expectation,
+                        validation_expectation=VALIDATION_EXPECTATION,
                     )
 
         self.context.update_expectation_suite(
             expectation_suite=self.suite,
         )
 
         suite_identifier = ExpectationSuiteIdentifier(
@@ -364,15 +378,15 @@
         Returns:
             adds expectation to self.suite
 
         """
         # Create an Expectation
         expectation_configuration = ExpectationConfiguration(
             # Name of expectation type being added
-            expectation_type=validation_expectation[rule.split(" ")[0]],
+            expectation_type=VALIDATION_EXPECTATION[rule.split(" ")[0]],
             # add arguments and meta message
             kwargs={**args},
             meta={**meta},
         )
         # Add the Expectation to the suite
         self.suite.add_expectation(expectation_configuration=expectation_configuration)
 
@@ -507,15 +521,15 @@
                 elif (
                     validation_types[rule.split(" ")[0]]["type"] == "content_validation"
                 ):
                     vr_errors, vr_warnings = GenerateError.generate_content_error(
                         val_rule=rule,
                         attribute_name=errColumn,
                         row_num=np_array_to_str_list(np.array(indices) + 2),
-                        error_val=iterable_to_str_list(values),
+                        invalid_entry=iterable_to_str_list(values),
                         dmge=self.dmge,
                     )
                     if vr_errors:
                         errors.append(vr_errors)
                         if rule.startswith("protectAges"):
                             self.censor_ages(vr_errors, errColumn)
```

### Comparing `schematicpy-24.2.1/schematic/models/commands.py` & `schematicpy-24.4.1/schematic/models/commands.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #!/usr/bin/env python3
 
+from typing import get_args
 from gc import callbacks
 import logging
 import sys
 from time import perf_counter
 
 import click
 import click_log
@@ -16,14 +17,15 @@
     query_dict,
     parse_syn_ids,
     parse_comma_str_to_list,
 )
 from schematic.help import model_commands
 from schematic.exceptions import MissingConfigValueError
 from schematic.configuration.configuration import CONFIG
+from schematic.utils.schema_utils import DisplayLabelType
 
 logger = logging.getLogger("schematic")
 click_log.basic_config(logger)
 
 CONTEXT_SETTINGS = dict(help_option_names=["--help", "-h"])  # help options
 
 
@@ -91,14 +93,21 @@
 @click.option(
     "-rr",
     "--restrict_rules",
     is_flag=True,
     help=query_dict(model_commands, ("model", "validate", "restrict_rules")),
 )
 @click.option(
+    "--file_annotations_upload/--no-file_annotations_upload",
+    "-fa/-no-fa",
+    default=True,
+    is_flag=True,
+    help=query_dict(model_commands, ("model", "submit", "file_annotations_upload")),
+)
+@click.option(
     "-ps",
     "--project_scope",
     default=None,
     callback=parse_syn_ids,
     help=query_dict(model_commands, ("model", "validate", "project_scope")),
 )
 @click.option(
@@ -108,15 +117,15 @@
     type=click.Choice(["replace", "upsert"], case_sensitive=True),
     help=query_dict(model_commands, ("model", "submit", "table_manipulation")),
 )
 @click.option(
     "--data_model_labels",
     "-dml",
     default="class_label",
-    type=click.Choice(["display_label", "class_label"], case_sensitive=True),
+    type=click.Choice(list(get_args(DisplayLabelType)), case_sensitive=True),
     help=query_dict(model_commands, ("model", "submit", "data_model_labels")),
 )
 @click.option(
     "--table_column_names",
     "-tcn",
     default="class_label",
     type=click.Choice(
@@ -141,14 +150,15 @@
     hide_blanks,
     restrict_rules,
     project_scope,
     table_manipulation,
     data_model_labels,
     table_column_names,
     annotation_keys,
+    file_annotations_upload: bool,
 ):
     """
     Running CLI with manifest validation (optional) and submission options.
     """
 
     jsonld = CONFIG.model_location
     log_value_from_config("jsonld", jsonld)
@@ -156,25 +166,25 @@
     metadata_model = MetadataModel(
         inputMModelLocation=jsonld,
         inputMModelLocationType="local",
         data_model_labels=data_model_labels,
     )
 
     manifest_id = metadata_model.submit_metadata_manifest(
-        path_to_json_ld=jsonld,
         manifest_path=manifest_path,
         dataset_id=dataset_id,
         validate_component=validate_component,
         manifest_record_type=manifest_record_type,
         restrict_rules=restrict_rules,
         hide_blanks=hide_blanks,
         project_scope=project_scope,
         table_manipulation=table_manipulation,
         table_column_names=table_column_names,
         annotation_keys=annotation_keys,
+        file_annotations_upload=file_annotations_upload,
     )
 
     if manifest_id:
         logger.info(
             f"File at '{manifest_path}' was successfully associated "
             f"with dataset '{dataset_id}'."
         )
```

### Comparing `schematicpy-24.2.1/schematic/models/metadata.py` & `schematicpy-24.4.1/schematic/models/metadata.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,25 +49,27 @@
         # extract extension of 'inputMModelLocation'
         # ensure that it is necessarily pointing to a '.jsonld' file
 
         logger.debug(
             f"Initializing DataModelGraphExplorer object from {inputMModelLocation} schema."
         )
 
+        # self.inputMModelLocation remains for backwards compatibility
         self.inputMModelLocation = inputMModelLocation
+        self.path_to_json_ld = inputMModelLocation
 
         data_model_parser = DataModelParser(path_to_data_model=self.inputMModelLocation)
         # Parse Model
         parsed_data_model = data_model_parser.parse_model()
 
         # Instantiate DataModelGraph
         data_model_grapher = DataModelGraph(parsed_data_model, data_model_labels)
 
         # Generate graph
-        self.graph_data_model = data_model_grapher.generate_data_model_graph()
+        self.graph_data_model = data_model_grapher.graph
 
         self.dmge = DataModelGraphExplorer(self.graph_data_model)
 
         # check if the type of MModel file is "local"
         # currently, the application only supports reading from local JSON-LD files
         if inputMModelLocationType == "local":
             self.inputMModelLocationType = inputMModelLocationType
@@ -229,14 +231,15 @@
         load_args = {
             "dtype": "string",
         }
         # get annotations from manifest (array of json annotations corresponding to manifest rows)
         manifest = load_df(
             manifestPath,
             preserve_raw_input=False,
+            allow_na_values=True,
             **load_args,
         )  # read manifest csv file as is from manifest path
 
         # handler for mismatched components/data types
         # throw TypeError if the value(s) in the "Component" column differ from the selected template type
         if ("Component" in manifest.columns) and (
             (len(manifest["Component"].unique()) > 1)
@@ -310,136 +313,157 @@
 
         emptyManifestURL = mg.get_manifest()
 
         return mg.populate_manifest_spreadsheet(
             manifestPath, emptyManifestURL, return_excel=return_excel, title=title
         )
 
-    def submit_metadata_manifest(
+    def submit_metadata_manifest(  # pylint: disable=too-many-arguments, too-many-locals
         self,
         manifest_path: str,
-        path_to_json_ld: str,
         dataset_id: str,
         manifest_record_type: str,
         restrict_rules: bool,
         access_token: Optional[str] = None,
         validate_component: Optional[str] = None,
+        file_annotations_upload: bool = True,
         hide_blanks: bool = False,
-        project_scope: List = None,
+        project_scope: Optional[list] = None,
         table_manipulation: str = "replace",
         table_column_names: str = "class_label",
         annotation_keys: str = "class_label",
     ) -> str:
-        """Wrap methods that are responsible for validation of manifests for a given component, and association of the
-        same manifest file with a specified dataset.
+        """
+        Wrap methods that are responsible for validation of manifests for a given component,
+          and association of the same manifest file with a specified dataset.
+
         Args:
-            manifest_path: Path to the manifest file, which contains the metadata.
-            dataset_id: Synapse ID of the dataset on Synapse containing the metadata manifest file.
-            validate_component: Component from the schema.org schema based on which the manifest template has been generated.
-        Returns:
-            Manifest ID: If both validation and association were successful.
-        Exceptions:
+            manifest_path (str): Path to the manifest file, which contains the metadata.
+            dataset_id (str): Synapse ID of the dataset on Synapse containing the
+              metadata manifest file.
+            manifest_record_type (str): How the manifest is stored in Synapse
+            restrict_rules (bool):
+              If True: bypass great expectations and restrict rule options to
+                those implemented in house
+            access_token (Optional[str], optional): Defaults to None.
+            validate_component (Optional[str], optional): Component from the schema.org
+              schema based on which the manifest template has been generated.
+            file_annotations_upload (bool, optional): Default to True. If false, do
+              not add annotations to files. Defaults to True.
+            hide_blanks (bool, optional): Defaults to False.
+            project_scope (Optional[list], optional): Defaults to None.
+            table_manipulation (str, optional): Defaults to "replace".
+            table_column_names (str, optional): Defaults to "class_label".
+            annotation_keys (str, optional): Defaults to "class_label".
+
+        Raises:
             ValueError: When validate_component is provided, but it cannot be found in the schema.
             ValidationError: If validation against data model was not successful.
-        """
 
+        Returns:
+            str: If both validation and association were successful.
+        """
         # TODO: avoid explicitly exposing Synapse store functionality
         # just instantiate a Store class and let it decide at runtime/config
         # the store type
         syn_store = SynapseStorage(
             access_token=access_token, project_scope=project_scope
         )
         manifest_id = None
-        censored_manifest_id = None
         restrict_maniest = False
         censored_manifest_path = manifest_path.replace(".csv", "_censored.csv")
         # check if user wants to perform validation or not
         if validate_component is not None:
             try:
-                # check if the component ("class" in schema) passed as argument is valid (present in schema) or not
+                # check if the component ("class" in schema) passed as argument is valid
+                # (present in schema) or not
                 self.dmge.is_class_in_schema(validate_component)
-            except:
-                # a KeyError exception is raised when validate_component fails in the try-block above
-                # here, we are suppressing the KeyError exception and replacing it with a more
-                # descriptive ValueError exception
+            except Exception as exc:
+                # a KeyError exception is raised when validate_component fails in the
+                # try-block above here, we are suppressing the KeyError exception and
+                # replacing it with a more descriptive ValueError exception
                 raise ValueError(
                     f"The component '{validate_component}' could not be found "
-                    f"in the schema here '{path_to_json_ld}'"
-                )
+                    f"in the schema here '{self.path_to_json_ld}'"
+                ) from exc
 
             # automatic JSON schema generation and validation with that JSON schema
-            val_errors, val_warnings = self.validateModelManifest(
+            val_errors, _ = self.validateModelManifest(
                 manifestPath=manifest_path,
                 rootNode=validate_component,
                 restrict_rules=restrict_rules,
                 project_scope=project_scope,
                 access_token=access_token,
             )
 
             # if there are no errors in validation process
             if val_errors == []:
                 # upload manifest file from `manifest_path` path to entity with Syn ID `dataset_id`
                 if os.path.exists(censored_manifest_path):
-                    censored_manifest_id = syn_store.associateMetadataWithFiles(
+                    syn_store.associateMetadataWithFiles(
                         dmge=self.dmge,
                         metadataManifestPath=censored_manifest_path,
                         datasetId=dataset_id,
                         manifest_record_type=manifest_record_type,
                         hideBlanks=hide_blanks,
                         table_manipulation=table_manipulation,
                         table_column_names=table_column_names,
                         annotation_keys=annotation_keys,
+                        file_annotations_upload=file_annotations_upload,
                     )
                     restrict_maniest = True
 
                 manifest_id = syn_store.associateMetadataWithFiles(
                     dmge=self.dmge,
                     metadataManifestPath=manifest_path,
                     datasetId=dataset_id,
                     manifest_record_type=manifest_record_type,
                     hideBlanks=hide_blanks,
                     restrict_manifest=restrict_maniest,
                     table_manipulation=table_manipulation,
                     table_column_names=table_column_names,
                     annotation_keys=annotation_keys,
+                    file_annotations_upload=file_annotations_upload,
                 )
 
-                logger.info(f"No validation errors occured during validation.")
+                logger.info("No validation errors occured during validation.")
                 return manifest_id
 
             else:
                 raise ValidationError(
                     "Manifest could not be validated under provided data model. "
                     f"Validation failed with the following errors: {val_errors}"
                 )
 
         # no need to perform validation, just submit/associate the metadata manifest file
         if os.path.exists(censored_manifest_path):
-            censored_manifest_id = syn_store.associateMetadataWithFiles(
+            syn_store.associateMetadataWithFiles(
                 dmge=self.dmge,
                 metadataManifestPath=censored_manifest_path,
                 datasetId=dataset_id,
                 manifest_record_type=manifest_record_type,
                 hideBlanks=hide_blanks,
                 table_manipulation=table_manipulation,
                 table_column_names=table_column_names,
                 annotation_keys=annotation_keys,
+                file_annotations_upload=file_annotations_upload,
             )
             restrict_maniest = True
 
         manifest_id = syn_store.associateMetadataWithFiles(
             dmge=self.dmge,
             metadataManifestPath=manifest_path,
             datasetId=dataset_id,
             manifest_record_type=manifest_record_type,
             hideBlanks=hide_blanks,
             restrict_manifest=restrict_maniest,
             table_manipulation=table_manipulation,
             table_column_names=table_column_names,
             annotation_keys=annotation_keys,
+            file_annotations_upload=file_annotations_upload,
         )
 
         logger.debug(
             "Optional validation was not performed on manifest before association."
         )
 
         return manifest_id
```

### Comparing `schematicpy-24.2.1/schematic/models/validate_manifest.py` & `schematicpy-24.4.1/schematic/models/validate_manifest.py`

 * *Files 8% similar despite different names*

```diff
@@ -61,14 +61,47 @@
                 f"specified. 'list' must be first."
             )
             logger.error(error_str)
             error_message = error_str
             error_val = f"Multiple Rules: list not first"
         return ["NA", error_col, error_message, error_val]
 
+    def check_max_rule_num(
+        self,
+        validation_rules: list[str],
+        col: pd.core.series.Series,
+        errors: list[list[str]],
+    ) -> list[list[str]]:
+        """Check that user isnt applying more rule combinations than allowed. Do not consider certain rules as a part of this rule limit.
+        Args:
+            validation_rules, list: Validation rules for current manifest column/attribute being evaluated
+            col, pd.core.series.Series: the current manifest column being evaluated
+            errors, list[list[str]]: list of errors being compiled.
+        Returns:
+            errors, list[list[str]]: list of errors being compiled, with additional error list being appended if appropriate
+        """
+        # Check that attribute rules conform to limits:
+        # IsNa and required is operate differently than most rules, do not consider it as a rule for evaluating
+        # if the number of rule pairs has been exceeded.
+        if "IsNa" in validation_rules:
+            validation_rules.remove("IsNa")
+
+        if "required" in validation_rules:
+            validation_rules.remove("required")
+
+        # no more than two rules for an attribute.
+        # As more combinations get added, may want to bring out into its own function / or use validate_rules_utils?
+        if len(validation_rules) > 2:
+            errors.append(
+                self.get_multiple_types_error(
+                    validation_rules, col, error_type="too_many_rules"
+                )
+            )
+        return errors
+
     def validate_manifest_rules(
         self,
         manifest: pd.core.frame.DataFrame,
         dmge: DataModelGraphExplorer,
         restrict_rules: bool,
         project_scope: List,
         access_token: Optional[str] = None,
@@ -112,26 +145,28 @@
 
         unimplemented_expectations = [
             "url",
             "list",
             "regex.*",
             "matchAtLeastOne.*",
             "matchExactlyOne.*",
+            "matchNone.*",
         ]
 
         in_house_rules = [
             "int",
             "float",
             "num",
             "str",
             "regex.*",
             "url",
             "list",
             "matchAtLeastOne.*",
             "matchExactlyOne.*",
+            "matchNone.*",
         ]
 
         # initialize error and warning handling lists.
         errors = []
         warnings = []
 
         if not restrict_rules:
@@ -176,72 +211,70 @@
             )
             logger.debug(f"GE elapsed time {perf_counter()-t_GE}")
         else:
             logger.info("Great Expetations suite will not be utilized.")
 
         t_err = perf_counter()
         regex_re = re.compile("regex.*")
+
+        # Instantiate Validate Attribute
+        validate_attribute = ValidateAttribute(dmge=dmge)
+
         for col in manifest.columns:
             # remove trailing/leading whitespaces from manifest
             manifest.map(lambda x: x.strip() if isinstance(x, str) else x)
             validation_rules = dmge.get_node_validation_rules(node_display_name=col)
 
             # Parse the validation rules
             if validation_rules and isinstance(validation_rules, dict):
                 validation_rules = extract_component_validation_rules(
                     manifest_component=manifest["Component"][0],
-                    validation_rules=validation_rules,
+                    validation_rules_dict=validation_rules,
                 )
 
-            # Check that attribute rules conform to limits:
-            # no more than two rules for an attribute.
-            # As more combinations get added, may want to bring out into its own function / or use validate_rules_utils?
-            if len(validation_rules) > 2:
-                errors.append(
-                    self.get_multiple_types_error(
-                        validation_rules, col, error_type="too_many_rules"
-                    )
-                )
+            # Check for max rule allowance
+            errors = self.check_max_rule_num(
+                validation_rules=validation_rules, col=col, errors=errors
+            )
 
             # Given a validation rule, run validation. Skip validations already performed by GE
             for rule in validation_rules:
                 validation_type = rule.split(" ")[0]
                 if rule_in_rule_list(rule, unimplemented_expectations) or (
                     rule_in_rule_list(rule, in_house_rules) and restrict_rules
                 ):
+                    # Note rules not listed in unimplemented_expectations or inhouse rules will not be run through
+                    # the validation steps. IsNA is not a true rule, so it will not have any validation run,
+                    # it is handled in validate_attribute
                     if not rule_in_rule_list(rule, in_house_rules):
                         logger.warning(
                             f"Validation rule {rule.split(' ')[0]} has not been implemented in house and cannnot be validated without Great Expectations."
                         )
                         continue
 
                     t_indiv_rule = perf_counter()
                     # Validate for each individual validation rule.
                     validation_method = getattr(
-                        ValidateAttribute, validation_types[validation_type]["type"]
+                        validate_attribute, validation_types[validation_type]["type"]
                     )
 
                     if validation_type == "list":
                         vr_errors, vr_warnings, manifest_col = validation_method(
-                            self,
                             rule,
                             manifest[col],
-                            dmge,
                         )
                         manifest[col] = manifest_col
                     elif validation_type.lower().startswith("match"):
                         vr_errors, vr_warnings = validation_method(
-                            self, rule, manifest[col], project_scope, dmge, access_token
+                            rule, manifest[col], project_scope, access_token
                         )
                     else:
                         vr_errors, vr_warnings = validation_method(
-                            self,
                             rule,
                             manifest[col],
-                            dmge,
                         )
                     # Check for validation rule errors and add them to other errors.
                     if vr_errors:
                         errors.extend(vr_errors)
                     if vr_warnings:
                         warnings.extend(vr_warnings)
                     logger.debug(
@@ -258,14 +291,17 @@
     ) -> (List[List[str]], List[List[str]]):
         t_json_schema = perf_counter()
 
         errors = []
         warnings = []
         col_attr = {}  # save the mapping between column index and attribute name
 
+        # Replace nans with empty strings so jsonschema
+        manifest = manifest.replace({np.nan: ""})
+
         # numerical values need to be type string for the jsonValidator
         for col in manifest.select_dtypes(
             include=[int, np.int64, float, np.float64]
         ).columns:
             manifest[col] = manifest[col].astype("string")
         manifest = manifest.map(
             lambda x: str(x) if isinstance(x, Number) else x, na_action="ignore"
@@ -280,15 +316,15 @@
                 errorColName = error.path[0] if len(error.path) > 0 else "Wrong schema"
                 errorMsg = error.message[0:500]
                 errorVal = error.instance if len(error.path) > 0 else "Wrong schema"
 
                 val_errors, val_warnings = GenerateError.generate_schema_error(
                     row_num=errorRow,
                     attribute_name=errorColName,
-                    error_msg=errorMsg,
+                    error_message=errorMsg,
                     invalid_entry=errorVal,
                     dmge=dmge,
                 )
 
                 if val_errors:
                     errors.append(val_errors)
                 if val_warnings:
```

### Comparing `schematicpy-24.2.1/schematic/schemas/commands.py` & `schematicpy-24.4.1/schematic/schemas/commands.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,43 @@
-#!/usr/bin/env python3
+"""Schema Commands"""
 
-import click
-import click_log
 import logging
-import sys
 import time
 import re
+from typing import get_args
+
+import click
+import click_log  # type: ignore
+
+# pylint: disable=logging-fstring-interpolation
 
 from schematic.schemas.data_model_parser import DataModelParser
-from schematic.schemas.data_model_graph import DataModelGraph, DataModelGraphExplorer
+from schematic.schemas.data_model_graph import DataModelGraph
 from schematic.schemas.data_model_validator import DataModelValidator
-from schematic.schemas.data_model_jsonld import DataModelJsonLD, convert_graph_to_jsonld
+from schematic.schemas.data_model_jsonld import convert_graph_to_jsonld
 
+from schematic.utils.schema_utils import DisplayLabelType
 from schematic.utils.cli_utils import query_dict
 from schematic.utils.schema_utils import export_schema
 from schematic.help import schema_commands
 
 logger = logging.getLogger("schematic")
 click_log.basic_config(logger)
 
-CONTEXT_SETTINGS = dict(help_option_names=["--help", "-h"])  # help options
+CONTEXT_SETTINGS = {"help_option_names": ["--help", "-h"]}  # help options
 
 
-# invoke_without_command=True -> forces the application not to show aids before losing them with a --h
+# invoke_without_command=True -> forces the application not to show aids before
+# losing them with a --h
 @click.group(context_settings=CONTEXT_SETTINGS, invoke_without_command=True)
 def schema():  # use as `schematic model ...`
     """
     Sub-commands for Schema related utilities/methods.
     """
-    pass
+    pass  # pylint: disable=unnecessary-pass
 
 
 # prototype based on submit_metadata_manifest()
 @schema.command(
     "convert",
     options_metavar="<options>",
     short_help=query_dict(schema_commands, ("schema", "convert", "short_help")),
@@ -41,74 +46,78 @@
 @click.argument(
     "schema", type=click.Path(exists=True), metavar="<DATA_MODEL_CSV>", nargs=1
 )
 @click.option(
     "--data_model_labels",
     "-dml",
     default="class_label",
-    type=click.Choice(["display_label", "class_label"], case_sensitive=True),
+    type=click.Choice(list(get_args(DisplayLabelType)), case_sensitive=True),
     help=query_dict(schema_commands, ("schema", "convert", "data_model_labels")),
 )
 @click.option(
     "--output_jsonld",
     "-o",
     metavar="<OUTPUT_PATH>",
     help=query_dict(schema_commands, ("schema", "convert", "output_jsonld")),
 )
 def convert(schema, data_model_labels, output_jsonld):
     """
     Running CLI to convert data model specification in CSV format to
     data model in JSON-LD format.
 
-    Note: Currently, not configured to build off of base model, so removing --base_schema argument for now
+    Note: Currently, not configured to build off of base model, so removing --base_schema
+      argument for now
     """
+    # pylint: disable=too-many-locals
+    # pylint: disable=redefined-outer-name
+    # pylint: disable=too-many-branches
 
     # get the start time
-    st = time.time()
+    start_time = time.time()
 
     # Instantiate Parser
     data_model_parser = DataModelParser(schema)
 
     # Parse Model
     logger.info("Parsing data model.")
     parsed_data_model = data_model_parser.parse_model()
 
     # Convert parsed model to graph
     # Instantiate DataModelGraph
     data_model_grapher = DataModelGraph(parsed_data_model, data_model_labels)
 
-    # Generate graph
+    # Generate graphschema
     logger.info("Generating data model graph.")
-    graph_data_model = data_model_grapher.generate_data_model_graph()
+    graph_data_model = data_model_grapher.graph
 
     # Validate generated data model.
     logger.info("Validating the data model internally.")
     data_model_validator = DataModelValidator(graph=graph_data_model)
     data_model_errors, data_model_warnings = data_model_validator.run_checks()
 
     # If there are errors log them.
     if data_model_errors:
         for err in data_model_errors:
             if isinstance(err, str):
                 logger.error(err)
             elif isinstance(err, list):
-                for e in err:
-                    logger.error(e)
+                for error in err:
+                    logger.error(error)
 
     # If there are warnings log them.
     if data_model_warnings:
         for war in data_model_warnings:
             if isinstance(war, str):
                 logger.warning(war)
             elif isinstance(war, list):
-                for w in war:
-                    logger.warning(w)
+                for warning in war:
+                    logger.warning(warning)
 
     logger.info("Converting data model to JSON-LD")
-    jsonld_data_model = convert_graph_to_jsonld(Graph=graph_data_model)
+    jsonld_data_model = convert_graph_to_jsonld(graph=graph_data_model)
 
     # output JSON-LD file alongside CSV file by default, get path.
     if output_jsonld is None:
         if not ".jsonld" in schema:
             csv_no_ext = re.sub("[.]csv$", "", schema)
             output_jsonld = csv_no_ext + ".jsonld"
         else:
@@ -122,18 +131,21 @@
 
     # saving updated schema.org schema
     try:
         export_schema(jsonld_data_model, output_jsonld)
         click.echo(
             f"The Data Model was created and saved to '{output_jsonld}' location."
         )
-    except:
+    except:  # pylint: disable=bare-except
         click.echo(
-            f"The Data Model could not be created by using '{output_jsonld}' location. Please check your file path again"
+            (
+                f"The Data Model could not be created by using '{output_jsonld}' location. "
+                "Please check your file path again"
+            )
         )
 
     # get the end time
-    et = time.time()
+    end_time = time.time()
 
     # get the execution time
-    elapsed_time = time.strftime("%M:%S", time.gmtime(et - st))
+    elapsed_time = time.strftime("%M:%S", time.gmtime(end_time - start_time))
     click.echo(f"Execution time: {elapsed_time} (M:S)")
```

### Comparing `schematicpy-24.2.1/schematic/schemas/data_model_edges.py` & `schematicpy-24.4.1/schematic/schemas/data_model_edges.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,43 +1,56 @@
-import networkx as nx
-
+"""Data Model Edges"""
+from typing import Union, Any
 from schematic.schemas.data_model_relationships import DataModelRelationships
 
 
-class DataModelEdges:
-    def __init__(self):
+class DataModelEdges:  # pylint: disable=too-few-public-methods
+    """Data Model Edges"""
+
+    def __init__(self) -> None:
         self.dmr = DataModelRelationships()
         self.data_model_relationships = self.dmr.relationships_dictionary
 
-    def generate_edge(
+    def generate_edge(  # pylint: disable=too-many-arguments
         self,
         node: str,
-        all_node_dict: dict,
-        attr_rel_dict: dict,
-        edge_relationships: dict,
-        edge_list: list,
-    ) -> list[tuple[str, str, dict[str:str, str:int]]]:
-        """Generate an edge between a target node and relevant other nodes the data model. In short, does this current node belong to a recorded relationship in the attribute, relationshps dictionary. Go through each attribute and relationship to find where the node may be.
+        all_node_dict: dict[str, dict[str, Any]],
+        attr_rel_dict: dict[str, dict[str, Any]],
+        edge_relationships: dict[str, str],
+        edge_list: list[tuple[str, str, dict[str, Union[str, int]]]],
+    ) -> list[tuple[str, str, dict[str, Union[str, int]]]]:
+        """
+
+        Generate an edge between a target node and relevant other nodes the data model.
+          In short, does this current node belong to a recorded relationship in the attribute,
+          relationshps dictionary.
+          Go through each attribute and relationship to find where the node may be.
+
         Args:
-            G, nx.MultiDiGraph: networkx graph representation of the data model, that is in the process of being fully built. At this point, all the nodes would have been added, and edges are being added per target node.
-            node, str: target node to look for connecting edges
-            all_node_dict, dict: a dictionary containing information about all nodes in the model
+            node (str): target node to look for connecting edges
+            all_node_dict (dict): a dictionary containing information about all nodes in the model
                 key: node display name
                 value: node attribute dict, containing attributes to attach to each node.
-            attr_rel_dict, dict:
-                {Attribute Display Name: {
-                        Relationships: {
-                                    CSV Header: Value}}}
-            edge_relationships: dict, rel_key: csv_header if the key represents a value relationship.
-            edge_list: list(tuple), list of tuples describing the edges and the edge attributes, organized as (node_1, node_2, {key:edge_relationship_key, weight:int})
-                At this point, the edge list will be in the process of being built. Adding edges from list so they will be added properly to the graph without being overwritten in the loop, and passing the Graph around more.
-        Returns:
-            edge_list: list(tuple), list of tuples describing the edges and the edge attributes, organized as (node_1, node_2, {key:edge_relationship_key, weight:int})
-                At this point, the edge list will have additional edges added related to the current node.
+            attr_rel_dict (dict):
+                {Attribute Display Name: {--disallow-untyped-defs
+                    Relationships: {
+                        CSV Header: Value}
+                    }
+                }
+            edge_relationships (dict): dict, rel_key: csv_header if the key represents a value
+              relationship.
+            edge_list (list): list of tuples describing the edges and the edge attributes,
+              organized as (node_1, node_2, {key:edge_relationship_key, weight:int})
+              At this point, the edge list will be in the process of being built.
+              Adding edges from list so they will be added properly to the graph without being
+              overwritten in the loop, and passing the Graph around more.
+
+
         """
+
         # For each attribute in the model.
         for attribute_display_name, relationship in attr_rel_dict.items():
             # Get the relationships associated with the current attribute
             relationships = relationship["Relationships"]
             # Add edge relationships one at a time
             for rel_key, csv_header in edge_relationships.items():
                 # If the attribute has a relationship that matches the current edge being added
@@ -45,31 +58,34 @@
                     # If the current node is part of that relationship and is not the current node
                     # Connect node to attribute as an edge.
                     if (
                         node in relationships[csv_header]
                         and node != attribute_display_name
                     ):
                         # Generate weights based on relationship type.
-                        # Weights will allow us to preserve the order of entries order in the data model in later steps.
+                        # Weights will allow us to preserve the order of entries order in the
+                        # data model in later steps.
                         if rel_key == "domainIncludes":
-                            # For 'domainIncludes'/properties relationship, users do not explicitly provide a list order (like for valid values, or dependsOn)
+                            # For 'domainIncludes'/properties relationship, users do not explicitly
+                            # provide a list order (like for valid values, or dependsOn)
                             # so we pull the order/weight from the order of the attributes.
                             weight = list(attr_rel_dict.keys()).index(
                                 attribute_display_name
                             )
-                        elif type(relationships[csv_header]) == list:
-                            # For other relationships that pull in lists of values, we can explicilty pull the weight by their order in the provided list
+                        elif isinstance(relationships[csv_header], list):
+                            # For other relationships that pull in lists of values, we can
+                            # explicilty pull the weight by their order in the provided list
                             weight = relationships[csv_header].index(node)
                         else:
                             # For single (non list) entries, add weight of 0
                             weight = 0
                         # Get the edge_key for the edge relationship we are adding at this step
                         edge_key = self.data_model_relationships[rel_key]["edge_key"]
                         # Add edges, in a manner that preserves directionality
-                        # TODO: rewrite to use edge_dir
+                        # TODO: rewrite to use edge_dir pylint: disable=fixme
                         if rel_key in ["subClassOf", "domainIncludes"]:
                             edge_list.append(
                                 (
                                     all_node_dict[node]["label"],
                                     all_node_dict[attribute_display_name]["label"],
                                     {
                                         "key": edge_key,
@@ -81,15 +97,16 @@
                             edge_list.append(
                                 (
                                     all_node_dict[attribute_display_name]["label"],
                                     all_node_dict[node]["label"],
                                     {"key": edge_key, "weight": weight},
                                 )
                             )
-                        # Add add rangeIncludes/valid value relationships in reverse as well, making the attribute the parent of the valid value.
+                        # Add add rangeIncludes/valid value relationships in reverse as well,
+                        # making the attribute the parent of the valid value.
                         if rel_key == "rangeIncludes":
                             edge_list.append(
                                 (
                                     all_node_dict[attribute_display_name]["label"],
                                     all_node_dict[node]["label"],
                                     {"key": "parentOf", "weight": weight},
                                 )
```

### Comparing `schematicpy-24.2.1/schematic/schemas/data_model_graph.py` & `schematicpy-24.4.1/schematic/schemas/data_model_graph.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,50 @@
-from copy import deepcopy
-import graphviz
+"""DataModel Graph"""
+
 import logging
-from typing import Any, Dict, Optional, Text
-import networkx as nx
-from rdflib import Namespace
+from typing import Optional, Union, Any
+
+import networkx as nx  # type: ignore
+import graphviz  # type: ignore
 
 from schematic.schemas.data_model_edges import DataModelEdges
 from schematic.schemas.data_model_nodes import DataModelNodes
 from schematic.schemas.data_model_relationships import DataModelRelationships
 
 from schematic.utils.schema_utils import (
     get_property_label_from_display_name,
     get_class_label_from_display_name,
     DisplayLabelType,
+    extract_component_validation_rules,
 )
 from schematic.utils.general import unlist
 from schematic.utils.viz_utils import visualize
+from schematic.utils.validate_utils import rule_in_rule_list
+
 
 logger = logging.getLogger(__name__)
 
 
-class DataModelGraphMeta(object):
-    _instances = {}
+class DataModelGraphMeta:  # pylint: disable=too-few-public-methods
+    """DataModelGraphMeta"""
+
+    _instances: dict = {}
 
-    def __call__(cls, *args, **kwargs):
+    def __call__(cls, *args: Any, **kwargs: Any):  # pylint: disable=no-self-argument
         """
         Possible changes to the value of the `__init__` argument do not affect
         the returned instance.
         """
         if cls not in cls._instances:
-            instance = super().__call__(*args, **kwargs)
+            instance = super().__call__(*args, **kwargs)  # pylint: disable=no-member
             cls._instances[cls] = instance
         return cls._instances[cls]
 
 
-class DataModelGraph:
+class DataModelGraph:  # pylint: disable=too-few-public-methods
     """
     Generate graph network (networkx) from the attributes and relationships returned
     from the data model parser.
 
     Create a singleton.
     """
 
@@ -52,45 +58,53 @@
         """Load parsed data model.
         Args:
             attributes_relationship_dict, dict: generated in data_model_parser
                 {Attribute Display Name: {
                         Relationships: {
                                     CSV Header: Value}}}
             data_model_labels: str, display_label or class_label.
-                display_label, use the display name as a label, if it is valid (contains no blacklisted characters) otherwise will default to schema_label.
-                class_label, default, use standard class or property label.         Raises:
+                display_label, use the display name as a label, if it is valid
+                (contains no blacklisted characters) otherwise will default to schema_label.
+                class_label, default, use standard class or property label.
+        Raises:
             ValueError, attribute_relationship_dict not loaded.
         """
         self.attribute_relationships_dict = attribute_relationships_dict
         self.dmn = DataModelNodes(self.attribute_relationships_dict)
         self.dme = DataModelEdges()
         self.dmr = DataModelRelationships()
         self.data_model_labels = data_model_labels
 
         if not self.attribute_relationships_dict:
             raise ValueError(
-                "Something has gone wrong, a data model was not loaded into the DataModelGraph Class. Please check that your paths are correct"
+                (
+                    "Something has gone wrong, a data model was not loaded into the DataModelGraph "
+                    "Class. Please check that your paths are correct"
+                )
             )
         self.graph = self.generate_data_model_graph()
 
     def generate_data_model_graph(self) -> nx.MultiDiGraph:
-        """Generate NetworkX Graph from the Relationships/attributes dictionary, the graph is built by first adding all nodes to the graph, then connecting nodes by the relationships defined in the attributes_relationship dictionary.
+        """
+        Generate NetworkX Graph from the Relationships/attributes dictionary, the graph is built
+          by first adding all nodes to the graph, then connecting nodes by the relationships defined
+          in the attributes_relationship dictionary.
         Returns:
             G: nx.MultiDiGraph, networkx graph representation of the data model
         """
         # Get all relationships with edges
         edge_relationships = self.dmr.retreive_rel_headers_dict(edge=True)
 
         # Find all nodes
         all_nodes = self.dmn.gather_all_nodes_in_model(
             attr_rel_dict=self.attribute_relationships_dict
         )
 
         # Instantiate NetworkX MultiDigraph
-        G = nx.MultiDiGraph()
+        graph = nx.MultiDiGraph()
 
         all_node_dict = {}
 
         ## Fill in MultiDigraph with nodes
         for node in all_nodes:
             # Gather information for each node
             node_dict = self.dmn.generate_node_dict(
@@ -99,81 +113,94 @@
                 data_model_labels=self.data_model_labels,
             )
 
             # Add each node to the all_node_dict to be used for generating edges
             all_node_dict[node] = node_dict
 
             # Generate node and attach information (attributes) to each node
-            G = self.dmn.generate_node(G, node_dict)
+            graph = self.dmn.generate_node(graph, node_dict)
 
-        edge_list = []
+        edge_list: list[tuple[str, str, dict[str, Union[str, int]]]] = []
         ## Connect nodes via edges
         for node in all_nodes:
             # Generate edges
             edge_list_2 = self.dme.generate_edge(
                 node,
                 all_node_dict,
                 self.attribute_relationships_dict,
                 edge_relationships,
                 edge_list,
             )
             edge_list = edge_list_2.copy()
 
         # Add edges to the Graph
         for node_1, node_2, edge_dict in edge_list:
-            G.add_edge(node_1, node_2, key=edge_dict["key"], weight=edge_dict["weight"])
-        return G
+            graph.add_edge(
+                node_1, node_2, key=edge_dict["key"], weight=edge_dict["weight"]
+            )
+        return graph
 
 
-class DataModelGraphExplorer:
+class DataModelGraphExplorer:  # pylint: disable=too-many-public-methods
+    """DataModelGraphExplorer"""
+
     def __init__(
         self,
-        G,
+        graph: nx.MultiDiGraph,
     ):
         """Load data model graph as a singleton.
         Args:
             G: nx.MultiDiGraph, networkx graph representation of the data model
         """
-        self.graph = G  # At this point the graph is expected to be fully formed.
+        self.graph = graph  # At this point the graph is expected to be fully formed.
         self.dmr = DataModelRelationships()
         self.rel_dict = self.dmr.relationships_dictionary
 
     def find_properties(self) -> set[str]:
-        """Identify all properties, as defined by the first node in a pair, connected with 'domainIncludes' edge type
+        """
+        Identify all properties, as defined by the first node in a pair, connected with
+        'domainIncludes' edge type
+
         Returns:
-            properties, set: All properties defined in the data model, each property name is defined by its label.
+            properties, set: All properties defined in the data model, each property name
+              is defined by its label.
         """
-        properties = []
-        for node_1, node_2, rel in self.graph.edges:
+        properties_list: list[str] = []
+        for node_1, _, rel in self.graph.edges:
             if rel == self.rel_dict["domainIncludes"]["edge_key"]:
-                properties.append(node_1)
-        properties = set(properties)
-        return properties
+                properties_list.append(node_1)
+        properties_set = set(properties_list)
+        return properties_set
 
     def find_classes(self) -> set[str]:
-        """Identify all classes, as defined but all nodes, minus all properties (which are explicitly defined)
+        """
+        Identify all classes, as defined but all nodes, minus all properties
+        (which are explicitly defined)
         Returns:
-            classes, set:  All classes defined in the data model, each class name is defined by its label.
+            classes, set:  All classes defined in the data model, each class
+              name is defined by its label.
         """
         nodes = self.graph.nodes
         properties = self.find_properties()
         classes = nodes - properties
         return classes
 
     def find_node_range(
         self, node_label: Optional[str] = None, node_display_name: Optional[str] = None
     ) -> list:
         """Get valid values for the given node (attribute)
         Args:
             node_label, str, Optional[str]: label of the node for which to retrieve valid values
-            node_display_name, str, Optional[str]: Display Name of the node for which to retrieve valid values
+            node_display_name, str, Optional[str]: Display Name of the node for which to
+              retrieve valid values
         Returns:
             valid_values, list: List of valid values associated with the provided node.
         """
         if not node_label:
+            assert node_display_name is not None
             node_label = self.get_node_label(node_display_name)
 
         valid_values = []
         for node_1, node_2, rel in self.graph.edges:
             if (
                 node_1 == node_label
                 and rel == self.rel_dict["rangeIncludes"]["edge_key"]
@@ -192,33 +219,124 @@
             relationship: the type of link(s) that the above node and its immediate neighbors share.
 
         Returns:
             List of nodes that are adjacent to the given node.
         #checked
         """
         nodes = set()
-        for node_1, node_2, key, _ in self.graph.out_edges(
-            node_label, data=True, keys=True
-        ):
+        for _, node_2, key, _ in self.graph.out_edges(node_label, data=True, keys=True):
             if key == relationship:
                 nodes.add(node_2)
 
         return list(nodes)
 
+    def get_component_node_required(
+        self,
+        manifest_component: str,
+        node_validation_rules: Optional[list[str]] = None,
+        node_label: Optional[str] = None,
+        node_display_name: Optional[str] = None,
+    ) -> bool:
+        """Check if a node is required taking into account the manifest component it is defined in
+        (requirements can be set in validaiton rule as well as required column)
+        Args:
+            manifest_component: str, manifest component display name that the node belongs to.
+            node_validation_rules: list[str], valdation rules for a given node and component.
+            node_label: str, Label of the node you would want to get the comment for.
+            node_display_name: str, node display name for the node being queried.
+        Returns:
+            True, if node is required, False if not
+        """
+        node_required = False
+
+        if not node_validation_rules:
+            # Get node validation rules for a given component
+            node_validation_rules = self.get_component_node_validation_rules(
+                manifest_component=manifest_component,
+                node_label=node_label,
+                node_display_name=node_display_name,
+            )
+
+        # Check if the valdation rule specifies that the node is required for this particular
+        # component.
+        if rule_in_rule_list("required", node_validation_rules):
+            node_required = True
+            # To prevent any unintended errors, ensure the Required field for this node is False
+            if self.get_node_required(
+                node_label=node_label, node_display_name=node_display_name
+            ):
+                if not node_display_name:
+                    assert node_label is not None
+                    node_display_name = self.graph.nodes[node_label][
+                        self.rel_dict["displayName"]["node_label"]
+                    ]
+                error_str = " ".join(
+                    [
+                        f"For component: {manifest_component} and attribute: {node_display_name}",
+                        "requirements are being specified in both the Required field and in the",
+                        "Validation Rules. If you desire to use validation rules to set component",
+                        "specific requirements for this attribute",
+                        "then the Required field needs to be set to False, or the validation may",
+                        "not work as intended, for other components where the attribute",
+                        "that should not be required.",
+                    ]
+                )
+
+                logger.error(error_str)
+        else:
+            # If requirements are not being set in the validaiton rule, then just pull the
+            # standard node requirements from the model
+            node_required = self.get_node_required(
+                node_label=node_label, node_display_name=node_display_name
+            )
+        return node_required
+
+    def get_component_node_validation_rules(
+        self,
+        manifest_component: str,
+        node_label: Optional[str] = None,
+        node_display_name: Optional[str] = None,
+    ) -> list[str]:
+        """Get valdation rules for a given node and component.
+        Args:
+            manifest_component: str, manifest component display name that the node belongs to.
+            node_label: str, Label of the node you would want to get the comment for.
+            node_display_name: str, node display name for the node being queried.
+        Returns:
+            validation_rules: list[str], validation rules list for a given node and component.
+        """
+        # get any additional validation rules associated with this node (e.g. can this node
+        # be mapped to a list of other nodes)
+        node_validation_rules = self.get_node_validation_rules(
+            node_label=node_label, node_display_name=node_display_name
+        )
+
+        # Parse the validation rules per component if applicable
+        if node_validation_rules and isinstance(node_validation_rules, dict):
+            node_validation_rules = extract_component_validation_rules(
+                manifest_component=manifest_component,
+                validation_rules_dict=node_validation_rules,
+            )
+        return node_validation_rules
+
     def get_component_requirements(
         self,
         source_component: str,
     ) -> list[str]:
-        """Get all components that are associated with a given source component and are required by it.
+        """
+        Get all components that are associated with a given source component and are
+          required by it.
 
         Args:
-            source_component: source component for which we need to find all required downstream components.
+            source_component: source component for which we need to find all required downstream
+              components.
 
         Returns:
-            List of nodes that are descendants from the source component are are related to the source through a specific component relationship.
+            List of nodes that are descendants from the source component are are related to the
+              source through a specific component relationship.
         """
 
         req_components = list(
             reversed(
                 self.get_descendants_by_edge_type(
                     source_component,
                     self.rel_dict["requiresComponent"]["edge_key"],
@@ -229,21 +347,25 @@
 
         return req_components
 
     def get_component_requirements_graph(
         self,
         source_component: str,
     ) -> nx.DiGraph:
-        """Get all components that are associated with a given source component and are required by it; return the components as a dependency graph (i.e. a DAG).
+        """
+        Get all components that are associated with a given source component and are required by it;
+          return the components as a dependency graph (i.e. a DAG).
 
         Args:
-            source_component, str: source component for which we need to find all required downstream components.
+            source_component, str: source component for which we need to find all required
+              downstream components.
 
         Returns:
-            A subgraph of the schema graph induced on nodes that are descendants from the source component and are related to the source through a specific component relationship.
+            A subgraph of the schema graph induced on nodes that are descendants from the source
+              component and are related to the source through a specific component relationship.
         """
 
         # get a list of required component nodes
         req_components = self.get_component_requirements(source_component)
 
         # get the subgraph induced on required component nodes
         req_components_graph = self.get_subgraph_by_edge_type(
@@ -255,121 +377,142 @@
     def get_descendants_by_edge_type(
         self,
         source_node: str,
         relationship: str,
         connected: bool = True,
         ordered: bool = False,
     ) -> list[str]:
-        """Get all nodes that are descendants of a given source node, based on a specific type of edge / relationship type.
+        """
+        Get all nodes that are descendants of a given source node, based on a specific
+          type of edge / relationship type.
 
         Args:
             source_node: The node whose descendants need to be retreived.
             relationship: Edge / link relationship type with possible values same as in above docs.
-            connected: If True, we need to ensure that all descendant nodes are reachable from the source node, i.e., they are part of the same connected component.
-                       If False, the descendants could be in multiple connected components.
-                       Default value is True.
-            ordered: If True, the list of descendants will be topologically ordered.
-                     If False, the list has no particular order (depends on the order in which the descendats were traversed in the subgraph).
+            connected:
+              If True, we need to ensure that all descendant nodes are reachable from the source
+                node, i.e., they are part of the same connected component.
+              If False, the descendants could be in multiple connected components.
+              Default value is True.
+            ordered:
+              If True, the list of descendants will be topologically ordered.
+              If False, the list has no particular order (depends on the order in which the
+                descendats were traversed in the subgraph).
 
         Returns:
             List of nodes that are descendants from a particular node (sorted / unsorted)
         """
 
         root_descendants = nx.descendants(self.graph, source_node)
 
         subgraph_nodes = list(root_descendants)
         subgraph_nodes.append(source_node)
         descendants_subgraph = self.graph.subgraph(subgraph_nodes)
 
-        # prune the descendants subgraph so as to include only those edges that match the relationship type
+        # prune the descendants subgraph so as to include only those edges that match
+        # the relationship type
         rel_edges = []
         for node_1, node_2, key, _ in descendants_subgraph.edges(data=True, keys=True):
             if key == relationship:
                 rel_edges.append((node_1, node_2))
 
         relationship_subgraph = nx.DiGraph()
         relationship_subgraph.add_edges_from(rel_edges)
 
         descendants = relationship_subgraph.nodes()
 
         if not descendants:
-            # return empty list if there are no nodes that are reachable from the source node based on this relationship type
+            # return empty list if there are no nodes that are reachable from the
+            # source node based on this relationship type
             return []
 
         if connected and ordered:
             # get the set of reachable nodes from the source node
             descendants = nx.descendants(relationship_subgraph, source_node)
             descendants.add(source_node)
 
-            # normally, the descendants from a node are unordered (peculiarity of nx descendants call)
+            # normally, the descendants from a node are unordered (peculiarity
+            # of nx descendants call)
             # form the subgraph on descendants and order it topologically
             # this assumes an acyclic subgraph
             descendants = nx.topological_sort(
                 relationship_subgraph.subgraph(descendants)
             )
         elif connected:
             # get the nodes that are reachable from a given source node
-            # after the pruning process above some nodes in the root_descendants subgraph might have become disconnected and will be omitted
+            # after the pruning process above some nodes in the
+            # root_descendants subgraph might have become disconnected and
+            # will be omitted
             descendants = nx.descendants(relationship_subgraph, source_node)
             descendants.add(source_node)
         elif ordered:
             # sort the nodes topologically
             # this requires the graph to be an acyclic graph
             descendants = nx.topological_sort(relationship_subgraph)
 
         return list(descendants)
 
     def get_digraph_by_edge_type(self, edge_type: str) -> nx.DiGraph:
         """Get a networkx digraph of the nodes connected via a given edge_type.
         Args:
             edge_type:
-                Edge type to search for, possible types are defined by 'edge_key' in relationship class
+                Edge type to search for, possible types are defined by 'edge_key'
+                  in relationship class
         Returns:
         """
         digraph = nx.DiGraph()
         for node_1, node_2, key, _ in self.graph.edges(data=True, keys=True):
             if key == edge_type:
                 digraph.add_edge(node_1, node_2)
         return digraph
 
     def get_edges_by_relationship(
         self,
         node: str,
         relationship: str,
-    ) -> list[str]:
+    ) -> list[tuple[str, str]]:
         """Get a list of out-edges of a node where the edges match a specifc type of relationship.
 
-        i.e., the edges connecting a node to its neighbors are of relationship type -- "parentOf" (set of edges to children / sub-class nodes).
+        i.e., the edges connecting a node to its neighbors are of relationship type -- "parentOf"
+          (set of edges to children / sub-class nodes).
 
         Args:
             node: the node whose edges we need to look at.
             relationship: the type of link(s) that the above node and its immediate neighbors share.
 
         Returns:
             List of edges that are connected to the node.
         """
-        edges = []
+        edges: list[tuple[str, str]] = []
 
         for node_1, node_2, key, _ in self.graph.out_edges(node, data=True, keys=True):
             if key == relationship:
                 edges.append((node_1, node_2))
 
         return edges
 
     def get_ordered_entry(self, key: str, source_node_label: str) -> list[str]:
-        """Order the values associated with a particular node and edge_key to match original ordering in schema.
+        """
+        Order the values associated with a particular node and edge_key to
+          match original ordering in schema.
+
         Args:
-            key: a key representing and edge relationship in DataModelRelationships.relationships_dictionary
-            source_node_label, str: node to look for edges of and order
-        Returns:
-            sorted_nodes, list: list of sorted nodes, that share the specified relationship with the source node
-            Example:
-                For the example data model, for key='rangeIncludes', source_node_label='CancerType' the return would be ['Breast, 'Colorectal', 'Lung', 'Prostate', 'Skin'] in that exact order.
+            key (str): a key representing and edge relationship in
+              DataModelRelationships.relationships_dictionary
+            source_node_label (str): node to look for edges of and order
+
         Raises:
-            KeyError, cannot find source node in graph
+            KeyError: cannot find source node in graph
+
+        Returns:
+            list[str]:
+              list of sorted nodes, that share the specified relationship with the source node
+              For the example data model, for key='rangeIncludes', source_node_label='CancerType'
+                the return would be ['Breast, 'Colorectal', 'Lung', 'Prostate', 'Skin'] in that
+                exact order.
         """
         # Check if node is in the graph, if not throw an error.
         if not self.is_class_in_schema(node_label=source_node_label):
             raise KeyError(
                 f"Cannot find node: {source_node_label} in the graph, please check entry."
             )
 
@@ -406,36 +549,39 @@
         )
 
         return sorted_nodes
 
     # Get values associated with a node
     def get_nodes_ancestors(self, subgraph: nx.DiGraph, node_label: str) -> list[str]:
         """Get a list of nodes reachable from source component in graph
+
         Args:
-            subgraph: networkx graph object
-            node_label, str: label of node to find ancestors for
+            subgraph (nx.DiGraph): networkx graph object
+            node_label (str): label of node to find ancestors for
+
         Returns:
-            all_ancestors, list: nodes reachable from source in graph
+            list[str]: nodes reachable from source in graph
         """
         all_ancestors = list(nx.ancestors(subgraph, node_label))
 
         return all_ancestors
 
     def get_node_comment(
-        self, node_display_name: str = None, node_label: str = None
+        self, node_display_name: Optional[str] = None, node_label: Optional[str] = None
     ) -> str:
         """Get the node definition, i.e., the "comment" associated with a given node display name.
 
         Args:
             node_display_name, str: Display name of the node which you want to get the comment for.
             node_label, str: Label of the node you would want to get the comment for.
         Returns:
             Comment associated with node, as a string.
         """
         if not node_label:
+            assert node_display_name is not None
             node_label = self.get_node_label(node_display_name)
 
         if not node_label:
             return ""
 
         node_definition = self.graph.nodes[node_label][
             self.rel_dict["comment"]["node_label"]
@@ -450,16 +596,18 @@
     ) -> list[str]:
         """Get the immediate dependencies that are related to a given source node.
 
         Args:
             source_node: The node whose dependencies we need to compute.
             display_names: if True, return list of display names of each of the dependencies.
                            if False, return list of node labels of each of the dependencies.
-            schema_ordered: if True, return the dependencies of the node following the order of the schema (slower).
-                            if False, return dependencies from graph without guaranteeing schema order (faster)
+            schema_ordered:
+              if True, return the dependencies of the node following the order of the schema
+                (slower).
+              if False, return dependencies from graph without guaranteeing schema order (faster)
 
         Returns:
             List of nodes that are dependent on the source node.
         """
 
         if schema_ordered:
             # get dependencies in the same order in which they are defined in the schema
@@ -544,37 +692,45 @@
 
     def get_node_range(
         self,
         node_label: Optional[str] = None,
         node_display_name: Optional[str] = None,
         display_names: bool = False,
     ) -> list[str]:
-        """Get the range, i.e., all the valid values that are associated with a node label.
+        """
+        Get the range, i.e., all the valid values that are associated with a node label.
+
 
         Args:
-            node_label: Node for which you need to retrieve the range.
-            display_names, bool: True
-        Returns:
-            required_range: Returned if display_names=False, list of valid values (labels) associated with a given node.
-            dependencies_display_name: Returned if display_names=True,
-                List of valid values (display names) associated with a given node
+            node_label (Optional[str], optional): Node for which you need to retrieve the range.
+              Defaults to None.
+            node_display_name (Optional[str], optional): _description_. Defaults to None.
+            display_names (bool, optional): _description_. Defaults to False.
+
         Raises:
             ValueError: If the node cannot be found in the graph.
+
+        Returns:
+            list[str]:
+              If display_names=False, a list of valid values (labels) associated with a given node.
+              If display_names=True, a list of valid values (display names) associated
+                with a given node
         """
         if not node_label:
+            assert node_display_name is not None
             node_label = self.get_node_label(node_display_name)
 
         try:
             # get node range in the order defined in schema for given node
             required_range = self.find_node_range(node_label=node_label)
-        except KeyError:
+        except KeyError as exc:
             raise ValueError(
                 f"The source node {node_label} does not exist in the graph. "
                 "Please use a different node."
-            )
+            ) from exc
 
         if display_names:
             # get the display name(s) of all dependencies
             dependencies_display_names = []
 
             for req in required_range:
                 dependencies_display_names.append(self.graph.nodes[req]["displayName"])
@@ -594,32 +750,34 @@
             node_label: Label of the node for which you need to look up.
             node_display_name: Display name of the node for which you want look up.
         Returns:
             True: If the given node is a "required" node.
             False: If the given node is not a "required" (i.e., an "optional") node.
         """
         if not node_label:
+            assert node_display_name is not None
             node_label = self.get_node_label(node_display_name)
 
         rel_node_label = self.rel_dict["required"]["node_label"]
         node_required = self.graph.nodes[node_label][rel_node_label]
         return node_required
 
     def get_node_validation_rules(
         self, node_label: Optional[str] = None, node_display_name: Optional[str] = None
-    ) -> str:
+    ) -> Union[list, dict[str, str]]:
         """Get validation rules associated with a node,
 
         Args:
             node_label: Label of the node for which you need to look up.
             node_display_name: Display name of the node which you want to get the label for.
         Returns:
             A set of validation rules associated with node, as a list.
         """
         if not node_label:
+            assert node_display_name is not None
             node_label = self.get_node_label(node_display_name)
 
         if not node_label:
             return []
 
         node_validation_rules = self.graph.nodes[node_label]["validationRules"]
 
@@ -631,15 +789,16 @@
         Args:
             relationship: edge / link relationship type with possible values same as in above docs.
 
         Returns:
             Directed graph on edges of a particular type (aka relationship)
         """
 
-        # prune the metadata model graph so as to include only those edges that match the relationship type
+        # prune the metadata model graph so as to include only those edges that
+        # match the relationship type
         rel_edges = []
         for node_1, node_2, key, _ in self.graph.out_edges(data=True, keys=True):
             if key == relationship:
                 rel_edges.append((node_1, node_2))
 
         relationship_subgraph = nx.DiGraph()
         relationship_subgraph.add_edges_from(rel_edges)
@@ -653,14 +812,15 @@
         Args:
             node_display_name: Display name of the node to look up.
             node_label: Label of the node to look up.
         Returns:
             List of nodes that are adjacent to the given node, by SubclassOf relationship.
         """
         if not node_label:
+            assert node_display_name is not None
             node_label = self.get_node_label(node_display_name)
 
         return self.get_adjacent_nodes_by_relationship(
             node_label=node_label, relationship=self.rel_dict["subClassOf"]["edge_key"]
         )
 
     def find_child_classes(self, schema_class: str) -> list:
@@ -680,21 +840,27 @@
             properties, list: List of properties associate with a given schema class.
         Raises:
             KeyError: Key error is raised if the provded schema_class is not in the graph
         """
 
         if not self.is_class_in_schema(schema_class):
             raise KeyError(
-                f"Schema_class provided: {schema_class} is not in the data model, please check that you are providing the proper class/node label"
+                (
+                    f"Schema_class provided: {schema_class} is not in the data model, please check "
+                    "that you are providing the proper class/node label"
+                )
             )
 
         properties = []
-        for n1, n2 in self.graph.edges():
-            if n2 == schema_class and "domainValue" in self.graph[n1][schema_class]:
-                properties.append(n1)
+        for node1, node2 in self.graph.edges():
+            if (
+                node2 == schema_class
+                and "domainValue" in self.graph[node1][schema_class]
+            ):
+                properties.append(node1)
         return properties
 
     def find_parent_classes(self, node_label: str) -> list[list[str]]:
         """Find all parents of the provided node
         Args:
             node_label: label of the node to find parents of
         Returns:
@@ -710,57 +876,57 @@
         paths = nx.all_simple_paths(self.graph, source=root_node, target=node_label)
 
         return [_path[:-1] for _path in paths]
 
     def full_schema_graph(self, size: Optional[int] = None) -> graphviz.Digraph:
         """Create a graph of the data model.
         Args:
-            size, float: max height and width of the graph, if one value provided it is used for both.
+            size, float: max height and width of the graph, if one value provided
+               it is used for both.
         Returns:
             schema graph viz
         """
         edges = self.graph.edges()
         return visualize(edges, size=size)
 
     def is_class_in_schema(self, node_label: str) -> bool:
         """Determine if provided node_label is in the schema graph/data model.
         Args:
             node_label: label of node to search for in the
         Returns:
             True, if node is in the graph schema
             False, if node is not in graph schema
         """
-        if node_label in self.graph.nodes():
-            return True
-        else:
-            return False
+        return node_label in self.graph.nodes()
 
     def sub_schema_graph(
-        self, source: str, direction: str, size=None
+        self, source: str, direction: str, size: Optional[float] = None
     ) -> Optional[graphviz.Digraph]:
         """Create a sub-schema graph
         Args:
             source, str: source node label to start graph
             direction, str: direction to create the vizualization, choose from "up", "down", "both"
-            size, float: max height and width of the graph, if one value provided it is used for both.
+            size, float: max height and width of the graph, if one value provided it is used for
+              both.
         Returns:
             Sub-schema graph viz
         """
         if direction == "down":
             edges = list(nx.edge_bfs(self.graph, [source]))
             return visualize(edges, size=size)
-        elif direction == "up":
+        if direction == "up":
             paths = self.find_parent_classes(source)
             edges = []
             for _path in paths:
                 _path.append(source)
                 for i in range(0, len(_path) - 1):
                     edges.append((_path[i], _path[i + 1]))
             return visualize(edges, size=size)
-        elif direction == "both":
+        if direction == "both":
             paths = self.find_parent_classes(source)
             edges = list(nx.edge_bfs(self.graph, [source]))
             for _path in paths:
                 _path.append(source)
                 for i in range(0, len(_path) - 1):
                     edges.append((_path[i], _path[i + 1]))
             return visualize(edges, size=size)
+        return None
```

### Comparing `schematicpy-24.2.1/schematic/schemas/data_model_json_schema.py` & `schematicpy-24.4.1/schematic/schemas/data_model_json_schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,136 +1,153 @@
+"Data Model Json Schema"
+
 import logging
-import networkx as nx
 import os
-from typing import Any, Dict, Optional, Text, List
+from typing import Any, Optional
+
+import networkx as nx  # type: ignore
 
 from schematic.schemas.data_model_graph import DataModelGraphExplorer
 from schematic.schemas.data_model_relationships import DataModelRelationships
-
 from schematic.utils.validate_utils import rule_in_rule_list
 
 logger = logging.getLogger(__name__)
 
 
 class DataModelJSONSchema:
+    "Data Model Json Schema"
+
     def __init__(
         self,
         jsonld_path: str,
         graph: nx.MultiDiGraph,
     ):
+        # pylint:disable=fixme
         # TODO: Change jsonld_path to data_model_path (can work with CSV too)
         self.jsonld_path = jsonld_path
+        self.jsonld_path_root: Optional[str] = None
         self.graph = graph  # Graph would be fully made at this point.
         self.dmge = DataModelGraphExplorer(self.graph)
         self.dmr = DataModelRelationships()
         self.rel_dict = self.dmr.relationships_dictionary
 
     def get_array_schema(
-        self, node_range: List[str], node_name: str, blank=False
-    ) -> Dict[str, Dict[str, List[str]]]:
-        """Add a list of nodes to the "enum" key in a given JSON schema object.
-           Allow a node to be mapped to any subset of the list
+        self, node_range: list[str], node_name: str, blank: bool = False
+    ) -> dict[str, dict[str, Any]]:
+        """
+        Add a list of nodes to the "enum" key in a given JSON schema object.
+        Allow a node to be mapped to any subset of the list
 
         Args:
-                node_name: Name of the "main" / "head" key in the JSON schema / object.
-                node_range: List of nodes to be added to the JSON object.
-                blank: If True, add empty node to end of node list.
-                           If False, do not add empty node to end of node list.
+            node_range (list[str]): List of nodes to be added to the JSON object.
+            node_name (str): Name of the "main" / "head" key in the JSON schema / object.
+            blank (bool, optional): Defaults to False.
+              If True, add empty node to end of node list.
+              If False, do not add empty node to end of node list.
 
         Returns:
-                JSON object with array validation rule.
+            dict[str, dict[str, Any]]: JSON object with array validation rule.
         """
-
         schema_node_range_array = {
             node_name: {
                 "type": "array",
                 "items": {"enum": node_range + [""] if blank else node_range},
                 "maxItems": len(node_range),
             }
         }
 
         return schema_node_range_array
 
     def get_non_blank_schema(
         self, node_name: str
-    ) -> Dict[str, dict[str, Any]]:  # can't define heterogenous Dict generic types
+    ) -> dict[str, dict[str, Any]]:  # can't define heterogenous Dict generic types
         """Get a schema rule that does not allow null or empty values.
 
         Args:
                 node_name: Name of the node on which the schema rule is to be applied.
 
         Returns:
                 Schema rule as a JSON object.
         """
         non_blank_schema = {node_name: {"not": {"type": "null"}, "minLength": 1}}
 
         return non_blank_schema
 
     def get_range_schema(
-        self, node_range: List[str], node_name: str, blank=False
-    ) -> Dict[str, Dict[str, List[str]]]:
-        """Add a list of nodes to the "enum" key in a given JSON schema object.
+        self, node_range: list[str], node_name: str, blank=False
+    ) -> dict[str, dict[str, list[str]]]:
+        """
+        Add a list of nodes to the "enum" key in a given JSON schema object.
 
         Args:
-                node_name: Name of the "main" / "head" key in the JSON schema / object.
-                node_range: List of nodes to be added to the JSON object.
-                blank: If True, add empty node to end of node list.
-                           If False, do not add empty node to end of node list.
+            node_range (list[str]): List of nodes to be added to the JSON object.
+            node_name (str): Name of the "main" / "head" key in the JSON schema / object.
+            blank (bool, optional): Defaults to False.
+              If True, add empty node to end of node list.
+              If False, do not add empty node to end of node list.
 
         Returns:
-                JSON object with nodes.
+            dict[str, dict[str, list[str]]]: JSON object with nodes.
         """
         if blank:
             schema_node_range = {node_name: {"enum": node_range + [""]}}
         else:
             schema_node_range = {node_name: {"enum": node_range}}
 
         return schema_node_range
 
     def get_json_validation_schema(
         self, source_node: str, schema_name: str
-    ) -> Dict[str, dict[str, Any]]:
+    ) -> dict[str, dict[str, Any]]:
         """
-        Consolidated method that aims to gather dependencies and value constraints across terms / nodes in a schema.org schema and store them in a jsonschema /JSON Schema schema.
+        Consolidated method that aims to gather dependencies and value constraints across terms
+        / nodes in a schema.org schema and store them in a jsonschema /JSON Schema schema.
 
-        It does so for any given node in the schema.org schema (recursively) using the given node as starting point in the following manner:
-        1) Find all the nodes / terms this node depends on (which are required as "additional metadata" given this node is "required").
-        2) Find all the allowable metadata values / nodes that can be assigned to a particular node (if such a constraint is specified on the schema).
+        It does so for any given node in the schema.org schema (recursively) using the given
+          node as starting point in the following manner:
+        1) Find all the nodes / terms this node depends on (which are required as
+          "additional metadata" given this node is "required").
+        2) Find all the allowable metadata values / nodes that can be assigned to a particular
+          node (if such a constraint is specified on the schema).
 
         Args:
-                source_node: Node from which we can start recursive dependancy traversal (as mentioned above).
-                schema_name: Name assigned to JSON-LD schema (to uniquely identify it via URI when it is hosted on the Internet).
+                source_node: Node from which we can start recursive dependancy traversal
+                  (as mentioned above).
+                schema_name: Name assigned to JSON-LD schema (to uniquely identify it via URI
+                  when it is hosted on the Internet).
 
         Returns:
                 JSON Schema as a dictionary.
         """
+        # pylint:disable=too-many-locals
+        # pylint:disable=too-many-branches
+        # pylint:disable=too-many-statements
+        # pylint:disable=too-many-nested-blocks
+        # pylint:disable=fixme
+
         json_schema = {
             "$schema": "http://json-schema.org/draft-07/schema#",
             "$id": "http://example.com/" + schema_name,
             "title": schema_name,
             "type": "object",
             "properties": {},
             "required": [],
             "allOf": [],
         }
 
-        nodes_to_process = (
-            []
-        )  # list of nodes to be checked for dependencies, starting with the source node
-        processed_nodes = (
-            []
-        )  # keep of track of nodes whose dependencies have been processed
-        reverse_dependencies = (
-            {}
-        )  # maintain a map between conditional nodes and their dependencies (reversed) -- {dependency : conditional_node}
-        range_domain_map = (
-            {}
-        )  # maintain a map between range nodes and their domain nodes {range_value : domain_value}
+        # list of nodes to be checked for dependencies, starting with the source node
+        nodes_to_process = []
+        # keep of track of nodes whose dependencies have been processed
+        processed_nodes = []
+        # maintain a map between conditional nodes and their dependencies
+        # (reversed) -- {dependency : conditional_node}
+        reverse_dependencies: dict[str, Any] = {}
+        # maintain a map between range nodes and their domain nodes {range_value : domain_value}
         # the domain node is very likely the parentof ("parentOf" relationship) of the range node
-
+        range_domain_map: dict[str, Any] = {}
         root_dependencies = self.dmge.get_adjacent_nodes_by_relationship(
             node_label=source_node,
             relationship=self.rel_dict["requiresDependency"]["edge_key"],
         )
 
         # if root_dependencies is empty it means that a class with name 'source_node' exists
         # in the schema, but it is not a valid component
@@ -161,26 +178,29 @@
 
                 # get process node display name
                 node_display_name = self.graph.nodes[process_node][
                     self.rel_dict["displayName"]["node_label"]
                 ]
 
                 # updating map between node and node's valid values
-                for n in node_range_d:
-                    if not n in range_domain_map:
-                        range_domain_map[n] = []
-                    range_domain_map[n].append(node_display_name)
-
-                # can this node be map to the empty set (if required no; if not required yes)
-                # TODO: change "required" to different term, required may be a bit misleading (i.e. is the node required in the schema)
-                node_required = self.dmge.get_node_required(node_label=process_node)
-
-                # get any additional validation rules associated with this node (e.g. can this node be mapped to a list of other nodes)
-                node_validation_rules = self.dmge.get_node_validation_rules(
-                    node_display_name=node_display_name
+                for node in node_range_d:
+                    if not node in range_domain_map:
+                        range_domain_map[node] = []
+                    range_domain_map[node].append(node_display_name)
+
+                # Get node validation rules for the current node, and the given component
+                node_validation_rules = self.dmge.get_component_node_validation_rules(
+                    manifest_component=source_node, node_display_name=node_display_name
+                )
+
+                # Get if the node is required for the given component
+                node_required = self.dmge.get_component_node_required(
+                    manifest_component=source_node,
+                    node_validation_rules=node_validation_rules,
+                    node_display_name=node_display_name,
                 )
 
                 if node_display_name in reverse_dependencies:
                     # if node has conditionals set schema properties and conditional dependencies
                     # set schema properties
                     if node_range:
                         # if process node has valid value range set it in schema properties
@@ -188,15 +208,16 @@
                             node_range=node_range_d,
                             node_name=node_display_name,
                             blank=True,
                         )
 
                         if node_validation_rules:
                             # if this node has extra validation rules process them
-                            # TODO: abstract this into its own validation rule constructor/generator module/class
+                            # TODO: abstract this into its own validation rule constructor/generator
+                            # module/class
                             if rule_in_rule_list("list", node_validation_rules):
                                 # if this node can be mapped to a list of nodes
                                 # set its schema accordingly
                                 schema_valid_vals = self.get_array_schema(
                                     node_range=node_range_d,
                                     node_name=node_display_name,
                                     blank=True,
@@ -207,15 +228,14 @@
                         schema_valid_vals = {node_display_name: {}}
 
                     json_schema["properties"].update(schema_valid_vals)
 
                     # set schema conditional dependencies
                     for node in reverse_dependencies[node_display_name]:
                         # set all of the conditional nodes that require this process node
-
                         # get node domain if any
                         # ow this node is a conditional requirement
                         if node in range_domain_map:
                             domain_nodes = range_domain_map[node]
                             conditional_properties = {}
 
                             for domain_node in domain_nodes:
@@ -223,27 +243,30 @@
                                 conditional_properties.update(
                                     {
                                         "properties": {domain_node: {"enum": [node]}},
                                         "required": [domain_node],
                                     }
                                 )
 
-                                # given node conditional are satisfied, this process node (which is dependent on these conditionals) has to be set or not depending on whether it is required
+                                # given node conditional are satisfied, this process node
+                                # (which is dependent on these conditionals) has to be set
+                                # or not depending on whether it is required
                                 if node_range:
                                     dependency_properties = self.get_range_schema(
                                         node_range=node_range_d,
                                         node_name=node_display_name,
                                         blank=not node_required,
                                     )
 
                                     if node_validation_rules:
                                         if rule_in_rule_list(
                                             "list", node_validation_rules
                                         ):
-                                            # TODO: get_range_schema and get_range_schema have similar behavior - combine in one module
+                                            # TODO: get_range_schema and get_range_schema have
+                                            # similar behavior - combine in one module
                                             dependency_properties = (
                                                 self.get_array_schema(
                                                     node_range=node_range_d,
                                                     node_name=node_display_name,
                                                     blank=not node_required,
                                                 )
                                             )
@@ -295,15 +318,16 @@
                             )
 
                         json_schema["properties"].update(schema_valid_vals)
                         # add node to required fields
                         json_schema["required"] += [node_display_name]
 
                     elif process_node in root_dependencies:
-                        # node doesn't have conditionals and is not required; it belongs in the schema only if it is in root's dependencies
+                        # node doesn't have conditionals and is not required; it belongs in the
+                        # schema only if it is in root's dependencies
 
                         if node_range:
                             schema_valid_vals = self.get_range_schema(
                                 node_range=node_range_d,
                                 node_name=node_display_name,
                                 blank=True,
                             )
@@ -318,17 +342,18 @@
 
                         else:
                             schema_valid_vals = {node_display_name: {}}
 
                         json_schema["properties"].update(schema_valid_vals)
 
                     else:
-                        # node doesn't have conditionals and it is not required and it is not a root dependency
-                        # the node doesn't belong in the schema
-                        # do not add to processed nodes since its conditional may be traversed at a later iteration (though unlikely for most schemas we consider)
+                        # node doesn't have conditionals and it is not required and it
+                        # is not a root dependency the node doesn't belong in the schema
+                        # do not add to processed nodes since its conditional may be traversed
+                        # at a later iteration (though unlikely for most schemas we consider)
                         node_is_processed = False
 
                 # add process node as a conditional to its dependencies
                 node_dependencies_d = self.dmge.get_nodes_display_names(
                     node_list=node_dependencies
                 )
 
@@ -354,30 +379,21 @@
             else:
                 # no more nodes to process
                 # exit the loop
                 break
 
         logger.info("JSON schema successfully generated from schema.org schema!")
 
-        # if no conditional dependencies were added we can't have an empty 'AllOf' block in the schema, so remove it
+        # if no conditional dependencies were added we can't have an empty 'AllOf'
+        # block in the schema, so remove it
         if not json_schema["allOf"]:
             del json_schema["allOf"]
 
         # If no config value and SchemaGenerator was initialized with
         # a JSON-LD path, construct
         if self.jsonld_path is not None:
-            self.jsonld_path_root, jsonld_ext = os.path.splitext(self.jsonld_path)
+            self.jsonld_path_root, _ = os.path.splitext(self.jsonld_path)
             prefix = self.jsonld_path_root
             prefix_root, prefix_ext = os.path.splitext(prefix)
             if prefix_ext == ".model":
                 prefix = prefix_root
-            json_schema_log_file = f"{prefix}.{source_node}.schema.json"
-        """
-		# Commenting out loggins since the JSON Schema file is not currently saved.
-		logger.info(
-			"The JSON schema file can be inspected by setting the following "
-			"nested key in the configuration: (model > location)."
-		)
-
-		logger.info(f"JSON schema file log stored as {json_schema_log_file}")
-		"""
         return json_schema
```

### Comparing `schematicpy-24.2.1/schematic/schemas/data_model_jsonld.py` & `schematicpy-24.4.1/schematic/schemas/data_model_jsonld.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,50 +1,60 @@
-import copy
-from dataclasses import dataclass, field, asdict
-from dataclasses_json import config, dataclass_json
+"""Data Model Jsonld"""
+
 import json
 import logging
+import copy
+from dataclasses import dataclass, field
+from dataclasses_json import config, dataclass_json
 
-from typing import Any, Dict, Optional, Text, List
 import networkx as nx
 
 from schematic.schemas.data_model_graph import DataModelGraphExplorer
 from schematic.schemas.data_model_relationships import DataModelRelationships
 from schematic.utils.schema_utils import (
     get_label_from_display_name,
     convert_bool_to_str,
-    strip_context,
 )
 
 logging.basicConfig()
 logger = logging.getLogger(__name__)
 
+# pylint:disable=fixme
+# pylint:disable=invalid-name
+# pylint:disable=too-many-instance-attributes
+
 
 @dataclass_json
 @dataclass
 class BaseTemplate:
-    magic_context: str = field(
+    """Base Template"""
+
+    magic_context: dict[str, str] = field(
         default_factory=lambda: {
             "bts": "http://schema.biothings.io/",
             "rdf": "http://www.w3.org/1999/02/22-rdf-syntax-ns#",
             "rdfs": "http://www.w3.org/2000/01/rdf-schema#",
             "schema": "http://schema.org/",
             "xsd": "http://www.w3.org/2001/XMLSchema#",
         },
         metadata=config(field_name="@context"),
     )
-    magic_graph: str = field(default_factory=list, metadata=config(field_name="@graph"))
+    magic_graph: list = field(
+        default_factory=list, metadata=config(field_name="@graph")
+    )
     magic_id: str = field(
         default="http://schema.biothings.io/#0.1", metadata=config(field_name="@id")
     )
 
 
 @dataclass_json
 @dataclass
 class PropertyTemplate:
+    """Property Template"""
+
     magic_id: str = field(default="", metadata=config(field_name="@id"))
     magic_type: str = field(default="rdf:Property", metadata=config(field_name="@type"))
     magic_comment: str = field(default="", metadata=config(field_name="rdfs:comment"))
     magic_label: str = field(default="", metadata=config(field_name="rdfs:label"))
     magic_domain_includes: list = field(
         default_factory=list, metadata=config(field_name="schema:domainIncludes")
     )
@@ -64,14 +74,15 @@
         default_factory=list, metadata=config(field_name="sms:validationRules")
     )
 
 
 @dataclass_json
 @dataclass
 class ClassTemplate:
+    "Class Template"
     magic_id: str = field(default="", metadata=config(field_name="@id"))
     magic_type: str = field(default="rdfs:Class", metadata=config(field_name="@type"))
     magic_comment: str = field(default="", metadata=config(field_name="rdfs:comment"))
     magic_label: str = field(default="", metadata=config(field_name="rdfs:label"))
     magic_subClassOf: list = field(
         default_factory=list, metadata=config(field_name="rdfs:subClassOf")
     )
@@ -94,199 +105,218 @@
         default_factory=list, metadata=config(field_name="sms:requiresComponent")
     )
     magic_validationRules: list = field(
         default_factory=list, metadata=config(field_name="sms:validationRules")
     )
 
 
-class DataModelJsonLD(object):
+class DataModelJsonLD:
     """
     #Interface to JSONLD_object
     """
 
-    def __init__(self, Graph: nx.MultiDiGraph, output_path: str = ""):
+    def __init__(self, graph: nx.MultiDiGraph, output_path: str = ""):
         # Setup
-        self.graph = Graph  # Graph would be fully made at this point.
+        self.graph = graph  # Graph would be fully made at this point.
         self.dmr = DataModelRelationships()
         self.rel_dict = self.dmr.relationships_dictionary
         self.dmge = DataModelGraphExplorer(self.graph)
         self.output_path = output_path
 
         # Gather the templates
         base_template = BaseTemplate()
-        self.base_jsonld_template = json.loads(base_template.to_json())
+        self.base_jsonld_template = json.loads(
+            base_template.to_json()  # pylint:disable=no-member
+        )
 
         property_template = PropertyTemplate()
-        self.property_template = json.loads(property_template.to_json())
+        self.property_template = json.loads(
+            property_template.to_json()  # pylint:disable=no-member
+        )
 
         class_template = ClassTemplate()
-        self.class_template = json.loads(class_template.to_json())
+        self.class_template = json.loads(
+            class_template.to_json()  # pylint:disable=no-member
+        )
 
     def get_edges_associated_with_node(
         self, node: str
-    ) -> List[tuple[str, str, dict[str, int]]]:
+    ) -> list[tuple[str, str, dict[str, int]]]:
         """Retrieve all edges traveling in and out of a node.
         Args:
             node, str: Label of node in the graph to look for assiciated edges
         Returns:
-            node_edges, list: List of Tuples of edges associated with the given node, tuple contains the two nodes, plus the weight dict associated with the edge connection.
+            node_edges, list: List of Tuples of edges associated with the given node,
+              tuple contains the two nodes, plus the weight dict associated with
+              the edge connection.
         """
         node_edges = list(self.graph.in_edges(node, data=True))
         node_edges.extend(list(self.graph.out_edges(node, data=True)))
         return node_edges
 
     def get_edges_associated_with_property_nodes(
         self, node: str
-    ) -> List[tuple[str, str, dict[str, int]]]:
+    ) -> list[tuple[str, str, dict[str, int]]]:
         """Get edges associated with property nodes to make sure we add that relationship.
         Args:
             node, str: Label of node property in the graph to look for assiciated edges
         Returns:
-            node_edges, list: List of Tuples of edges associated with the given node, tuple contains the two nodes, plus the weight dict associated with the edge connection.
+            node_edges, list: List of Tuples of edges associated with the given node,
+              tuple contains the two nodes, plus the weight dict associated with the
+              edge connection.
         """
         # Get edge keys for domainIncludes and subclassOf
-        domainIncludes_edge_key = self.rel_dict["domainIncludes"]["edge_key"]
+        domain_includes_edge_key = self.rel_dict["domainIncludes"]["edge_key"]
         node_edges = []
         # Get dict of edges for the current property node
         node_edges_dict = self.graph[node]
         for node_2, edge_dict in node_edges_dict.items():
             # Look through relationships in the edge dictionary
             for edge_key in edge_dict:
                 # If the edge is a property or subclass then add the edges to the list
-                if edge_key in [domainIncludes_edge_key]:
+                if edge_key in [domain_includes_edge_key]:
                     node_edges.append((node, node_2, edge_dict[edge_key]))
         return node_edges
 
-    def add_edge_rels_to_template(self, template: dict, rel_vals: dict, node: str):
+    def add_edge_rels_to_template(
+        self, template: dict, rel_vals: dict, node: str
+    ):  # pylint:disable=too-many-branches
         """
         Args:
-            template, dict: single class or property JSONLD template that is in the process of being filled.
-            rel_vals, dict: sub relationship dict for a given relationship (contains informtion like, 'edge_rel', 'jsonld_key' etc..)
+            template, dict: single class or property JSONLD template that is in the process of being
+             filled.
+            rel_vals, dict: sub relationship dict for a given relationship (contains informtion
+              like 'edge_rel', 'jsonld_key' etc..)
             node, str: node whose edge information is presently being added to the JSONLD
         Returns:
         """
         # Get all edges associated with the current node
         node_edges = self.get_edges_associated_with_node(node=node)
 
         # For properties look for reverse relationships too
         if node in self.dmge.find_properties():
             property_node_edges = self.get_edges_associated_with_property_nodes(
                 node=node
             )
             node_edges.extend(property_node_edges)
 
         # Get node pairs and weights for each edge
-        for node_1, node_2, weight in node_edges:
+        for node_1, node_2, _ in node_edges:  # pylint:disable=too-many-nested-blocks
             # Retrieve the relationship(s) and related info between the two nodes
             node_edge_relationships = self.graph[node_1][node_2]
 
             # Get the relationship edge key
             edge_key = rel_vals["edge_key"]
 
             # Check if edge_key is even one of the relationships for this node pair.
             if edge_key in node_edge_relationships:
                 # for each relationship between the given nodes
-                for relationship, weight_dict in node_edge_relationships.items():
+                for relationship in node_edge_relationships.keys():
                     # If the relationship defined and edge_key
                     if relationship == edge_key:
                         # TODO: rewrite to use edge_dir
-                        domainIncludes_edge_key = self.rel_dict["domainIncludes"][
+                        domain_includes_edge_key = self.rel_dict["domainIncludes"][
                             "edge_key"
                         ]
-                        subclassOf_edge_key = self.rel_dict["subClassOf"]["edge_key"]
-                        if edge_key in [subclassOf_edge_key]:
+                        subclass_of_edge_key = self.rel_dict["subClassOf"]["edge_key"]
+                        if edge_key in [subclass_of_edge_key]:
                             if node_2 == node:
-                                # Make sure the key is in the template (differs between properties and classes)
+                                # Make sure the key is in the template
+                                # (differs between properties and classes)
                                 if rel_vals["jsonld_key"] in template.keys():
                                     node_1_id = {"@id": "bts:" + node_1}
                                     # TODO Move this to a helper function to clear up.
                                     if (
                                         isinstance(
                                             template[rel_vals["jsonld_key"]], list
                                         )
                                         and node_1_id
                                         not in template[rel_vals["jsonld_key"]]
                                     ):
                                         template[rel_vals["jsonld_key"]].append(
                                             node_1_id
                                         )
-                                    else:
-                                        template[rel_vals["jsonld_key"]] == node_1
-                        elif edge_key in [domainIncludes_edge_key]:
+                        elif edge_key in [domain_includes_edge_key]:
                             if node_1 == node:
-                                # Make sure the key is in the template (differs between properties and classes)
+                                # Make sure the key is in the template
+                                # (differs between properties and classes)
                                 if rel_vals["jsonld_key"] in template.keys():
                                     node_2_id = {"@id": "bts:" + node_2}
                                     # TODO Move this to a helper function to clear up.
                                     if (
                                         isinstance(
                                             template[rel_vals["jsonld_key"]], list
                                         )
                                         and node_2_id
                                         not in template[rel_vals["jsonld_key"]]
                                     ):
                                         template[rel_vals["jsonld_key"]].append(
                                             node_2_id
                                         )
-                                    else:
-                                        template[rel_vals["jsonld_key"]] == node_2
                         else:
                             if node_1 == node:
-                                # Make sure the key is in the template (differs between properties and classes)
+                                # Make sure the key is in the template
+                                # (differs between properties and classes)
                                 if rel_vals["jsonld_key"] in template.keys():
                                     node_2_id = {"@id": "bts:" + node_2}
                                     # TODO Move this to a helper function to clear up.
                                     if (
                                         isinstance(
                                             template[rel_vals["jsonld_key"]], list
                                         )
                                         and node_2_id
                                         not in template[rel_vals["jsonld_key"]]
                                     ):
                                         template[rel_vals["jsonld_key"]].append(
                                             node_2_id
                                         )
-                                    else:
-                                        template[rel_vals["jsonld_key"]] == node_2
         return template
 
     def add_node_info_to_template(self, template, rel_vals, node):
         """For a given node and relationship, add relevant value to template
         Args:
-            template, dict: single class or property JSONLD template that is in the process of being filled.
-            rel_vals, dict: sub relationship dict for a given relationship (contains informtion like, 'edge_rel', 'jsonld_key' etc..)
+            template, dict: single class or property JSONLD template that is in the process
+              of being filled.
+            rel_vals, dict: sub relationship dict for a given relationship
+              (contains informtion like, 'edge_rel', 'jsonld_key' etc..)
             node, str: node whose information is presently being added to the JSONLD
         Returns:
-            template, dict: single class or property JSONLD template that is in the process of being filled, and now has had additional node information added.
+            template, dict: single class or property JSONLD template that is in the
+              process of being filled, and now has had additional node information added.
         """
         # Get label for relationship used in the graph
         node_label = rel_vals["node_label"]
 
         # Get recorded info for current node, and the attribute type
         node_info = nx.get_node_attributes(self.graph, node_label)[node]
 
         # Add this information to the template
         template[rel_vals["jsonld_key"]] = node_info
         return template
 
     def fill_entry_template(self, template: dict, node: str) -> dict:
-        """Fill in a blank JSONLD template with information for each node. All relationships are filled from the graph, based on the type of information (node or edge)
+        """
+        Fill in a blank JSONLD template with information for each node.
+        All relationships are filled from the graph, based on the type of information
+          (node or edge)
+
         Args:
-            template, dict: empty class or property template to be filled with information for the given node.
+            template, dict: empty class or property template to be filled with
+              information for the given node.
             node, str: target node to fill the template out for.
         Returns:
-            template, dict: filled class or property template, that has been processed and cleaned up.
+            template, dict: filled class or property template, that has been
+              processed and cleaned up.
         """
         data_model_relationships = self.dmr.relationships_dictionary
 
         # For each field in template fill out with information from the graph
-        for rel, rel_vals in data_model_relationships.items():
-            key_context, key_rel = strip_context(context_value=rel_vals["jsonld_key"])
-
-            # Fill in the JSONLD template for this node, with data from the graph by looking up the nodes edge relationships, and the value information attached to the node.
+        for rel_vals in data_model_relationships.values():
+            # Fill in the JSONLD template for this node, with data from the graph by looking
+            # up the nodes edge relationships, and the value information attached to the node.
 
             # Fill edge information (done per edge type)
             if rel_vals["edge_rel"]:
                 template = self.add_edge_rels_to_template(
                     template=template, rel_vals=rel_vals, node=node
                 )
 
@@ -313,39 +343,42 @@
         )
 
         return template
 
     def add_contexts_to_entries(self, template: dict) -> dict:
         """
         Args:
-            template, dict: JSONLD template that has been filled up to the current node, with information
+            template, dict: JSONLD template that has been filled up to
+              the current node, with information
         Returns:
             template, dict: JSONLD template where contexts have been added back to certain values.
         Note: This will likely need to be modified when Contexts are truly added to the model
         """
-        for jsonld_key, entry in template.items():
+        # pylint:disable=comparison-with-callable
+        for jsonld_key in template.keys():
             # Retrieve the relationships key using the jsonld_key
             rel_key = []
 
             for rel, rel_vals in self.rel_dict.items():
                 if "jsonld_key" in rel_vals and jsonld_key == rel_vals["jsonld_key"]:
                     rel_key.append(rel)
 
             if rel_key:
                 rel_key = rel_key[0]
                 # If the current relationship can be defined with a 'node_attr_dict'
                 if "node_attr_dict" in self.rel_dict[rel_key].keys():
                     try:
                         # if possible pull standard function to get node information
                         rel_func = self.rel_dict[rel_key]["node_attr_dict"]["standard"]
-                    except:
+                    except:  # pylint:disable=bare-except
                         # if not pull default function to get node information
                         rel_func = self.rel_dict[rel_key]["node_attr_dict"]["default"]
 
-                    # Add appropritae contexts that have been removed in previous steps (for JSONLD) or did not exist to begin with (csv)
+                    # Add appropritae contexts that have been removed in previous steps
+                    # (for JSONLD) or did not exist to begin with (csv)
                     if (
                         rel_key == "id"
                         and rel_func == get_label_from_display_name
                         and "bts" not in str(template[jsonld_key]).lower()
                     ):
                         template[jsonld_key] = "bts:" + template[jsonld_key]
                     elif (
@@ -356,85 +389,105 @@
                         template[jsonld_key] = (
                             "sms:" + str(template[jsonld_key]).lower()
                         )
 
         return template
 
     def clean_template(self, template: dict, data_model_relationships: dict) -> dict:
-        """Get rid of empty k:v pairs. Fill with a default if specified in the relationships dictionary.
+        """
+        Get rid of empty k:v pairs. Fill with a default if specified in the
+          relationships dictionary.
+
         Args:
-            template, dict: JSONLD template for a single entry, keys specified in property and class templates.
-            data_model_relationships, dict: dictionary containing information for each relationship type supported.
+            template, dict: JSONLD template for a single entry, keys specified in property
+              and class templates.
+            data_model_relationships, dict: dictionary containing information for each
+              relationship type supported.
         Returns:
-            template: JSONLD template where unfilled entries have been removed, or filled with default depending on specifications in the relationships dictionary.
+            template: JSONLD template where unfilled entries have been removed,
+              or filled with default depending on specifications in the relationships dictionary.
         """
         for rels in data_model_relationships.values():
             # Get the current relationships, jsonld key
             relationship_jsonld_key = rels["jsonld_key"]
-            # Check if the relationship_relationship_key is part of the template, and if it is, look to see if it has an entry
+            # Check if the relationship_relationship_key is part of the template,
+            # and if it is, look to see if it has an entry
             if (
                 relationship_jsonld_key in template.keys()
                 and not template[rels["jsonld_key"]]
             ):
-                # If there is no value recorded, fill out the template with the default relationship value (if recorded.)
+                # If there is no value recorded, fill out the template with the
+                # default relationship value (if recorded.)
                 if "jsonld_default" in rels.keys():
                     template[relationship_jsonld_key] = rels["jsonld_default"]
                 else:
-                    # If there is no default specified in the relationships dictionary, delete the empty value from the template.
+                    # If there is no default specified in the relationships dictionary,
+                    # delete the empty value from the template.
                     del template[relationship_jsonld_key]
         return template
 
     def reorder_template_entries(self, template: dict) -> dict:
-        """In JSONLD some classes or property keys have list values. We want to make sure these lists are ordered according to the order supplied by the user.
+        """
+        In JSONLD some classes or property keys have list values.
+        We want to make sure these lists are ordered according to the order supplied by the user.
         This will look specically in lists and reorder those.
+
         Args:
-            template, dict: JSONLD template for a single entry, keys specified in property and class templates.
+            template, dict: JSONLD template for a single entry, keys specified in
+              property and class templates.
         Returns:
             template, dict: list entries re-ordered to match user supplied order.
         Note:
             User order only matters for nodes that are also attributes
         """
         template_label = template["rdfs:label"]
 
         for jsonld_key, entry in template.items():
             # Make sure dealing with an edge relationship:
             is_edge = [
                 "True"
-                for rel_key, rel_vals in self.rel_dict.items()
+                for rel_vals in self.rel_dict.values()
                 if rel_vals["jsonld_key"] == jsonld_key
-                if rel_vals["edge_rel"] == True
+                if rel_vals["edge_rel"]
             ]
 
-            # if the entry is of type list and theres more than one value in the list attempt to reorder
+            # if the entry is of type list and theres more than one value in the
+            # list attempt to reorder
             if is_edge and isinstance(entry, list) and len(entry) > 1:
                 # Get edge key from data_model_relationships using the jsonld_key:
-                key, edge_key = [
+                key, _ = [
                     (rel_key, rel_vals["edge_key"])
                     for rel_key, rel_vals in self.rel_dict.items()
                     if jsonld_key == rel_vals["jsonld_key"]
                 ][0]
 
                 # Order edges
                 sorted_edges = self.dmge.get_ordered_entry(
                     key=key, source_node_label=template_label
                 )
                 if not len(entry) == len(sorted_edges):
                     logger.error(
-                        "There is an error with sorting values in the JSONLD, please issue a bug report."
+                        (
+                            "There is an error with sorting values in the JSONLD, "
+                            "please issue a bug report."
+                        )
                     )
 
                 edge_weights_dict = {edge: i for i, edge in enumerate(sorted_edges)}
                 ordered_edges = [0] * len(edge_weights_dict.keys())
                 for edge, normalized_weight in edge_weights_dict.items():
                     ordered_edges[normalized_weight] = {"@id": "bts:" + edge}
 
                 # Throw an error if ordered_edges does not get fully filled as expected.
                 if 0 in ordered_edges:
                     logger.error(
-                        "There was an issue getting values to match order specified in the data model, please submit a help request."
+                        (
+                            "There was an issue getting values to match order specified in "
+                            "the data model, please submit a help request."
+                        )
                     )
                 template[jsonld_key] = ordered_edges
         return template
 
     def generate_jsonld_object(self):
         """Create the JSONLD object.
         Returns:
@@ -456,12 +509,13 @@
                 # Get class template
                 class_template = copy.deepcopy(self.class_template)
                 obj = self.fill_entry_template(template=class_template, node=node)
             json_ld_template["@graph"].append(obj)
         return json_ld_template
 
 
-def convert_graph_to_jsonld(Graph):
+def convert_graph_to_jsonld(graph):
+    """convert graph to jsonld"""
     # Make the JSONLD object
-    data_model_jsonld_converter = DataModelJsonLD(Graph=Graph)
+    data_model_jsonld_converter = DataModelJsonLD(graph=graph)
     jsonld_dm = data_model_jsonld_converter.generate_jsonld_object()
     return jsonld_dm
```

### Comparing `schematicpy-24.2.1/schematic/schemas/data_model_nodes.py` & `schematicpy-24.4.1/schematic/schemas/data_model_nodes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,48 +1,55 @@
+"""Data model Nodes"""
+
+from typing import Optional, Callable
+
 from inspect import isfunction
-import networkx as nx
+import networkx as nx  # type: ignore
 from rdflib import Namespace
-from typing import Any, Dict, Optional, Text, List, Literal, Callable
 
-from schematic.schemas.data_model_parser import DataModelJSONLDParser
 from schematic.schemas.data_model_relationships import DataModelRelationships
 
 from schematic.utils.schema_utils import (
     get_label_from_display_name,
     get_attribute_display_name_from_label,
     convert_bool_to_str,
     parse_validation_rules,
     DisplayLabelType,
 )
-from schematic.utils.validate_rules_utils import validate_schema_rules
-from schematic.schemas.curie import uri2curie, curie2uri
 
 
 class DataModelNodes:
+    """Data model Nodes"""
+
     def __init__(self, attribute_relationships_dict):
-        self.namespaces = dict(
-            rdf=Namespace("http://www.w3.org/1999/02/22-rdf-syntax-ns#")
-        )
+        self.namespaces = {
+            "rdf": Namespace("http://www.w3.org/1999/02/22-rdf-syntax-ns#")
+        }
         self.data_model_relationships = DataModelRelationships()
         self.value_relationships = (
             self.data_model_relationships.retreive_rel_headers_dict(edge=False)
         )
         self.edge_relationships_dictionary = (
             self.data_model_relationships.retreive_rel_headers_dict(edge=True)
         )
         self.properties = self.get_data_model_properties(
             attr_rel_dict=attribute_relationships_dict
         )
         # retrieve a list of relationship types that will produce nodes.
         self.node_relationships = list(self.edge_relationships_dictionary.values())
 
     def gather_nodes(self, attr_info: tuple) -> list:
-        """Take in a tuple containing attriute name and relationship dictionary, and find all nodes defined in attribute information.
+        """
+        Take in a tuple containing attriute name and relationship dictionary,
+          and find all nodes defined in attribute information.
+
         Args:
-            attr_info, tuple: (Display Name, Relationships Dictionary portion of attribute_relationships dictionary)
+            attr_info, tuple: (Display Name, Relationships Dictionary portion of
+              attribute_relationships dictionary)
+
         Returns:
             nodes, list: nodes related to the given node (specified in attr_info).
         Note:
             Extracting nodes in this fashion ensures order is preserved.
         """
 
         # Extract attribute and relationship dictionary
@@ -61,15 +68,16 @@
         """Gather all nodes in the data model, in order.
         Args:
             attr_rel_dict, dict: generated in data_model_parser
                 {Attribute Display Name: {
                         Relationships: {
                                     CSV Header: Value}}}
         Returns:
-            all_nodes, list: List of all node display names in the data model preserving order entered.
+            all_nodes, list: List of all node display names in the data model
+              preserving order entered.
         Note:
             Gathering nodes in this fashion ensures order is preserved.
         """
         all_nodes = []
         for attr_info in attr_rel_dict.items():
             nodes = self.gather_nodes(attr_info=attr_info)
             all_nodes.extend(nodes)
@@ -79,36 +87,41 @@
 
     def get_rel_node_dict_info(self, relationship: str) -> Optional[tuple[str, dict]]:
         """For each display name get defaults for nodes.
         Args:
             relationship, str: relationship key to match.
         Returns:
             rel_key, str: relationship node label
-            rel_node_dict, dict: node_attr_dict, from relationships dictionary for a given relationship
+            rel_node_dict, dict: node_attr_dict, from relationships dictionary for a
+              given relationship
         TODO: Move to data_model_relationships.
         """
-        for k, v in self.data_model_relationships.relationships_dictionary.items():
-            if k == relationship:
-                if "node_attr_dict" in v.keys():
-                    rel_key = v["node_label"]
-                    rel_node_dict = v["node_attr_dict"]
+        for (
+            key,
+            value,
+        ) in self.data_model_relationships.relationships_dictionary.items():
+            if key == relationship:
+                if "node_attr_dict" in value:
+                    rel_key = value["node_label"]
+                    rel_node_dict = value["node_attr_dict"]
                     return rel_key, rel_node_dict
+        return None
 
     def get_data_model_properties(self, attr_rel_dict: dict) -> list:
         """Identify all properties defined in the data model.
         Args:
             attr_rel_dict, dict:
                 {Attribute Display Name: {
                         Relationships: {
                                     CSV Header: Value}}}
         Returns:
             properties,list: properties defined in the data model
         """
         properties = []
-        for attribute, relationships in attr_rel_dict.items():
+        for relationships in attr_rel_dict.values():
             if "Properties" in relationships["Relationships"].keys():
                 properties.extend(relationships["Relationships"]["Properties"])
         properties = list(set(properties))
         return properties
 
     def get_entry_type(self, node_display_name: str) -> str:
         """Get the entry type of the node, property or class.
@@ -121,92 +134,117 @@
             entry_type = "property"
         else:
             entry_type = "class"
         return entry_type
 
     def run_rel_functions(
         self,
-        rel_func: callable,
+        rel_func: Callable,
         node_display_name: str = "",
         key: str = "",
-        attr_relationships={},
+        attr_relationships=None,
         csv_header="",
         entry_type="",
         data_model_labels: DisplayLabelType = "class_label",
     ):
-        """This function exists to centralzie handling of functions for filling out node information, makes sure all the proper parameters are passed to each function.
+        """
+        This function exists to centralzie handling of functions for filling out node information,
+          makes sure all the proper parameters are passed to each function.
+
         Args:
             rel_func, callable: Function to call to get information to attach to the node
             node_display_name, str: node display name
             key, str: relationship key
             attr_relationships, dict: relationships portion of attributes_relationships dictionary
             csv_header, str: csv header
             entry_type, str: 'class' or 'property' defines how
 
         Returns:
             Outputs of specified rel_func (relationship function)
 
         For legacy:
         elif key == 'id' and rel_func == get_label_from_display_name:
-            func_output = get_label_from_display_name(display_name =node_display_name, entry_type=entry_type)
+            func_output = get_label_from_display_name(
+                display_name =node_display_name, entry_type=entry_type
+            )
         """
+        # pylint: disable=too-many-arguments
+        # pylint: disable=too-many-return-statements
+        # pylint: disable=comparison-with-callable
+        if attr_relationships is None:
+            attr_relationships = {}
+
         if rel_func == get_attribute_display_name_from_label:
             return get_attribute_display_name_from_label(
                 node_display_name, attr_relationships
             )
 
-        elif rel_func == parse_validation_rules:
-            return parse_validation_rules(attr_relationships[csv_header])
+        if rel_func == parse_validation_rules:
+            rules = attr_relationships[csv_header]
+            if isinstance(rules, (dict, list)):
+                return parse_validation_rules(rules)
 
-        elif rel_func == get_label_from_display_name:
+        if rel_func == get_label_from_display_name:
             return get_label_from_display_name(
                 display_name=node_display_name,
                 entry_type=entry_type,
                 data_model_labels=data_model_labels,
             )
 
-        elif rel_func == convert_bool_to_str:
-            if type(attr_relationships[csv_header]) == str:
+        if rel_func == convert_bool_to_str:
+            if isinstance(attr_relationships[csv_header], str):
                 if attr_relationships[csv_header].lower() == "true":
                     return True
-                elif attr_relationships[csv_header].lower() == "false":
+                if attr_relationships[csv_header].lower() == "false":
                     return False
+                return None
 
-            elif type(attr_relationships[csv_header]) == bool:
+            if isinstance(attr_relationships[csv_header], bool):
                 return attr_relationships[csv_header]
 
-        else:
-            # Raise Error if the rel_func provided is not captured.
-            raise ValueError(
-                f"The function provided ({rel_func}) to define the relationship {key} is not captured in the function run_rel_functions, please update."
+            return None
+
+        # Raise Error if the rel_func provided is not captured.
+        raise ValueError(
+            (
+                f"The function provided ({rel_func}) to define the relationship {key} "
+                "is not captured in the function run_rel_functions, please update."
             )
+        )
 
     def generate_node_dict(
         self,
         node_display_name: str,
         attr_rel_dict: dict,
         data_model_labels: DisplayLabelType = "class_label",
     ) -> dict:
         """Gather information to be attached to each node.
+
+        Note:
+            If the default calls function, call that function for the default or alternate
+              implementation.
+            May need to update this logic for varying function calls. (for example the current
+              function takes in the node display name would need to update if new function took
+              in something else.)
+
         Args:
-            node_display_name, str: display name for current node
-            attr_rel_dict, dict: generated in data_model_parser
-                {Attribute Display Name: {
+            node_display_name (str): display name for current node
+            attr_rel_dict (dict): generated in data_model_parser
+              {Attribute Display Name: {
                         Relationships: {
                                     CSV Header: Value}}}
-            data_model_labels: str, display_label or class_label.
-                display_label, use the display name as a label, if it is valid (contains no blacklisted characters) otherwise will default to schema_label.
+            data_model_labels (DisplayLabelType, optional):str, display_label or class_label.
+                display_label, use the display name as a label, if it is valid (contains no
+                  blacklisted characters) otherwise will default to schema_label.
                 class_label, default, use standard class or property label.
+
         Returns:
-            node_dict, dict: dictionary of relationship information about the current node
-                {'displayName': '', 'label': '', 'comment': 'TBD', 'required': None, 'validationRules': [], 'isPartOf': '', 'uri': ''}
-        Note:
-            If the default calls function, call that function for the default or alternate implementation.
-            May need to update this logic for varying function calls. (for example the current function takes in the node display name
-            would need to update if new function took in something else.)
+            dict: dictionary of relationship information about the current node
+                {'displayName': '', 'label': '', 'comment': 'TBD', 'required': None,
+                 'validationRules': [], 'isPartOf': '', 'uri': ''}
         """
         # Strip whitespace from node display name
         node_display_name = node_display_name.strip()
 
         # Determine if property or class
         entry_type = self.get_entry_type(node_display_name=node_display_name)
 
@@ -267,21 +305,23 @@
                     )
                 else:
                     # Set value to defaults.
                     node_dict.update({rel_key: rel_node_dict["default"]})
 
         return node_dict
 
-    def generate_node(self, G: nx.MultiDiGraph, node_dict: dict) -> nx.MultiDiGraph:
+    def generate_node(self, graph: nx.MultiDiGraph, node_dict: dict) -> nx.MultiDiGraph:
         """Create a node and add it to the networkx multidigraph being built
         Args:
-            G, nx.MultiDigraph: networkx multidigraph object, that is in the process of being fully built.
+            graph, nx.MultiDigraph: networkx multidigraph object, that is in the process of
+              being fully built.
             node_dict, dict: dictionary of relationship information about the current node
         Returns:
-            G, nx.MultiDigraph: networkx multidigraph object, that has had an additional node added to it.
+            nx.MultiDigraph: networkx multidigraph object, that has had an additional
+              node added to it.
         """
-        G.add_node(node_dict["label"], **node_dict)
-        return G
+        graph.add_node(node_dict["label"], **node_dict)
+        return graph
 
     def edit_node(self):
         """Stub for future node editor."""
         return
```

### Comparing `schematicpy-24.2.1/schematic/schemas/data_model_parser.py` & `schematicpy-24.4.1/schematic/schemas/data_model_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-import logging
-import pandas as pd
+"Data Model Parser"
+
 import pathlib
+from typing import Any, Union, Optional
 
-from typing import Any, Dict, Optional, Text, List, Union
+import logging
+import pandas as pd
 
 from schematic.utils.df_utils import load_df
 from schematic.utils.io_utils import load_json
 from schematic.utils.schema_utils import attr_dict_template
 
 from schematic.schemas.data_model_relationships import DataModelRelationships
 
@@ -29,17 +31,17 @@
         """
         Args:
             path_to_data_model, str: path to data model.
         """
 
         self.path_to_data_model = path_to_data_model
         self.model_type = self.get_model_type()
-        self.base_schema_path = None
+        self.base_schema_path: Optional[str] = None
 
-    def _get_base_schema_path(self, base_schema: str = None) -> str:
+    def _get_base_schema_path(self, base_schema: Optional[str] = None) -> str:
         """Evaluate path to base schema.
 
         Args:
             base_schema: Path to base data model. BioThings data model is loaded by default.
 
         Returns:
             base_schema_path: Path to base schema based on provided argument.
@@ -48,24 +50,27 @@
         self.base_schema_path = (
             biothings_schema_path if base_schema is None else base_schema
         )
 
         return self.base_schema_path
 
     def get_model_type(self) -> str:
-        """Parses the path to the data model to extract the extension and determine the data model type.
+        """
+        Parses the path to the data model to extract the extension and determine the
+          data model type.
+
         Args:
             path_to_data_model, str: path to data model
         Returns:
             str: uppercase, data model file extension.
         Note: Consider moving this to Utils.
         """
         return pathlib.Path(self.path_to_data_model).suffix.replace(".", "").upper()
 
-    def parse_base_model(self) -> Dict:
+    def parse_base_model(self) -> dict:
         """Parse base data model that new model could be built upon.
         Returns:
             base_model, dict:
                     {Attribute Display Name: {
                         Relationships: {
                                     CSV Header: Value}}}
         Note: Not configured yet to successfully parse biothings.
@@ -75,115 +80,126 @@
         base_model_path = self._get_base_schema_path(self.base_schema_path)
 
         # Parse
         jsonld_parser = DataModelJSONLDParser()
         base_model = jsonld_parser.parse_jsonld_model(base_model_path)
         return base_model
 
-    def parse_model(self) -> Dict[str, dict[str, Any]]:
+    def parse_model(self) -> dict[str, dict[str, Any]]:
         """Given a data model type, instantiate and call the appropriate data model parser.
         Returns:
             model_dict, dict:
                 {Attribute Display Name: {
                         Relationships: {
                                     CSV Header: Value}}}
         Raises:
             Value Error if an incorrect model type is passed.
-        Note: in future will add base model parsing in this step too and extend new model off base model.
+        Note: in future will add base model parsing in this step too and extend new model
+          off base model.
         """
         # base_model = self.parse_base_model()
 
         # Call appropriate data model parser and return parsed model.
         if self.model_type == "CSV":
             csv_parser = DataModelCSVParser()
             model_dict = csv_parser.parse_csv_model(self.path_to_data_model)
         elif self.model_type == "JSONLD":
             jsonld_parser = DataModelJSONLDParser()
             model_dict = jsonld_parser.parse_jsonld_model(self.path_to_data_model)
         else:
             raise ValueError(
-                f"Schematic only accepts models of type CSV or JSONLD, you provided a model type {self.model_type}, please resubmit in the proper format."
+                (
+                    "Schematic only accepts models of type CSV or JSONLD, "
+                    "you provided a model type "
+                    f"{self.model_type}, please resubmit in the proper format."
+                )
             )
         return model_dict
 
 
 class DataModelCSVParser:
+    """DataModelCSVParser"""
+
     def __init__(self):
         # Instantiate DataModelRelationships
         self.dmr = DataModelRelationships()
         # Load relationships dictionary.
         self.rel_dict = self.dmr.define_data_model_relationships()
         # Get edge relationships
         self.edge_relationships_dictionary = self.dmr.retreive_rel_headers_dict(
             edge=True
         )
         # Load required csv headers
         self.required_headers = self.dmr.define_required_csv_headers()
         # Get the type for each value that needs to be submitted.
         # using csv_headers as keys to match required_headers/relationship_types
         self.rel_val_types = {
-            v["csv_header"]: v["type"]
-            for k, v in self.rel_dict.items()
-            if "type" in v.keys()
+            value["csv_header"]: value["type"]
+            for value in self.rel_dict.values()
+            if "type" in value
         }
 
-    def check_schema_definition(self, model_df: pd.DataFrame) -> bool:
+    def check_schema_definition(self, model_df: pd.DataFrame) -> None:
         """Checks if a schema definition data frame contains the right required headers.
         Args:
-            model_df: a pandas dataframe containing schema definition; see example here: https://docs.google.com/spreadsheets/d/1J2brhqO4kpeHIkNytzlqrdIiRanXDr6KD2hqjOTC9hs/edit#gid=0
+            model_df: a pandas dataframe containing schema definition; see example here:
+              https://docs.google.com/spreadsheets/d/1J2brhqO4kpeHIkNytzlqrdIiRanXDr6KD2hqjOTC9hs/edit#gid=0
         Raises: Exception if model_df does not have the required headers.
         """
-        if set(self.required_headers).issubset(set(list(model_df.columns))):
-            logger.debug("Schema definition csv ready for processing!")
-            return
-        elif "Requires" in list(model_df.columns) or "Requires Component" in list(
+        if "Requires" in list(model_df.columns) or "Requires Component" in list(
             model_df.columns
         ):
             raise ValueError(
                 "The input CSV schema file contains the 'Requires' and/or the 'Requires "
                 "Component' column headers. These columns were renamed to 'DependsOn' and "
                 "'DependsOn Component', respectively. Switch to the new column names."
             )
-        elif not set(self.required_headers).issubset(set(list(model_df.columns))):
+        if not set(self.required_headers).issubset(set(list(model_df.columns))):
             raise ValueError(
                 f"Schema extension headers: {set(list(model_df.columns))} "
                 f"do not match required schema headers: {self.required_headers}"
             )
-        return
+        if set(self.required_headers).issubset(set(list(model_df.columns))):
+            logger.debug("Schema definition csv ready for processing!")
 
     def parse_entry(self, attr: dict, relationship: str) -> Any:
         """Parse attr entry baed on type
         Args:
-            attr, dict: single row of a csv model in dict form, where only the required headers are keys. Values are the entries under each header.
+            attr, dict: single row of a csv model in dict form, where only the required
+              headers are keys. Values are the entries under each header.
             relationship, str: one of the header relationships to parse the entry of.
         Returns:
             parsed_rel_entry, any: parsed entry for downstream processing based on the entry type.
         """
 
         rel_val_type = self.rel_val_types[relationship]
         # Parse entry based on type:
         # If the entry should be preserved as a bool dont convert to str.
-        if rel_val_type == bool and type(attr[relationship]) == bool:
+        if rel_val_type == bool and isinstance(attr[relationship], bool):
             parsed_rel_entry = attr[relationship]
-        # Move strings to list if they are comma separated. Schema order is preserved, remove any empty strings added by trailing commas
+        # Move strings to list if they are comma separated. Schema order is preserved,
+        # remove any empty strings added by trailing commas
         elif rel_val_type == list:
             parsed_rel_entry = attr[relationship].strip().split(",")
             parsed_rel_entry = [r.strip() for r in parsed_rel_entry if r]
         # Convert value string if dictated by rel_val_type, strip whitespace.
         elif rel_val_type == str:
             parsed_rel_entry = str(attr[relationship]).strip()
         else:
             raise ValueError(
-                "The value type recorded for this relationship, is not currently supported for CSV parsing. Please check with your DCC."
+                (
+                    "The value type recorded for this relationship, is not currently "
+                    "supported for CSV parsing. Please check with your DCC."
+                )
             )
         return parsed_rel_entry
 
     def gather_csv_attributes_relationships(
         self, model_df: pd.DataFrame
-    ) -> Dict[str, dict[str, Any]]:
+    ) -> dict[str, dict[str, Any]]:
         """Parse csv into a attributes:relationshps dictionary to be used in downstream efforts.
         Args:
             model_df: pd.DataFrame, data model that has been loaded into pandas DataFrame.
         Returns:
             attr_rel_dictionary: dict,
                 {Attribute Display Name: {
                     Relationships: {
@@ -232,46 +248,81 @@
         # Gather info from the model
         model_dict = self.gather_csv_attributes_relationships(model_df)
 
         return model_dict
 
 
 class DataModelJSONLDParser:
+    """DataModelJSONLDParser"""
+
     def __init__(
         self,
     ):
         # Instantiate DataModelRelationships
         self.dmr = DataModelRelationships()
         # Load relationships dictionary.
         self.rel_dict = self.dmr.define_data_model_relationships()
 
+    def parse_jsonld_dicts(
+        self, rel_entry: dict[str, str]
+    ) -> Union[str, dict[str, str]]:
+        """Parse incoming JSONLD dictionaries, only supported dictionaries are non-edge
+            dictionaries.
+        Note:
+            The only two dictionaries we expect are a single entry dictionary containing
+            id information and dictionaries where the key is the attribute label
+            (and it is expected to stay as the label). The individual rules per component are not
+            attached to nodes but rather parsed later in validation rule parsing.
+            So the keys do not need to be converted to display names.
+        Args:
+            rel_entry, Any: Given a single entry and relationship in a JSONLD data model,
+                the recorded value
+        Returns:
+            str, the JSONLD entry ID
+            dict, JSONLD dictionary entry returned.
+        """
+
+        # Retrieve ID from a dictionary recording the ID
+        if set(rel_entry.keys()) == {"@id"}:
+            parsed_rel_entry = rel_entry["@id"]
+        # Parse any remaining dictionaries
+        else:
+            parsed_rel_entry = rel_entry
+        return parsed_rel_entry
+
     def parse_entry(
         self,
-        rel_entry: any,
+        rel_entry: Any,
         id_jsonld_key: str,
-        dn_label_dict: dict[str:str],
-        model_jsonld: dict,
+        model_jsonld: list[dict],
     ) -> Any:
         """Parse an input entry based on certain attributes
+
         Args:
-            rel_entry: Given a single entry and relationship in a JSONLD data model, the recorded value
-            id_jsonld_key, str: the jsonld key for id
-        Returns:
-            parsed_rel_entry: an entry that has been parsed base on its input type and characteristics.
-        """
-        # Retrieve ID from single value dictionary
-        if type(rel_entry) == dict and len(rel_entry.keys()) == 1:
-            parsed_rel_entry = rel_entry["@id"]
-        # Parse list of dictionaries to make a list of entries with context stripped (will update this section when contexts added.)
-        elif type(rel_entry) == list and type(rel_entry[0]) == dict:
+            rel_entry: Given a single entry and relationship in a JSONLD data model,
+                the recorded value
+            id_jsonld_key: str, the jsonld key for id
+            model_jsonld: list[dict], list of dictionaries, each dictionary is an entry
+                in the jsonld data model
+        Returns:
+            Any: n entry that has been parsed base on its input type and
+              characteristics.
+        """
+        # Parse dictionary entries
+        if isinstance(rel_entry, dict):
+            parsed_rel_entry = self.parse_jsonld_dicts(rel_entry)
+
+        # Parse list of dictionaries to make a list of entries with context stripped (will update
+        # this section when contexts added.)
+        elif isinstance(rel_entry, list) and isinstance(rel_entry[0], dict):
             parsed_rel_entry = self.convert_entry_to_dn_label(
                 [r[id_jsonld_key].split(":")[1] for r in rel_entry], model_jsonld
             )
         # Strip context from string and convert true/false to bool
-        elif type(rel_entry) == str:
+        elif isinstance(rel_entry, str):
             # Remove contexts and treat strings as appropriate.
             if ":" in rel_entry and "http:" not in rel_entry:
                 parsed_rel_entry = rel_entry.split(":")[1]
                 # Convert true/false strings to boolean
                 if parsed_rel_entry.lower() == "true":
                     parsed_rel_entry = True
                 elif parsed_rel_entry.lower == "false":
@@ -284,15 +335,17 @@
         # For anything else get that
         else:
             parsed_rel_entry = self.convert_entry_to_dn_label(rel_entry, model_jsonld)
 
         return parsed_rel_entry
 
     def label_to_dn_dict(self, model_jsonld: list[dict]):
-        """Generate a dictionary of labels to display name, so can easily look up display names using the label.
+        """
+        Generate a dictionary of labels to display name, so can easily look up
+          display names using the label.
         Args:
             model_jsonld: list of dictionaries, each dictionary is an entry in the jsonld data model
         Returns:
             dn_label_dict: dict of model labels to display names
         """
         jsonld_keys_to_extract = ["label", "displayName"]
         label_jsonld_key, dn_jsonld_key = [
@@ -304,111 +357,123 @@
         return dn_label_dict
 
     def convert_entry_to_dn_label(
         self, parsed_rel_entry: Union[str, list], model_jsonld: list[dict]
     ) -> Union[str, list]:
         """Convert a parsed entry to display name, taking into account the entry type
         Args:
-            parsed_rel_entry: an entry that has been parsed base on its input type and characteristics.
+            parsed_rel_entry: an entry that has been parsed base on its input type
+              and characteristics.
             model_jsonld: list of dictionaries, each dictionary is an entry in the jsonld data model
         Returns:
-            parsed_rel_entry: an entry that has been parsed based on its input type and characteristics, and converted to display names.
+            parsed_rel_entry: an entry that has been parsed based on its input type and
+              characteristics, and converted to display names.
         """
         # Get a dictionary of display_names mapped to labels
         dn_label_dict = self.label_to_dn_dict(model_jsonld=model_jsonld)
         # Handle if using the display name as the label
-        if type(parsed_rel_entry) == list:
+        if isinstance(parsed_rel_entry, list):
             parsed_rel_entry = [
                 dn_label_dict.get(entry) if dn_label_dict.get(entry) else entry
                 for entry in parsed_rel_entry
             ]
-        elif type(parsed_rel_entry) == str:
+        elif isinstance(parsed_rel_entry, str):
             converted_label = dn_label_dict.get(parsed_rel_entry)
             if converted_label:
                 parsed_rel_entry = dn_label_dict.get(parsed_rel_entry)
         return parsed_rel_entry
 
-    def gather_jsonld_attributes_relationships(self, model_jsonld: List[dict]) -> Dict:
+    def gather_jsonld_attributes_relationships(self, model_jsonld: list[dict]) -> dict:
         """
         Args:
             model_jsonld: list of dictionaries, each dictionary is an entry in the jsonld data model
         Returns:
             attr_rel_dictionary: dict,
                 {Node Display Name:
                     {Relationships: {
                                      CSV Header: Value}}}
         Notes:
             - Unlike a CSV the JSONLD might already have a base schema attached to it.
               So the attributes:relationship dictionary for importing a CSV vs JSONLD may not match.
-            - It is also just about impossible to extract attributes explicitly. Using a dictionary should avoid duplications.
+            - It is also just about impossible to extract attributes explicitly. Using a dictionary
+              should avoid duplications.
             - This is a promiscuous capture and will create an attribute for each model entry.
             - Currently only designed to capture the same information that would be encoded in CSV,
                 can be updated in the future.
         TODO:
-            - Find a way to delete non-attribute keys, is there a way to reliable distinguish after the fact?
+            - Find a way to delete non-attribute keys, is there a way to reliable distinguish
+              after the fact?
             - Right now, here we are stripping contexts, will need to track them in the future.
         """
+        # pylint:disable=too-many-locals
+        # pylint:disable=too-many-branches
+        # pylint:disable=too-many-nested-blocks
 
         # Retrieve relevant JSONLD keys.
         jsonld_keys_to_extract = ["label", "subClassOf", "id", "displayName"]
-        label_jsonld_key, subclassof_jsonld_key, id_jsonld_key, dn_jsonld_key = [
+        label_jsonld_key, _, id_jsonld_key, dn_jsonld_key = [
             self.rel_dict[key]["jsonld_key"] for key in jsonld_keys_to_extract
         ]
 
-        # Get a dictionary of display names to labels to identify values explicitly recorded
-        dn_label_dict = self.label_to_dn_dict(model_jsonld=model_jsonld)
-
         # Build the attr_rel_dictionary
         attr_rel_dictionary = {}
         # Move through each entry in the jsonld model
         for entry in model_jsonld:
             # Get the attr key for the dictionary
             if dn_jsonld_key in entry:
                 # The attr_key is the entry display name if one was recorded
                 attr_key = entry[dn_jsonld_key]
             else:
                 # If not we wil use the get the label.
                 attr_key = entry[label_jsonld_key]
 
             # If the entry has not already been added to the dictionary, add it.
-            if attr_key not in attr_rel_dictionary.keys():
+            if attr_key not in attr_rel_dictionary:
                 attr_rel_dictionary.update(attr_dict_template(attr_key))
 
             # Add relationships for each entry
             # Go through each defined relationship type (rel_key) and its attributes (rel_vals)
             for rel_key, rel_vals in self.rel_dict.items():
-                # Determine if current entry in the for loop, can be described by the current relationship that is being cycled through.
-                # used to also check "csv_header" in rel_vals.keys() which allows all JSONLD values through even if it does not have a CSV counterpart, will allow other values thorough in the else statement now
+                # Determine if current entry in the for loop, can be described by the current
+                # relationship that is being cycled through.
+                # used to also check "csv_header" in rel_vals.keys() which allows all JSONLD
+                # values through even if it does not have a CSV counterpart, will allow other
+                # values thorough in the else statement now
                 if rel_vals["jsonld_key"] in entry.keys() and rel_vals["csv_header"]:
                     # Retrieve entry value associated with the given relationship
                     rel_entry = entry[rel_vals["jsonld_key"]]
-                    # If there is an entry parse it by type and add to the attr:relationships dictionary.
+                    # If there is an entry parse it by type and add to the attr:relationships
+                    # dictionary.
                     if rel_entry:
                         parsed_rel_entry = self.parse_entry(
                             rel_entry=rel_entry,
                             id_jsonld_key=id_jsonld_key,
-                            dn_label_dict=dn_label_dict,
                             model_jsonld=model_jsonld,
                         )
-                        rel_csv_header = self.rel_dict[rel_key]["csv_header"]
+                        rel_csv_header = rel_vals["csv_header"]
                         if rel_key == "domainIncludes":
-                            # In the JSONLD the domain includes field contains the ids of attributes that the current attribute is the property/parent of.
+                            # In the JSONLD the domain includes field contains the ids of
+                            # attributes that the current attribute is the property/parent of.
                             # Because of this we need to handle these values differently.
-                            # We will get the values in the field (parsed_val), then add the current attribute as to the property key in the attr_rel_dictionary[p_attr_key].
+                            # We will get the values in the field (parsed_val), then add the
+                            # current attribute as to the property key in the
+                            # attr_rel_dictionary[p_attr_key].
                             for parsed_val in parsed_rel_entry:
                                 attr_in_dict = False
                                 # Get propert/parent key (displayName)
                                 p_attr_key = ""
-                                # Check if the parsed value is already a part of the attr_rel_dictionary
-                                for attr_dn, rels in attr_rel_dictionary.items():
+                                # Check if the parsed value is already a part of the
+                                # attr_rel_dictionary
+                                for attr_dn in attr_rel_dictionary:
                                     if parsed_val == attr_dn:
                                         p_attr_key = attr_dn
                                         attr_in_dict = True
-                                # If it is part of the dictionary update add current attribute as a property of the parsed value
-                                if attr_in_dict == True:
+                                # If it is part of the dictionary update add current
+                                # attribute as a property of the parsed value
+                                if attr_in_dict:
                                     if (
                                         not rel_csv_header
                                         in attr_rel_dictionary[p_attr_key][
                                             "Relationships"
                                         ]
                                     ):
                                         attr_rel_dictionary[p_attr_key][
@@ -416,16 +481,17 @@
                                         ].update(
                                             {rel_csv_header: [entry[dn_jsonld_key]]}
                                         )
                                     else:
                                         attr_rel_dictionary[p_attr_key][
                                             "Relationships"
                                         ][rel_csv_header].extend([entry[dn_jsonld_key]])
-                                # If the parsed_val is not already recorded in the dictionary, add it
-                                elif attr_in_dict == False:
+                                # If the parsed_val is not already recorded in the dictionary,
+                                # add it
+                                elif not attr_in_dict:
                                     # Get the display name for the parsed value
                                     p_attr_key = self.convert_entry_to_dn_label(
                                         parsed_val, model_jsonld
                                     )
 
                                     attr_rel_dictionary.update(
                                         attr_dict_template(p_attr_key)
@@ -443,20 +509,20 @@
 
                 elif (
                     rel_vals["jsonld_key"] in entry.keys()
                     and not rel_vals["csv_header"]
                 ):
                     # Retrieve entry value associated with the given relationship
                     rel_entry = entry[rel_vals["jsonld_key"]]
-                    # If there is an entry parset it by type and add to the attr:relationships dictionary.
+                    # If there is an entry parset it by type and add to the
+                    # attr:relationships dictionary.
                     if rel_entry:
                         parsed_rel_entry = self.parse_entry(
                             rel_entry=rel_entry,
                             id_jsonld_key=id_jsonld_key,
-                            dn_label_dict=dn_label_dict,
                             model_jsonld=model_jsonld,
                         )
                         # Add relationships for each attribute and relationship to the dictionary
                         attr_rel_dictionary[attr_key]["Relationships"].update(
                             {rel_key: parsed_rel_entry}
                         )
         return attr_rel_dictionary
@@ -472,14 +538,17 @@
             model_dict: dict,
                 {Node Display Name:
                     {Relationships: {
                                      CSV Header: Value}}}
         """
         # Log warning that JSONLD parsing is in beta mode.
         logger.warning(
-            "JSONLD parsing is in Beta Mode. Please inspect outputs carefully and report any errors."
+            (
+                "JSONLD parsing is in Beta Mode. "
+                "Please inspect outputs carefully and report any errors."
+            )
         )
         # Load the json_ld model to df
         json_load = load_json(path_to_data_model)
         # Convert dataframe to attributes relationship dictionary.
         model_dict = self.gather_jsonld_attributes_relationships(json_load["@graph"])
         return model_dict
```

### Comparing `schematicpy-24.2.1/schematic/schemas/data_model_relationships.py` & `schematicpy-24.4.1/schematic/schemas/data_model_relationships.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,26 @@
-from typing import Dict
+"""Data Model Relationships"""
+
 from schematic.utils.schema_utils import (
     get_label_from_display_name,
     get_attribute_display_name_from_label,
     convert_bool_to_str,
     parse_validation_rules,
 )
-from schematic.schemas.curie import uri2curie, curie2uri
 
 
 class DataModelRelationships:
+    """Data Model Relationships"""
+
     def __init__(self) -> None:
         self.relationships_dictionary = self.define_data_model_relationships()
 
-    def define_data_model_relationships(self) -> Dict:
-        """Define the relationships and their attributes so they can be accessed through other classes.
+    def define_data_model_relationships(self) -> dict:
+        """Define the relationships and their attributes so they can be accessed
+          through other classes.
         The key is how it the relationship will be referenced througout Schematic.
         Note: Though we could use other keys to determine which keys define nodes and edges,
             edge_rel is used as an explicit definition, for easier code readablity.
         key:
             jsonld_key: Name for relationship in the JSONLD.
                         Include in all sub-dictionaries.
             csv_header: Str, name for this relationshp in the CSV data model.
@@ -25,25 +28,28 @@
             node_label: Name for relationship in the graph representation of the data model.
                         Do not include this key for edge relationships.
             type: type, type of expected to be read into graph creation.
             edge_rel: True, if this relationship defines an edge
                       False, if is a value relationship
                       Include in all sub-dictionaries.
             required_header: True, if relationship header is required for the csv
-            jsonld_default: Defines default values to fill for JSONLD generation.
-                        Used during func DataModelJsonLD.clean_template(), to fill value with a default, if not supplied in the data model.
-            node_attr_dict: This is used to add information to nodes in the model. Only include for nodes not edges.
-                            set default values for this relationship
-                                key is the node relationship name, value is the default value.
-                                If want to set default as a function create a nested dictionary.
-                                    {'default': default_function,
-                                     'standard': alternative function to call if relationship is present for a node}
-                                    }
-                                If adding new functions to node_dict will
-                                    need to modify data_model_nodes.generate_node_dict in
+            jsonld_default:
+                Defines default values to fill for JSONLD generation.
+                Used during func DataModelJsonLD.clean_template(), to fill value with a default,
+                  if not supplied in the data model.
+            node_attr_dict: This is used to add information to nodes in the model.
+                Only include for nodes not edges.
+                set default values for this relationship
+                key is the node relationship name, value is the default value.
+                If want to set default as a function create a nested dictionary.
+                    {'default': default_function,
+                     'standard': alternative function to call if relationship is present for a node
+                    }
+                If adding new functions to node_dict will
+                    need to modify data_model_nodes.generate_node_dict in
             edge_dir: str, 'in'/'out' is the edge an in or out edge. Define for edge relationships
             jsonld_dir: str, 'in'/out is the direction in or out in the JSONLD.
 
         TODO:
             - Use class inheritance to set up
         """
         map_data_model_relationships = {
@@ -183,41 +189,49 @@
                 },
             },
         }
 
         return map_data_model_relationships
 
     def define_required_csv_headers(self):
-        """Helper function to retrieve required CSV headers, alert if required header was not provided.
+        """
+        Helper function to retrieve required CSV headers, alert if required header was
+          not provided.
         Returns:
             required_headers: lst, Required CSV headers.
         """
         required_headers = []
-        for k, v in self.relationships_dictionary.items():
+        for key, value in self.relationships_dictionary.items():
             try:
-                if v["required_header"]:
-                    required_headers.append(v["csv_header"])
+                if value["required_header"]:
+                    required_headers.append(value["csv_header"])
             except KeyError:
                 print(
-                    f"Did not provide a 'required_header' key, value pair for the nested dictionary {k} : {key}"
+                    (
+                        "Did not provide a 'required_header' key, value pair for the "
+                        f"nested dictionary {key} : {value}"
+                    )
                 )
 
         return required_headers
 
-    def retreive_rel_headers_dict(self, edge: bool) -> Dict[str, str]:
-        """Helper function to retrieve CSV headers for edge and non-edge relationships defined by edge_type.
+    def retreive_rel_headers_dict(self, edge: bool) -> dict[str, str]:
+        """
+        Helper function to retrieve CSV headers for edge and non-edge relationships
+          defined by edge_type.
+
         Args:
             edge, bool: True if looking for edge relationships
         Returns:
             rel_headers_dict: dict, key: csv_header if the key represents an edge relationship.
         """
         rel_headers_dict = {}
         for rel, rel_dict in self.relationships_dictionary.items():
             if "edge_rel" in rel_dict:
                 if rel_dict["edge_rel"] and edge:
                     rel_headers_dict.update({rel: rel_dict["csv_header"]})
-                elif rel_dict["edge_rel"] == False and edge == False:
+                elif not rel_dict["edge_rel"] and not edge:
                     rel_headers_dict.update({rel: rel_dict["csv_header"]})
             else:
                 raise ValueError(f"Did not provide a 'edge_rel' for relationship {rel}")
 
         return rel_headers_dict
```

### Comparing `schematicpy-24.2.1/schematic/schemas/data_model_validator.py` & `schematicpy-24.4.1/schematic/schemas/data_model_validator.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+"""Data Model Validator"""
+
+import time
 import logging
+
 import multiprocessing
-import networkx as nx
-import time
-from typing import Any, Dict, Optional, Text, List, Tuple
+import networkx as nx  # type: ignore
 
 from schematic.schemas.data_model_relationships import DataModelRelationships
 
 logger = logging.getLogger(__name__)
 
 
 class DataModelValidator:
@@ -16,143 +18,177 @@
 
     def __init__(
         self,
         graph: nx.MultiDiGraph,
     ):
         """
         Args:
-                graph, nx.MultiDiGraph: Graph representation of the data model.
-        TODO: put blacklisted chars and reserved_names in some global space where they can be accessed centrally
+            graph (nx.MultiDiGraph): Graph representation of the data model.
+        TODO: put blacklisted chars and reserved_names in some global space where
+          they can be accessed centrally
         """
         self.graph = graph
-        self.DMR = DataModelRelationships()
+        self.dmr = DataModelRelationships()
         # Define blacklisted characters, taken from store.synapse
         self.blacklisted_chars = ["(", ")", ".", "-"]
         # Define reserved_names, taken from Documentation
         self.reserved_names = {"entityId"}
 
-    def run_checks(self) -> Tuple[list, list]:
+    def run_checks(self) -> tuple[list, list]:
         """Run all validation checks on the data model graph.
-        Returns, tuple(list, list): Returns a tuple of errors and warnings generated.
-        TODO: In future could design a way for groups to customize tests run for their groups, run additional tests, or move some to issuing only warnings, vice versa.
+
+        Returns:
+            tuple[list, list]:  Returns a tuple of errors and warnings generated.
+
+        TODO: In future could design a way for groups to customize tests run for their groups,
+           run additional tests, or move some to issuing only warnings, vice versa.
         """
         error_checks = [
             self.check_graph_has_required_node_fields(),
             self.check_is_dag(),
             self.check_reserved_names(),
         ]
         warning_checks = [
             self.check_blacklisted_characters(),
         ]
         errors = [error for error in error_checks if error]
         warnings = [warning for warning in warning_checks if warning]
         return errors, warnings
 
-    def check_graph_has_required_node_fields(self) -> List[str]:
+    def check_graph_has_required_node_fields(self) -> list[str]:
         """Checks that the graph has the required node fields for all nodes.
         Returns:
                 error, list: List of error messages for each missing field.
         """
         # Get all the fields that should be recorded per node
-        rel_dict = self.DMR.relationships_dictionary
+        rel_dict = self.dmr.relationships_dictionary
         node_fields = []
-        for k, v in rel_dict.items():
-            if "node_label" in v.keys():
-                node_fields.append(v["node_label"])
+        for value in rel_dict.values():
+            if "node_label" in value.keys():
+                node_fields.append(value["node_label"])
 
         error = []
         missing_fields = []
         # Check that required fields are present for each node.
         for node, node_dict in self.graph.nodes(data=True):
             missing_fields.extend(
                 [(node, f) for f in node_fields if f not in node_dict.keys()]
             )
 
         if missing_fields:
-            for mf in missing_fields:
+            for missing_field in missing_fields:
                 error.append(
-                    f"For entry: {mf[0]}, the required field {mf[1]} is missing in the data model graph, please double check your model and generate the graph again."
+                    (
+                        f"For entry: {missing_field[0]}, the required field {missing_field[1]} "
+                        "is missing in the data model graph, please double check your model and "
+                        "generate the graph again."
+                    )
                 )
         return error
 
-    def run_cycles(self, graph):
+    def run_cycles(self):
+        """run_cycles"""
         cycles = nx.simple_cycles(self.graph)
-        if cycles:
+        if cycles:  # pylint:disable=using-constant-test
             for cycle in cycles:
-                logger.warning(
-                    f"Schematic requires models be a directed acyclic graph (DAG). Your graph is not a DAG, we found a loop between: {cycle[0]} and {cycle[1]}, please remove this loop from your model and submit again."
+                logger.warning(  # pylint:disable=logging-fstring-interpolation
+                    (
+                        f"Schematic requires models be a directed acyclic graph (DAG). Your graph "
+                        f"is not a DAG, we found a loop between: {cycle[0]} and {cycle[1]}, "
+                        "please remove this loop from your model and submit again."
+                    )
                 )
 
-    def check_is_dag(self) -> List[str]:
+    def check_is_dag(self) -> list[str]:
         """Check that generated graph is a directed acyclic graph
+
         Returns:
-                error, list: List of error messages if graph is not a DAG. List will include a message for each cycle found, if not there is a more generic message for the graph as a whole.
+            list[str]:
+              List of error messages if graph is not a DAG. List will include a message
+                for each cycle found, if not there is a more generic message for the
+                graph as a whole.
         """
         error = []
         if not nx.is_directed_acyclic_graph(self.graph):
             cycles = multiprocessing.Process(
-                target=self.run_cycles, name="Get Cycles", args=(self.graph,)
+                target=self.run_cycles,
+                name="Get Cycles",
             )
             cycles.start()
 
             # Give up to 5 seconds to find cycles, if not exit and issue standard error
             time.sleep(5)
 
             # If thread is active
             if cycles.is_alive():
                 # Terminate foo
                 cycles.terminate()
                 # Cleanup
                 cycles.join()
 
             error.append(
-                f"Schematic requires models be a directed acyclic graph (DAG). Please inspect your model."
+                (
+                    "Schematic requires models be a directed acyclic graph (DAG). "
+                    "Please inspect your model."
+                )
             )
 
         return error
 
-    def check_blacklisted_characters(self) -> List[str]:
-        """We strip these characters in store, so not sure if it matter if we have them now, maybe add warning
+    def check_blacklisted_characters(self) -> list[str]:
+        """
+        We strip these characters in store, so not sure if it matter if we have them now,
+         maybe add warning
+
         Returns:
-                warning, list: list of warnings for each node in the graph, that has a Display name that contains blacklisted characters.
+            list[str]: list of warnings for each node in the graph, that has a Display
+              name that contains blacklisted characters.
         """
         warning = []
-        for node, node_dict in self.graph.nodes(data=True):
+        for _, node_dict in self.graph.nodes(data=True):
             if any(
                 bl_char in node_dict["displayName"]
                 for bl_char in self.blacklisted_chars
             ):
                 node_display_name = node_dict["displayName"]
                 blacklisted_characters_found = [
                     bl_char
                     for bl_char in self.blacklisted_chars
                     if bl_char in node_dict["displayName"]
                 ]
                 blacklisted_characters_str = ",".join(blacklisted_characters_found)
                 warning.append(
-                    f"Node: {node_display_name} contains a blacklisted character(s): {blacklisted_characters_str}, they will be striped if used in Synapse annotations."
+                    (
+                        f"Node: {node_display_name} contains a blacklisted character(s): "
+                        f"{blacklisted_characters_str}, they will be striped if used in "
+                        "Synapse annotations."
+                    )
                 )
         return warning
 
-    def check_reserved_names(self) -> List[str]:
+    def check_reserved_names(self) -> list[str]:
         """Identify if any names nodes in the data model graph are the same as reserved name.
         Returns:
-                error, list: List of erros for every node in the graph whose name overlaps with the reserved names.
+            error, list: List of erros for every node in the graph whose name overlaps
+              with the reserved names.
         """
         error = []
         reserved_names_found = [
             (name, node)
             for node in self.graph.nodes
             for name in self.reserved_names
             if name.lower() == node.lower()
         ]
         if reserved_names_found:
             for reserved_name, node_name in reserved_names_found:
                 error.append(
-                    f"Your data model entry name: {node_name} overlaps with the reserved name: {reserved_name}. Please change this name in your data model."
+                    (
+                        f"Your data model entry name: {node_name} overlaps with the reserved name: "
+                        f"{reserved_name}. Please change this name in your data model."
+                    )
                 )
         return error
 
     def check_namespace_overlap(self):
         """
         Check if name is repeated.
         Implement in the future
@@ -166,12 +202,13 @@
         Implement in future
         """
         warning = []
         return warning
 
     def check_namespace_similarity(self):
         """
-        Using AI, check if submitted attributes or valid values are similar to other ones, warn users.
+        Using AI, check if submitted attributes or valid values are similar to other ones,
+          warn users.
         Implement in future
         """
         warning = []
         return warning
```

### Comparing `schematicpy-24.2.1/schematic/schemas/json_schema_validator.py` & `schematicpy-24.4.1/schematic/schemas/json_schema_validator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,18 @@
+"""Json Schema Validator"""
+
 import os
 from jsonschema import validate
 
-from schematic.utils.io_utils import load_schemaorg, load_json, load_default
+from schematic.utils.io_utils import load_schemaorg, load_json
 from schematic.utils.general import str2list, dict2list, find_duplicates
 from schematic.utils.curie_utils import (
     expand_curies_in_schema,
     extract_name_from_uri_or_curie,
 )
-from schematic.utils.validate_utils import (
-    validate_class_schema,
-    validate_property_schema,
-    validate_schema,
-)
 
 
 class SchemaValidator:
     """Validate Schema against SchemaOrg standard
 
     Validation Criterias:
     1. Data Structure wise:
@@ -30,23 +27,26 @@
       > all prefixes used in the file should be defined in "@context"
       > There should be no duplicate "@id"
       > Class specific
         > rdfs:label field should be capitalize the first character of each
           word for a class;
         > the value of "rdfs:subClassOf" should be present in the schema or in
           the core vocabulary
-        > sms:displayName ideally should contain capitalized words separated by space, but that's not enforced by validation
+        > sms:displayName ideally should contain capitalized words separated by space,
+          but that's not enforced by validation
       > Property specific
         > rdfs:label field should be cammelCase
         > the value of "schema:domainIncludes" should be present in the schema
           or in the core vocabulary
         > the value of "schema:rangeIncludes" should be present in the schema
           or in the core vocabulary
-        > sms:displayName ideally should contain capitalized words separated by space, but that's not enforced by validation
-        TODO: add dependencies and component dependencies to class structure documentation; as well as value range and required property
+        > sms:displayName ideally should contain capitalized words separated
+          by space, but that's not enforced by validation
+        TODO: add dependencies and component dependencies to class
+          structure documentation; as well as value range and required property
 
     """
 
     def __init__(self, schema):
         self.schemaorg = {"schema": load_schemaorg(), "classes": [], "properties": []}
         for _schema in self.schemaorg["schema"]["@graph"]:
             for _record in _schema["@graph"]:
@@ -81,49 +81,46 @@
 
     def validate_subclassof_field(self, subclassof_value):
         """Check if the value of "subclassof" is included in the schema file"""
         subclassof_value = dict2list(subclassof_value)
         for record in subclassof_value:
             assert record["@id"] in self.all_classes
 
-    def validate_domainIncludes_field(self, domainincludes_value):
+    def validate_domain_includes_field(self, domainincludes_value):
         """Check if the value of "domainincludes" is included in the schema
         file
         """
         domainincludes_value = dict2list(domainincludes_value)
         for record in domainincludes_value:
-            assert record["@id"] in self.all_classes, (
-                "value of domainincludes not recorded in schema: %r"
-                % domainincludes_value
-            )
+            assert (
+                record["@id"] in self.all_classes
+            ), f"value of domainincludes not recorded in schema: {domainincludes_value}"
 
-    def validate_rangeIncludes_field(self, rangeincludes_value):
+    def validate_range_includes_field(self, rangeincludes_value):
         """Check if the value of "rangeincludes" is included in the schema
         file
         """
         rangeincludes_value = dict2list(rangeincludes_value)
         for record in rangeincludes_value:
             assert record["@id"] in self.all_classes
 
     def check_whether_atid_and_label_match(self, record):
         """Check if @id field matches with the "rdfs:label" field"""
         _id = extract_name_from_uri_or_curie(record["@id"])
-        assert _id == record["rdfs:label"], "id and label not match: %r" % record
+        assert _id == record["rdfs:label"], f"id and label not match: {record}"
 
     def check_duplicate_labels(self):
         """Check for duplication in the schema"""
         labels = [
             _record["rdfs:label"]
             for _record in self.extension_schema["schema"]["@graph"]
         ]
         duplicates = find_duplicates(labels)
-        try:
-            assert len(duplicates) == 0
-        except:
-            raise Exception("Duplicates detected in graph: ", duplicates)
+        if len(duplicates) == 0:
+            raise ValueError("Duplicates detected in graph: ", duplicates)
 
     def validate_schema(self, schema):
         """Validate schema against SchemaORG standard"""
         json_schema_path = os.path.join("validation_schemas", "schema.json")
         json_schema = load_json(json_schema_path)
         return validate(schema, json_schema)
 
@@ -138,23 +135,24 @@
     def validate_class_schema(self, schema):
         """Validate schema against SchemaORG class definition standard"""
         json_schema_path = os.path.join("validation_schemas", "class_json_schema.json")
         json_schema = load_json(json_schema_path)
         return validate(schema, json_schema)
 
     def validate_full_schema(self):
+        """validate full schema"""
         self.check_duplicate_labels()
         for record in self.extension_schema["schema"]["@graph"]:
             self.check_whether_atid_and_label_match(record)
             if record["@type"] == "rdf:Class":
                 self.validate_class_schema(record)
                 self.validate_class_label(record["@id"])
             elif record["@type"] == "rdf:Property":
                 self.validate_property_schema(record)
                 self.validate_property_label(record["@id"])
-                self.validate_domainIncludes_field(
+                self.validate_domain_includes_field(
                     record["http://schema.org/domainIncludes"]
                 )
                 if "http://schema.org/rangeIncludes" in record:
-                    self.validate_rangeIncludes_field(
+                    self.validate_range_includes_field(
                         record["http://schema.org/rangeIncludes"]
                     )
```

### Comparing `schematicpy-24.2.1/schematic/store/synapse.py` & `schematicpy-24.4.1/schematic/store/synapse.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
+"""Synapse storage class"""
+
 import atexit
-from collections import OrderedDict
 from copy import deepcopy
-from datetime import datetime, timedelta
 from dataclasses import dataclass
-import json
 import logging
 import numpy as np
 import pandas as pd
 import os
 import re
 import secrets
 import shutil
@@ -22,63 +21,56 @@
     retry_if_exception_type,
 )
 from time import sleep
 
 # allows specifying explicit variable types
 from typing import Dict, List, Tuple, Sequence, Union, Optional
 
-
 from synapseclient import (
     Synapse,
     File,
     Folder,
     Table,
     Schema,
     EntityViewSchema,
     EntityViewType,
     Column,
     as_table_columns,
 )
 from synapseclient.entity import File
 from synapseclient.table import CsvFileTable, build_table, Schema
-from synapseclient.annotations import from_synapse_annotations
 from synapseclient.core.exceptions import (
     SynapseHTTPError,
     SynapseAuthenticationError,
     SynapseUnmetAccessRestrictions,
+    SynapseHTTPError,
 )
 import synapseutils
-from synapseutils.copy_functions import changeFileMetaData
-
-import uuid
 
 from schematic_db.rdb.synapse_database import SynapseDatabase
 
 from schematic.schemas.data_model_graph import DataModelGraphExplorer
 
 from schematic.utils.df_utils import update_df, load_df, col_in_dataframe
 from schematic.utils.validate_utils import comma_separated_list_regex, rule_in_rule_list
 
 # entity_type_mapping, get_dir_size, create_temp_folder, check_synapse_cache_size, and clear_synapse_cache functions are used for AWS deployment
 # Please do not remove these import statements
 from schematic.utils.general import (
     entity_type_mapping,
     get_dir_size,
-    convert_gb_to_bytes,
     create_temp_folder,
     check_synapse_cache_size,
     clear_synapse_cache,
-    profile,
-    calculate_datetime,
 )
 
 from schematic.utils.schema_utils import get_class_label_from_display_name
 
 from schematic.store.base import BaseStorage
-from schematic.exceptions import MissingConfigValueError, AccessCredentialsError
+from schematic.exceptions import AccessCredentialsError
 from schematic.configuration.configuration import CONFIG
 
 logger = logging.getLogger("Synapse storage")
 
 
 @dataclass
 class ManifestDownload(object):
@@ -198,54 +190,60 @@
     """
 
     def __init__(
         self,
         token: Optional[str] = None,  # optional parameter retrieved from browser cookie
         access_token: Optional[str] = None,
         project_scope: Optional[list] = None,
+        synapse_cache_path: Optional[str] = None,
     ) -> None:
         """Initializes a SynapseStorage object.
+
         Args:
-            syn: an object of type synapseclient.
-            token: optional token parameter (typically a 'str') as found in browser cookie upon login to synapse.
-            access_token: optional access token (personal or oauth)
-            TODO: move away from specific project setup and work with an interface that Synapse specifies (e.g. based on schemas).
-        Exceptions:
-            KeyError: when the 'storage' config object is missing values for essential keys.
-            AttributeError: when the 'storageFileview' attribute (of class SynapseStorage) does not have a value associated with it.
-            synapseclient.core.exceptions.SynapseHTTPError: check if the current user has permission to access the Synapse entity.
-            ValueError: when Admin fileview cannot be found (describe further).
-        Typical usage example:
-            syn_store = SynapseStorage()
+            token (Optional[str], optional):
+              Optional token parameter as found in browser cookie upon login to synapse.
+              Defaults to None.
+            access_token (Optional[list], optional):
+              Optional access token (personal or oauth).
+              Defaults to None.
+            project_scope (Optional[list], optional): Defaults to None.
+            synapse_cache_path (Optional[str], optional):
+              Location of synapse cache.
+              Defaults to None.
         """
-        # TODO: turn root_synapse_cache to a parameter in init
-        self.syn = self.login(token, access_token)
+        self.syn = self.login(synapse_cache_path, token, access_token)
         self.project_scope = project_scope
         self.storageFileview = CONFIG.synapse_master_fileview_id
         self.manifest = CONFIG.synapse_manifest_basename
-        self.root_synapse_cache = "/root/.synapseCache"
+        self.root_synapse_cache = self.syn.cache.cache_root_dir
         self._query_fileview()
 
-    def _purge_synapse_cache(self, maximum_storage_allowed_cache_gb=1):
+    def _purge_synapse_cache(
+        self, maximum_storage_allowed_cache_gb: int = 1, minute_buffer: int = 15
+    ) -> None:
         """
         Purge synapse cache if it exceeds a certain size. Default to 1GB.
         Args:
-            maximum_storage_allowed_cache_gb: the maximum storage allowed before purging cache. Default is 1 GB.
+            maximum_storage_allowed_cache_gb (int): the maximum storage allowed
+              before purging cache. Default is 1 GB.
+            minute_buffer (int): All files created this amount of time or older will be deleted
         """
         # try clearing the cache
         # scan a directory and check size of files
         if os.path.exists(self.root_synapse_cache):
-            maximum_storage_allowed_cache_bytes = convert_gb_to_bytes(
-                maximum_storage_allowed_cache_gb
+            maximum_storage_allowed_cache_bytes = maximum_storage_allowed_cache_gb * (
+                1024**3
             )
             nbytes = get_dir_size(self.root_synapse_cache)
             dir_size_bytes = check_synapse_cache_size(directory=self.root_synapse_cache)
             # if 1 GB has already been taken, purge cache before 15 min
             if dir_size_bytes >= maximum_storage_allowed_cache_bytes:
-                num_of_deleted_files = clear_synapse_cache(self.syn.cache, minutes=15)
+                num_of_deleted_files = clear_synapse_cache(
+                    self.syn.cache, minutes=minute_buffer
+                )
                 logger.info(
                     f"{num_of_deleted_files}  files have been deleted from {self.root_synapse_cache}"
                 )
             else:
                 # on AWS, OS takes around 14-17% of our ephemeral storage (20GiB)
                 # instead of guessing how much space that we left, print out .synapseCache here
                 logger.info(f"the total size of .synapseCache is: {nbytes} bytes")
@@ -264,38 +262,60 @@
                 self.storageFileviewTable = self.syn.tableQuery(
                     "SELECT * FROM " + self.storageFileview
                 ).asDataFrame()
         except SynapseHTTPError:
             raise AccessCredentialsError(self.storageFileview)
 
     @staticmethod
-    def login(token=None, access_token=None):
+    def login(
+        synapse_cache_path: Optional[str] = None,
+        token: Optional[str] = None,
+        access_token: Optional[str] = None,
+    ) -> synapseclient.Synapse:
+        """Login to Synapse
+
+        Args:
+            token (Optional[str], optional): A Synapse token. Defaults to None.
+            access_token (Optional[str], optional): A synapse access token. Defaults to None.
+            synapse_cache_path (Optional[str]): location of synapse cache
+
+        Raises:
+            ValueError: If unable to login with token
+            ValueError: If unable to loging with access token
+
+        Returns:
+            synapseclient.Synapse: A Synapse object that is logged in
+        """
         # If no token is provided, try retrieving access token from environment
         if not token and not access_token:
             access_token = os.getenv("SYNAPSE_ACCESS_TOKEN")
 
         # login using a token
         if token:
-            syn = synapseclient.Synapse()
-
+            syn = synapseclient.Synapse(cache_root_dir=synapse_cache_path)
             try:
                 syn.login(sessionToken=token, silent=True)
-            except synapseclient.core.exceptions.SynapseHTTPError:
-                raise ValueError("Please make sure you are logged into synapse.org.")
+            except SynapseHTTPError as exc:
+                raise ValueError(
+                    "Please make sure you are logged into synapse.org."
+                ) from exc
         elif access_token:
             try:
-                syn = synapseclient.Synapse()
+                syn = synapseclient.Synapse(cache_root_dir=synapse_cache_path)
                 syn.default_headers["Authorization"] = f"Bearer {access_token}"
-            except synapseclient.core.exceptions.SynapseHTTPError:
+            except SynapseHTTPError as exc:
                 raise ValueError(
                     "No access to resources. Please make sure that your token is correct"
-                )
+                ) from exc
         else:
             # login using synapse credentials provided by user in .synapseConfig (default) file
-            syn = synapseclient.Synapse(configPath=CONFIG.synapse_configuration_path)
+            syn = synapseclient.Synapse(
+                configPath=CONFIG.synapse_configuration_path,
+                cache_root_dir=synapse_cache_path,
+            )
             syn.login(silent=True)
         return syn
 
     def missing_entity_handler(method):
         def wrapper(*args, **kwargs):
             try:
                 return method(*args, **kwargs)
@@ -570,15 +590,17 @@
             manifestId: synapse ID of a manifest
         """
         # get manifest file path
         manifest_filepath = self.syn.get(manifestId).path
 
         # load manifest dataframe
         manifest = load_df(
-            manifest_filepath, preserve_raw_input=False, data_model=False
+            manifest_filepath,
+            preserve_raw_input=False,
+            data_model=False,
         )
 
         # convert the dataFrame to use best possible dtypes.
         manifest_new = manifest.convert_dtypes()
 
         # get data types of columns
         result = manifest_new.dtypes.to_frame("dtypes").reset_index()
@@ -1299,19 +1321,19 @@
 
         manifestSynapseFile = File(
             metadataManifestPath,
             description="Manifest for dataset " + datasetId,
             parent=datasetId,
             name=file_name_new,
         )
-
         manifest_synapse_file_id = self.syn.store(
             manifestSynapseFile, isRestricted=restrict_manifest
         ).id
-        changeFileMetaData(
+
+        synapseutils.copy_functions.changeFileMetaData(
             syn=self.syn, entity=manifest_synapse_file_id, downloadAs=file_name_new
         )
 
         return manifest_synapse_file_id
 
     @missing_entity_handler
     def format_row_annotations(
@@ -1504,15 +1526,18 @@
         """
         # read new manifest csv
         try:
             load_args = {
                 "dtype": "string",
             }
             manifest = load_df(
-                metadataManifestPath, preserve_raw_input=False, **load_args
+                metadataManifestPath,
+                preserve_raw_input=False,
+                allow_na_values=False,
+                **load_args,
             )
         except FileNotFoundError as err:
             raise FileNotFoundError(
                 f"No manifest file was found at this path: {metadataManifestPath}"
             ) from err
         return manifest
 
@@ -1646,19 +1671,19 @@
             datasetId (str): synapse ID of folder containing the dataset
             hideBlanks (bool): Default is false -Boolean flag that does not upload annotation keys with blank values when true. Uploads Annotation keys with empty string values when false.
             manifest_synapse_table_id (str): Default is an empty string ''.
             annotation_keys: (str) display_label/class_label(default), Determines labeling syle for annotation keys. class_label will format the display
                 name as upper camelcase, and strip blacklisted characters, display_label will strip blacklisted characters including spaces, to retain
                 display label formatting while ensuring the label is formatted properly for Synapse annotations.
         Returns:
-            manifest (pd.DataFrame): modified to add entitiyId as appropriate.
+            manifest (pd.DataFrame): modified to add entitiyId as appropriate
 
         """
 
-        # Expected behavior is to annotate files if `Filename` is present regardless of `-mrt` setting
+        # Expected behavior is to annotate files if `Filename` is present and if file_annotations_upload is set to True regardless of `-mrt` setting
         if "filename" in [col.lower() for col in manifest.columns]:
             # get current list of files and store as dataframe
             dataset_files = self.getFilesInStorageDataset(datasetId)
             files_and_entityIds = self._get_file_entityIds(
                 dataset_files=dataset_files, only_new_files=False
             )
             file_df = pd.DataFrame(files_and_entityIds)
@@ -1702,14 +1727,15 @@
         component_name: str,
         restrict: bool,
         manifest_record_type: str,
         hideBlanks: bool,
         table_manipulation: str,
         table_column_names: str,
         annotation_keys: str,
+        file_annotations_upload: bool = True,
     ):
         """Upload manifest to Synapse as a table and csv.
         Args:
             dmge: DataModelGraphExplorer object
             manifest (pd.DataFrame): loaded df containing user supplied data.
             metadataManifestPath: path to csv containing a validated metadata manifest.
             datasetId (str): synapse ID of folder containing the dataset
@@ -1721,37 +1747,39 @@
             table_malnipulation (str): Specify the way the manifest tables should be store as on Synapse when one with the same name already exists. Options are 'replace' and 'upsert'.
             table_column_names: (str): display_name/display_label/class_label (default). Sets labeling style for table column names. display_name will use the raw display name as the column name. class_label will format the display
                 name as upper camelcase, and strip blacklisted characters, display_label will strip blacklisted characters including spaces, to retain
                 display label formatting.
             annotation_keys: (str) display_label/class_label (default), Sets labeling syle for annotation keys. class_label will format the display
                 name as upper camelcase, and strip blacklisted characters, display_label will strip blacklisted characters including spaces, to retain
                 display label formatting while ensuring the label is formatted properly for Synapse annotations.
+            file_annotations_upload (bool): Default to True. If false, do not add annotations to files.
         Return:
             manifest_synapse_file_id: SynID of manifest csv uploaded to synapse.
         """
         # Upload manifest as a table, get the ID and updated manifest.
         manifest_synapse_table_id, manifest, table_manifest = self.uploadDB(
             dmge=dmge,
             manifest=manifest,
             datasetId=datasetId,
             table_name=table_name,
             restrict=restrict,
             table_manipulation=table_manipulation,
             table_column_names=table_column_names,
         )
 
-        manifest = self.add_annotations_to_entities_files(
-            dmge,
-            manifest,
-            manifest_record_type,
-            datasetId,
-            hideBlanks,
-            manifest_synapse_table_id,
-            annotation_keys,
-        )
+        if file_annotations_upload:
+            manifest = self.add_annotations_to_entities_files(
+                dmge,
+                manifest,
+                manifest_record_type,
+                datasetId,
+                hideBlanks,
+                manifest_synapse_table_id,
+                annotation_keys,
+            )
         # Load manifest to synapse as a CSV File
         manifest_synapse_file_id = self.upload_manifest_file(
             manifest,
             metadataManifestPath,
             datasetId,
             restrict,
             component_name=component_name,
@@ -1789,38 +1817,41 @@
         metadataManifestPath,
         datasetId,
         restrict,
         manifest_record_type,
         hideBlanks,
         component_name,
         annotation_keys: str,
+        file_annotations_upload: bool = True,
     ):
         """Upload manifest to Synapse as a csv only.
         Args:
             dmge: DataModelGraphExplorer object
             manifest (pd.DataFrame): loaded df containing user supplied data.
             metadataManifestPath: path to csv containing a validated metadata manifest.
             datasetId (str): synapse ID of folder containing the dataset
             restrict (bool): Flag for censored data.
             manifest_record_type: valid values are 'entity', 'table' or 'both'. Specifies whether to create entity ids and folders for each row in a manifest, a Synapse table to house the entire manifest or do both.
             hideBlanks (bool): Default is False -Boolean flag that does not upload annotation keys with blank values when true. Uploads Annotation keys with empty string values when false.
             annotation_keys: (str) display_label/class_label (default), Sets labeling syle for annotation keys. class_label will format the display
                 name as upper camelcase, and strip blacklisted characters, display_label will strip blacklisted characters including spaces, to retain
                 display label formatting while ensuring the label is formatted properly for Synapse annotations.
+            file_annotations_upload (bool): Default to True. If false, do not add annotations to files.
         Return:
             manifest_synapse_file_id (str): SynID of manifest csv uploaded to synapse.
         """
-        manifest = self.add_annotations_to_entities_files(
-            dmge,
-            manifest,
-            manifest_record_type,
-            datasetId,
-            hideBlanks,
-            annotation_keys=annotation_keys,
-        )
+        if file_annotations_upload:
+            manifest = self.add_annotations_to_entities_files(
+                dmge,
+                manifest,
+                manifest_record_type,
+                datasetId,
+                hideBlanks,
+                annotation_keys=annotation_keys,
+            )
 
         # Load manifest to synapse as a CSV File
         manifest_synapse_file_id = self.upload_manifest_file(
             manifest,
             metadataManifestPath,
             datasetId,
             restrict,
@@ -1847,14 +1878,15 @@
         component_name,
         restrict,
         manifest_record_type,
         hideBlanks,
         table_manipulation,
         table_column_names: str,
         annotation_keys: str,
+        file_annotations_upload: bool = True,
     ):
         """Upload manifest to Synapse as a table and CSV with entities.
         Args:
             dmge: DataModelGraphExplorer object
             manifest (pd.DataFrame): loaded df containing user supplied data.
             metadataManifestPath: path to csv containing a validated metadata manifest.
             datasetId (str): synapse ID of folder containing the dataset
@@ -1866,36 +1898,38 @@
             table_malnipulation (str): Specify the way the manifest tables should be store as on Synapse when one with the same name already exists. Options are 'replace' and 'upsert'.
             table_column_names: (str): display_name/display_label/class_label (default). Sets labeling style for table column names. display_name will use the raw display name as the column name. class_label will format the display
                 name as upper camelcase, and strip blacklisted characters, display_label will strip blacklisted characters including spaces, to retain
                 display label formatting.
             annotation_keys: (str) display_label/class_label (default), Sets labeling syle for annotation keys. class_label will format the display
                 name as upper camelcase, and strip blacklisted characters, display_label will strip blacklisted characters including spaces, to retain
                 display label formatting while ensuring the label is formatted properly for Synapse annotations.
+            file_annotations_upload (bool): Default to True. If false, do not add annotations to files.
         Return:
             manifest_synapse_file_id (str): SynID of manifest csv uploaded to synapse.
         """
         manifest_synapse_table_id, manifest, table_manifest = self.uploadDB(
             dmge=dmge,
             manifest=manifest,
             datasetId=datasetId,
             table_name=table_name,
             restrict=restrict,
             table_manipulation=table_manipulation,
             table_column_names=table_column_names,
         )
 
-        manifest = self.add_annotations_to_entities_files(
-            dmge,
-            manifest,
-            manifest_record_type,
-            datasetId,
-            hideBlanks,
-            manifest_synapse_table_id,
-            annotation_keys=annotation_keys,
-        )
+        if file_annotations_upload:
+            manifest = self.add_annotations_to_entities_files(
+                dmge,
+                manifest,
+                manifest_record_type,
+                datasetId,
+                hideBlanks,
+                manifest_synapse_table_id,
+                annotation_keys=annotation_keys,
+            )
 
         # Load manifest to synapse as a CSV File
         manifest_synapse_file_id = self.upload_manifest_file(
             manifest, metadataManifestPath, datasetId, restrict, component_name
         )
 
         # Set annotations for the file manifest.
@@ -1930,14 +1964,15 @@
         datasetId: str,
         manifest_record_type: str = "table_file_and_entities",
         hideBlanks: bool = False,
         restrict_manifest=False,
         table_manipulation: str = "replace",
         table_column_names: str = "class_label",
         annotation_keys: str = "class_label",
+        file_annotations_upload: bool = True,
     ) -> str:
         """Associate metadata with files in a storage dataset already on Synapse.
         Upload metadataManifest in the storage dataset folder on Synapse as well. Return synapseId of the uploaded manifest file.
 
         If this is a new manifest there could be no Synapse entities associated with the rows of this manifest
         this may be due to data type (e.g. clinical data) being tabular
         and not requiring files; to utilize uniform interfaces downstream
@@ -1969,26 +2004,26 @@
         # Read new manifest CSV:
         manifest = self._read_manifest(metadataManifestPath)
         manifest = self._add_id_columns_to_manifest(manifest, dmge)
 
         table_name, component_name = self._generate_table_name(manifest)
 
         # Upload manifest to synapse based on user input (manifest_record_type)
-
         if manifest_record_type == "file_only":
             manifest_synapse_file_id = self.upload_manifest_as_csv(
                 dmge,
                 manifest,
                 metadataManifestPath,
                 datasetId=datasetId,
                 restrict=restrict_manifest,
                 hideBlanks=hideBlanks,
                 manifest_record_type=manifest_record_type,
                 component_name=component_name,
                 annotation_keys=annotation_keys,
+                file_annotations_upload=file_annotations_upload,
             )
         elif manifest_record_type == "table_and_file":
             manifest_synapse_file_id = self.upload_manifest_as_table(
                 dmge,
                 manifest,
                 metadataManifestPath,
                 datasetId=datasetId,
@@ -1996,26 +2031,28 @@
                 component_name=component_name,
                 restrict=restrict_manifest,
                 hideBlanks=hideBlanks,
                 manifest_record_type=manifest_record_type,
                 table_manipulation=table_manipulation,
                 table_column_names=table_column_names,
                 annotation_keys=annotation_keys,
+                file_annotations_upload=file_annotations_upload,
             )
         elif manifest_record_type == "file_and_entities":
             manifest_synapse_file_id = self.upload_manifest_as_csv(
                 dmge,
                 manifest,
                 metadataManifestPath,
                 datasetId=datasetId,
                 restrict=restrict_manifest,
                 hideBlanks=hideBlanks,
                 manifest_record_type=manifest_record_type,
                 component_name=component_name,
                 annotation_keys=annotation_keys,
+                file_annotations_upload=file_annotations_upload,
             )
         elif manifest_record_type == "table_file_and_entities":
             manifest_synapse_file_id = self.upload_manifest_combo(
                 dmge,
                 manifest,
                 metadataManifestPath,
                 datasetId=datasetId,
@@ -2023,14 +2060,15 @@
                 component_name=component_name,
                 restrict=restrict_manifest,
                 hideBlanks=hideBlanks,
                 manifest_record_type=manifest_record_type,
                 table_manipulation=table_manipulation,
                 table_column_names=table_column_names,
                 annotation_keys=annotation_keys,
+                file_annotations_upload=file_annotations_upload,
             )
         else:
             raise ValueError("Please enter a valid manifest_record_type.")
         return manifest_synapse_file_id
 
     def getTableAnnotations(self, table_id: str):
         """Generate dictionary of annotations for the given Synapse file.
```

### Comparing `schematicpy-24.2.1/schematic/utils/cli_utils.py` & `schematicpy-24.4.1/schematic/utils/cli_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
     def extract(dictionary: Any, key: Any) -> Union[Any, None]:
         """Get value associated with key, defaulting to None."""
         if dictionary is None or not isinstance(dictionary, dict):
             return None
         return dictionary.get(key)
 
-    return reduce(extract, keys, dictionary)
+    return reduce(extract, keys, dictionary)  # type: ignore
 
 
 def log_value_from_config(arg_name: str, config_value: Any) -> None:
     """Logs when getting a value from the config
 
     Args:
         arg_name (str): Name of the argument. Used for logging.
```

### Comparing `schematicpy-24.2.1/schematic/utils/curie_utils.py` & `schematicpy-24.4.1/schematic/utils/curie_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 """Curie utils"""
 
 import logging
+from typing import Any, Union
 
+Context = dict[str, str]
+Record = dict[str, Union[str, list, dict, None]]
+Graph = list[Record]
+Schema = dict[str, Any]
 
 logger = logging.getLogger(__name__)
 
 
 def extract_name_from_uri_or_curie(item: str) -> str:
     """Extract name from uri or curie"""
     if "http" not in item and len(item.split(":")) == 2:
         return item.split(":")[-1]
     if len(item.split("//")[-1].split("/")) > 1:
         return item.split("//")[-1].split("/")[-1]
     raise ValueError("Error extracting name from URI or Curie.")
 
 
-def expand_curie_to_uri(curie: str, context_info: dict[str, str]) -> str:
+def expand_curie_to_uri(curie: str, context_info: Context) -> str:
     """Expand curie to uri based on the context given
 
     parmas
     ======
     curie: curie to be expanded (e.g. bts:BiologicalEntity)
     context_info: jsonld context specifying prefix-uri relation (e.g. {"bts":
     "http://schema.biothings.io/"})
@@ -32,45 +37,45 @@
         if prefix in context_info and prefix not in prefixes_not_expand:
             return context_info[prefix] + value
         # if the input is not curie, return the input unmodified
         return curie
     return curie
 
 
-def expand_curies_in_schema(schema):
+def expand_curies_in_schema(schema: Schema) -> Schema:
     """Expand all curies in a SchemaOrg JSON-LD file into URI"""
-    context = schema["@context"]
-    graph = schema["@graph"]
+    context: Context = schema["@context"]
+    graph: Graph = schema["@graph"]
     new_schema = {"@context": context, "@graph": [], "@id": schema["@id"]}
     for record in graph:
-        new_record = {}
+        new_record: Record = {}
         for key, value in record.items():
             if isinstance(value, str):
                 new_record[expand_curie_to_uri(key, context)] = expand_curie_to_uri(
                     value, context
                 )
             elif isinstance(value, list):
+                uri = expand_curie_to_uri(key, context)
                 if isinstance(value[0], dict):
-                    new_record[expand_curie_to_uri(key, context)] = []
+                    lst: list[dict[str, str]] = []
+                    new_record[uri] = lst
                     for _item in value:
-                        new_record[expand_curie_to_uri(key, context)].append(
-                            {"@id": expand_curie_to_uri(_item["@id"], context)}
-                        )
+                        lst.append({"@id": expand_curie_to_uri(_item["@id"], context)})
                 else:
-                    new_record[expand_curie_to_uri(key, context)] = [
+                    new_record[uri] = [
                         expand_curie_to_uri(_item, context) for _item in value
                     ]
             elif isinstance(value, dict) and "@id" in value:
                 new_record[expand_curie_to_uri(key, context)] = {
                     "@id": expand_curie_to_uri(value["@id"], context)
                 }
             elif value is None:
                 new_record[expand_curie_to_uri(key, context)] = None
         new_schema["@graph"].append(new_record)
     return new_schema
 
 
-def uri2label(uri, schema):
+def uri2label(uri: str, schema: Schema) -> list:
     """Given a URI, return the label"""
     return [
         record["rdfs:label"] for record in schema["@graph"] if record["@id"] == uri
     ][0]
```

### Comparing `schematicpy-24.2.1/schematic/utils/df_utils.py` & `schematicpy-24.4.1/schematic/utils/df_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 """df utils"""
 
 # pylint: disable=logging-fstring-interpolation
 
 import logging
 from copy import deepcopy
 from time import perf_counter
-from typing import Union
+from typing import Union, Any, Optional
 from datetime import datetime
 import dateparser as dp
 import pandas as pd
 import numpy as np
 from pandarallel import pandarallel  # type: ignore
 
 logger = logging.getLogger(__name__)
 
 
 def load_df(
     file_path: str,
     preserve_raw_input: bool = True,
     data_model: bool = False,
-    **load_args: dict,
+    allow_na_values: bool = False,
+    **load_args: Any,
 ) -> pd.DataFrame:
     """
     Universal function to load CSVs and return DataFrames
     Parses string entries to convert as appropriate to type int, float, and pandas timestamp
     Pandarallel is used for type inference for large manifests to improve performance
 
     Args:
         file_path (str): path of csv to open
         preserve_raw_input (bool, optional): If false, convert cell datatypes to an inferred type
         data_model (bool, optional): bool, indicates if importing a data model
+        allow_na_values (bool, optional): If true, allow pd.NA values in the dataframe
         **load_args(dict): dict of key value pairs to be passed to the pd.read_csv function
 
     Raises:
         ValueError: When pd.read_csv on the file path doesn't return as dataframe
 
     Returns:
         pd.DataFrame: a processed dataframe for manifests or unprocessed df for data models and
@@ -52,23 +54,20 @@
                 "Pandas did not return a dataframe. "
                 "Pandas will return a TextFileReader if chunksize parameter is used."
             )
         )
 
     # only trim if not data model csv
     if not data_model:
-        org_df = trim_commas_df(org_df)
+        org_df = trim_commas_df(org_df, allow_na_values=allow_na_values)
 
     if preserve_raw_input:
         logger.debug(f"Load Elapsed time {perf_counter()-t_load_df}")
         return org_df
 
-    is_null = org_df.isnull()
-    org_df = org_df.astype(str).mask(is_null, "")
-
     ints, is_int = find_and_convert_ints(org_df)
 
     float_df = convert_floats(org_df)
 
     # Store values that were converted to type int in the final dataframe
     processed_df = float_df.mask(is_int, other=ints)
 
@@ -88,39 +87,44 @@
     """
     # pylint: disable=unnecessary-lambda
     large_manifest_cutoff_size = 1000
     # Find integers stored as strings and replace with entries of type np.int64
     if (
         dataframe.size < large_manifest_cutoff_size
     ):  # If small manifest, iterate as normal for improved performance
-        ints = dataframe.map(
+        ints = dataframe.map(  # type:ignore
             lambda cell: convert_ints(cell), na_action="ignore"
         ).fillna(False)
 
     else:  # parallelize iterations for large manifests
         pandarallel.initialize(verbose=1)
-        ints = dataframe.parallel_applymap(
+        ints = dataframe.parallel_applymap(  # type:ignore
             lambda cell: convert_ints(cell), na_action="ignore"
         ).fillna(False)
 
     # Identify cells converted to integers
-    is_int = ints.map(pd.api.types.is_integer)
+    is_int = ints.map(pd.api.types.is_integer)  # type:ignore
+
+    assert isinstance(ints, pd.DataFrame)
+    assert isinstance(is_int, pd.DataFrame)
 
     return ints, is_int
 
 
 def convert_ints(string: str) -> Union[np.int64, bool]:
     """
     Lambda function to convert a string to an integer if possible, otherwise returns False
     Args:
         string: string to attempt conversion to int
     Returns:
         string converted to type int if possible, otherwise False
     """
-    return np.int64(string) if str.isdigit(string) else False
+    if isinstance(string, str) and str.isdigit(string):
+        return np.int64(string)
+    return False
 
 
 def convert_floats(dataframe: pd.DataFrame) -> pd.DataFrame:
     """
     Convert strings that represent floats to type float
     Args:
         dataframe: dataframe with nulls masked as empty strings
@@ -230,31 +234,36 @@
     # Sometimes pandas update can change the column datatype, recast
     for col in input_df_idx.columns:
         input_df_idx[col] = input_df_idx[col].astype(input_df.dtypes[col])
 
     return input_df_idx
 
 
-def trim_commas_df(dataframe: pd.DataFrame) -> pd.DataFrame:
+def trim_commas_df(
+    dataframe: pd.DataFrame,
+    allow_na_values: Optional[bool] = False,
+) -> pd.DataFrame:
     """Removes empty (trailing) columns and empty rows from pandas dataframe (manifest data).
 
     Args:
         dataframe: pandas dataframe with data from manifest file.
+        allow_na_values (bool, optional): If true, allow pd.NA values in the dataframe
 
     Returns:
         df: cleaned-up pandas dataframe.
     """
     # remove all columns which have substring "Unnamed" in them
     dataframe = dataframe.loc[:, ~dataframe.columns.str.contains("^Unnamed")]
 
     # remove all completely empty rows
     dataframe = dataframe.dropna(how="all", axis=0)
 
-    # Fill in nan cells with empty strings
-    dataframe.fillna("", inplace=True)
+    if allow_na_values is False:
+        # Fill in nan cells with empty strings
+        dataframe.fillna("", inplace=True)
     return dataframe
 
 
 def col_in_dataframe(col: str, dataframe: pd.DataFrame) -> bool:
     """Check if a column is in a dataframe, without worrying about case
 
     Args:
```

### Comparing `schematicpy-24.2.1/schematic/utils/general.py` & `schematicpy-24.4.1/schematic/utils/general.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,22 +62,25 @@
     if isinstance(item, str):
         return [item]
     if isinstance(item, list):
         return item
     return None
 
 
-def unlist(seq: Sequence) -> Any:
+X = TypeVar("X")
+
+
+def unlist(seq: Sequence[X]) -> Union[Sequence[X], X]:
     """Returns the first item of a sequence
 
     Args:
-        seq (Sequence): Any sequence
+        seq (Sequence[X]): A Sequence of any type
 
     Returns:
-        Any:
+        Union[Sequence[X], X]:
           if sequence is length one, return the first item
           otherwise return the sequence
     """
     if len(seq) == 1:
         return seq[0]
     return seq
 
@@ -122,22 +125,22 @@
     else:
         raise ValueError("Invalid value. Use either 'before' or 'after'.")
     return date_time_result
 
 
 def check_synapse_cache_size(
     directory: str = "/root/.synapseCache",
-) -> Union[float, int]:
+) -> float:
     """use du --sh command to calculate size of .synapseCache.
 
     Args:
         directory (str, optional): .synapseCache directory. Defaults to '/root/.synapseCache'
 
     Returns:
-        float or integer: returns size of .synapsecache directory in bytes
+        float: returns size of .synapsecache directory in bytes
     """
     # Note: this command might fail on windows user.
     # But since this command is primarily for running on AWS, it is fine.
     command = ["du", "-sh", directory]
     output = subprocess.run(command, capture_output=True, check=False).stdout.decode(
         "utf-8"
     )
@@ -148,19 +151,19 @@
         size_in_kb = float(size.rstrip("K"))
         byte_size = size_in_kb * 1000
     elif "M" in size:
         size_in_mb = float(size.rstrip("M"))
         byte_size = size_in_mb * 1000000
     elif "G" in size:
         size_in_gb = float(size.rstrip("G"))
-        byte_size = convert_gb_to_bytes(size_in_gb)
+        byte_size = size_in_gb * (1024**3)
     elif "B" in size:
         byte_size = float(size.rstrip("B"))
     else:
-        logger.error("Cannot recongize the file size unit")
+        logger.error("Cannot recognize the file size unit")
     return byte_size
 
 
 def clear_synapse_cache(synapse_cache: cache.Cache, minutes: int) -> int:
     """clear synapse cache before a certain time
 
     Args:
@@ -173,23 +176,14 @@
     minutes_earlier = calculate_datetime(
         input_date=current_date, minutes=minutes, before_or_after="before"
     )
     num_of_deleted_files = synapse_cache.purge(before_date=minutes_earlier)
     return num_of_deleted_files
 
 
-def convert_gb_to_bytes(g_bytes: int) -> int:
-    """convert gb to bytes
-    Args:
-        g_bytes: number of gb
-    return: total number of bytes
-    """
-    return g_bytes * 1024 * 1024 * 1024
-
-
 def entity_type_mapping(syn: Synapse, entity_id: str) -> str:
     """Return the entity type of manifest
 
     Args:
         syn (Synapse): Synapse object
         entity_id (str): id of an entity
 
@@ -271,17 +265,17 @@
             This is also useful in reducing the size of the printout
             Defaults to False.
 
     Returns:
         Callable: Profile of the decorated function
     """
 
-    def inner(func):
+    def inner(func: Callable) -> Callable:
         @wraps(func)
-        def wrapper(*args, **kwargs):
+        def wrapper(*args: Any, **kwargs: Any) -> Callable:
             _output_file = output_file or func.__name__ + ".prof"
             profiler = Profile()
             profiler.enable()
             retval = func(*args, **kwargs)
             profiler.disable()
             profiler.dump_stats(_output_file)
 
@@ -295,15 +289,15 @@
                     p_stats = pstats.Stats(profiler, stream=fle)
                     if strip_dirs:
                         p_stats.strip_dirs()
                     if isinstance(sort_by, (tuple, list)):
                         p_stats.sort_stats(*sort_by)
                     else:
                         p_stats.sort_stats(sort_by)
-                    p_stats.print_stats(lines_to_print)
+                    p_stats.print_stats(lines_to_print)  # type: ignore
             return retval
 
         return wrapper
 
     return inner
```

### Comparing `schematicpy-24.2.1/schematic/utils/google_api_utils.py` & `schematicpy-24.4.1/schematic/utils/google_api_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,44 @@
 """Google API utils"""
 
 # pylint: disable=logging-fstring-interpolation
 
 import os
 import logging
 import json
-from typing import Any, Union
+from typing import Any, Union, no_type_check, TypedDict
 
 import pandas as pd
-from googleapiclient.discovery import build  # type: ignore
+from googleapiclient.discovery import build, Resource  # type: ignore
 from google.oauth2 import service_account  # type: ignore
 from schematic.configuration.configuration import CONFIG
 from schematic.store.synapse import SynapseStorage
 
 logger = logging.getLogger(__name__)
 
 
 # If modifying these scopes, delete the file token.pickle.
 SCOPES = [
     "https://www.googleapis.com/auth/spreadsheets",
     "https://www.googleapis.com/auth/drive",
 ]
 
 
-def build_service_account_creds() -> dict[str, Any]:
+class GoogleServiceAcountCreds(TypedDict):
+    "Service account credentials for Google sheets"
+    sheet_service: Resource
+    drive_service: Resource
+    creds: service_account.Credentials
+
+
+def build_service_account_creds() -> GoogleServiceAcountCreds:
     """Build Google service account credentials
 
     Returns:
-        dict[str, Any]: The credentials
+        GoogleServiceAcountCreds: The credentials
     """
     if "SERVICE_ACCOUNT_CREDS" in os.environ:
         dict_creds = json.loads(os.environ["SERVICE_ACCOUNT_CREDS"])
         credentials = service_account.Credentials.from_service_account_info(
             dict_creds, scopes=SCOPES
         )
 
@@ -44,23 +51,24 @@
         )
     else:
         credentials = service_account.Credentials.from_service_account_file(
             CONFIG.service_account_credentials_path, scopes=SCOPES
         )
 
     # get a Google Sheet API service
-    sheet_service = build("sheets", "v4", credentials=credentials)
+    sheet_service: Resource = build("sheets", "v4", credentials=credentials)
     # get a Google Drive API service
-    drive_service = build("drive", "v3", credentials=credentials)
+    drive_service: Resource = build("drive", "v3", credentials=credentials)
 
-    return {
+    creds: GoogleServiceAcountCreds = {
         "sheet_service": sheet_service,
         "drive_service": drive_service,
         "creds": credentials,
     }
+    return creds
 
 
 def download_creds_file() -> None:
     """Download google credentials file"""
     syn = SynapseStorage.login()
 
     # if file path of service_account does not exist
@@ -88,15 +96,16 @@
     elif "SERVICE_ACCOUNT_CREDS" in os.environ:
         # remind users that "SERVICE_ACCOUNT_CREDS" as an environment variable is being used
         logger.info(
             "Using environment variable SERVICE_ACCOUNT_CREDS as the credential file."
         )
 
 
-def execute_google_api_requests(service: Any, requests_body: Any, **kwargs) -> Any:
+@no_type_check
+def execute_google_api_requests(service, requests_body, **kwargs) -> Any:
     """
     Execute google API requests batch; attempt to execute in parallel.
 
     Args:
         service (Any): google api service; for now assume google sheets service that is
           instantiated and authorized
         requests_body (Any): _description_
```

### Comparing `schematicpy-24.2.1/schematic/utils/io_utils.py` & `schematicpy-24.4.1/schematic/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `schematicpy-24.2.1/schematic/utils/schema_utils.py` & `schematicpy-24.4.1/schematic/utils/schema_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,49 @@
-import inflection
+"""Schema utils"""
+
+# pylint: disable=logging-fstring-interpolation
+
 import json
 import logging
-import networkx as nx
-import re
 import string
-from typing import List, Literal, Dict, Tuple, Union
+from typing import Literal, Union, Optional
+
+import inflection
 
 
 logger = logging.getLogger(__name__)
 
 DisplayLabelType = Literal["class_label", "display_label"]
+EntryType = Literal["class", "property"]
 BLACKLISTED_CHARS = ["(", ")", ".", " ", "-"]
 COMPONENT_NAME_DELIMITER = "#"
 COMPONENT_RULES_DELIMITER = "^^"
 RULE_DELIMITER = "::"
 
 
-def attr_dict_template(key_name: str) -> Dict[str, dict[str, dict]]:
+def attr_dict_template(key_name: str) -> dict[str, dict[str, dict]]:
+    """Create a single empty attribute_dict template.
+
+    Args:
+        key_name (str): Attribute/node to use as the key in the dict.
+
+    Returns:
+        dict[str, dict[str, dict]]: template single empty attribute_relationships dictionary
+    """
     return {key_name: {"Relationships": {}}}
 
 
 def get_property_label_from_display_name(
     display_name: str, strict_camel_case: bool = False
 ) -> str:
     """Convert a given display name string into a proper property label string
     Args:
         display_name, str: node display name
-        strict_camel_case, bool: Default, False; defines whether or not to use strict camel case or not for conversion.
+        strict_camel_case, bool: Default, False; defines whether or not to use
+          strict camel case or not for conversion.
     Returns:
         label, str: property label of display name
     """
     # This is the newer more strict method
     if strict_camel_case:
         display_name = display_name.strip().translate(
             {ord(c): "_" for c in string.whitespace}
@@ -47,15 +60,16 @@
 
 def get_class_label_from_display_name(
     display_name: str, strict_camel_case: bool = False
 ) -> str:
     """Convert a given display name string into a proper class label string
     Args:
         display_name, str: node display name
-        strict_camel_case, bool: Default, False; defines whether or not to use strict camel case or not for conversion.
+        strict_camel_case, bool: Default, False; defines whether or not to
+         use strict camel case or not for conversion.
     Returns:
         label, str: class label of display name
     """
     # This is the newer more strict method
     if strict_camel_case:
         display_name = display_name.strip().translate(
             {ord(c): "_" for c in string.whitespace}
@@ -69,58 +83,70 @@
 
     return label
 
 
 def get_attribute_display_name_from_label(
     node_name: str, attr_relationships: dict
 ) -> str:
-    """Get attribute display name for a node, using the node label, requires the attr_relationships dicitonary from the data model parser
+    """
+    Get attribute display name for a node, using the node label, requires the attr_relationships
+      dictionary from the data model parser
+
     Args:
         node_name, str: node label
-        attr_relationships, dict: dictionary defining attributes and relationships, generated in data model parser.
+        attr_relationships, dict: dictionary defining attributes and relationships,
+          generated in data model parser.
     Returns:
         display_name, str: node display name, recorded in attr_relationships.
     """
     if "Attribute" in attr_relationships.keys():
         display_name = attr_relationships["Attribute"]
     else:
         display_name = node_name
     return display_name
 
 
 def check_if_display_name_is_valid_label(
     display_name: str,
-    blacklisted_chars: list[str] = BLACKLISTED_CHARS,
+    blacklisted_chars: Optional[list[str]] = None,
 ) -> bool:
     """Check if the display name can be used as a display label
+
     Args:
-        display_name, str: node display name
-        blacklisted_chars, list[str]: characters that are not permitted for synapse annotations uploads.
+        display_name (str): node display name
+        blacklisted_chars (Optional[list[str]], optional):
+          characters that are not permitted for synapse annotations uploads.
+          Defaults to None.
+
     Returns:
-        valid_label, bool: True, if the display name can be used as a label, False, if it cannot.
+        bool: True, if the display name can be used as a label, False, if it cannot.
     """
-    valid_label = True
-    if any(map(display_name.__contains__, blacklisted_chars)):
-        valid_label = False
+    if blacklisted_chars is None:
+        blacklisted_chars = BLACKLISTED_CHARS
+    valid_label = not any(char in display_name for char in blacklisted_chars)
     return valid_label
 
 
 def get_stripped_label(
     display_name: str,
-    entry_type: str,
-    blacklisted_chars: list[str] = BLACKLISTED_CHARS,
+    entry_type: EntryType,
+    blacklisted_chars: Optional[list[str]] = None,
 ) -> str:
     """
     Args:
         display_name, str: node display name
-        entry_type, str: 'class' or 'property', defines what type the entry is.
-        blacklisted_chars, list[str]: characters that are not permitted for synapse annotations uploads.
+        entry_type, EntryType: 'class' or 'property', defines what type the entry is.
+        blacklisted_chars, list[str]: characters that are not permitted for
+          synapse annotations uploads.
     Returns:
-        stripped_label, str: class or property label that has been stripped of blacklisted characters.
+        stripped_label, str: class or property label that has been stripped
+          of blacklisted characters.
     """
+    if blacklisted_chars is None:
+        blacklisted_chars = BLACKLISTED_CHARS
     if entry_type.lower() == "class":
         stripped_label = [
             get_class_label_from_display_name(str(display_name)).translate(
                 {ord(x): "" for x in blacklisted_chars}
             )
         ][0]
 
@@ -128,27 +154,33 @@
         stripped_label = [
             get_property_label_from_display_name(str(display_name)).translate(
                 {ord(x): "" for x in blacklisted_chars}
             )
         ][0]
 
     logger.warning(
-        f"Cannot use display name {display_name} as the data model label, becaues it is not formatted properly. Please remove all spaces and blacklisted characters: {str(blacklisted_chars)}. The following label was assigned instead: {stripped_label}"
+        (
+            f"Cannot use display name {display_name} as the data model label, "
+            "because it is not formatted properly. Please remove all spaces and "
+            f"blacklisted characters: {str(blacklisted_chars)}. "
+            f"The following label was assigned instead: {stripped_label}"
+        )
     )
     return stripped_label
 
 
 def get_schema_label(
-    display_name: str, entry_type: str, strict_camel_case: bool
+    display_name: str, entry_type: EntryType, strict_camel_case: bool
 ) -> str:
     """Get the class or property label for a given display name
     Args:
         display_name, str: node display name
-        entry_type, str: 'class' or 'property', defines what type the entry is.
-        strict_camel_case, bool: Default, False; defines whether or not to use strict camel case or not for conversion.
+        entry_type, EntryType: 'class' or 'property', defines what type the entry is.
+        strict_camel_case, bool: Default, False; defines whether or not to use strict
+          camel case or not for conversion.
     Returns:
         label, str: class label of display name
     Raises:
         Error Logged if entry_type.lower(), is not either 'class' or 'property'
     """
     if entry_type.lower() == "class":
         label = get_class_label_from_display_name(
@@ -157,30 +189,34 @@
 
     elif entry_type.lower() == "property":
         label = get_property_label_from_display_name(
             display_name=display_name, strict_camel_case=strict_camel_case
         )
     else:
         logger.error(
-            f"The entry type submitted: {entry_type}, is not one of the permitted types: 'class' or 'property'"
+            (
+                f"The entry type submitted: {entry_type}, is not one of the "
+                "permitted types: 'class' or 'property'"
+            )
         )
     return label
 
 
 def get_label_from_display_name(
     display_name: str,
-    entry_type: str,
+    entry_type: EntryType,
     strict_camel_case: bool = False,
     data_model_labels: DisplayLabelType = "class_label",
 ) -> str:
     """Get node label from provided display name, based on whether the node is a class or property
     Args:
         display_name, str: node display name
-        entry_type, str: 'class' or 'property', defines what type the entry is.
-        strict_camel_case, bool: Default, False; defines whether or not to use strict camel case or not for conversion.
+        entry_type, EntryType: 'class' or 'property', defines what type the entry is.
+        strict_camel_case, bool: Default, False; defines whether or not to use strict camel
+          case or not for conversion.
     Returns:
         label, str: label to be used for the provided display name.
     """
     if data_model_labels == "display_label":
         # Check that display name can be used as a label.
         valid_display_name = check_if_display_name_is_valid_label(
             display_name=display_name
@@ -208,46 +244,50 @@
         provided_bool, str: true or false bool
     Returns:
         Boolean converted to 'true' or 'false' str as appropriate.
     """
     return str(provided_bool)
 
 
-def get_individual_rules(
-    rule: str, validation_rules: list[Union[str, None]]
-) -> Union[str, list]:
+def get_individual_rules(rule: str, validation_rules: list) -> list:
     """Extract individual rules from a string and add to a list of rules
     Args:
-        rule, str: valdation rule that has been parsed from a component rule.
-        validaiton_rules, list: list of rules being collected,
+        rule, str: validation rule that has been parsed from a component rule.
+        validation_rules, list: list of rules being collected,
             if this is the first time the list is being added to, it will be empty
     Returns:
-        validaiton_rules, list: list of rules being collected.
+        validation_rules, list: list of rules being collected.
     """
     # Separate multiple rules (defined by addition of the rule delimiter)
     if RULE_DELIMITER in rule:
         validation_rules.append(parse_single_set_validation_rules(rule))
     # Get single rule
     else:
         validation_rules.append(rule)
     return validation_rules
 
 
 def get_component_name_rules(
-    component_names: list[Union[str, None]], component_rule: str
-) -> Tuple[list, str]:
-    """Get component name and rule from an string that was initilly split by the COMPONENT_RULES_DELIMITER
+    component_names: list[str], component_rule: str
+) -> tuple[list[str], str]:
+    """
+    Get component name and rule from an string that was initially split by the
+      COMPONENT_RULES_DELIMITER
+
     Args:
-        component_names, list[Union[str,None]]: list of components, will be empty if being added to for the first time.
-        component_rule, str: component rule string that has only been split by the COMPONENT_RULES_DELIMETER
+        component_names, list[str]: list of components, will be empty
+          if being added to for the first time.
+        component_rule, str: component rule string that has only been split by
+          the COMPONENT_RULES_DELIMITER
     Returns:
         Tuple[list,str]: list with the a new component name or 'all_other_components' appended,
             rule with the component name stripped off.
     Raises:
-        Error Logged if it looks like a component name should have been added to the list, but wass not.
+        Error Logged if it looks like a component name should have been added to the
+          list, but was not.
     """
     # If a component name is not attached to the rule, have it apply to all other components
     if COMPONENT_NAME_DELIMITER != component_rule[0]:
         component_names.append("all_other_components")
     # Get the component name if available
     else:
         component_names.append(
@@ -264,42 +304,48 @@
         component_rule = component_rule.strip()
     return component_names, component_rule
 
 
 def check_for_duplicate_components(
     component_names: list[str], validation_rule_string: str
 ) -> None:
-    """Check if component names are repeated in a validation rule
+    """
+    Check if component names are repeated in a validation rule
+    Error Logged if a component name is duplicated.
+
     Args:
-        component_names, list[str]: list of components identified in the validation rule
-        validation_rule_str, str: validation rule, used if error needs to be raised.
-    Returns:
-        None
-    Raises: Error Logged if a component name is duplicated.
+        component_names (list[str]): list of components identified in the validation rule
+        validation_rule_string (str): validation rule, used if error needs to be raised.
     """
     duplicated_entries = [cn for cn in component_names if component_names.count(cn) > 1]
     if duplicated_entries:
         logger.error(
-            f"Oops, it looks like the following rule {validation_rule_string}, contains the same component "
-            f"name more than once. An attribute can only have a single rule applied per manifest/component."
+            f"Oops, it looks like the following rule {validation_rule_string}, "
+            "contains the same component name more than once. An attribute can "
+            "only have a single rule applied per manifest/component."
         )
-    return
 
 
-def parse_component_validation_rules(validation_rule_string: str) -> Dict:
-    """If a validation rule is identified to be fomatted as a component validation rule, parse to a dictionary of components:rules
+def parse_component_validation_rules(
+    validation_rule_string: str,
+) -> dict[str, list[str]]:
+    """
+    If a validation rule is identified to be formatted as a component validation rule,
+      parse to a dictionary of components:rules
+
     Args:
-        validation_rule_string, str: validation rule provided by user.
+        validation_rule_string (str):  validation rule provided by user.
+
     Returns:
-        validation_rules_dict, dict: validation rules parsed to a dictionary where
-            the key is the component name (or 'all_other_components') and the value is the parsed validaiton rule for
-            the given component.
+        dict[str, list[str]]: validation rules parsed to a dictionary where the key
+          is the component name (or 'all_other_components') and the value is the parsed
+          validation rule for the given component.
     """
-    component_names = []
-    validation_rules = []
+    component_names: list[str] = []
+    validation_rules: list[list[str]] = []
 
     component_rules = validation_rule_string.split(COMPONENT_RULES_DELIMITER)
     # Extract component rules, per component
     for component_rule in component_rules:
         component_rule = component_rule.strip()
         if component_rule:
             # Get component name attached to rule
@@ -323,119 +369,116 @@
     check_for_duplicate_components(component_names, validation_rule_string)
 
     validation_rules_dict = dict(zip(component_names, validation_rules))
 
     return validation_rules_dict
 
 
-def parse_single_set_validation_rules(validation_rule_string: str) -> list:
+def parse_single_set_validation_rules(validation_rule_string: str) -> list[str]:
     """Parse a single set of validation rules.
+
     Args:
-        validation_rule_string, str: validation rule provided by user.
+        validation_rule_string (str): validation rule provided by user.
+
     Returns:
-        list, the valiation rule string split by the rule delimiter
-    Raise:
-        ValueEror if the string contains a component name delimter in the beginning.
-            This would indicate that a user was trying to set component rules, but did so improperly.
+        list: the validation rule string split by the rule delimiter
     """
     # Try to catch an improperly formatted rule
     if COMPONENT_NAME_DELIMITER == validation_rule_string[0]:
         logger.error(
-            f"The provided validation rule {validation_rule_string}, looks to be formatted as a component "
-            f"based rule, but is missing the necessary formatting, "
-            f"please refer to the SchemaHub documentation for more details."
+            f"The provided validation rule {validation_rule_string}, looks to be formatted as a "
+            "component based rule, but is missing the necessary formatting, "
+            "please refer to the SchemaHub documentation for more details."
         )
 
     return validation_rule_string.split(RULE_DELIMITER)
 
 
 def parse_validation_rules(validation_rules: Union[list, dict]) -> Union[list, dict]:
     """Split multiple validation rules based on :: delimiter
+
     Args:
-        validation_rules, Any[List[str], Dict]: List or Dictionary of validation rules,
-            if list, contains a string validation rule; if dictionary, key is the component the
-            rule (value) is applied to
+        validation_rules (Union[list, dict]): List or Dictionary of validation rules,
+            if list:, contains a string validation rule
+            if dict:, key is the component the rule (value) is applied to
+
     Returns:
-        validation_rules, Union[list,dict]: Parsed validation rules, component rules are output as a dictionary,
-            single sets are a list.
-    Raises:
-        Error Logged if Rule is not formatted properly
+        Union[list, dict]: Parsed validation rules, component rules are output
+          as a dictionary, single sets are a list.
     """
-
     if isinstance(validation_rules, dict):
         # Rules pulled in as a dict can be used directly
         return validation_rules
-    elif isinstance(validation_rules, list):
-        # If rules are already parsed from the JSONLD
-        if len(validation_rules) > 1 and isinstance(validation_rules[-1], str):
-            return validation_rules
-        # Parse rules set for a subset of components/manifests
-        elif COMPONENT_RULES_DELIMITER in validation_rules[0]:
-            return parse_component_validation_rules(
-                validation_rule_string=validation_rules[0]
-            )
-        # Parse rules that are set across *all* components/manifests
-        else:
-            return parse_single_set_validation_rules(
-                validation_rule_string=validation_rules[0]
-            )
-    return
+
+    # If rules are already parsed from the JSONLD
+    if len(validation_rules) > 1 and isinstance(validation_rules[-1], str):
+        return validation_rules
+    # Parse rules set for a subset of components/manifests
+    if COMPONENT_RULES_DELIMITER in validation_rules[0]:
+        return parse_component_validation_rules(
+            validation_rule_string=validation_rules[0]
+        )
+    # Parse rules that are set across *all* components/manifests
+    return parse_single_set_validation_rules(validation_rule_string=validation_rules[0])
 
 
 def extract_component_validation_rules(
-    manifest_component: str, validation_rules: dict[str, list]
-) -> list:
-    """Parse a component validation rule dictionary to pull out the rule (if any) for a given manifest
+    manifest_component: str, validation_rules_dict: dict[str, Union[list, str]]
+) -> list[Union[str, list]]:
+    """
+    Parse a component validation rule dictionary to pull out the rule (if any) for a given manifest
+
     Args:
         manifest_component, str: Component label, pulled from the manifest directly
-        validation_rules, dict[str, list[Union[list,str]]: Validation rules dictionary, where keys are the manifest component label,
-            and the value is a parsed set of validation rules.
+        validation_rules_dict, dict[str, list[Union[list,str]]: Validation rules dictionary,
+          where keys are the manifest component label, and the value is a parsed set of
+          validation rules.
     Returns:
         validation_rules, list[str]: rule for the provided manifest component if one is available,
-            if a validation rule is not specified for a given component but "all_other_components" is specified (as a key), then pull that one,
-            otherwise return an empty list.
+            if a validation rule is not specified for a given component but "all_other_components"
+            is specified (as a key), then pull that one, otherwise return an empty list.
     """
-    manifest_component_rule = validation_rules.get(manifest_component)
-    all_component_rules = validation_rules.get("all_other_components")
+    manifest_component_rule = validation_rules_dict.get(manifest_component)
+    all_component_rules = validation_rules_dict.get("all_other_components")
 
     # Capture situation where manifest_component rule is an empty string
     if manifest_component_rule is not None:
         if isinstance(manifest_component_rule, str):
             if manifest_component_rule == "":
-                validation_rules = []
+                validation_rules_list: list[Union[str, list]] = []
             else:
-                validation_rules = [manifest_component_rule]
+                validation_rules_list = [manifest_component_rule]
         elif isinstance(manifest_component_rule, list):
-            validation_rules = manifest_component_rule
+            validation_rules_list = manifest_component_rule
     elif all_component_rules:
         if isinstance(all_component_rules, str):
-            validation_rules = [all_component_rules]
+            validation_rules_list = [all_component_rules]
         elif isinstance(all_component_rules, list):
-            validation_rules = all_component_rules
+            validation_rules_list = all_component_rules
     else:
-        validation_rules = []
-    return validation_rules
+        validation_rules_list = []
+    return validation_rules_list
 
 
 def export_schema(schema: dict, file_path: str) -> None:
     """Export schema to given filepath.
     Args:
         schema, dict: JSONLD schema
         filepath, str: path to store the schema
     """
-    with open(file_path, "w") as f:
-        json.dump(schema, f, sort_keys=True, indent=4, ensure_ascii=False)
+    with open(file_path, "w", encoding="utf-8") as json_file:
+        json.dump(schema, json_file, sort_keys=True, indent=4, ensure_ascii=False)
 
 
-def strip_context(context_value: str) -> tuple[str]:
+def strip_context(context_value: str) -> tuple[str, str]:
     """Strip contexts from str entry.
     Args:
         context_value, str: string from which to strip context from
     Returns:
         context, str: the original context
-        v, str: value separated from context
+        value, str: value separated from context
     """
     if ":" in context_value:
-        context, v = context_value.split(":")
+        context, value = context_value.split(":")
     elif "@" in context_value:
-        context, v = context_value.split("@")
-    return context, v
+        context, value = context_value.split("@")
+    return context, value
```

### Comparing `schematicpy-24.2.1/schematic/utils/validate_rules_utils.py` & `schematicpy-24.4.1/schematic/utils/validate_rules_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,29 @@
 """validate rules utils"""
 
 import logging
-from typing import Union
+from typing import TypedDict, Optional, Literal
+from typing_extensions import assert_never
 from jsonschema import ValidationError
 
 
 logger = logging.getLogger(__name__)
 
 
-def validation_rule_info() -> (
-    dict[str, dict[str, Union[tuple[int, int], str, list[str], None]]]
-):
+class Rule(TypedDict):
+    """A validation rule"""
+
+    arguments: tuple[int, int]
+    type: str
+    complementary_rules: Optional[list[str]]
+    default_message_level: Optional[str]
+    fixed_arg: Optional[list[str]]
+
+
+def validation_rule_info() -> dict[str, Rule]:
     """
     Function to return dict that holds information about each rule
     Will be pulled into validate_single_rule, validate_manifest_rules, validate_schema_rules
     Structure:
         Rule:{
             'arguments':(<num arguments allowed>, <num arguments required>),
             'type': <rule type>,
@@ -23,113 +32,136 @@
     """
     return {
         "int": {
             "arguments": (1, 0),
             "type": "type_validation",
             "complementary_rules": ["inRange", "IsNA"],
             "default_message_level": "error",
+            "fixed_arg": None,
         },
         "float": {
             "arguments": (1, 0),
             "type": "type_validation",
             "complementary_rules": ["inRange", "IsNA"],
             "default_message_level": "error",
+            "fixed_arg": None,
         },
         "num": {
             "arguments": (1, 0),
             "type": "type_validation",
             "complementary_rules": ["inRange", "IsNA"],
             "default_message_level": "error",
+            "fixed_arg": None,
         },
         "str": {
             "arguments": (1, 0),
             "type": "type_validation",
             "complementary_rules": None,
             "default_message_level": "error",
+            "fixed_arg": None,
         },
         "date": {
             "arguments": (1, 0),
             "type": "content_validation",
             "complementary_rules": None,
             "default_message_level": "error",
+            "fixed_arg": None,
         },
         "regex": {
             "arguments": (3, 2),
             "fixed_arg": ["strict"],
             "type": "regex_validation",
             "complementary_rules": ["list"],
             "default_message_level": "error",
         },
         "url": {
             "arguments": (101, 0),
             "type": "url_validation",
             "complementary_rules": None,
             "default_message_level": "error",
+            "fixed_arg": None,
         },
         "list": {
             "arguments": (2, 0),
             "type": "list_validation",
             "complementary_rules": ["regex"],
             "default_message_level": "error",
+            "fixed_arg": None,
         },
         "matchAtLeastOne": {
             "arguments": (3, 2),
             "type": "cross_validation",
             "complementary_rules": None,
             "default_message_level": "warning",
+            "fixed_arg": None,
         },
         "matchExactlyOne": {
             "arguments": (3, 2),
             "type": "cross_validation",
             "complementary_rules": None,
             "default_message_level": "warning",
+            "fixed_arg": None,
+        },
+        "matchNone": {
+            "arguments": (3, 2),
+            "type": "cross_validation",
+            "complementary_rules": None,
+            "default_message_level": "warning",
+            "fixed_arg": None,
         },
         "recommended": {
             "arguments": (1, 0),
             "type": "content_validation",
             "complementary_rules": None,
             "default_message_level": "warning",
+            "fixed_arg": None,
         },
         "protectAges": {
             "arguments": (1, 0),
             "type": "content_validation",
             "complementary_rules": [
                 "inRange",
             ],
             "default_message_level": "warning",
+            "fixed_arg": None,
         },
         "unique": {
             "arguments": (1, 0),
             "type": "content_validation",
             "complementary_rules": None,
             "default_message_level": "error",
+            "fixed_arg": None,
         },
         "inRange": {
             "arguments": (3, 2),
             "type": "content_validation",
             "complementary_rules": ["int", "float", "num", "protectAges"],
             "default_message_level": "error",
+            "fixed_arg": None,
         },
         "IsNA": {
-            "arguments": (1, 0),
+            "arguments": (0, 0),
             "type": "content_validation",
             "complementary_rules": [
                 "int",
                 "float",
                 "num",
             ],
-            "default_message_level": "warning",
+            "default_message_level": None,
+            "fixed_arg": None,
         },
     }
 
 
 def get_error(
     validation_rules: str,
     attribute_name: str,
-    error_type: str,
+    error_type: Literal[
+        "delimiter", "not_rule", "args_not_allowed", "incorrect_num_args"
+    ],
     input_filetype: str,
 ) -> list[str]:
     """
     Generate error message for errors when trying to specify
     multiple validation rules.
     """
     error_col = attribute_name  # Attribute name
@@ -141,36 +173,37 @@
             f"({validation_rules}) are improperly "
             "specified. Please check your delimiter is '::'"
         )
         logging.error(error_str)
         error_message = error_str
         error_val = "Multiple Rules: Delimiter"
 
-    if error_type == "not_rule":
+    elif error_type == "not_rule":
         error_str = (
             f"The {input_filetype}, has an error in the validation rule "
             f"for the attribute: {attribute_name}, the provided validation rules "
             f"({validation_rules}) is not "
             "a valid rule. Please check spelling."
         )
         logging.error(error_str)
         error_message = error_str
         error_val = "Not a Rule"
 
-    if error_type == "args_not_allowed":
+    elif error_type == "args_not_allowed":
         error_str = (
             f"The {input_filetype}, has an error in the validation rule "
             f"for the attribute: {attribute_name}, the provided validation rules "
             f"({validation_rules}) is not"
             "formatted properly. No additional arguments are allowed for this rule."
         )
         logging.error(error_str)
         error_message = error_str
         error_val = "Args not allowed."
-    if error_type == "incorrect_num_args":
+
+    elif error_type == "incorrect_num_args":
         rule_type = validation_rules.split(" ")[0]
 
         if rule_type in validation_rule_info():
             arg_tuple = validation_rule_info()[rule_type]["arguments"]
             assert isinstance(arg_tuple, tuple)
             assert len(arg_tuple) == 2
             number_allowed = str(arg_tuple[0])
@@ -185,30 +218,35 @@
             "formatted properly. The number of provided arguments does not match the "
             f"number allowed({number_allowed}) or required({number_required})."
         )
         logging.error(error_str)
         error_message = error_str
         error_val = "Incorrect num arguments."
 
+    else:
+        assert_never(error_type)
+
     return ["NA", error_col, error_message, error_val]
 
 
-def validate_single_rule(validation_rule: str, attribute: str, input_filetype: str):
+def validate_single_rule(
+    validation_rule: str, attribute: str, input_filetype: str
+) -> list[list[str]]:
     """
     Perform validation for a single rule to ensure it is specified
       correctly with an appropriate number of arguments
     Inputs:
         validation_rule: single rule being validated
         attribute: attribute validation rule was specified for
         input_filetype: filetype of model input
 
     Returns:
         errors: List of errors
     """
-    errors = []
+    errors: list[list[str]] = []
     validation_types = validation_rule_info()
     validation_rule_with_args = [
         val_rule.strip() for val_rule in validation_rule.strip().split(" ")
     ]
 
     rule_type = validation_rule_with_args[0]
 
@@ -235,17 +273,16 @@
     # if the rule is indeed a rule and formatted correctly, check that arguments are appropriate
     else:
         arg_tuple = validation_rule_info()[rule_type]["arguments"]
         assert isinstance(arg_tuple, tuple)
         assert len(arg_tuple) == 2
         arguments_allowed, arguments_required = arg_tuple
         # Remove any fixed args from our calc.
-        if "fixed_arg" in validation_types[rule_type]:
-            fixed_args = validation_types[rule_type]["fixed_arg"]
-            assert isinstance(fixed_args, list)
+        fixed_args = validation_types[rule_type]["fixed_arg"]
+        if fixed_args:
             num_args = (
                 len([vr for vr in validation_rule_with_args if vr not in fixed_args])
                 - 1
             )
         else:
             num_args = len(validation_rule_with_args) - 1
```

### Comparing `schematicpy-24.2.1/schematic/visualization/attributes_explorer.py` & `schematicpy-24.4.1/schematic/visualization/attributes_explorer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,51 +1,59 @@
 """Attributes Explorer Class"""
 import json
 import logging
 import os
-
+from typing import Optional, no_type_check
 import numpy as np
 import pandas as pd
 
 from schematic.schemas.data_model_parser import DataModelParser
 from schematic.schemas.data_model_graph import DataModelGraph, DataModelGraphExplorer
 from schematic.schemas.data_model_json_schema import DataModelJSONSchema
+from schematic.utils.schema_utils import DisplayLabelType
 from schematic.utils.io_utils import load_json
 
 logger = logging.getLogger(__name__)
 
 
 class AttributesExplorer:
     """AttributesExplorer class"""
 
+    # pylint: disable=too-many-arguments
     def __init__(
         self,
         path_to_jsonld: str,
-        data_model_labels: str,
+        data_model_labels: DisplayLabelType,
+        data_model_grapher: Optional[DataModelGraph] = None,
+        data_model_graph_explorer: Optional[DataModelGraphExplorer] = None,
+        parsed_data_model: Optional[dict] = None,
     ) -> None:
         self.path_to_jsonld = path_to_jsonld
 
         self.jsonld = load_json(self.path_to_jsonld)
 
-        # Instantiate Data Model Parser
-        data_model_parser = DataModelParser(
-            path_to_data_model=self.path_to_jsonld,
-        )
-
         # Parse Model
-        parsed_data_model = data_model_parser.parse_model()
+        if not parsed_data_model:
+            data_model_parser = DataModelParser(
+                path_to_data_model=self.path_to_jsonld,
+            )
+            parsed_data_model = data_model_parser.parse_model()
 
         # Instantiate DataModelGraph
-        data_model_grapher = DataModelGraph(parsed_data_model, data_model_labels)
+        if not data_model_grapher:
+            data_model_grapher = DataModelGraph(parsed_data_model, data_model_labels)
 
         # Generate graph
-        self.graph_data_model = data_model_grapher.generate_data_model_graph()
+        self.graph_data_model = data_model_grapher.graph
 
         # Instantiate Data Model Graph Explorer
-        self.dmge = DataModelGraphExplorer(self.graph_data_model)
+        if not data_model_graph_explorer:
+            self.dmge = DataModelGraphExplorer(self.graph_data_model)
+        else:
+            self.dmge = data_model_graph_explorer
 
         # Instantiate Data Model Json Schema
         self.data_model_js = DataModelJSONSchema(
             jsonld_path=self.path_to_jsonld, graph=self.graph_data_model
         )
 
         self.output_path = self.create_output_path("merged_csv")
@@ -62,98 +70,105 @@
         output_path = os.path.join(
             base_dir, "visualization", self.schema_name, terminal_folder
         )
         if not os.path.exists(output_path):
             os.makedirs(output_path)
         return output_path
 
-    def convert_string_cols_to_json(
+    def _convert_string_cols_to_json(
         self, dataframe: pd.DataFrame, cols_to_modify: list[str]
     ) -> pd.DataFrame:
         """Converts values in a column from strings to JSON list
         for upload to Synapse.
         """
         for col in dataframe.columns:
             if col in cols_to_modify:
                 dataframe[col] = dataframe[col].apply(
                     lambda x: json.dumps([y.strip() for y in x])
                     if x != "NaN" and x and x == np.nan
                     else x
                 )
         return dataframe
 
-    def parse_attributes(self, save_file: bool = True) -> pd.DataFrame:
+    def parse_attributes(self, save_file: bool = True) -> Optional[str]:
         """
-        Args: save_file (bool):
-                True: merged_df is saved locally to output_path.
-                False: merged_df is returned.
+        Args:
+            save_file (bool, optional):
+              True: merged_df is saved locally to output_path.
+              False: merged_df is returned as a string
+              Defaults to True.
 
         Returns:
-            merged_df (pd.DataFrame): dataframe containing data relating to attributes
-                for the provided data model for all components in the data model.
-                Dataframe is saved locally as a csv if save_file == True, or returned if
-                save_file == False.
+            Optional[str]: if save_file=False, the dataframe as a string, otherwise None
 
         """
         # get all components
         component_dg = self.dmge.get_digraph_by_edge_type("requiresComponent")
         components = component_dg.nodes()
 
         # For each data type to be loaded gather all attributes the user would
         # have to provide.
         return self._parse_attributes(components, save_file)
 
-    def parse_component_attributes(
-        self, component=None, save_file: bool = True, include_index: bool = True
-    ) -> pd.DataFrame:
+    def _parse_component_attributes(
+        self,
+        component: Optional[str] = None,
+        save_file: bool = True,
+        include_index: bool = True,
+    ) -> Optional[str]:
         """
-        Args: save_file (bool):
-                True: merged_df is saved locally to output_path.
-                False: merged_df is returned.
-              include_index (bool):
-                Whether to include the index in the returned dataframe (True) or not (False)
+
+        Args:
+            component (Optional[str], optional): A component. Defaults to None.
+            save_file (bool, optional):
+              True: merged_df is saved locally to output_path.
+              False: merged_df is returned as a string
+              Defaults to True.
+            include_index (bool, optional):
+              Whether to include the index in the returned dataframe (True) or not (False)
+              Defaults to True.
+
+        Raises:
+            ValueError: If Component is None
 
         Returns:
-            merged_df (pd.DataFrame): dataframe containing data relating to attributes
-                for the provided data model for the specified component in the data model.
-                Dataframe is saved locally as a csv if save_file == True, or returned if
-                save_file == False.
+            Optional[str]: if save_file=False, the dataframe as a string, otherwise None
         """
-
         if not component:
             raise ValueError("You must provide a component to visualize.")
         return self._parse_attributes([component], save_file, include_index)
 
+    @no_type_check
     def _parse_attributes(
-        self, components: list, save_file=True, include_index=True
-    ) -> pd.DataFrame:
+        self, components: list[str], save_file: bool = True, include_index: bool = True
+    ) -> Optional[str]:
         """
         Args: save_file (bool):
                 True: merged_df is saved locally to output_path.
                 False: merged_df is returned.
-              components (list):
+              components (list[str]):
                 list of components to parse attributes for
               include_index (bool):
                 Whether to include the index in the returned dataframe (True) or not (False)
 
         Returns:
-            merged_df (pd.DataFrame): dataframe containing data relating to attributes
-                for the provided data model for specified components in the data model.
-                Dataframe is saved locally as a csv if save_file == True, or returned if
-                save_file == False.
+            Optional[str]:
+              if save_file=False, the dataframe as a string, otherwise None
+
         Raises:
             ValueError:
                 If unable hits an error while attempting to get conditional requirements.
                 This error is likely to be found if there is a mismatch in naming.
         """
         # This function needs to be refactored, temporarily disabling some pylint errors
         # pylint: disable=too-many-locals
         # pylint: disable=too-many-nested-blocks
         # pylint: disable=too-many-branches
         # pylint: disable=too-many-statements
+        # type
 
         # For each data type to be loaded gather all attributes the user would
         # have to provide.
         df_store = []
         for component in components:
             data_dict: dict = {}
 
@@ -260,15 +275,15 @@
                 "Valid Values",
                 "Conditional Requirements",
                 "Validation Rules",
                 "Component",
             ]
             cols = [col for col in cols if col in data_dict_df.columns]
             data_dict_df = data_dict_df[cols]
-            data_dict_df = self.convert_string_cols_to_json(
+            data_dict_df = self._convert_string_cols_to_json(
                 data_dict_df, ["Valid Values"]
             )
             df_store.append(data_dict_df)
 
         merged_attributes_df = pd.concat(df_store, join="outer")
         cols = [
             "Attribute",
```

### Comparing `schematicpy-24.2.1/schematic/visualization/commands.py` & `schematicpy-24.4.1/schematic/visualization/commands.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 # pylint: disable=unused-argument
 # pylint: disable=useless-return
 # pylint: disable=unused-variable
 # pylint: disable=logging-fstring-interpolation
 
 import logging
 import sys
-from typing import Any
+from typing import Any, get_args, cast
 
 import click
 import click_log  # type: ignore
 
 from schematic.visualization.attributes_explorer import AttributesExplorer
-from schematic.visualization.tangled_tree import TangledTree
+from schematic.visualization.tangled_tree import TangledTree, FigureType, TextType
 from schematic.utils.cli_utils import log_value_from_config, query_dict
 from schematic.utils.schema_utils import DisplayLabelType
 from schematic.help import viz_commands
 from schematic.help import model_commands
 from schematic.configuration.configuration import CONFIG
 
 logger = logging.getLogger(__name__)
@@ -55,109 +55,131 @@
     "attributes",
 )
 @click_log.simple_verbosity_option(logger)
 @click.option(
     "--data_model_labels",
     "-dml",
     default="class_label",
-    type=click.Choice(["display_label", "class_label"], case_sensitive=True),
+    type=click.Choice(list(get_args(DisplayLabelType)), case_sensitive=True),
     help=query_dict(
         viz_commands, ("visualization", "tangled_tree", "data_model_labels")
     ),
 )
 @click.pass_obj
 def get_attributes(
     ctx: Any,
-    data_model_labels: DisplayLabelType,
+    data_model_labels: str,
 ) -> None:
     """Gets attributes"""
     # Get JSONLD file path
     path_to_jsonld = CONFIG.model_location
     log_value_from_config("jsonld", path_to_jsonld)
+
+    # Validate inputs are literals
+    assert data_model_labels in get_args(DisplayLabelType)
+    data_model_labels = cast(DisplayLabelType, data_model_labels)
+
     # Run attributes explorer
     AttributesExplorer(path_to_jsonld, data_model_labels).parse_attributes(
         save_file=True
     )
     return
 
 
 @viz.command("tangled_tree_text")
 @click_log.simple_verbosity_option(logger)
 @click.option(
     "-ft",
     "--figure_type",
     required=True,
-    type=click.Choice(["component", "dependency"], case_sensitive=False),
+    type=click.Choice(list(get_args(FigureType)), case_sensitive=False),
     help=query_dict(viz_commands, ("visualization", "tangled_tree", "figure_type")),
 )
 @click.option(
     "-tf",
     "--text_format",
     required=True,
-    type=click.Choice(["plain", "highlighted"], case_sensitive=False),
+    type=click.Choice(list(get_args(TextType)), case_sensitive=False),
     help=query_dict(viz_commands, ("visualization", "tangled_tree", "text_format")),
 )
 @click.option(
     "--data_model_labels",
     "-dml",
     default="class_label",
-    type=click.Choice(["display_label", "class_label"], case_sensitive=True),
+    type=click.Choice(list(get_args(DisplayLabelType)), case_sensitive=True),
     help=query_dict(
         viz_commands, ("visualization", "tangled_tree", "data_model_labels")
     ),
 )
 @click.pass_obj
 def get_tangled_tree_text(
     ctx: Any,
     figure_type: str,
     text_format: str,
-    data_model_labels: DisplayLabelType,
+    data_model_labels: str,
 ) -> None:
     """Get text to be placed on the tangled tree visualization."""
     # Get JSONLD file path
     path_to_jsonld = CONFIG.model_location
     log_value_from_config("jsonld", path_to_jsonld)
 
+    # Validate inputs are literals
+    figure_type = figure_type.lower()
+    text_format = text_format.lower()
+    assert figure_type in get_args(FigureType)
+    assert text_format in get_args(TextType)
+    assert data_model_labels in get_args(DisplayLabelType)
+    figure_type = cast(FigureType, figure_type)
+    text_format = cast(TextType, text_format)
+    data_model_labels = cast(DisplayLabelType, data_model_labels)
+
     # Initialize TangledTree
     tangled_tree = TangledTree(path_to_jsonld, figure_type, data_model_labels)
 
     # Get text for tangled tree.
     text_df = tangled_tree.get_text_for_tangled_tree(text_format, save_file=True)
     return
 
 
 @viz.command("tangled_tree_layers")
 @click_log.simple_verbosity_option(logger)
 @click.option(
     "-ft",
     "--figure_type",
     required=True,
-    type=click.Choice(["component", "dependency"], case_sensitive=False),
+    type=click.Choice(list(get_args(FigureType)), case_sensitive=False),
     help=query_dict(viz_commands, ("visualization", "tangled_tree", "figure_type")),
 )
 @click.option(
     "--data_model_labels",
     "-dml",
     default="class_label",
-    type=click.Choice(["display_label", "class_label"], case_sensitive=True),
+    type=click.Choice(list(get_args(DisplayLabelType)), case_sensitive=True),
     help=query_dict(
         viz_commands, ("visualization", "tangled_tree", "data_model_labels")
     ),
 )
 @click.pass_obj
 def get_tangled_tree_component_layers(
     ctx: Any,
     figure_type: str,
-    data_model_labels: DisplayLabelType,
+    data_model_labels: str,
 ) -> None:
     """Get the components that belong in each layer of the tangled tree visualization."""
     # Get JSONLD file path
     path_to_jsonld = CONFIG.model_location
     log_value_from_config("jsonld", path_to_jsonld)
 
+    # Validate inputs are literal types
+    figure_type = figure_type.lower()
+    assert figure_type in get_args(FigureType)
+    assert data_model_labels in get_args(DisplayLabelType)
+    figure_type = cast(FigureType, figure_type)
+    data_model_labels = cast(DisplayLabelType, data_model_labels)
+
     # Initialize Tangled Tree
     tangled_tree = TangledTree(path_to_jsonld, figure_type, data_model_labels)
 
     # Get tangled trees layers JSON.
     layers = tangled_tree.get_tangled_tree_layers(save_file=True)
 
     return
```

### Comparing `schematicpy-24.2.1/schematic/visualization/tangled_tree.py` & `schematicpy-24.4.1/schematic/visualization/tangled_tree.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,59 @@
 """Tangled tree class"""
 
 # pylint: disable=logging-fstring-interpolation
+# pylint: disable=too-many-lines
 
 from io import StringIO
 import json
 import logging
 import os
 from os import path
-from typing import Optional, Any, Literal
+from typing import Optional, Literal, TypedDict, Union
+from typing_extensions import assert_never
 
 import networkx as nx  # type: ignore
 from networkx.classes.reportviews import NodeView, EdgeDataView  # type: ignore
-import numpy as np
 import pandas as pd
 
 from schematic.visualization.attributes_explorer import AttributesExplorer
 from schematic.schemas.data_model_parser import DataModelParser
 from schematic.schemas.data_model_graph import DataModelGraph, DataModelGraphExplorer
 from schematic.utils.io_utils import load_json
 from schematic.utils.schema_utils import DisplayLabelType
 
 
 logger = logging.getLogger(__name__)
 
+FigureType = Literal["component", "dependency"]
+TextType = Literal["highlighted", "plain"]
+# A list of lists, nodes in layers
+NodeLayers = list[list[str]]
+# A dict where the keys are node names and the values are lists of node names
+NodeDict = dict[str, list[str]]
+# A dict where the keys are node names and the values are the number of a level
+NodeLevelDict = dict[str, int]
+
+
+class Node(TypedDict):
+    """Represents a node and its relationships as a dict"""
+
+    id: str
+    parents: list[str]
+    direct_children: list[str]
+    children: list[str]
+
 
 class TangledTree:  # pylint: disable=too-many-instance-attributes
     """Tangled tree class"""
 
     def __init__(
         self,
         path_to_json_ld: str,
-        figure_type: str,
+        figure_type: FigureType,
         data_model_labels: DisplayLabelType,
     ) -> None:
         # Load jsonld
         self.path_to_json_ld = path_to_json_ld
         self.json_data_model = load_json(self.path_to_json_ld)
 
         # Parse schema name
@@ -48,41 +67,45 @@
         # Parse Model
         parsed_data_model = data_model_parser.parse_model()
 
         # Instantiate DataModelGraph
         data_model_grapher = DataModelGraph(parsed_data_model, data_model_labels)
 
         # Generate graph
-        self.graph_data_model = data_model_grapher.generate_data_model_graph()
+        self.graph_data_model = data_model_grapher.graph
 
         # Instantiate Data Model Graph Explorer
         self.dmge = DataModelGraphExplorer(self.graph_data_model)
 
         # Set Parameters
-        self.figure_type = figure_type.lower()
+        self.figure_type: FigureType = figure_type
         self.dependency_type = "".join(("requires", self.figure_type.capitalize()))
 
         # Get names
         self.schema = load_json(self.path_to_json_ld)
         self.schema_abbr = self.schema_name.split("_")[0]
 
         # Initialize AttributesExplorer
         self.attributes_explorer = AttributesExplorer(
-            self.path_to_json_ld, data_model_labels
+            self.path_to_json_ld,
+            data_model_labels,
+            data_model_grapher=data_model_grapher,
+            data_model_graph_explorer=self.dmge,
+            parsed_data_model=parsed_data_model,
         )
 
         # Create output paths.
         self.text_csv_output_path = self.attributes_explorer.create_output_path(
             "text_csv"
         )
         self.json_output_path = self.attributes_explorer.create_output_path(
             "tangled_tree_json"
         )
 
-    def strip_double_quotes(self, string: str) -> str:
+    def _strip_double_quotes(self, string: str) -> str:
         """Removes double quotes from string
 
         Args:
             string (str): The string to remove quotes from
 
         Returns:
             str: The processed string
@@ -91,15 +114,15 @@
         if string.startswith('"') and string.endswith('"'):
             string = string[1:-1]
         # now remove whitespace
         string = "".join(string.split())
         return string
 
     def get_text_for_tangled_tree(
-        self, text_type: Literal["highlighted", "plain"], save_file: bool = False
+        self, text_type: TextType, save_file: bool = False
     ) -> Optional[str]:
         """
         Gather the text that needs to be either highlighted or plain for the
           tangled tree visualization.
         Args:
             text_type (str): Choices = ['highlighted', 'plain'], determines the type of text
                 rendering to return.
@@ -109,34 +132,38 @@
                save_file==False: Returns plain or highlighted text as a csv string.
         """
         # pylint: disable=too-many-locals
         # Get nodes in the digraph, many more nodes returned if figure type is dependency
         cdg = self.dmge.get_digraph_by_edge_type(self.dependency_type)
         nodes = cdg.nodes()
 
-        if self.dependency_type == "requiresComponent":
+        if self.figure_type == "component":
             component_nodes = nodes
-        else:
+        elif self.figure_type == "dependency":
             # get component nodes if making dependency figure
             component_dg = self.dmge.get_digraph_by_edge_type("requiresComponent")
             component_nodes = component_dg.nodes()
+        else:
+            assert_never(self.figure_type)
 
         # Initialize lists
         highlighted = []
         plain = []
 
         # For each component node in the tangled tree gather the plain and highlighted text.
         for node in component_nodes:
             # Get the highlighted components based on figure_type
             if self.figure_type == "component":
                 highlight_descendants = self.dmge.get_descendants_by_edge_type(
                     node, "requiresComponent"
                 )
             elif self.figure_type == "dependency":
                 highlight_descendants = [node]
+            else:
+                assert_never(self.figure_type)
 
             # Format text to be highlighted and gather text to be formatted plain.
             if not highlight_descendants:
                 # If there are no highlighted descendants just highlight the selected
                 # node (format for observable.)
                 highlighted.append([node, "id", node])
                 # Gather all the text as plain text.
@@ -152,31 +179,31 @@
 
             # Format all the plain text for observable.
             for descendant in plain_descendants:
                 plain.append([node, "id", descendant])
 
         # Prepare df depending on what type of text we need.
         dataframe = pd.DataFrame(
-            locals()[text_type.lower()], columns=["Component", "type", "name"]
+            locals()[text_type], columns=["Component", "type", "name"]
         )
 
         # Depending on input either export csv locally to disk or as a string.
         if save_file:
             file_name = f"{self.schema_abbr}_{self.figure_type}_{text_type}.csv"
             dataframe.to_csv(os.path.join(self.text_csv_output_path, file_name))
             return None
 
         return dataframe.to_csv()
 
-    def get_topological_generations(
+    def _get_topological_generations(
         self,
-    ) -> tuple[list[list], NodeView, EdgeDataView, nx.DiGraph]:
+    ) -> tuple[NodeLayers, NodeView, EdgeDataView, nx.DiGraph]:
         """Gather topological_gen, nodes and edges based on figure type.
         Outputs:
-            topological_gen (List(list)):list of lists. Indicates layers of nodes.
+            topological_gen (NodeLayers):list of lists. Indicates layers of nodes.
             nodes: (Networkx NodeView) Nodes of the component or dependency graph.
               When iterated over it functions like a list.
             edges: (Networkx EdgeDataView) Edges of component or dependency graph.
               When iterated over it works like a list of tuples.
         """
         # Get nodes in the digraph
         digraph = self.dmge.get_digraph_by_edge_type(self.dependency_type)
@@ -191,17 +218,20 @@
             topological_gen = list(reversed(list(nx.topological_generations(subgraph))))
 
         elif self.figure_type == "dependency":
             rev_digraph = nx.DiGraph.reverse(digraph)
             edges = rev_digraph.edges()
             topological_gen = list(nx.topological_generations(subgraph))
 
+        else:
+            assert_never(self.figure_type)
+
         return topological_gen, nodes, edges, subgraph
 
-    def remove_unwanted_characters_from_conditional_statement(
+    def _remove_unwanted_characters_from_conditional_statement(
         self, cond_req: str
     ) -> str:
         """Remove unwanted characters from conditional statement
         Example of conditional requirement: If File Format IS "BAM" OR "CRAM" OR
           "CSV/TSV" then Genome Build is required
         Example output: File Format IS "BAM" OR "CRAM" OR "CSV/TSV"
         """
@@ -209,51 +239,51 @@
             # remove everything after "then"
             cond_req_new = cond_req.split("then")[0]
 
             # remove "If" and empty space
             cond_req = cond_req_new.replace("If", "").lstrip().rstrip()
         return cond_req
 
-    def get_ca_alias(self, conditional_requirements: list) -> dict[str, str]:
+    def _get_ca_alias(self, conditional_requirements: list[str]) -> dict[str, str]:
         """Get the alias for each conditional attribute.
 
         NOTE: Obtaining attributes(attr) and aliases(ali) in this function is specific
           to how formatting is set in AttributesExplorer. If that formatting changes,
           this section will likely break or in the worst case have a silent error.
         Input:
             conditional_requirements_list (list): list of strings of conditional
               requirements from outputs of AttributesExplorer.
         Output:
             ca_alias (dict):
                 key: alias (attribute response)
                 value: attribute
         """
-        ca_alias = {}
+        ca_alias: dict[str, str] = {}
 
         # clean up conditional requirements
         conditional_requirements = [
-            self.remove_unwanted_characters_from_conditional_statement(req)
+            self._remove_unwanted_characters_from_conditional_statement(req)
             for req in conditional_requirements
         ]
 
         for req in conditional_requirements:
             if "OR" not in req:
                 attr, ali = req.split(" is ")
                 attr = "".join(attr.split())
-                ali = self.strip_double_quotes(ali)
+                ali = self._strip_double_quotes(ali)
                 ca_alias[ali] = attr
             else:
                 attr, alias_str = req.split(" is ")
                 alias_lst = alias_str.split(" OR ")
                 for elem in alias_lst:
-                    elem = self.strip_double_quotes(elem)
+                    elem = self._strip_double_quotes(elem)
                     ca_alias[elem] = attr
         return ca_alias
 
-    def gather_component_dependency_info(
+    def _gather_component_dependency_info(
         self, component_name: str, attributes_df: pd.DataFrame
     ) -> tuple[list[str], dict[str, str], list[str]]:
         """Gather all component dependency information.
         Inputs:
             component name: (str) component name
             attributes_df: (Pandas DataFrame) Details for all attributes across all components.
               From AttributesExplorer.
@@ -272,38 +302,38 @@
 
         # Dont want to display `Component` in the figure so remove
         if "Component" in component_attributes:
             component_attributes.remove("Component")
 
         # Gather conditional attributes so they can be added to the figure.
         if "Cond_Req" in attributes_df.columns:
-            conditional_attributes = list(
+            conditional_attributes: list[str] = list(
                 attributes_df[
                     (attributes_df["Cond_Req"])
                     & (attributes_df["Component"] == component_name)
                 ]["Label"]
             )
             conditional_requirements = list(
                 attributes_df[
                     (attributes_df["Cond_Req"])
                     & (attributes_df["Component"] == component_name)
                 ]["Conditional Requirements"]
             )
-            ca_alias = self.get_ca_alias(conditional_requirements)
+            ca_alias = self._get_ca_alias(conditional_requirements)
         else:
             # If there are no conditional attributes/requirements, initialize blank lists.
             conditional_attributes = []
             ca_alias = {}
 
         # Gather a list of all attributes for the current component.
-        all_attributes = list(np.append(component_attributes, conditional_attributes))
+        all_attributes = component_attributes + conditional_attributes
 
         return conditional_attributes, ca_alias, all_attributes
 
-    def find_source_nodes(
+    def _find_source_nodes(
         self,
         nodes: NodeView,
         edges: EdgeDataView,
         all_attributes: Optional[list[str]] = None,
     ) -> list[str]:
         """Find all nodes in the graph that do not have a parent node.
         Inputs:
@@ -333,15 +363,15 @@
                 if node not in not_source and node in all_attributes:
                     source_nodes.append(node)
             else:
                 if node not in not_source:
                     source_nodes.append(node)
         return source_nodes
 
-    def get_parent_child_dictionary(
+    def _get_parent_child_dictionary(
         self, edges: EdgeDataView, all_attributes: Optional[list[str]] = None
     ) -> tuple[dict[str, list[str]], dict[str, list[str]]]:
         """
         Based on the dependency type, create dictionaries between parent and
           child and child and parent attributes.
         Input:
             edges: (Networkx EdgeDataView (component figure) or List(list) (dependency figure))
@@ -356,15 +386,15 @@
                 value: list of the parents children
         """
         # pylint: disable=too-many-branches
         all_attributes_list = [] if all_attributes is None else all_attributes
         child_parents: dict[str, list[str]] = {}
         parent_children: dict[str, list[str]] = {}
 
-        if self.dependency_type == "requiresComponent":
+        if self.figure_type == "component":
             # Construct child_parents dictionary
             for edge in edges:
                 # Add child as a key
                 if edge[0] not in child_parents:
                     child_parents[edge[0]] = []
 
                 # Add parents to list
@@ -375,15 +405,15 @@
                 # Add parent as a key
                 if edge[1] not in parent_children:
                     parent_children[edge[1]] = []
 
                 # Add children to list
                 parent_children[edge[1]].append(edge[0])
 
-        elif self.dependency_type == "requiresDependency":
+        elif self.figure_type == "dependency":
             # Construct child_parents dictionary
             for edge in edges:
                 # Check if child is an attribute for the current component
                 if edge[0] in all_attributes_list:
                     # Add child as a key
                     if edge[0] not in child_parents:
                         child_parents[edge[0]] = []
@@ -400,17 +430,20 @@
                     if edge[1] not in parent_children:
                         parent_children[edge[1]] = []
 
                     # Add child to list if it is an attribute for the current component
                     if edge[0] in all_attributes_list:
                         parent_children[edge[1]].append(edge[0])
 
+        else:
+            assert_never(self.dependency_type)
+
         return child_parents, parent_children
 
-    def alias_edges(self, ca_alias: dict[str, str], edges: EdgeDataView) -> list[list]:
+    def _alias_edges(self, ca_alias: dict[str, str], edges: EdgeDataView) -> NodeLayers:
         """Create new edges based on aliasing between an attribute and its response.
         Purpose:
             Create aliased edges.
             For example:
                 If BiospecimenType (attribute) is AnalyteBiospecimenType (response)
                 Then ShippingConditionType (conditional requirement) is now required.
             In the model the edges that connect these options are:
@@ -423,64 +456,69 @@
         Inputs:
             ca_alias (dict):
                 key: alias (attribute response)
                 value: attribute
             edges (Networkx EdgeDataView): Edges of component or dependency graph.
               When iterated over it works like a list of tuples.
         Output:
-            aliased_edges (list[list]) of aliased edges.
+            aliased_edges (NodeLayers) of aliased edges.
         """
-        aliased_edges = []
+        aliased_edges: NodeLayers = []
         for edge in edges:
             # construct one set of edges at a time
-            edge_set = []
+            edge_set: list[str] = []
+
+            first_edge = edge[0]
+            second_edge = edge[1]
+            assert isinstance(first_edge, str)
+            assert isinstance(second_edge, str)
 
             # If the first edge has an alias add alias to the first
             # position in the current edge set
-            if edge[0] in ca_alias.keys():
-                edge_set.append(ca_alias[edge[0]])
+            if first_edge in ca_alias.keys():
+                edge_set.append(ca_alias[first_edge])
 
             # Else add the non-aliased edge
             else:
-                edge_set.append(edge[0])
+                edge_set.append(first_edge)
 
             # If the second edge has an alias add alias to the first
             # position in the current edge set
-            if edge[1] in ca_alias.keys():
-                edge_set.append(ca_alias[edge[1]])
+            if second_edge in ca_alias.keys():
+                edge_set.append(ca_alias[second_edge])
 
             # Else add the non-aliased edge
             else:
-                edge_set.append(edge[1])
+                edge_set.append(second_edge)
 
             # Add new edge set to a the list of aliased edges.
             aliased_edges.append(edge_set)
 
         return aliased_edges
 
-    def prune_expand_topological_gen(
+    def _prune_expand_topological_gen(
         self,
-        topological_gen: list[list[str]],
+        topological_gen: NodeLayers,
         all_attributes: list[str],
         conditional_attributes: list[str],
-    ) -> list[list[str]]:
+    ) -> NodeLayers:
         """
         Purpose:
             Remake topological_gen with only relevant nodes.
                 This is necessary since for the figure this function is being used in we
                 only want to display a portion of the graph data.
             In addition to only displaying relevant nodes, we want to add conditional
                 attributes to topological_gen so we can visualize them in the tangled tree
                 as well.
         Input:
-            topological_gen (List[list]): Indicates layers of nodes.
-            all_attributes (list): all attributes associated with a particular component.
+            topological_gen (NodeLayers): Indicates layers of nodes.
+            all_attributes (list(str)): all attributes associated with a particular component.
             conditional_attributes (list): List of conditional attributes for a particular component
         Output:
-            new_top_gen (List[list]): mimics structure of topological_gen but only
+            new_top_gen (NodeLayers): mimics structure of topological_gen but only
                 includes the nodes we want
         """
 
         pruned_topological_gen = []
 
         # For each layer(gen) in the topological generation list
         for layer in topological_gen:
@@ -502,52 +540,48 @@
             if current_layer:
                 pruned_topological_gen.append(current_layer)
             if next_layer:
                 pruned_topological_gen.append(next_layer)
 
         return pruned_topological_gen
 
-    def get_base_layers(
+    def _get_base_layers(
         self,
-        topological_gen: list[list],
-        child_parents: dict,
-        source_nodes: list,
+        topological_gen: NodeLayers,
+        child_parents: NodeDict,
+        source_nodes: list[str],
         component_name: str,
-    ) -> tuple[dict[str, Any], dict[str, Any]]:
+    ) -> tuple[NodeLevelDict, NodeLevelDict]:
         """
-        Purpose:
-            Reconfigure topological gen to move things back appropriate layers if
+
+        Reconfigure topological gen to move things back appropriate layers if
             they would have a back reference.
 
-            The Tangle Tree figure requires an acyclic directed graph that has additional
-                layering rules between connected nodes.
-                - If there is a backward connection then the line connecting them will
-                    break (this would suggest a cyclic connection.)
-                - Additionally if two or more nodes are connecting to a downstream node it is
-                    best to put both parent nodes at the same level, if possible, to
-                    prevent line breaks.
-                - Also want to move any children nodes one layer below
-                    the parent node(s). If there are multiple parents, put one layer below the
-                    parent that is furthest from the origin.
+        The Tangle Tree figure requires an acyclic directed graph that has additional
+            layering rules between connected nodes.
+            - If there is a backward connection then the line connecting them will
+                break (this would suggest a cyclic connection.)
+            - Additionally if two or more nodes are connecting to a downstream node it is
+                best to put both parent nodes at the same level, if possible, to
+                prevent line breaks.
+            - Also want to move any children nodes one layer below
+                the parent node(s). If there are multiple parents, put one layer below the
+                parent that is furthest from the origin.
 
-            This is an iterative process that needs to run twice to move all the nodes to their
-            appropriate positions.
-        Input:
-            topological_gen: list of lists. Indicates layers of nodes.
-            child_parents (dict):
-                key: child
-                value: list of the child's parents
-            source_nodes: list, list of nodes that do not have a parent.
-            component_name: str, component name, default=''
-        Output:
-            base_layers: dict, key: component name, value: layer
-                represents initial layering of topological_gen
-            base_layers_copy_copy: dict, key: component name, value: layer
-                represents the final layering after moving the components/attributes to
-                their desired layer.c
+        This is an iterative process that needs to run twice to move all the nodes to their
+        appropriate positions.
+
+        Args:
+            topological_gen (NodeLayers): Indicates layers of nodes.
+            child_parents (NodeDict): The child nodes parents
+            source_nodes (list[str]): list of nodes that do not have a parent.
+            component_name (str): component name
+
+        Returns:
+            tuple[NodeLevelDict, NodeLevelDict]: _description_
         """
         # Convert topological_gen to a dictionary
         base_layers = {com: i for i, lev in enumerate(topological_gen) for com in lev}
 
         # Make another version to iterate on -- Cant set to equal or will overwrite the original.
         base_layers_copy = {
             com: i for i, lev in enumerate(topological_gen) for com in lev
@@ -617,31 +651,33 @@
                     # For each parental position to modify, move the parents level up to
                     # the max_parent_level.
                     for par in modify_par:
                         base_layers_copy_copy[par] = max_parent_level
 
         return base_layers, base_layers_copy_copy
 
-    def adjust_node_placement(
+    def _adjust_node_placement(
         self,
-        base_layers_copy_copy: dict[str, Any],
-        base_layers: dict[str, Any],
-        topological_gen: list[list],
-    ) -> list[list]:
-        """Reorder nodes within topological_generations to match how they were ordered in
-         base_layers_copy_copy
-        Input:
-            topological_gen: list of lists. Indicates layers of nodes.
-            base_layers: dict, key: component name, value: layer
-                represents initial layering of topological_gen
-            base_layers_copy_copy: dict, key: component name, value: layer
-                represents the final layering after moving the components/attributes to
-                their desired layer.
-        Output:
-            topological_gen: same format but as the incoming topological_gen but
+        base_layers_copy_copy: NodeLevelDict,
+        base_layers: NodeLevelDict,
+        topological_gen: NodeLayers,
+    ) -> NodeLayers:
+        """
+
+        Reorder nodes within topological_generations to match how they were ordered in
+          base_layers_copy_copy
+
+        Args:
+            base_layers_copy_copy (NodeLevelDict): represents the final layering after moving
+              the components/attributes to their desired layer.
+            base_layers (NodeLevelDict): represents initial layering of topological_gen
+            topological_gen (NodeLayers): Indicates layers of nodes.
+
+        Returns:
+            NodeLayers: same format but as the incoming topological_gen but
                 ordered to match base_layers_copy_copy.
         """
         if self.figure_type == "component":
             # For each node get its new layer in the tangled tree
             for node, i in base_layers_copy_copy.items():
                 # Check if node is not already in the proper layer
                 if node not in topological_gen[i]:
@@ -665,63 +701,68 @@
                 # Else, check if node is not already in the proper layer
                 elif node not in topological_gen[i]:
                     # If not put it in the appropriate layer
                     topological_gen[i].append(node)
 
                     # Remove from inappropriate layer.
                     topological_gen[base_layers[node]].remove(node)
+
+        else:
+            assert_never(self.figure_type)
+
         return topological_gen
 
-    def move_source_nodes_to_bottom_of_layer(
-        self, node_layers: list[list], source_nodes: list
-    ) -> list[list]:
+    def _move_source_nodes_to_bottom_of_layer(
+        self, node_layers: NodeLayers, source_nodes: list[str]
+    ) -> NodeLayers:
         """For aesthetic purposes move source nodes to the bottom of their respective layers.
         Input:
-            node_layers (List(list)): Lists of lists of each layer and the nodes contained
+            node_layers (NodeLayers): Lists of lists of each layer and the nodes contained
               in that layer as strings.
-            source_nodes (list): list of nodes that do not have a parent.
+            source_nodes (list[str]): list of nodes that do not have a parent.
         Output:
-            node_layers (List(list)): modified to move source nodes to the bottom of each layer.
+            node_layers (NodeLayers): modified to move source nodes to the bottom of each layer.
         """
         for layer in node_layers:
             nodes_to_move = []
             for node in layer:
                 if node in source_nodes:
                     nodes_to_move.append(node)
             for node in nodes_to_move:
                 layer.remove(node)
                 layer.append(node)
         return node_layers
 
-    def get_layers_dict_list(
+    def _get_layers_dict_list(
         self,
-        node_layers: list[list],
-        child_parents: dict,
-        parent_children: dict,
-        all_parent_children: dict,
-    ) -> list[list[dict[str, list[str]]]]:
+        node_layers: NodeLayers,
+        child_parents: NodeDict,
+        parent_children: NodeDict,
+        all_parent_children: NodeDict,
+    ) -> list[list[Node]]:
         """Convert node_layers to a list of lists of dictionaries that specifies each node and
          its parents (if applicable).
-        Inputs:
-            node_layers: list of lists of each layer and the nodes contained in that layer
-              as strings.
-            child_parents (dict):
-                key: child
-                value: list of the child's parents
-            parent_children (dict):
-                key: parent
-                value: list of the parents children
-        Outputs:
-            layers_list (List(list): list of lists of dictionaries that specifies each node and its
+
+        Args:
+            node_layers (NodeLayers): list of lists of each layer and the nodes contained in
+              that layer as strings.
+            child_parents (NodeDict):
+              key: child
+              value: list of the child's parents
+            parent_children (NodeDict):
+              key: parent
+              value: list of the parents children
+            all_parent_children (NodeDict): _description_
+
+        Returns:
+            list[list[Node]]: list of lists of dictionaries that specifies each node and its
              parents (if applicable)
         """
         num_layers = len(node_layers)
-        layers_list: list[list[dict[str, list[str]]]] = [
-            [] for i in range(0, num_layers)
-        ]
+        layers_list: list[list[Node]] = [[] for _ in range(0, num_layers)]
         for i, layer in enumerate(node_layers):
             for node in layer:
                 if node in child_parents.keys():
                     parents = child_parents[node]
                 else:
                     parents = []
 
@@ -730,33 +771,32 @@
                 else:
                     direct_children = []
 
                 if node in all_parent_children.keys():
                     all_children = all_parent_children[node]
                 else:
                     all_children = []
-                layers_list[i].append(
-                    {
-                        "id": node,
-                        "parents": parents,
-                        "direct_children": direct_children,
-                        "children": all_children,
-                    }
-                )
+                node_dict: Node = {
+                    "id": node,
+                    "parents": parents,
+                    "direct_children": direct_children,
+                    "children": all_children,
+                }
+                layers_list[i].append(node_dict)
 
         return layers_list
 
-    def get_node_layers_json(  # pylint: disable=too-many-arguments
+    def _get_node_layers_json(  # pylint: disable=too-many-arguments
         self,
-        topological_gen: list[list],
+        topological_gen: NodeLayers,
         source_nodes: list[str],
-        child_parents: dict,
-        parent_children: dict,
+        child_parents: NodeDict,
+        parent_children: NodeDict,
         component_name: str = "",
-        all_parent_children: Optional[dict] = None,
+        all_parent_children: Optional[NodeDict] = None,
     ) -> str:
         """Return all the layers of a single tangled tree as a JSON String.
         Inputs:
             topological_gen:list of lists. Indicates layers of nodes.
             source_nodes: list of nodes that do not have a parent.
             child_parents (dict):
                 key: child
@@ -768,62 +808,64 @@
                 key: parent
                 value: list of the parents children (including all downstream nodes).
                   Default to an empty dictionary
         Outputs:
             layers_json (JSON String): Layers of nodes in the tangled tree as a json string.
         """
 
-        base_layers, base_layers_copy_copy = self.get_base_layers(
+        base_layers, base_layers_copy_copy = self._get_base_layers(
             topological_gen, child_parents, source_nodes, component_name
         )
 
         # Rearrange node_layers to follow the pattern laid out in component layers.
-        node_layers = self.adjust_node_placement(
+        node_layers = self._adjust_node_placement(
             base_layers_copy_copy, base_layers, topological_gen
         )
 
         # Move source nodes to the bottom of each layer.
-        node_layers = self.move_source_nodes_to_bottom_of_layer(
+        node_layers = self._move_source_nodes_to_bottom_of_layer(
             node_layers, source_nodes
         )
 
         # Convert layers to a list of dictionaries
         if not all_parent_children:
             # default to an empty dictionary
             all_parent_children = {}
 
-        layers_dicts = self.get_layers_dict_list(
+        layers_dicts = self._get_layers_dict_list(
             node_layers, child_parents, parent_children, all_parent_children
         )
 
         # Convert dictionary to a JSON string
         layers_json = json.dumps(layers_dicts)
 
         return layers_json
 
-    def save_outputs(
+    def _save_outputs(
         self,
         save_file: bool,
-        layers_json,
+        layers_json: str,
         component_name: str = "",
         all_layers: Optional[list[str]] = None,
-    ) -> list[str]:
+    ) -> Union[str, list[str]]:
         """
-        Inputs:
-            save_file (bool): Indicates whether to save a file locally or not.:
-            layers_json (JSON String): Layers of nodes in the tangled tree as a json string.
-            component_name (str): component name, default=''
-            all_layers (list of json strings): Each string represents contains the layers for
-                a single tangled tree. If a dependency figure the list is added to each time
-                this function is called, so starts incomplete. default=[].
-        Outputs:
-            all_layers (list of json strings):
-                If save_file == False: Each string represents contains the layers for a single
-                 tangled tree.
-                If save_file ==True: is an empty list.
+        Args:
+            save_file (bool): Indicates whether to save a file locally or not.
+            layers_json (str): Layers of nodes in the tangled tree as a json string.
+            component_name (str, optional): component name. Defaults to "".
+            all_layers (Optional[list[str]], optional):
+                Each string represents contains the layers for a single tangled tree. If a
+                dependency figure the list is added to each time this function is called,
+                so starts incomplete. Defaults to None.
+
+        Returns:
+            Union[str, list[str]]:
+                If save_file == False: [list[str]], Each string represents contains the layers
+                  for a single tangled tree.
+                If save_file == True: str, the layers_json is returned
         """
         all_layers_list = [] if all_layers is None else all_layers
         if save_file:
             if component_name:
                 output_file_name = (
                     f"{self.schema_abbr}_{self.figure_type}_"
                     f"{component_name}_tangled_tree.json"
@@ -841,20 +883,21 @@
 
             logger.info(
                 (
                     "Tangled Tree JSON String saved to "
                     f"{os.path.join(self.json_output_path, output_file_name)}"
                 )
             )
-            all_layers_list = layers_json
+            result: Union[str, list[str]] = layers_json
         else:
-            all_layers_list.append(layers_json)
-        return all_layers_list
+            result = all_layers_list
+            result.append(layers_json)
+        return result
 
-    def get_ancestors_nodes(
+    def _get_ancestors_nodes(
         self, subgraph: nx.DiGraph, components: list[str]
     ) -> dict[str, list[str]]:
         """
         Inputs:
             subgraph: networkX graph object
             components: a list of nodes
         outputs:
@@ -866,106 +909,112 @@
             all_ancestors = self.dmge.get_nodes_ancestors(
                 subgraph=subgraph, node_label=component
             )
             all_parent_children[component] = all_ancestors
 
         return all_parent_children
 
-    def get_tangled_tree_layers(self, save_file: bool = True):
-        """Based on user indicated figure type, construct the layers of nodes of a tangled tree.
-        Inputs:
-            save_file (bool): Indicates whether to save a file locally or not.
-        Outputs:
-            all_layers (list of json strings):
-                If save_file == False: Each string represents contains the layers
-                  for a single tangled tree.
-                If save_file ==True: is an empty list.
+    def get_tangled_tree_layers(self, save_file: bool = True) -> Union[str, list[str]]:
+        """
+
+        Based on user indicated figure type, construct the layers of nodes of a tangled tree.
 
         Note on Dependency Tangled Tree:
             If there are many conditional requirements associated with a dependency, and those
             conditional requirements have overlapping attributes associated with them
             the tangled tree will only report one
 
+        Args:
+            save_file (bool, optional):
+             Indicates whether to save a file locally or not.
+             Defaults to True.
+
+        Returns:
+            Union[str, list[str]]:
+                If save_file == False: [list[str]], Each string represents contains the layers
+                  for a single tangled tree.
+                If save_file == True: str, the layers_json is returned
         """
         # pylint: disable=too-many-locals
         # Gather the data model's, topological generations, nodes and edges
-        topological_gen, nodes, edges, subgraph = self.get_topological_generations()
+        topological_gen, nodes, edges, subgraph = self._get_topological_generations()
 
         if self.figure_type == "component":
             # Gather all source nodes
-            source_nodes = self.find_source_nodes(nodes, edges)
+            source_nodes = self._find_source_nodes(nodes, edges)
 
             # Map all children to their parents and vice versa
-            child_parents, parent_children = self.get_parent_child_dictionary(
+            child_parents, parent_children = self._get_parent_child_dictionary(
                 edges=edges
             )
 
             # find all the downstream nodes
-            all_parent_children = self.get_ancestors_nodes(
-                subgraph, parent_children.keys()
+            all_parent_children = self._get_ancestors_nodes(
+                subgraph, list(parent_children.keys())
             )
 
             # Get the layers that each node belongs to.
-            layers_json = self.get_node_layers_json(
+            layers_json = self._get_node_layers_json(
                 topological_gen,
                 source_nodes,
                 child_parents,
                 parent_children,
                 all_parent_children=all_parent_children,
             )
 
             # If indicated save outputs locally else gather all layers.
-            all_layers = self.save_outputs(save_file, layers_json)
+            all_layers = self._save_outputs(save_file, layers_json)
 
-        if self.figure_type == "dependency":
+        elif self.figure_type == "dependency":
             # Get component digraph and nodes.
             component_dg = self.dmge.get_digraph_by_edge_type("requiresComponent")
             component_nodes = component_dg.nodes()
 
             # Get table of attributes.
             attributes_csv_str = self.attributes_explorer.parse_attributes(
                 save_file=False
             )
             attributes_df = pd.read_table(StringIO(attributes_csv_str), sep=",")
 
-            all_layers = []
             for component_name in component_nodes:
                 # Gather attribute and dependency information per node
                 (
                     conditional_attributes,
                     ca_alias,
                     all_attributes,
-                ) = self.gather_component_dependency_info(component_name, attributes_df)
+                ) = self._gather_component_dependency_info(
+                    component_name, attributes_df
+                )
 
                 # Gather all source nodes
-                source_nodes = self.find_source_nodes(
+                source_nodes = self._find_source_nodes(
                     component_nodes, edges, all_attributes
                 )
 
                 # Alias the conditional requirement edge back to its actual parent label,
                 # then apply aliasing back to the edges
-                aliased_edges = self.alias_edges(ca_alias, edges)
+                aliased_edges = self._alias_edges(ca_alias, edges)
 
                 # Gather relationships between children and their parents.
-                child_parents, parent_children = self.get_parent_child_dictionary(
+                child_parents, parent_children = self._get_parent_child_dictionary(
                     aliased_edges, all_attributes
                 )
 
                 # Remake topological_gen so it has only relevant nodes.
-                pruned_topological_gen = self.prune_expand_topological_gen(
+                pruned_topological_gen = self._prune_expand_topological_gen(
                     topological_gen, all_attributes, conditional_attributes
                 )
 
                 # Get the layers that each node belongs to.
-                layers_json = self.get_node_layers_json(
+                layers_json = self._get_node_layers_json(
                     pruned_topological_gen,
                     source_nodes,
                     child_parents,
                     parent_children,
                     component_name,
                 )
 
                 # If indicated save outputs locally else, gather all layers.
-                all_layers = self.save_outputs(
-                    save_file, layers_json, component_name, all_layers
-                )
+                all_layers = self._save_outputs(save_file, layers_json, component_name)
+        else:
+            assert_never(self.figure_type)
         return all_layers
```

### Comparing `schematicpy-24.2.1/setup.py` & `schematicpy-24.4.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,16 +12,15 @@
  'schematic.visualization']
 
 package_data = \
 {'': ['*'],
  'schematic': ['etc/*', 'etc/data_models/*', 'etc/validation_schemas/*']}
 
 install_requires = \
-['MarkupSafe==2.1.0',
- 'PyYAML>=6.0.0,<7.0.0',
+['PyYAML>=6.0.0,<7.0.0',
  'click-log>=0.4.0,<0.5.0',
  'click>=8.0.0,<9.0.0',
  'dataclasses-json>=0.6.1,<0.7.0',
  'dateparser>=1.1.4,<2.0.0',
  'google-api-python-client>=2.0.0,<3.0.0',
  'google-auth-httplib2>=0.1.0,<0.2.0',
  'google-auth-oauthlib>=0.8.0,<0.9.0',
@@ -34,40 +33,40 @@
  'numpy>=1.21.1,<2.0.0',
  'oauth2client>=4.1.0,<5.0.0',
  'openpyxl>=3.0.9,<4.0.0',
  'pandarallel>=1.6.4,<2.0.0',
  'pandas>=2.0.0,<3.0.0',
  'pdoc>=12.2.0,<13.0.0',
  'pygsheets>=2.0.4,<3.0.0',
- 'pyopenssl>=23.0.0,<24.0.0',
  'rdflib>=6.0.0,<7.0.0',
- 'schematic-db[synapse]==0.0.34',
+ 'schematic-db[synapse]==0.0.41',
  'setuptools>=66.0.0,<67.0.0',
  'sphinx-click>=4.0.0,<5.0.0',
- 'synapseclient>=3.2.0,<4.0.0',
+ 'synapseclient>=4.1.0,<5.0.0',
  'tenacity>=8.0.1,<9.0.0',
  'toml>=0.10.2,<0.11.0',
  'typing-extensions<4.6.0']
 
 extras_require = \
 {':python_version < "3.9"': ['backports.zoneinfo>=0.2.1,<0.3.0'],
- 'api': ['connexion[swagger-ui]>=2.8.0,<3.0.0',
-         'Flask>=2.0.0,<3.0.0',
+ 'api': ['pyopenssl>=23.0.0,<24.0.0',
+         'connexion[swagger-ui]>=2.8.0,<3.0.0',
+         'Flask==2.1.3',
          'Flask-Cors>=3.0.10,<4.0.0',
          'Jinja2>2.11.3'],
  'aws': ['uWSGI>=2.0.21,<3.0.0']}
 
 entry_points = \
 {'console_scripts': ['schematic = schematic.__main__:main']}
 
 setup_kwargs = {
     'name': 'schematicpy',
-    'version': '24.2.1',
+    'version': '24.4.1',
     'description': 'Package for biomedical data model and metadata ingress management',
-    'long_description': '# Schematic\n[![Build Status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2FSage-Bionetworks%2Fschematic%2Fbadge%3Fref%3Ddevelop&style=flat)](https://actions-badge.atrox.dev/Sage-Bionetworks/schematic/goto?ref=develop) [![Documentation Status](https://readthedocs.org/projects/sage-schematic/badge/?version=develop)](https://sage-schematic.readthedocs.io/en/develop/?badge=develop) [![PyPI version](https://badge.fury.io/py/schematicpy.svg)](https://badge.fury.io/py/schematicpy)\n\n# Table of contents\n- [Introduction](#introduction)\n- [Installation](#installation)\n  - [Installation Requirements](#installation-requirements)\n  - [Installation guide for data curator app](#installation-guide-for-data-curator-app)\n  - [Installation guide for developers/contributors](#installation-guide-for-developerscontributors)\n- [Other Contribution Guidelines](#other-contribution-guidelines)\n    - [Update readthedocs documentation](#update-readthedocs-documentation)\n- [Command Line Usage](#command-line-usage)\n- [Testing](#testing)\n  - [Updating Synapse test resources](#updating-synapse-test-resources)\n- [Code Style](#code-style)\n- [Contributors](#contributors)\n\n# Introduction\nSCHEMATIC is an acronym for _Schema Engine for Manifest Ingress and Curation_. The Python based infrastructure provides a _novel_ schema-based, metadata ingress ecosystem, that is meant to streamline the process of biomedical dataset annotation, metadata validation and submission to a data repository for various data contributors.\n\n# Installation\n## Installation Requirements\n* Python version 3.9.0≤x<3.11.0 \n\nNote: You need to be a registered and certified user on [`synapse.org`](https://www.synapse.org/), and also have the right permissions to download the Google credentials files from Synapse.\n\n\n## Installation guide for data curator app\n\nCreate and activate a virtual environment within which you can install the package:\n\n```\npython3 -m venv .venv\nsource .venv/bin/activate\n```\n\nNote: Python 3 has a built-in support for virtual environment [venv](https://docs.python.org/3/library/venv.html#module-venv) so you no longer need to install virtualenv.\n\nInstall and update the package using [pip](https://pip.pypa.io/en/stable/quickstart/):\n\n```\npython3 -m pip install schematicpy\n```\n\nIf you run into error: Failed building wheel for numpy, the error might be able to resolve by upgrading pip. Please try to upgrade pip by:\n\n```\npip3 install --upgrade pip\n```\n\n## Installation guide for developers/contributors \n\nWhen contributing to this repository, please first discuss the change you wish to make via issue, email, or any other method with the owners of this repository before making a change.\n\nPlease note we have a [code of conduct](CODE_OF_CONDUCT.md), please follow it in all your interactions with the project.\n\n### Development environment setup\n1. Clone the `schematic` package repository.\n```\ngit clone https://github.com/Sage-Bionetworks/schematic.git\n```\n2. Install `poetry` (version 1.3.0 or later) using either the [official installer](https://python-poetry.org/docs/#installing-with-the-official-installer) or [pipx](https://python-poetry.org/docs/#installing-with-pipx). If you have an older installation of Poetry, we recommend uninstalling it first. \n\n3. Start the virtual environment by doing: \n```\npoetry shell\n```\n4. Install the dependencies by doing: \n```\npoetry install\n```\nThis command will install the dependencies based on what we specify in poetry.lock. If this step is taking a long time, try to go back to step 2 and check your version of poetry. Alternatively, you could also try deleting the lock file and regenerate it by doing `poetry install` (Please note this method should be used as a last resort because this would force other developers to change their development environment)\n\nIf you want to install the API you will need to install those dependencies as well:\n\n```\npoetry install --extras "api"\n```\n\nIf you want to install the uwsgi:\n\n```\npoetry install --extras "api"\n```\n\n5. Fill in credential files: \n*Note*: If you won\'t interact with Synapse, please ignore this section.\n\nThere are two main configuration files that need to be edited:\nconfig.yml\nand [synapseConfig](https://raw.githubusercontent.com/Sage-Bionetworks/synapsePythonClient/v2.3.0-rc/synapseclient/.synapseConfig)\n\n<strong>Configure .synapseConfig File</strong>\n\nDownload a copy of the ``.synapseConfig`` file, open the file in the\neditor of your choice and edit the `username` and `authtoken` attribute under the `authentication` section \n\n*Note*: You could also visit [configparser](https://docs.python.org/3/library/configparser.html#module-configparser>) doc to see the format that `.synapseConfig` must have. For instance:\n>[authentication]<br> username = ABC <br> authtoken = abc\n\n<strong>Configure config.yml File</strong>\n\nThere are some defaults in schematic that can be configured. These fields are in ``config_example.yml``:\n\n```text\n\n# This is an example config for Schematic.\n# All listed values are those that are the default if a config is not used.\n# Save this as config.yml, this will be gitignored.\n# Remove any fields in the config you don\'t want to change\n# Change the values of any fields you do want to change\n\n\n# This describes where assets such as manifests are stored\nasset_store:\n  # This is when assets are stored in a synapse project\n  synapse:\n    # Synapse ID of the file view listing all project data assets.\n    master_fileview_id: "syn23643253"\n    # Path to the synapse config file, either absolute or relative to this file\n    config: ".synapseConfig"\n    # Base name that manifest files will be saved as\n    manifest_basename: "synapse_storage_manifest"\n\n# This describes information about manifests as it relates to generation and validation\nmanifest:\n  # Location where manifests will saved to\n  manifest_folder: "manifests"\n  # Title or title prefix given to generated manifest(s)\n  title: "example"\n  # Data types of manifests to be generated or data type (singular) to validate manifest against\n  data_type:\n    - "Biospecimen"\n    - "Patient"\n\n# Describes the location of your schema\nmodel:\n  # Location of your schema jsonld, it must be a path relative to this file or absolute\n  location: "tests/data/example.model.jsonld"\n\n# This section is for using google sheets with Schematic\ngoogle_sheets:\n  # The Synapse id of the Google service account credentials.\n  service_acct_creds_synapse_id: "syn25171627"\n  # Path to the synapse config file, either absolute or relative to this file\n  service_acct_creds: "schematic_service_account_creds.json"\n  # When doing google sheet validation (regex match) with the validation rules.\n  #   true is alerting the user and not allowing entry of bad values.\n  #   false is warning but allowing the entry on to the sheet.\n  strict_validation: true\n```\n\nIf you want to change any of these copy ``config_example.yml`` to ``config.yml``, change any fields you want to, and remove any fields you don\'t.\n\nFor example if you wanted to change the folder where manifests are downloaded your config should look like:\n\n```text\n\nmanifest:\n  manifest_folder: "my_manifest_folder_path"\n```\n\n_Note_: `config.yml` is ignored by git.\n\n_Note_: Paths can be specified relative to the `config.yml` file or as absolute paths.\n\n6. Login to Synapse by using the command line\nOn the CLI in your virtual environment, run the following command: \n```\nsynapse login -u <synapse username> -p <synapse password> --rememberMe\n```\nPlease make sure that you run the command before running `schematic init` below\n\n7. Obtain Google credential Files\nTo obtain  ``schematic_service_account_creds.json``, please run: \n```\nschematic init --config ~/path/to/config.yml\n```\n> As v22.12.1 version of schematic, using `token` mode of authentication (in other words, using `token.pickle` and `credentials.json`) is no longer supported due to Google\'s decision to move away from using OAuth out-of-band (OOB) flow. Click [here](https://developers.google.com/identity/protocols/oauth2/resources/oob-migration) to learn more. \n\n*Notes*: Use the ``schematic_service_account_creds.json`` file for the service\naccount mode of authentication (*for Google services/APIs*). Service accounts \nare special Google accounts that can be used by applications to access Google APIs \nprogrammatically via OAuth2.0, with the advantage being that they do not require \nhuman authorization. \n\n*Background*: schematic uses Google’s API to generate google sheet templates that users fill in to provide (meta)data.\nMost Google sheet functionality could be authenticated with service account. However, more complex Google sheet functionality\nrequires token-based authentication. As browser support that requires the token-based authentication diminishes, we are hoping to deprecate\ntoken-based authentication and keep only service account authentication in the future. \n\n\n### Development process instruction\n\nFor new features, bugs, enhancements\n\n1. Pull the latest code from [develop branch in the upstream repo](https://github.com/Sage-Bionetworks/schematic)\n2. Checkout a new branch develop-<feature/fix-name> from the develop branch\n3. Do development on branch develop-<feature/fix-name>\n   a. may need to ensure that schematic poetry toml and lock files are compatible with your local environment\n4. Add changed files for tracking and commit changes using [best practices](https://www.perforce.com/blog/vcs/git-best-practices-git-commit)\n5. Have granular commits: not “too many” file changes, and not hundreds of code lines of changes\n6. Commits with work in progress are encouraged:\n   a. add WIP to the beginning of the commit message for “Work In Progress” commits\n7. Keep commit messages descriptive but less than a page long, see best practices\n8. Push code to develop-<feature/fix-name> in upstream repo\n9. Branch out off develop-<feature/fix-name> if needed to work on multiple features associated with the same code base\n10. After feature work is complete and before creating a PR to the develop branch in upstream\n    a. ensure that code runs locally\n    b. test for logical correctness locally\n    c. wait for git workflow to complete (e.g. tests are run) on github\n11. Create a PR from develop-<feature/fix-name> into the develop branch of the upstream repo\n12. Request a code review on the PR\n13. Once code is approved merge in the develop branch\n14. Delete the develop-<feature/fix-name> branch\n\n*Note*: Make sure you have the latest version of the `develop` branch on your local machine.\n\n## Installation Guide - Docker \n\n1. Install docker from https://www.docker.com/ . <br>\n2.  Identify docker image of interest from [Schematic DockerHub](https://hub.docker.com/r/sagebionetworks/schematic/tags) <br>\n    Ex `docker pull sagebionetworks/schematic:latest` from the CLI or, run `docker compose up` after cloning the schematic github repo <br>\n    in this case, `sagebionetworks/schematic:latest` is the name of the image chosen\n3. Run Schematic Command with `docker run <flags> <schematic command and args>`. <br>\n<t> - For more information on flags for `docker run` and what they do, visit the [Docker Documentation](https://docs.docker.com/engine/reference/commandline/run/) <br>\n<t> - These example commands assume that you have navigated to the directory you want to run schematic from. To specify your working directory, use `$(pwd)` on MacOS/Linux or `%cd%` on Windows.  <br>\n<t> - If not using the latest image, then the full name should be specified: ie `sagebionetworks/schematic:commit-e611e4a` <br>\n<t> - If using local image created by `docker compose up`, then the docker image name should be changed: i.e. `schematic_schematic` <br>\n<t> - Using the `--name` flag sets the name of the container running locally on your machine <br>\n\n### Example For REST API <br>\n\n#### Use file path of `config.yml` to run API endpoints: \n```\ndocker run --rm -p 3001:3001 \\\n  -v $(pwd):/schematic -w /schematic --name schematic \\\n  -e SCHEMATIC_CONFIG=/schematic/config.yml \\\n  -e GE_HOME=/usr/src/app/great_expectations/ \\\n  sagebionetworks/schematic \\\n  python /usr/src/app/run_api.py\n``` \n\n#### Use content of `config.yml` and `schematic_service_account_creds.json`as an environment variable to run API endpoints: \n1. save content of `config.yml` as to environment variable `SCHEMATIC_CONFIG_CONTENT` by doing: `export SCHEMATIC_CONFIG_CONTENT=$(cat /path/to/config.yml)`\n\n2. Similarly, save the content of `schematic_service_account_creds.json` as `SERVICE_ACCOUNT_CREDS` by doing: `export SERVICE_ACCOUNT_CREDS=$(cat /path/to/schematic_service_account_creds.json)`\n\n3. Pass `SCHEMATIC_CONFIG_CONTENT` and `schematic_service_account_creds` as environment variables by using `docker run`\n\n```\ndocker run --rm -p 3001:3001 \\\n  -v $(pwd):/schematic -w /schematic --name schematic \\\n  -e GE_HOME=/usr/src/app/great_expectations/ \\\n  -e SCHEMATIC_CONFIG_CONTENT=$SCHEMATIC_CONFIG_CONTENT \\\n  -e SERVICE_ACCOUNT_CREDS=$SERVICE_ACCOUNT_CREDS \\\n  sagebionetworks/schematic \\\n  python /usr/src/app/run_api.py\n``` \n\n\n### Example For Schematic on mac/linux <br>\nTo run example below, first clone schematic into your home directory  `git clone https://github.com/sage-bionetworks/schematic ~/schematic` <br>\nThen update .synapseConfig with your credentials\n```\ndocker run \\\n  -v ~/schematic:/schematic \\\n  -w /schematic \\\n  -e SCHEMATIC_CONFIG=/schematic/config.yml \\\n  -e GE_HOME=/usr/src/app/great_expectations/ \\\n  sagebionetworks/schematic schematic model \\\n  -c /schematic/config.yml validate \\\n  -mp /schematic/tests/data/mock_manifests/Valid_Test_Manifest.csv \\\n  -dt MockComponent \\\n  -js /schematic/tests/data/example.model.jsonld\n``` \n\n### Example For Schematic on Windows <br>\n```\ndocker run -v %cd%:/schematic \\\n  -w /schematic \\\n  -e GE_HOME=/usr/src/app/great_expectations/ \\\n  sagebionetworks/schematic \\\n  schematic model \\\n  -c config.yml validate -mp tests/data/mock_manifests/inValid_Test_Manifest.csv -dt MockComponent -js /schematic/data/example.model.jsonld\n```\n\n# Other Contribution Guidelines\n## Updating readthedocs documentation\n1. `cd docs`\n2. After making relevant changes, you could run the `make html` command to re-generate the `build` folder.\n3. Please contact the dev team to publish your updates\n\n*Other helpful resources*:\n\n1. [Getting started with Sphinx](https://haha.readthedocs.io/en/latest/intro/getting-started-with-sphinx.html)\n2. [Installing Sphinx](https://haha.readthedocs.io/en/latest/intro/getting-started-with-sphinx.html)\n\n## Update toml file and lock file\nIf you install external libraries by using `poetry add <name of library>`, please make sure that you include `pyproject.toml` and `poetry.lock` file in your commit.\n\n## Reporting bugs or feature requests\nYou can **create bug and feature requests** through [Sage Bionetwork\'s FAIR Data service desk](https://sagebionetworks.jira.com/servicedesk/customer/portal/5/group/8). Providing enough details to the developers to verify and troubleshoot your issue is paramount:\n- **Provide a clear and descriptive title as well as a concise summary** of the issue to identify the problem.\n- **Describe the exact steps which reproduce the problem** in as many details as possible.\n- **Describe the behavior you observed after following the steps** and point out what exactly is the problem with that behavior.\n- **Explain which behavior you expected to see** instead and why.\n- **Provide screenshots of the expected or actual behaviour** where applicable.\n\n# Command Line Usage\nPlease visit more documentation [here](https://sage-schematic.readthedocs.io/en/develop/cli_reference.html)\n\n\n\n# Testing \n\nAll code added to the client must have tests. The Python client uses pytest to run tests. The test code is located in the [tests](https://github.com/Sage-Bionetworks/schematic/tree/develop-docs-update/tests) subdirectory.\n\nYou can run the test suite in the following way:\n\n```\npytest -vs tests/\n```\n\n## Updating Synapse test resources\n\n1. Duplicate the entity being updated (or folder if applicable).\n2. Edit the duplicates (_e.g._ annotations, contents, name).\n3. Update the test suite in your branch to use these duplicates, including the expected values in the test assertions.\n4. Open a PR as per the usual process (see above).\n5. Once the PR is merged, leave the original copies on Synapse to maintain support for feature branches that were forked from `develop` before your update.\n   - If the old copies are problematic and need to be removed immediately (_e.g._ contain sensitive data), proceed with the deletion and alert the other contributors that they need to merge the latest `develop` branch into their feature branches for their tests to work.\n\n# Code style\n\n* Please consult the [Google Python style guide](http://google.github.io/styleguide/pyguide.html) prior to contributing code to this project.\n* Be consistent and follow existing code conventions and spirit.\n\n\n# Contributors\n\nMain contributors and developers:\n\n- [Milen Nikolov](https://github.com/milen-sage)\n- [Mialy DeFelice](https://github.com/mialy-defelice)\n- [Sujay Patil](https://github.com/sujaypatil96)\n- [Bruno Grande](https://github.com/BrunoGrandePhD)\n- [Robert Allaway](https://github.com/allaway)\n- [Gianna Jordan](https://github.com/giajordan)\n- [Lingling Peng](https://github.com/linglp)\n',
+    'long_description': '# Schematic\n[![Build Status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2FSage-Bionetworks%2Fschematic%2Fbadge%3Fref%3Ddevelop&style=flat)](https://actions-badge.atrox.dev/Sage-Bionetworks/schematic/goto?ref=develop) [![Documentation Status](https://readthedocs.org/projects/sage-schematic/badge/?version=develop)](https://sage-schematic.readthedocs.io/en/develop/?badge=develop) [![PyPI version](https://badge.fury.io/py/schematicpy.svg)](https://badge.fury.io/py/schematicpy)\n\n# Table of contents\n- [Introduction](#introduction)\n- [Installation](#installation)\n  - [Installation Requirements](#installation-requirements)\n  - [Installation guide for data curator app](#installation-guide-for-data-curator-app)\n  - [Installation guide for developers/contributors](#installation-guide-for-developerscontributors)\n- [Other Contribution Guidelines](#other-contribution-guidelines)\n    - [Update readthedocs documentation](#update-readthedocs-documentation)\n- [Command Line Usage](#command-line-usage)\n- [Testing](#testing)\n  - [Updating Synapse test resources](#updating-synapse-test-resources)\n- [Code Style](#code-style)\n- [Contributors](#contributors)\n\n# Introduction\nSCHEMATIC is an acronym for _Schema Engine for Manifest Ingress and Curation_. The Python based infrastructure provides a _novel_ schema-based, metadata ingress ecosystem, that is meant to streamline the process of biomedical dataset annotation, metadata validation and submission to a data repository for various data contributors.\n\n# Installation\n## Installation Requirements\n* Python version 3.9.0≤x<3.11.0\n* You need to be a registered and certified user on [`synapse.org`](https://www.synapse.org/)\n\nNote: Our credential policy for Google credentials in order to create Google sheet files from Schematic, see tutorial [\'HERE\'](https://scribehow.com/shared/Get_Credentials_for_Google_Drive_and_Google_Sheets_APIs_to_use_with_schematicpy__yqfcJz_rQVeyTcg0KQCINA). If you plan to use `config.yml`, please ensure that the path of `schematic_service_account_creds.json` is indicated there (see `google_sheets > service_account_creds` section)\n\n\n## Installation guide for data curator app\n\nCreate and activate a virtual environment within which you can install the package:\n\n```\npython3 -m venv .venv\nsource .venv/bin/activate\n```\n\nNote: Python 3 has a built-in support for virtual environment [venv](https://docs.python.org/3/library/venv.html#module-venv) so you no longer need to install virtualenv.\n\nInstall and update the package using [pip](https://pip.pypa.io/en/stable/quickstart/):\n\n```\npython3 -m pip install schematicpy\n```\n\nIf you run into error: Failed building wheel for numpy, the error might be able to resolve by upgrading pip. Please try to upgrade pip by:\n\n```\npip3 install --upgrade pip\n```\n\n## Installation guide for developers/contributors \n\nWhen contributing to this repository, please first discuss the change you wish to make via issue, email, or any other method with the owners of this repository before making a change.\n\nPlease note we have a [code of conduct](CODE_OF_CONDUCT.md), please follow it in all your interactions with the project.\n\n### Development environment setup\n1. Clone the `schematic` package repository.\n```\ngit clone https://github.com/Sage-Bionetworks/schematic.git\n```\n2. Install `poetry` (version 1.3.0 or later) using either the [official installer](https://python-poetry.org/docs/#installing-with-the-official-installer) or [pipx](https://python-poetry.org/docs/#installing-with-pipx). If you have an older installation of Poetry, we recommend uninstalling it first. \n\n3. Start the virtual environment by doing: \n```\npoetry shell\n```\n4. Install the dependencies by doing: \n```\npoetry install\n```\nThis command will install the dependencies based on what we specify in poetry.lock. If this step is taking a long time, try to go back to step 2 and check your version of poetry. Alternatively, you could also try deleting the lock file and regenerate it by doing `poetry install` (Please note this method should be used as a last resort because this would force other developers to change their development environment)\n\nIf you want to install the API you will need to install those dependencies as well:\n\n```\npoetry install --extras "api"\n```\n\nIf you want to install the uwsgi:\n\n```\npoetry install --extras "api"\n```\n\n5. Fill in credential files: \n*Note*: If you won\'t interact with Synapse, please ignore this section.\n\nThere are two main configuration files that need to be edited:\nconfig.yml\nand [synapseConfig](https://raw.githubusercontent.com/Sage-Bionetworks/synapsePythonClient/v2.3.0-rc/synapseclient/.synapseConfig)\n\n<strong>Configure .synapseConfig File</strong>\n\nDownload a copy of the ``.synapseConfig`` file, open the file in the\neditor of your choice and edit the `username` and `authtoken` attribute under the `authentication` section \n\n*Note*: You could also visit [configparser](https://docs.python.org/3/library/configparser.html#module-configparser>) doc to see the format that `.synapseConfig` must have. For instance:\n>[authentication]<br> username = ABC <br> authtoken = abc\n\n<strong>Configure config.yml File</strong>\n\nThere are some defaults in schematic that can be configured. These fields are in ``config_example.yml``:\n\n```text\n\n# This is an example config for Schematic.\n# All listed values are those that are the default if a config is not used.\n# Save this as config.yml, this will be gitignored.\n# Remove any fields in the config you don\'t want to change\n# Change the values of any fields you do want to change\n\n\n# This describes where assets such as manifests are stored\nasset_store:\n  # This is when assets are stored in a synapse project\n  synapse:\n    # Synapse ID of the file view listing all project data assets.\n    master_fileview_id: "syn23643253"\n    # Path to the synapse config file, either absolute or relative to this file\n    config: ".synapseConfig"\n    # Base name that manifest files will be saved as\n    manifest_basename: "synapse_storage_manifest"\n\n# This describes information about manifests as it relates to generation and validation\nmanifest:\n  # Location where manifests will saved to\n  manifest_folder: "manifests"\n  # Title or title prefix given to generated manifest(s)\n  title: "example"\n  # Data types of manifests to be generated or data type (singular) to validate manifest against\n  data_type:\n    - "Biospecimen"\n    - "Patient"\n\n# Describes the location of your schema\nmodel:\n  # Location of your schema jsonld, it must be a path relative to this file or absolute\n  location: "tests/data/example.model.jsonld"\n\n# This section is for using google sheets with Schematic\ngoogle_sheets:\n  # The Synapse id of the Google service account credentials.\n  service_acct_creds_synapse_id: "syn25171627"\n  # Path to the synapse config file, either absolute or relative to this file\n  service_acct_creds: "schematic_service_account_creds.json"\n  # When doing google sheet validation (regex match) with the validation rules.\n  #   true is alerting the user and not allowing entry of bad values.\n  #   false is warning but allowing the entry on to the sheet.\n  strict_validation: true\n```\n\nIf you want to change any of these copy ``config_example.yml`` to ``config.yml``, change any fields you want to, and remove any fields you don\'t.\n\nFor example if you wanted to change the folder where manifests are downloaded your config should look like:\n\n```text\n\nmanifest:\n  manifest_folder: "my_manifest_folder_path"\n```\n\n_Note_: `config.yml` is ignored by git.\n\n_Note_: Paths can be specified relative to the `config.yml` file or as absolute paths.\n\n6. Login to Synapse by using the command line\nOn the CLI in your virtual environment, run the following command: \n```\nsynapse login -u <synapse username> -p <synapse password> --rememberMe\n```\n\n7. Obtain Google credential Files\nRunning `schematic init` is no longer supported due to security concerns. To obtain  `schematic_service_account_creds.json`, please follow the instructions [here](https://scribehow.com/shared/Enable_Google_Drive_and_Google_Sheets_APIs_for_project__yqfcJz_rQVeyTcg0KQCINA). \n\n> As v22.12.1 version of schematic, using `token` mode of authentication (in other words, using `token.pickle` and `credentials.json`) is no longer supported due to Google\'s decision to move away from using OAuth out-of-band (OOB) flow. Click [here](https://developers.google.com/identity/protocols/oauth2/resources/oob-migration) to learn more. \n\n*Notes*: Use the ``schematic_service_account_creds.json`` file for the service\naccount mode of authentication (*for Google services/APIs*). Service accounts \nare special Google accounts that can be used by applications to access Google APIs \nprogrammatically via OAuth2.0, with the advantage being that they do not require \nhuman authorization. \n\n*Background*: schematic uses Google’s API to generate google sheet templates that users fill in to provide (meta)data.\nMost Google sheet functionality could be authenticated with service account. However, more complex Google sheet functionality\nrequires token-based authentication. As browser support that requires the token-based authentication diminishes, we are hoping to deprecate\ntoken-based authentication and keep only service account authentication in the future. \n\n8. Set up pre-commit hooks\n\nThis repository is configured to utilize pre-commit hooks as part of the development process. To enable these hooks, please run the following command and look for the following success message:\n```\n$ pre-commit install\npre-commit installed at .git/hooks/pre-commit\n```\n\n### Development process instruction\n\nFor new features, bugs, enhancements\n\n1. Pull the latest code from [develop branch in the upstream repo](https://github.com/Sage-Bionetworks/schematic)\n2. Checkout a new branch develop-<feature/fix-name> from the develop branch\n3. Do development on branch develop-<feature/fix-name>\n   a. may need to ensure that schematic poetry toml and lock files are compatible with your local environment\n4. Add changed files for tracking and commit changes using [best practices](https://www.perforce.com/blog/vcs/git-best-practices-git-commit)\n5. Have granular commits: not “too many” file changes, and not hundreds of code lines of changes\n6. Commits with work in progress are encouraged:\n   a. add WIP to the beginning of the commit message for “Work In Progress” commits\n7. Keep commit messages descriptive but less than a page long, see best practices\n8. Push code to develop-<feature/fix-name> in upstream repo\n9. Branch out off develop-<feature/fix-name> if needed to work on multiple features associated with the same code base\n10. After feature work is complete and before creating a PR to the develop branch in upstream\n    a. ensure that code runs locally\n    b. test for logical correctness locally\n    c. wait for git workflow to complete (e.g. tests are run) on github\n11. Create a PR from develop-<feature/fix-name> into the develop branch of the upstream repo\n12. Request a code review on the PR\n13. Once code is approved merge in the develop branch\n14. Delete the develop-<feature/fix-name> branch\n\n*Note*: Make sure you have the latest version of the `develop` branch on your local machine.\n\n## Installation Guide - Docker \n\n1. Install docker from https://www.docker.com/ . <br>\n2.  Identify docker image of interest from [Schematic DockerHub](https://hub.docker.com/r/sagebionetworks/schematic/tags) <br>\n    Ex `docker pull sagebionetworks/schematic:latest` from the CLI or, run `docker compose up` after cloning the schematic github repo <br>\n    in this case, `sagebionetworks/schematic:latest` is the name of the image chosen\n3. Run Schematic Command with `docker run <flags> <schematic command and args>`. <br>\n<t> - For more information on flags for `docker run` and what they do, visit the [Docker Documentation](https://docs.docker.com/engine/reference/commandline/run/) <br>\n<t> - These example commands assume that you have navigated to the directory you want to run schematic from. To specify your working directory, use `$(pwd)` on MacOS/Linux or `%cd%` on Windows.  <br>\n<t> - If not using the latest image, then the full name should be specified: ie `sagebionetworks/schematic:commit-e611e4a` <br>\n<t> - If using local image created by `docker compose up`, then the docker image name should be changed: i.e. `schematic_schematic` <br>\n<t> - Using the `--name` flag sets the name of the container running locally on your machine <br>\n\n### Example For REST API <br>\n\n#### Use file path of `config.yml` to run API endpoints: \n```\ndocker run --rm -p 3001:3001 \\\n  -v $(pwd):/schematic -w /schematic --name schematic \\\n  -e SCHEMATIC_CONFIG=/schematic/config.yml \\\n  -e GE_HOME=/usr/src/app/great_expectations/ \\\n  sagebionetworks/schematic \\\n  python /usr/src/app/run_api.py\n``` \n\n#### Use content of `config.yml` and `schematic_service_account_creds.json`as an environment variable to run API endpoints: \n1. save content of `config.yml` as to environment variable `SCHEMATIC_CONFIG_CONTENT` by doing: `export SCHEMATIC_CONFIG_CONTENT=$(cat /path/to/config.yml)`\n\n2. Similarly, save the content of `schematic_service_account_creds.json` as `SERVICE_ACCOUNT_CREDS` by doing: `export SERVICE_ACCOUNT_CREDS=$(cat /path/to/schematic_service_account_creds.json)`\n\n3. Pass `SCHEMATIC_CONFIG_CONTENT` and `schematic_service_account_creds` as environment variables by using `docker run`\n\n```\ndocker run --rm -p 3001:3001 \\\n  -v $(pwd):/schematic -w /schematic --name schematic \\\n  -e GE_HOME=/usr/src/app/great_expectations/ \\\n  -e SCHEMATIC_CONFIG_CONTENT=$SCHEMATIC_CONFIG_CONTENT \\\n  -e SERVICE_ACCOUNT_CREDS=$SERVICE_ACCOUNT_CREDS \\\n  sagebionetworks/schematic \\\n  python /usr/src/app/run_api.py\n``` \n\n\n### Example For Schematic on mac/linux <br>\nTo run example below, first clone schematic into your home directory  `git clone https://github.com/sage-bionetworks/schematic ~/schematic` <br>\nThen update .synapseConfig with your credentials\n```\ndocker run \\\n  -v ~/schematic:/schematic \\\n  -w /schematic \\\n  -e SCHEMATIC_CONFIG=/schematic/config.yml \\\n  -e GE_HOME=/usr/src/app/great_expectations/ \\\n  sagebionetworks/schematic schematic model \\\n  -c /schematic/config.yml validate \\\n  -mp /schematic/tests/data/mock_manifests/Valid_Test_Manifest.csv \\\n  -dt MockComponent \\\n  -js /schematic/tests/data/example.model.jsonld\n``` \n\n### Example For Schematic on Windows <br>\n```\ndocker run -v %cd%:/schematic \\\n  -w /schematic \\\n  -e GE_HOME=/usr/src/app/great_expectations/ \\\n  sagebionetworks/schematic \\\n  schematic model \\\n  -c config.yml validate -mp tests/data/mock_manifests/inValid_Test_Manifest.csv -dt MockComponent -js /schematic/data/example.model.jsonld\n```\n\n# Other Contribution Guidelines\n## Updating readthedocs documentation\n1. `cd docs`\n2. After making relevant changes, you could run the `make html` command to re-generate the `build` folder.\n3. Please contact the dev team to publish your updates\n\n*Other helpful resources*:\n\n1. [Getting started with Sphinx](https://haha.readthedocs.io/en/latest/intro/getting-started-with-sphinx.html)\n2. [Installing Sphinx](https://haha.readthedocs.io/en/latest/intro/getting-started-with-sphinx.html)\n\n## Update toml file and lock file\nIf you install external libraries by using `poetry add <name of library>`, please make sure that you include `pyproject.toml` and `poetry.lock` file in your commit.\n\n## Reporting bugs or feature requests\nYou can **create bug and feature requests** through [Sage Bionetwork\'s FAIR Data service desk](https://sagebionetworks.jira.com/servicedesk/customer/portal/5/group/8). Providing enough details to the developers to verify and troubleshoot your issue is paramount:\n- **Provide a clear and descriptive title as well as a concise summary** of the issue to identify the problem.\n- **Describe the exact steps which reproduce the problem** in as many details as possible.\n- **Describe the behavior you observed after following the steps** and point out what exactly is the problem with that behavior.\n- **Explain which behavior you expected to see** instead and why.\n- **Provide screenshots of the expected or actual behaviour** where applicable.\n\n# Command Line Usage\nPlease visit more documentation [here](https://sage-schematic.readthedocs.io/en/develop/cli_reference.html)\n\n\n\n# Testing \n\nAll code added to the client must have tests. The Python client uses pytest to run tests. The test code is located in the [tests](https://github.com/Sage-Bionetworks/schematic/tree/develop-docs-update/tests) subdirectory.\n\nYou can run the test suite in the following way:\n\n```\npytest -vs tests/\n```\n\n## Updating Synapse test resources\n\n1. Duplicate the entity being updated (or folder if applicable).\n2. Edit the duplicates (_e.g._ annotations, contents, name).\n3. Update the test suite in your branch to use these duplicates, including the expected values in the test assertions.\n4. Open a PR as per the usual process (see above).\n5. Once the PR is merged, leave the original copies on Synapse to maintain support for feature branches that were forked from `develop` before your update.\n   - If the old copies are problematic and need to be removed immediately (_e.g._ contain sensitive data), proceed with the deletion and alert the other contributors that they need to merge the latest `develop` branch into their feature branches for their tests to work.\n\n# Code style\n\n* Please consult the [Google Python style guide](http://google.github.io/styleguide/pyguide.html) prior to contributing code to this project.\n* Be consistent and follow existing code conventions and spirit.\n\n\n# Contributors\n\nMain contributors and developers:\n\n- [Milen Nikolov](https://github.com/milen-sage)\n- [Mialy DeFelice](https://github.com/mialy-defelice)\n- [Sujay Patil](https://github.com/sujaypatil96)\n- [Bruno Grande](https://github.com/BrunoGrandePhD)\n- [Robert Allaway](https://github.com/allaway)\n- [Gianna Jordan](https://github.com/giajordan)\n- [Lingling Peng](https://github.com/linglp)\n',
     'author': 'Milen Nikolov',
     'author_email': 'milen.nikolov@sagebase.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/Sage-Bionetworks/schematic',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `schematicpy-24.2.1/PKG-INFO` & `schematicpy-24.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schematicpy
-Version: 24.2.1
+Version: 24.4.1
 Summary: Package for biomedical data model and metadata ingress management
 Home-page: https://github.com/Sage-Bionetworks/schematic
 Keywords: schema,metadata,validation,data model,linked data
 Author: Milen Nikolov
 Author-email: milen.nikolov@sagebase.org
 Requires-Python: >=3.9.0,<3.11
 Classifier: Development Status :: 4 - Beta
@@ -12,18 +12,17 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: api
 Provides-Extra: aws
-Requires-Dist: Flask (>=2.0.0,<3.0.0) ; extra == "api"
+Requires-Dist: Flask (==2.1.3) ; extra == "api"
 Requires-Dist: Flask-Cors (>=3.0.10,<4.0.0) ; extra == "api"
 Requires-Dist: Jinja2 (>2.11.3) ; extra == "api"
-Requires-Dist: MarkupSafe (==2.1.0)
 Requires-Dist: PyYAML (>=6.0.0,<7.0.0)
 Requires-Dist: backports.zoneinfo (>=0.2.1,<0.3.0) ; python_version < "3.9"
 Requires-Dist: click (>=8.0.0,<9.0.0)
 Requires-Dist: click-log (>=0.4.0,<0.5.0)
 Requires-Dist: connexion[swagger-ui] (>=2.8.0,<3.0.0) ; extra == "api"
 Requires-Dist: dataclasses-json (>=0.6.1,<0.7.0)
 Requires-Dist: dateparser (>=1.1.4,<2.0.0)
@@ -39,20 +38,20 @@
 Requires-Dist: numpy (>=1.21.1,<2.0.0)
 Requires-Dist: oauth2client (>=4.1.0,<5.0.0)
 Requires-Dist: openpyxl (>=3.0.9,<4.0.0)
 Requires-Dist: pandarallel (>=1.6.4,<2.0.0)
 Requires-Dist: pandas (>=2.0.0,<3.0.0)
 Requires-Dist: pdoc (>=12.2.0,<13.0.0)
 Requires-Dist: pygsheets (>=2.0.4,<3.0.0)
-Requires-Dist: pyopenssl (>=23.0.0,<24.0.0)
+Requires-Dist: pyopenssl (>=23.0.0,<24.0.0) ; extra == "api"
 Requires-Dist: rdflib (>=6.0.0,<7.0.0)
-Requires-Dist: schematic-db[synapse] (==0.0.34)
+Requires-Dist: schematic-db[synapse] (==0.0.41)
 Requires-Dist: setuptools (>=66.0.0,<67.0.0)
 Requires-Dist: sphinx-click (>=4.0.0,<5.0.0)
-Requires-Dist: synapseclient (>=3.2.0,<4.0.0)
+Requires-Dist: synapseclient (>=4.1.0,<5.0.0)
 Requires-Dist: tenacity (>=8.0.1,<9.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: typing-extensions (<4.6.0)
 Requires-Dist: uWSGI (>=2.0.21,<3.0.0) ; extra == "aws"
 Project-URL: Documentation, https://github.com/Sage-Bionetworks/schematic
 Project-URL: Repository, https://github.com/Sage-Bionetworks/schematic
 Description-Content-Type: text/markdown
@@ -75,17 +74,18 @@
 - [Contributors](#contributors)
 
 # Introduction
 SCHEMATIC is an acronym for _Schema Engine for Manifest Ingress and Curation_. The Python based infrastructure provides a _novel_ schema-based, metadata ingress ecosystem, that is meant to streamline the process of biomedical dataset annotation, metadata validation and submission to a data repository for various data contributors.
 
 # Installation
 ## Installation Requirements
-* Python version 3.9.0≤x<3.11.0 
+* Python version 3.9.0≤x<3.11.0
+* You need to be a registered and certified user on [`synapse.org`](https://www.synapse.org/)
 
-Note: You need to be a registered and certified user on [`synapse.org`](https://www.synapse.org/), and also have the right permissions to download the Google credentials files from Synapse.
+Note: Our credential policy for Google credentials in order to create Google sheet files from Schematic, see tutorial ['HERE'](https://scribehow.com/shared/Get_Credentials_for_Google_Drive_and_Google_Sheets_APIs_to_use_with_schematicpy__yqfcJz_rQVeyTcg0KQCINA). If you plan to use `config.yml`, please ensure that the path of `schematic_service_account_creds.json` is indicated there (see `google_sheets > service_account_creds` section)
 
 
 ## Installation guide for data curator app
 
 Create and activate a virtual environment within which you can install the package:
 
 ```
@@ -224,34 +224,38 @@
 _Note_: Paths can be specified relative to the `config.yml` file or as absolute paths.
 
 6. Login to Synapse by using the command line
 On the CLI in your virtual environment, run the following command: 
 ```
 synapse login -u <synapse username> -p <synapse password> --rememberMe
 ```
-Please make sure that you run the command before running `schematic init` below
 
 7. Obtain Google credential Files
-To obtain  ``schematic_service_account_creds.json``, please run: 
-```
-schematic init --config ~/path/to/config.yml
-```
+Running `schematic init` is no longer supported due to security concerns. To obtain  `schematic_service_account_creds.json`, please follow the instructions [here](https://scribehow.com/shared/Enable_Google_Drive_and_Google_Sheets_APIs_for_project__yqfcJz_rQVeyTcg0KQCINA). 
+
 > As v22.12.1 version of schematic, using `token` mode of authentication (in other words, using `token.pickle` and `credentials.json`) is no longer supported due to Google's decision to move away from using OAuth out-of-band (OOB) flow. Click [here](https://developers.google.com/identity/protocols/oauth2/resources/oob-migration) to learn more. 
 
 *Notes*: Use the ``schematic_service_account_creds.json`` file for the service
 account mode of authentication (*for Google services/APIs*). Service accounts 
 are special Google accounts that can be used by applications to access Google APIs 
 programmatically via OAuth2.0, with the advantage being that they do not require 
 human authorization. 
 
 *Background*: schematic uses Google’s API to generate google sheet templates that users fill in to provide (meta)data.
 Most Google sheet functionality could be authenticated with service account. However, more complex Google sheet functionality
 requires token-based authentication. As browser support that requires the token-based authentication diminishes, we are hoping to deprecate
 token-based authentication and keep only service account authentication in the future. 
 
+8. Set up pre-commit hooks
+
+This repository is configured to utilize pre-commit hooks as part of the development process. To enable these hooks, please run the following command and look for the following success message:
+```
+$ pre-commit install
+pre-commit installed at .git/hooks/pre-commit
+```
 
 ### Development process instruction
 
 For new features, bugs, enhancements
 
 1. Pull the latest code from [develop branch in the upstream repo](https://github.com/Sage-Bionetworks/schematic)
 2. Checkout a new branch develop-<feature/fix-name> from the develop branch
```

