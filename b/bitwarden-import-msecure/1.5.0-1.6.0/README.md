# Comparing `tmp/bitwarden_import_msecure-1.5.0.tar.gz` & `tmp/bitwarden_import_msecure-1.6.0.tar.gz`

## Comparing `bitwarden_import_msecure-1.5.0.tar` & `bitwarden_import_msecure-1.6.0.tar`

### file list

```diff
@@ -1,47 +1,48 @@
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/.coveragerc
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/.flake8
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/.mypy.ini
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/.pylintrc
--rwxr-xr-x   0        0        0     1340 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/activate.sh
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/invoke.yml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/pytest.ini
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/requirements.dev.in
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/requirements.dev.txt
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/requirements.in
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/requirements.txt
--rw-r--r--   0        0        0     2947 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/tasks.py
--rw-r--r--   0        0        0     3274 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/.github/workflows/docs.yml
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/.github/workflows/pip_publish.yml
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/.github/workflows/static.yml
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/docs/mkdocs.yml
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/docs/src/en/index.md
--rw-r--r--   0        0        0     2778 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/docs/src/ru/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/scripts/__init__.py
--rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/scripts/build-docs.sh
--rwxr-xr-x   0        0        0       91 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/scripts/build.sh
--rwxr-xr-x   0        0        0      420 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/scripts/docs-render-config.sh
--rwxr-xr-x   0        0        0     2243 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/scripts/include_pyproject_requirements.py
--rwxr-xr-x   0        0        0      153 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/scripts/upload.sh
--rwxr-xr-x   0        0        0     2525 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/scripts/verup.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/src/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/src/bitwarden_import_msecure/__about__.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/src/bitwarden_import_msecure/__init__.py
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/src/bitwarden_import_msecure/bitwarden_csv.py
--rw-r--r--   0        0        0     3564 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/src/bitwarden_import_msecure/bitwarden_json.py
--rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/src/bitwarden_import_msecure/main.py
--rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/src/bitwarden_import_msecure/msecure.py
--rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/tests/conftest.py
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/tests/test_bitwarden_import_msecure.py
--rw-r--r--   0        0        0     4638 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/tests/test_e2e.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/tests/resources/bitwarden_export.csv
--rw-r--r--   0        0        0     5032 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/tests/resources/bitwarden_export.json
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/tests/resources/bitwarden_notes_export.csv
--rw-r--r--   0        0        0     5068 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/tests/resources/bitwarden_notes_export.json
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/tests/resources/mSecure Export File.csv
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/LICENSE.txt
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/README.md
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     3219 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/.coveragerc
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/.flake8
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/.mypy.ini
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/.pylintrc
+-rwxr-xr-x   0        0        0     1340 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/activate.sh
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/invoke.yml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/pytest.ini
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/requirements.dev.in
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/requirements.dev.txt
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/requirements.in
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/requirements.txt
+-rw-r--r--   0        0        0     2947 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/tasks.py
+-rw-r--r--   0        0        0     3274 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/.github/workflows/docs.yml
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/.github/workflows/pip_publish.yml
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/.github/workflows/static.yml
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/docs/mkdocs.yml
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/docs/src/en/index.md
+-rw-r--r--   0        0        0     2778 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/docs/src/ru/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/scripts/__init__.py
+-rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/scripts/build-docs.sh
+-rwxr-xr-x   0        0        0       91 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/scripts/build.sh
+-rwxr-xr-x   0        0        0      420 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/scripts/docs-render-config.sh
+-rwxr-xr-x   0        0        0     2243 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/scripts/include_pyproject_requirements.py
+-rwxr-xr-x   0        0        0      153 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/scripts/upload.sh
+-rwxr-xr-x   0        0        0     2525 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/scripts/verup.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/src/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/src/bitwarden_import_msecure/__about__.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/src/bitwarden_import_msecure/__init__.py
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/src/bitwarden_import_msecure/bitwarden_csv.py
+-rw-r--r--   0        0        0     3643 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/src/bitwarden_import_msecure/bitwarden_json.py
+-rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/src/bitwarden_import_msecure/main.py
+-rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/src/bitwarden_import_msecure/msecure.py
+-rw-r--r--   0        0        0     3829 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/src/bitwarden_import_msecure/patch_export.py
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/tests/conftest.py
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/tests/test_bitwarden_import_msecure.py
+-rw-r--r--   0        0        0     4638 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/tests/test_e2e.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/tests/resources/bitwarden_export.csv
+-rw-r--r--   0        0        0     5024 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/tests/resources/bitwarden_export.json
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/tests/resources/bitwarden_notes_export.csv
+-rw-r--r--   0        0        0     5060 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/tests/resources/bitwarden_notes_export.json
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/tests/resources/mSecure Export File.csv
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/LICENSE.txt
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/README.md
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0     3219 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.6.0/PKG-INFO
```

### Comparing `bitwarden_import_msecure-1.5.0/.pre-commit-config.yaml` & `bitwarden_import_msecure-1.6.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.5.0/activate.sh` & `bitwarden_import_msecure-1.6.0/activate.sh`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.5.0/requirements.dev.txt` & `bitwarden_import_msecure-1.6.0/requirements.dev.txt`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.5.0/tasks.py` & `bitwarden_import_msecure-1.6.0/tasks.py`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.5.0/.github/workflows/ci.yml` & `bitwarden_import_msecure-1.6.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.5.0/.github/workflows/docs.yml` & `bitwarden_import_msecure-1.6.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.5.0/.github/workflows/pip_publish.yml` & `bitwarden_import_msecure-1.6.0/.github/workflows/pip_publish.yml`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.5.0/.github/workflows/static.yml` & `bitwarden_import_msecure-1.6.0/.github/workflows/static.yml`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.5.0/docs/mkdocs.yml` & `bitwarden_import_msecure-1.6.0/docs/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.5.0/docs/src/en/index.md` & `bitwarden_import_msecure-1.6.0/docs/src/en/index.md`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.5.0/docs/src/ru/index.md` & `bitwarden_import_msecure-1.6.0/docs/src/ru/index.md`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.5.0/scripts/include_pyproject_requirements.py` & `bitwarden_import_msecure-1.6.0/scripts/include_pyproject_requirements.py`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.5.0/scripts/verup.sh` & `bitwarden_import_msecure-1.6.0/scripts/verup.sh`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.5.0/src/bitwarden_import_msecure/bitwarden_csv.py` & `bitwarden_import_msecure-1.6.0/src/bitwarden_import_msecure/bitwarden_csv.py`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.5.0/src/bitwarden_import_msecure/bitwarden_json.py` & `bitwarden_import_msecure-1.6.0/src/bitwarden_import_msecure/bitwarden_json.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,22 +66,24 @@
             "collectionIds": None,
         }
         if data["type"] == "login":
             item["login"] = {
                 "fido2Credentials": [],
                 "uris": [
                     {
-                        "match": "null",
+                        "match": None,
                         "uri": data["login_uri"],
                     }
                 ],
                 "username": data["login_username"],
                 "password": data["login_password"],
                 "totp": None,
             }
+            if not data["login_uri"]:
+                item["login"]["uris"] = []
         if data["type"] == "card":
             exp_month, exp_year = (
                 data["fields"].pop("Expiration Date", "").split("/") + ["", ""]
             )[:2]
             cardholder_name = data["fields"].pop("Name on Card", "") or data["fields"].pop(
                 "Name", ""
             )
```

### Comparing `bitwarden_import_msecure-1.5.0/src/bitwarden_import_msecure/main.py` & `bitwarden_import_msecure-1.6.0/src/bitwarden_import_msecure/main.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,28 +5,33 @@
 
 import rich_click as click
 
 from bitwarden_import_msecure.bitwarden_csv import BitwardenCsv
 from bitwarden_import_msecure.bitwarden_json import BitwardenJson
 from bitwarden_import_msecure.msecure import import_msecure_row
 from bitwarden_import_msecure.__about__ import __version__
+from bitwarden_import_msecure import patch_export
 
 click.rich_click.USE_MARKDOWN = True
 
 
 OUTPUT_FILE_DEFAULT = "bitwarden"
 NOTES_MODE = "notes"
 
 
 @click.command()
 @click.version_option(version=__version__, prog_name="bitwarden-import-msecure")
-@click.argument("input_file", type=click.Path(exists=True))  # ~/Downloads/mSecure Export File.csv
+@click.argument("input_file", type=click.Path(exists=True), required=False)
 @click.argument("output_file", type=click.Path(), required=False)
 @click.option("--force", is_flag=True, help="Overwrite the output file if it exists.")
 @click.option(
+    "--patch", is_flag=True, help="Fix old exports, see `--patch-help` for more details."
+)
+@click.option("--patch-help", is_flag=True, help="Show help for `--patch` option.")
+@click.option(
     "--extra-fields",
     type=click.Choice(["custom-fields", NOTES_MODE]),
     default="custom-fields",
     help=(
         "How to handle mSecure fields that don't match Bitwarden fields."
         f"By default, they are added as custom fields. Use '{NOTES_MODE}' to add them to notes."
     ),
@@ -34,45 +39,71 @@
 @click.option(
     "--format",
     "output_format",
     type=click.Choice(["csv", "json"]),
     default="json",
     help="Output file format. JSON by default. CSV is legacy format with less features.",
 )
-def bitwarden_import_msecure(
-    input_file: str, output_file: str, force: bool, extra_fields: str, output_format: str
+def bitwarden_import_msecure(  # pylint: disable=too-many-arguments
+    input_file: str,
+    output_file: str,
+    force: bool,
+    patch: bool,
+    extra_fields: str,
+    output_format: str,
+    patch_help: bool,
 ) -> None:
     """
     Converts file `INPUT_FILE` exported from mSecure to Bitwarden compatible format
     to `OUTPUT_FILE`.
 
-     - Export CSV from mSecure
-     - Run this script on the exported CSV file
-     - Import the processed file into Bitwarden
+    - Export CSV from mSecure
+    - Run this script on the exported CSV file
+    - Import the processed file into Bitwarden
     """
+    if patch_help:
+        patch_export.show_help()
+        return
+
+    input_path = Path(input_file)
+    if not input_path.exists():
+        click.echo(f"Input file `{input_path}` does not exist.")
+        raise click.Abort()
+
+    if force and patch:
+        click.echo("--force and --patch cannot be used simultaneously.")
+        raise click.Abort()
+
     output_path = (
         Path(output_file)
         if output_file
-        else Path(input_file).parent / f"{OUTPUT_FILE_DEFAULT}.{output_format}"
+        else input_path.parent / f"{OUTPUT_FILE_DEFAULT}.{output_format}"
     )
-    if output_path.exists() and not force:
-        click.echo(f"Output file {output_path} already exists. Use --force to overwrite.")
-        raise click.Abort()
 
-    if output_format == "csv":
-        writer = BitwardenCsv(output_path)
+    if patch:
+        if not output_path.exists():
+            click.echo(f"Cannot patch `{output_path}` - does not exists.")
+            raise click.Abort()
+        patch_export.patch(input_path, output_path)
     else:
-        writer = BitwardenJson(output_path)
-
-    with open(input_file, newline="", encoding="utf-8") as infile:
-        reader = csv.reader(infile, delimiter=",")
-        for row in reader:
-            if row and not row[0].startswith("mSecure"):
-                data = import_msecure_row(row, extra_fields == NOTES_MODE)
-                writer.write_record(data)
+        if output_path.exists() and not force:
+            click.echo(f"Output file `{output_path}` already exists. Use --force to overwrite.")
+            raise click.Abort()
+
+        if output_format == "csv":
+            writer = BitwardenCsv(output_path)
+        else:
+            writer = BitwardenJson(output_path)
+
+        with input_path.open(newline="", encoding="utf-8") as infile:
+            reader = csv.reader(infile, delimiter=",")
+            for row in reader:
+                if row and not row[0].startswith("mSecure"):
+                    data = import_msecure_row(row, extra_fields == NOTES_MODE)
+                    writer.write_record(data)
 
-    writer.close()
-    click.echo(f"File to import into Bitwarden saved to {output_path}")
+        writer.close()
+    click.echo(f"File to import into Bitwarden saved to `{output_path}`")
 
 
 if __name__ == "__main__":  # pragma: no cover
     bitwarden_import_msecure()  # pylint: disable=no-value-for-parameter
```

### Comparing `bitwarden_import_msecure-1.5.0/src/bitwarden_import_msecure/msecure.py` & `bitwarden_import_msecure-1.6.0/src/bitwarden_import_msecure/msecure.py`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.5.0/tests/conftest.py` & `bitwarden_import_msecure-1.6.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.5.0/tests/test_e2e.py` & `bitwarden_import_msecure-1.6.0/tests/test_e2e.py`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.5.0/tests/resources/bitwarden_export.csv` & `bitwarden_import_msecure-1.6.0/tests/resources/bitwarden_export.csv`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.5.0/tests/resources/bitwarden_export.json` & `bitwarden_import_msecure-1.6.0/tests/resources/bitwarden_export.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998888888888889%*

 * *Differences: {"'items'": "{0: {'login': {'uris': {0: {'match': None}}}}, 1: {'login': {'uris': {0: {'match': "*

 * *            "None}}}}, 2: {'login': {'uris': {0: {'match': None}}}}, 4: {'login': {'uris': {0: "*

 * *            "{'match': None}}}}}"}*

```diff
@@ -17,15 +17,15 @@
             "id": "12345678-1234-5678-1234-567812345678",
             "login": {
                 "fido2Credentials": [],
                 "password": "my-cool-password",
                 "totp": null,
                 "uris": [
                     {
-                        "match": "null",
+                        "match": null,
                         "uri": "https://www.openstreetmap.org"
                     }
                 ],
                 "username": "andrey@sorokin.engineer"
             },
             "name": " OpenStreetMap",
             "notes": "",
@@ -45,15 +45,15 @@
             "id": "12345678-1234-5678-1234-567812345678",
             "login": {
                 "fido2Credentials": [],
                 "password": "",
                 "totp": null,
                 "uris": [
                     {
-                        "match": "null",
+                        "match": null,
                         "uri": "vk.com"
                     }
                 ],
                 "username": "+1 555 555 5555"
             },
             "name": " VK",
             "notes": "",
@@ -73,15 +73,15 @@
             "id": "12345678-1234-5678-1234-567812345678",
             "login": {
                 "fido2Credentials": [],
                 "password": "my-cool-password",
                 "totp": null,
                 "uris": [
                     {
-                        "match": "null",
+                        "match": null,
                         "uri": "https://airtable.com/"
                     }
                 ],
                 "username": "andrey@sorokin.engineer"
             },
             "name": "(deleted) airtable sheets",
             "notes": "",
@@ -132,15 +132,15 @@
             "id": "12345678-1234-5678-1234-567812345678",
             "login": {
                 "fido2Credentials": [],
                 "password": "my-cool-password",
                 "totp": null,
                 "uris": [
                     {
-                        "match": "null",
+                        "match": null,
                         "uri": "hub.docker.com"
                     }
                 ],
                 "username": "sorokin.engineer"
             },
             "name": "Docker hub",
             "notes": "andrey@sorokin.engineer\nBefore 20190429 my-cool-password",
```

### Comparing `bitwarden_import_msecure-1.5.0/tests/resources/bitwarden_notes_export.csv` & `bitwarden_import_msecure-1.6.0/tests/resources/bitwarden_notes_export.csv`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.5.0/tests/resources/bitwarden_notes_export.json` & `bitwarden_import_msecure-1.6.0/tests/resources/bitwarden_notes_export.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998888888888889%*

 * *Differences: {"'items'": "{0: {'login': {'uris': {0: {'match': None}}}}, 1: {'login': {'uris': {0: {'match': "*

 * *            "None}}}}, 2: {'login': {'uris': {0: {'match': None}}}}, 4: {'login': {'uris': {0: "*

 * *            "{'match': None}}}}}"}*

```diff
@@ -17,15 +17,15 @@
             "id": "12345678-1234-5678-1234-567812345678",
             "login": {
                 "fido2Credentials": [],
                 "password": "my-cool-password",
                 "totp": null,
                 "uris": [
                     {
-                        "match": "null",
+                        "match": null,
                         "uri": "https://www.openstreetmap.org"
                     }
                 ],
                 "username": "andrey@sorokin.engineer"
             },
             "name": " OpenStreetMap",
             "notes": "",
@@ -45,15 +45,15 @@
             "id": "12345678-1234-5678-1234-567812345678",
             "login": {
                 "fido2Credentials": [],
                 "password": "",
                 "totp": null,
                 "uris": [
                     {
-                        "match": "null",
+                        "match": null,
                         "uri": "vk.com"
                     }
                 ],
                 "username": "+1 555 555 5555"
             },
             "name": " VK",
             "notes": "",
@@ -73,15 +73,15 @@
             "id": "12345678-1234-5678-1234-567812345678",
             "login": {
                 "fido2Credentials": [],
                 "password": "my-cool-password",
                 "totp": null,
                 "uris": [
                     {
-                        "match": "null",
+                        "match": null,
                         "uri": "https://airtable.com/"
                     }
                 ],
                 "username": "andrey@sorokin.engineer"
             },
             "name": "(deleted) airtable sheets",
             "notes": "",
@@ -132,15 +132,15 @@
             "id": "12345678-1234-5678-1234-567812345678",
             "login": {
                 "fido2Credentials": [],
                 "password": "my-cool-password",
                 "totp": null,
                 "uris": [
                     {
-                        "match": "null",
+                        "match": null,
                         "uri": "hub.docker.com"
                     }
                 ],
                 "username": "sorokin.engineer"
             },
             "name": "Docker hub",
             "notes": "andrey@sorokin.engineer\nBefore 20190429 my-cool-password",
```

### Comparing `bitwarden_import_msecure-1.5.0/tests/resources/mSecure Export File.csv` & `bitwarden_import_msecure-1.6.0/tests/resources/mSecure Export File.csv`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.5.0/LICENSE.txt` & `bitwarden_import_msecure-1.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.5.0/README.md` & `bitwarden_import_msecure-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.5.0/pyproject.toml` & `bitwarden_import_msecure-1.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.5.0/PKG-INFO` & `bitwarden_import_msecure-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bitwarden-import-msecure
-Version: 1.5.0
+Version: 1.6.0
 Summary: Migration from mSecure to Bitwarden
 Project-URL: Homepage, https://andgineer.github.io/bitwarden-import-msecure/
 Project-URL: Documentation, https://andgineer.github.io/bitwarden-import-msecure/
 Author-email: Andrey Sorokin <andrey@sorokin.engineer>
 License: Copyright (c) 2024 Andrey Sorokin <andrey@sorokin.engineer>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_sp8m1_a4_/tmp36y9ge3g_TarContainer/0/46", line 74, column 102: CDATA terminal not found*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: bitwarden-import-msecure Version: 1.5.0 Summary:
+Metadata-Version: 2.3 Name: bitwarden-import-msecure Version: 1.6.0 Summary:
 Migration from mSecure to Bitwarden Project-URL: Homepage, https://
 andgineer.github.io/bitwarden-import-msecure/ Project-URL: Documentation,
 https://andgineer.github.io/bitwarden-import-msecure/ Author-email: Andrey
 Sorokin
 sorokin.engineer> License: Copyright (c) 2024 Andrey Sorokin
 sorokin.engineer> Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
```

