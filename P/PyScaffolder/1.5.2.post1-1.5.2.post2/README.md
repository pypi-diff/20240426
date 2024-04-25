# Comparing `tmp/PyScaffolder-1.5.2.post1.tar.gz` & `tmp/PyScaffolder-1.5.2.post2-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyScaffolder-1.5.2.post1.tar", last modified: Sun Apr 30 11:19:36 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

