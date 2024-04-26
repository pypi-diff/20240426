# Comparing `tmp/screenapi_cli-0.1.5a4.tar.gz` & `tmp/screenapi_cli-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "screenapi_cli-0.1.5a4.tar", max compression
+gzip compressed data, was "screenapi_cli-0.1.6.tar", max compression
```

## Comparing `screenapi_cli-0.1.5a4.tar` & `screenapi_cli-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1092 2024-03-23 16:06:49.120124 screenapi_cli-0.1.5a4/LICENSE
--rw-r--r--   0        0        0     1381 2024-03-25 19:41:34.179648 screenapi_cli-0.1.5a4/README.md
--rw-r--r--   0        0        0        0 2024-03-26 06:15:38.237432 screenapi_cli-0.1.5a4/app/__init__.py
--rw-r--r--   0        0        0     9369 2024-04-17 05:58:50.361946 screenapi_cli-0.1.5a4/app/__main__.py
--rw-r--r--   0        0        0     1360 2024-04-01 07:33:03.304661 screenapi_cli-0.1.5a4/app/common.py
--rw-r--r--   0        0        0        0 2024-03-24 18:09:29.678307 screenapi_cli-0.1.5a4/app/export/__init__.py
--rw-r--r--   0        0        0     1689 2024-04-15 17:50:49.954658 screenapi_cli-0.1.5a4/app/export/cli.py
--rw-r--r--   0        0        0        0 2024-03-24 14:33:45.903715 screenapi_cli-0.1.5a4/app/setup/__init__.py
--rw-r--r--   0        0        0     1083 2024-03-25 19:15:41.722738 screenapi_cli-0.1.5a4/app/setup/utils.py
--rw-r--r--   0        0        0       97 2024-03-24 17:32:30.550768 screenapi_cli-0.1.5a4/app/txt/__init__.py
--rw-r--r--   0        0        0     5737 2024-03-29 09:45:40.583647 screenapi_cli-0.1.5a4/app/txt/cli.py
--rw-r--r--   0        0        0     6056 2024-03-25 18:55:58.756247 screenapi_cli-0.1.5a4/app/txt/deprecated_cli.py
--rw-r--r--   0        0        0        0 2024-03-27 04:52:19.596215 screenapi_cli-0.1.5a4/app/xlsx/__init__.py
--rw-r--r--   0        0        0    11650 2024-04-20 11:04:14.938423 screenapi_cli-0.1.5a4/app/xlsx/main.py
--rw-r--r--   0        0        0      795 2024-04-21 17:34:41.710687 screenapi_cli-0.1.5a4/pyproject.toml
--rw-r--r--   0        0        0     2092 1970-01-01 00:00:00.000000 screenapi_cli-0.1.5a4/PKG-INFO
+-rw-r--r--   0        0        0     1092 2024-03-23 16:06:49.120124 screenapi_cli-0.1.6/LICENSE
+-rw-r--r--   0        0        0     1381 2024-03-25 19:41:34.179648 screenapi_cli-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2024-03-26 06:15:38.237432 screenapi_cli-0.1.6/app/__init__.py
+-rw-r--r--   0        0        0     9464 2024-04-25 10:20:05.820380 screenapi_cli-0.1.6/app/__main__.py
+-rw-r--r--   0        0        0     1360 2024-04-01 07:33:03.304661 screenapi_cli-0.1.6/app/common.py
+-rw-r--r--   0        0        0        0 2024-03-24 18:09:29.678307 screenapi_cli-0.1.6/app/export/__init__.py
+-rw-r--r--   0        0        0     1689 2024-04-15 17:50:49.954658 screenapi_cli-0.1.6/app/export/cli.py
+-rw-r--r--   0        0        0        0 2024-03-24 14:33:45.903715 screenapi_cli-0.1.6/app/setup/__init__.py
+-rw-r--r--   0        0        0     1083 2024-03-25 19:15:41.722738 screenapi_cli-0.1.6/app/setup/utils.py
+-rw-r--r--   0        0        0       97 2024-03-24 17:32:30.550768 screenapi_cli-0.1.6/app/txt/__init__.py
+-rw-r--r--   0        0        0     5737 2024-03-29 09:45:40.583647 screenapi_cli-0.1.6/app/txt/cli.py
+-rw-r--r--   0        0        0     6056 2024-03-25 18:55:58.756247 screenapi_cli-0.1.6/app/txt/deprecated_cli.py
+-rw-r--r--   0        0        0        0 2024-03-27 04:52:19.596215 screenapi_cli-0.1.6/app/xlsx/__init__.py
+-rw-r--r--   0        0        0    11640 2024-04-25 12:40:20.712870 screenapi_cli-0.1.6/app/xlsx/main.py
+-rw-r--r--   0        0        0      793 2024-04-26 07:57:46.388956 screenapi_cli-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2090 1970-01-01 00:00:00.000000 screenapi_cli-0.1.6/PKG-INFO
```

### Comparing `screenapi_cli-0.1.5a4/LICENSE` & `screenapi_cli-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `screenapi_cli-0.1.5a4/README.md` & `screenapi_cli-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `screenapi_cli-0.1.5a4/app/__main__.py` & `screenapi_cli-0.1.6/app/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -202,14 +202,15 @@
 ):
     from app.xlsx.main import main
 
     print(f"[bold]Updating sheet from {input_path}[/]")
     print(f"Number of workers: {max_workers}")
     print(f"Overwrite existing data: {overwrite}")
     print(f"Skip saving images: {skip_images}")
+    print(f"Check for `{check}` while checking already parsed data: {check}" if check else "")
 
     main(
         input_path=input_path,
         site=site,
         max_workers=max_workers,
         output_dir=output_dir,
         overwrite=overwrite,
```

### Comparing `screenapi_cli-0.1.5a4/app/common.py` & `screenapi_cli-0.1.6/app/common.py`

 * *Files identical despite different names*

### Comparing `screenapi_cli-0.1.5a4/app/export/cli.py` & `screenapi_cli-0.1.6/app/export/cli.py`

 * *Files identical despite different names*

### Comparing `screenapi_cli-0.1.5a4/app/setup/utils.py` & `screenapi_cli-0.1.6/app/setup/utils.py`

 * *Files identical despite different names*

### Comparing `screenapi_cli-0.1.5a4/app/txt/cli.py` & `screenapi_cli-0.1.6/app/txt/cli.py`

 * *Files identical despite different names*

### Comparing `screenapi_cli-0.1.5a4/app/txt/deprecated_cli.py` & `screenapi_cli-0.1.6/app/txt/deprecated_cli.py`

 * *Files identical despite different names*

### Comparing `screenapi_cli-0.1.5a4/app/xlsx/main.py` & `screenapi_cli-0.1.6/app/xlsx/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -119,19 +119,19 @@
     #             if not bool(
     #                 re.search(r"marketplace|posts|groups|profile", data["url"]),
     #             ):
     #                 data.update({"type": "posts"})
     #     return jsonData
 
     if save:
-        with open(os.path.join(OUTPUT_DIR, "converted.json"), "w") as f:
+        with open(os.path.join(OUTPUT_DIR, "dump"), "w") as f:
             f.write(json.dumps(jsonData, indent=4))
         print(
             "[bold]Converted to json, Saved to: ",
-            os.path.join(OUTPUT_DIR, "converted.json"),
+            os.path.join(OUTPUT_DIR, "dump"),
         )
     return jsonData
 
 
 def convert_to_xlsx(
     input_path: Path,
     output_file: str,
@@ -155,52 +155,47 @@
             continue
         for file in files:
             if file.startswith("converted"):
                 continue
             if file.endswith(".json"):
                 df = process_and_append_data(os.path.join(root, file), df)
 
-    df.drop(columns=["key", "endpoint", "type"], inplace=True)
     df.sort_values(by=sort_by, inplace=True)
-
+    df.drop(columns=["key", "endpoint", "type", "description"], inplace=True)
     df.rename(columns=read_mapping(site.value, swap=True), inplace=True)
-
     df.to_excel(output_file, index=False)
 
 
 def doneIds(output_dir: str, check: Optional[str] = None):
-    ids = []
-    for root, dirs, files in os.walk(output_dir):
-        if root.startswith(("images")):
+    ids = set()
+    ids_to_remove = set()
+    for root, _, files in os.walk(output_dir):
+        if "images" in root.split(os.sep):
             continue
-        for file in files:
-            if file.startswith("converted"):
-                continue
-            if file.endswith(".json"):
-                with open(os.path.join(root, file)) as _f:
-                    d = json.loads(_f.read())
-                    try:
-                        if check:
-                            if d.get(check) in ["", "0", None]:
-                                os.remove(os.path.join(root, file))
-
-                        if d.get("title") in ["", "0"] or d.get("description") in [
-                            "",
-                            "0",
-                        ]:
-                            os.remove(os.path.join(root, file))
-                        else:
-                            ids.append(int(os.path.basename(file).split(".")[0]))
-                    except FileNotFoundError:
-                        continue
-                    except Exception as e:
-                        print(e)
-
-    print("Already done: ", len(ids))
-    return ids
+        for file in filter(lambda x: x.endswith(".json"), files):
+            with open(os.path.join(root, file)) as f:
+                d = json.load(f)
+                if check:
+                    if (
+                        d.get("title") in ["", "0"]
+                        or d.get("description") in ["", "0"]
+                        or d.get(check) in ["", "0"]
+                    ):
+                        ids_to_remove.add(os.path.join(root, file))
+                    else:
+                        ids.add(int(os.path.basename(file).split(".")[0]))
+                else:
+                    if d.get("title") in ["", "0"] or d.get("description") in ["", "0"]:
+                        ids_to_remove.add(os.path.join(root, file))
+                    else:
+                        ids.add(int(os.path.basename(file).split(".")[0]))
+
+    [os.remove(i) for i in ids_to_remove]
+    print(f"Total: {len(ids)}")
+    return list(ids)
 
 
 def request(options: dict[str, Any]):
     client: Client = options["client"]
     skipImages: bool = options["skip_images"]
     taskId: TaskID = options["task_id"]
     progress: Progress = options["progress"]
@@ -359,14 +354,15 @@
     )
 
     print("Done!")
 
 
 if __name__ == "__main__":
     main(
-        input_path=Path("dumps/Redbus_SM_4thApril (1).xlsx"),
-        site=sheetType.social,
+        input_path=Path("dumps/15APR_MZ_PAYALTEAM.xlsx"),
+        site=sheetType.ecom,
         save=True,
-        overwrite=True,
-        skip_images=True,
+        overwrite=False,
+        skip_images=False,
         max_workers=5,
+        check="sellerName",
     )
```

### Comparing `screenapi_cli-0.1.5a4/pyproject.toml` & `screenapi_cli-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "screenapi-cli"
-version = "0.1.5a4"
+version = "0.1.6"
 description = "A cli interface to interact with screenapi"
 authors = ["RONY <iamrony777@pm.me>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "app" },
 ]
```

### Comparing `screenapi_cli-0.1.5a4/PKG-INFO` & `screenapi_cli-0.1.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: screenapi-cli
-Version: 0.1.5a4
+Version: 0.1.6
 Summary: A cli interface to interact with screenapi
 License: MIT
 Author: RONY
 Author-email: iamrony777@pm.me
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

