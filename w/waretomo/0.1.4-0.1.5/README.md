# Comparing `tmp/waretomo-0.1.4.tar.gz` & `tmp/waretomo-0.1.5.tar.gz`

## Comparing `waretomo-0.1.4.tar` & `waretomo-0.1.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 waretomo-0.1.4/.cruft.json
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 waretomo-0.1.4/.github_changelog_generator
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 waretomo-0.1.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 waretomo-0.1.4/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 waretomo-0.1.4/.github/TEST_FAIL_TEMPLATE.md
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 waretomo-0.1.4/.github/dependabot.yml
--rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 waretomo-0.1.4/.github/workflows/ci.yml
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 waretomo-0.1.4/src/waretomo/__init__.py
--rw-r--r--   0        0        0     4944 2020-02-02 00:00:00.000000 waretomo-0.1.4/src/waretomo/_aretomo.py
--rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 waretomo-0.1.4/src/waretomo/_fix_mdoc.py
--rw-r--r--   0        0        0     5458 2020-02-02 00:00:00.000000 waretomo-0.1.4/src/waretomo/_parse.py
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 waretomo-0.1.4/src/waretomo/_stack.py
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 waretomo-0.1.4/src/waretomo/_threaded.py
--rw-r--r--   0        0        0     3372 2020-02-02 00:00:00.000000 waretomo-0.1.4/src/waretomo/_topaz.py
--rw-r--r--   0        0        0    12368 2020-02-02 00:00:00.000000 waretomo-0.1.4/src/waretomo/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 waretomo-0.1.4/src/waretomo/py.typed
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 waretomo-0.1.4/tests/test_waretomo.py
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 waretomo-0.1.4/.gitignore
--rw-r--r--   0        0        0    34502 2020-02-02 00:00:00.000000 waretomo-0.1.4/LICENSE
--rw-r--r--   0        0        0     3897 2020-02-02 00:00:00.000000 waretomo-0.1.4/README.md
--rw-r--r--   0        0        0     4122 2020-02-02 00:00:00.000000 waretomo-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     5299 2020-02-02 00:00:00.000000 waretomo-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 waretomo-0.1.5/.cruft.json
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 waretomo-0.1.5/.github_changelog_generator
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 waretomo-0.1.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 waretomo-0.1.5/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 waretomo-0.1.5/.github/TEST_FAIL_TEMPLATE.md
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 waretomo-0.1.5/.github/dependabot.yml
+-rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 waretomo-0.1.5/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 waretomo-0.1.5/src/waretomo/__init__.py
+-rw-r--r--   0        0        0     4944 2020-02-02 00:00:00.000000 waretomo-0.1.5/src/waretomo/_aretomo.py
+-rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 waretomo-0.1.5/src/waretomo/_fix_mdoc.py
+-rw-r--r--   0        0        0     5537 2020-02-02 00:00:00.000000 waretomo-0.1.5/src/waretomo/_parse.py
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 waretomo-0.1.5/src/waretomo/_stack.py
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 waretomo-0.1.5/src/waretomo/_threaded.py
+-rw-r--r--   0        0        0     3380 2020-02-02 00:00:00.000000 waretomo-0.1.5/src/waretomo/_topaz.py
+-rw-r--r--   0        0        0    13009 2020-02-02 00:00:00.000000 waretomo-0.1.5/src/waretomo/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 waretomo-0.1.5/src/waretomo/py.typed
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 waretomo-0.1.5/tests/test_waretomo.py
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 waretomo-0.1.5/.gitignore
+-rw-r--r--   0        0        0    34502 2020-02-02 00:00:00.000000 waretomo-0.1.5/LICENSE
+-rw-r--r--   0        0        0     3897 2020-02-02 00:00:00.000000 waretomo-0.1.5/README.md
+-rw-r--r--   0        0        0     4122 2020-02-02 00:00:00.000000 waretomo-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     5299 2020-02-02 00:00:00.000000 waretomo-0.1.5/PKG-INFO
```

### Comparing `waretomo-0.1.4/.cruft.json` & `waretomo-0.1.5/.cruft.json`

 * *Files identical despite different names*

### Comparing `waretomo-0.1.4/.pre-commit-config.yaml` & `waretomo-0.1.5/.pre-commit-config.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -9,21 +9,21 @@
   # - repo: https://github.com/compilerla/conventional-pre-commit
   #   rev: v2.1.1
   #   hooks:
   #     - id: conventional-pre-commit
   #       stages: [commit-msg]
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.252
+    rev: v0.4.1
     hooks:
       - id: ruff
         args: [--fix]
 
   - repo: https://github.com/psf/black
-    rev: 23.1.0
+    rev: 24.4.1
     hooks:
       - id: black
 
   - repo: https://github.com/abravalheri/validate-pyproject
-    rev: v0.12.1
+    rev: v0.16
     hooks:
       - id: validate-pyproject
```

### Comparing `waretomo-0.1.4/.github/workflows/ci.yml` & `waretomo-0.1.5/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `waretomo-0.1.4/src/waretomo/_aretomo.py` & `waretomo-0.1.5/src/waretomo/_aretomo.py`

 * *Files identical despite different names*

### Comparing `waretomo-0.1.4/src/waretomo/_fix_mdoc.py` & `waretomo-0.1.5/src/waretomo/_fix_mdoc.py`

 * *Files identical despite different names*

### Comparing `waretomo-0.1.4/src/waretomo/_parse.py` & `waretomo-0.1.5/src/waretomo/_parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,23 @@
 from pathlib import Path, PureWindowsPath
 from xml.etree import ElementTree
 
 from mdocfile.data_models import Mdoc
 
 
 def parse_data(
-    progress, warp_dir, mdoc_dir, output_dir, roi_dir, just=(), exclude=(), train=False
+    progress,
+    warp_dir,
+    mdoc_dir,
+    output_dir,
+    roi_dir,
+    just=(),
+    exclude=(),
+    train=False,
+    dose=None,
 ):
     log = logging.getLogger("waretomo")
 
     imod_dir = warp_dir / "imod"
     if not imod_dir.exists():
         raise FileNotFoundError("warp directory does not have an `imod` subdirectory")
 
@@ -30,14 +38,15 @@
     even_dir = warp_dir / "average" / "even"
 
     tilt_series = []
     tilt_series_excluded = []
     tilt_series_unprocessed = []
 
     for mdoc_file in progress.track(mdocs, description="Reading mdocs..."):
+        log.info(f"Parsing {mdoc_file}.")
         mdoc = Mdoc.from_file(mdoc_file)
 
         # warp uses mdoc name in many places, but some times the ts_name is important
         mdoc_name = mdoc_file.stem
         ts_name = mdoc.global_data.ImageFile.stem
         stack = imod_dir / mdoc_name / (mdoc_name + ".st")
 
@@ -106,36 +115,35 @@
             if len(roi_files) == 1:
                 roi_file = roi_files[0]
             else:
                 roi_file = None
         else:
             roi_file = None
 
-        dose = mdoc.section_data[0].ExposureDose
+        dose = mdoc.section_data[0].ExposureDose if dose is None else dose
         if not dose:
             log.error("Exposure dose not present in mdoc! Setting to 0.")
         px_size_raw = mdoc.section_data[0].PixelSpacing
         if not px_size_raw:
             log.error("Pixel spacing not present in mdoc! Setting to 1.")
 
         # aretomo being weird about paths and names splitting needs extra care...
-        ts_stripped = ts_name.split(".")[0]
-        ts_aligned = ts_stripped + "_aligned"
+        ts_aligned = ts_name.split(".")[0] + "_aligned"
         alignment_result_dir = output_dir / (ts_aligned + ".st_Imod")
 
         tilt_series.append(
             {
                 "name": ts_name,
+                "mdoc": mdoc_file,
                 "stack": stack,
                 "rawtlt": stack.with_suffix(".rawtlt"),
-                "aln": output_dir / (ts_stripped + ".aln"),
                 "xf": alignment_result_dir / (ts_aligned + ".xf"),
                 "tlt": alignment_result_dir / (ts_aligned + ".tlt"),
+                "aln": output_dir / (mdoc_name + ".st.aln"),
                 "skipped_tilts": skipped_tilts,
-                "mdoc": mdoc_file,
                 "roi": roi_file,
                 "odd": odd,
                 "even": even,
                 "stack_odd": output_dir / (ts_name + "_odd.st"),
                 "stack_even": output_dir / (ts_name + "_even.st"),
                 "recon_odd": output_dir / "odd" / (ts_name + ".mrc"),
                 "recon_even": output_dir / "even" / (ts_name + ".mrc"),
```

### Comparing `waretomo-0.1.4/src/waretomo/_stack.py` & `waretomo-0.1.5/src/waretomo/_stack.py`

 * *Files identical despite different names*

### Comparing `waretomo-0.1.4/src/waretomo/_threaded.py` & `waretomo-0.1.5/src/waretomo/_threaded.py`

 * *Files identical despite different names*

### Comparing `waretomo-0.1.4/src/waretomo/_topaz.py` & `waretomo-0.1.5/src/waretomo/_topaz.py`

 * *Files 5% similar despite different names*

```diff
@@ -74,17 +74,17 @@
                 progress,
                 task,
                 train_model,
                 even_path=even,
                 odd_path=odd,
                 save_prefix=str(outdir / "trained_models" / model_name),
                 save_interval=10,
-                device=-2
-                if gpus is None
-                else next(iter(gpus)),  # TODO: actually run with multiple gpus?
+                device=(
+                    -2 if gpus is None else next(iter(gpus))
+                ),  # TODO: actually run with multiple gpus?
                 tilesize=patch_size,
                 base_kernel_width=11,
                 num_workers=multiprocessing.cpu_count(),
             )
         else:
             with contextlib.redirect_stdout(std):
                 model = load_model(model_name, base_kernel_width=11)
```

### Comparing `waretomo-0.1.4/src/waretomo/main.py` & `waretomo-0.1.5/src/waretomo/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,20 @@
 )
 @click.option(
     "-d",
     "--dry-run",
     is_flag=True,
     help="only print some info, without running the commands.",
 )
-@click.option("-v", "--verbose", count=True, help="echo all individual commands")
+@click.option(
+    "-v",
+    "--verbose",
+    count=True,
+    help="level of verbosity; can be passed multiple times.",
+)
 @click.option(
     "-j",
     "--just",
     type=str,
     multiple=True,
     help="reconstruct just this tomogram (can be passed multiple times)",
 )
@@ -79,14 +84,19 @@
     "-b",
     "--binning",
     type=int,
     default=4,
     help="binning for aretomo reconstruction (relative to warp pre-processed binning)",
 )
 @click.option(
+    "--dose",
+    type=float,
+    help="exposure dose (e/A^2/tilt_image). If not passed, guess from mdocs.",
+)
+@click.option(
     "-a", "--tilt-axis", type=float, help="starting tilt axis for AreTomo, if any"
 )
 @click.option(
     "-p",
     "--patches",
     type=int,
     help="number of patches for local alignment in aretomo (NxN), if any",
@@ -155,14 +165,15 @@
     dry_run,
     verbose,
     just,
     exclude,
     sample_thickness,
     z_thickness,
     binning,
+    dose,
     tilt_axis,
     patches,
     roi_dir,
     overwrite,
     train,
     topaz_tile_size,
     topaz_patch_size,
@@ -242,14 +253,15 @@
             warp_dir,
             mdoc_dir=mdoc_dir,
             output_dir=output_dir,
             roi_dir=roi_dir,
             just=just,
             exclude=exclude,
             train=train,
+            dose=dose,
         )
 
         aretomo_kwargs = {
             "cmd": aretomo,
             "tilt_axis": tilt_axis,
             "patches": patches,
             "thickness_align": sample_thickness,
@@ -317,15 +329,29 @@
             """
         )
         print(Panel(summary))
 
         ts = tilt_series[0]
         ts_name = ts["name"]
         ts_info = {k: v for k, v in ts.items() if k not in ("even", "odd")}
-        log.info(f'Metadata from tiltseries "{ts_name}": {ts_info}')
+        ts_info = {
+            k: (str(v.relative_to(warp_dir)) if isinstance(v, Path) else v)
+            for k, v in ts_info.items()
+            if k
+        }
+        ts_info.update(ts_info.pop("aretomo_kwargs"))
+        ts_info = "".join(f'{nl}{" " * 12}- {k}: {v}' for k, v in ts_info.items())
+        first_ts_summary = cleandoc(
+            f"""
+            Double check that these values make sense for {ts_name}:
+            {ts_info}
+            """
+        )
+
+        print(Panel(first_ts_summary))
 
         if not dry_run:
             with open(output_dir / "waretomo.log", "a") as f:
                 print("=" * 80, file=f)
                 print(datetime.now().strftime("%d/%m/%Y %H:%M:%S"), file=f)
                 print(f'Command: {" ".join(sys.argv)}', file=f)
                 print(summary, "\n", file=f)
```

### Comparing `waretomo-0.1.4/.gitignore` & `waretomo-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `waretomo-0.1.4/LICENSE` & `waretomo-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `waretomo-0.1.4/README.md` & `waretomo-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `waretomo-0.1.4/pyproject.toml` & `waretomo-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `waretomo-0.1.4/PKG-INFO` & `waretomo-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: waretomo
-Version: 0.1.4
+Version: 0.1.5
 Summary: Overengineered batch processing script for tomography data with Warp and aretomo.
 Project-URL: homepage, https://github.com/brisvag/waretomo
 Project-URL: repository, https://github.com/brisvag/waretomo
 Author-email: Lorenzo Gaifas <brisvag@gmail.com>
 License: GPLv3
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
```

