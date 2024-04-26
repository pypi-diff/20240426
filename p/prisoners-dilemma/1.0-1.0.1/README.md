# Comparing `tmp/prisoners-dilemma-1.0.tar.gz` & `tmp/prisoners_dilemma-1.0.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prisoners-dilemma-1.0.tar", last modified: Fri Apr 26 13:23:24 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```
