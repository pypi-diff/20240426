# Comparing `tmp/sortedintersect-0.4.1.tar.gz` & `tmp/sortedintersect-0.4.2-cp310-cp310-macosx_13_0_arm64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sortedintersect-0.4.1.tar", last modified: Fri Apr 12 20:50:10 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

