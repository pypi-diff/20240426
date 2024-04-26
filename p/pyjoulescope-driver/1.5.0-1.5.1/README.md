# Comparing `tmp/pyjoulescope_driver-1.5.0.tar.gz` & `tmp/pyjoulescope_driver-1.5.1-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjoulescope_driver-1.5.0.tar", last modified: Wed Apr 24 20:27:27 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

