# Comparing `tmp/eqsolver-0.1.0.tar.gz` & `tmp/eqsolver-0.2.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eqsolver-0.1.0.tar", last modified: Thu Apr 25 03:35:02 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

