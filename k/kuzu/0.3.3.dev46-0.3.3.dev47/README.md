# Comparing `tmp/kuzu-0.3.3.dev46.tar.gz` & `tmp/kuzu-0.3.3.dev47-cp37-cp37m-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kuzu-0.3.3.dev46.tar", last modified: Thu Apr 25 08:04:37 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

