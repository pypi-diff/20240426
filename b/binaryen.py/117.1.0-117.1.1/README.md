# Comparing `tmp/binaryen_py-117.1.0.tar.gz` & `tmp/binaryen.py-117.1.1-cp312-cp312-macosx_10_9_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "binaryen_py-117.1.0.tar", last modified: Sun Apr 21 20:33:00 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

