# Comparing `tmp/network-symmetry-0.3.0.tar.gz` & `tmp/network_symmetry-0.4.1-cp39-cp39-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "network-symmetry-0.3.0.tar", last modified: Wed Sep 21 18:47:20 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

