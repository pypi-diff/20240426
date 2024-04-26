# Comparing `tmp/spacepy-0.5.0.tar.gz` & `tmp/spacepy-0.6.0-cp36-cp36m-macosx_10_9_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacepy-0.5.0.tar", last modified: Fri Mar  8 20:58:47 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

