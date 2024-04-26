# Comparing `tmp/botocore-a-la-carte-b2bi-1.34.91.tar.gz` & `tmp/botocore_a_la_carte_b2bi-1.34.92-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-b2bi-1.34.91.tar", last modified: Thu Apr 25 01:03:25 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```
