# Comparing `tmp/tensorcat-0.1.tar.gz` & `tmp/tensorcat-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorcat-0.1.tar", max compression
+gzip compressed data, was "tensorcat-0.1.1.tar", max compression
```

## Comparing `tensorcat-0.1.tar` & `tensorcat-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     5058 2024-04-26 03:47:48.996699 tensorcat-0.1/README.md
--rw-r--r--   0        0        0      458 2024-04-26 03:48:34.509656 tensorcat-0.1/pyproject.toml
--rw-r--r--   0        0        0       72 2024-04-22 08:44:47.453857 tensorcat-0.1/tensorcat/__init__.py
--rw-r--r--   0        0        0     2001 2024-04-22 08:44:47.453976 tensorcat-0.1/tensorcat/cli.py
--rw-r--r--   0        0        0     2477 2024-04-22 08:44:47.454112 tensorcat-0.1/tensorcat/iterm2.py
--rw-r--r--   0        0        0     5952 2024-04-22 08:44:47.454301 tensorcat-0.1/tensorcat/tensorcat.py
--rw-r--r--   0        0        0     5691 1970-01-01 00:00:00.000000 tensorcat-0.1/PKG-INFO
+-rw-r--r--   0        0        0      673 2024-04-18 18:32:11.216006 tensorcat-0.1.1/README.md
+-rw-r--r--   0        0        0      460 2024-04-18 19:06:56.451714 tensorcat-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       72 2024-04-18 18:11:23.238156 tensorcat-0.1.1/tensorcat/__init__.py
+-rw-r--r--   0        0        0     1936 2024-04-18 18:58:32.811965 tensorcat-0.1.1/tensorcat/cli.py
+-rw-r--r--   0        0        0     2477 2024-04-18 18:11:23.278104 tensorcat-0.1.1/tensorcat/iterm2.py
+-rw-r--r--   0        0        0     4471 2024-04-18 18:11:23.283467 tensorcat-0.1.1/tensorcat/tensorcat.py
+-rw-r--r--   0        0        0     1469 1970-01-01 00:00:00.000000 tensorcat-0.1.1/setup.py
+-rw-r--r--   0        0        0     1206 1970-01-01 00:00:00.000000 tensorcat-0.1.1/PKG-INFO
```

### Comparing `tensorcat-0.1/tensorcat/cli.py` & `tensorcat-0.1.1/tensorcat/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,37 +3,37 @@
 
 from PIL import Image, ImageOps
 
 from .iterm2 import print_img
 
 
 def main():
-    parser = argparse.ArgumentParser(description="Display or download an image in terminal")
+    parser = argparse.ArgumentParser(description="Display an image in terminal cli")
     parser.add_argument("image", type=Path, help="Path to the image file")
     parser.add_argument(
         "--download", "-d", action="store_true", help="Download the image"
     )
 
     parser.add_argument(
         "--orig_res",
         "-or",
         action="store_true",
-        help="No downsample, use original resolution, ignoring max_width and max_height",
+        help="No downsaple, use original resolution",
     )
     parser.add_argument(
         "--max_width", "-mw", type=int, default=1024, help="Downsample to the max width"
     )
     parser.add_argument(
         "--max_height",
         "-mh",
         type=int,
         default=1024,
         help="Downsample to the max height",
     )
-    parser.add_argument("--name", "-n", type=str, help="Name of the image (download file name)")
+    parser.add_argument("--name", "-n", type=str, help="Name of the image")
 
     parser.add_argument(
         "--render_width", "-rw", type=str, help="Render width of the image"
     )
     parser.add_argument(
         "--render_height", "-rh", type=str, help="Render height of the image"
     )
```

### Comparing `tensorcat-0.1/tensorcat/iterm2.py` & `tensorcat-0.1.1/tensorcat/iterm2.py`

 * *Files identical despite different names*

