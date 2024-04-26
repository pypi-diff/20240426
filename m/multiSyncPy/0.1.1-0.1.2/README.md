# Comparing `tmp/multiSyncPy-0.1.1.tar.gz` & `tmp/multiSyncPy-0.1.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multiSyncPy-0.1.1.tar", last modified: Thu Jul  6 08:55:24 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

