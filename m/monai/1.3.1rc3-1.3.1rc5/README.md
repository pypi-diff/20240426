# Comparing `tmp/monai-1.3.1rc3.tar.gz` & `tmp/monai-1.3.1rc5-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monai-1.3.1rc3.tar", last modified: Mon Apr 15 13:09:18 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

