# Comparing `tmp/gs_edit-0.2.4.tar.gz` & `tmp/GS_Edit-0.2.5-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gs_edit-0.2.4.tar", last modified: Wed Apr 24 05:21:32 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

