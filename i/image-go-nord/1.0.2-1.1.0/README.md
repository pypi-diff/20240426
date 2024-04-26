# Comparing `tmp/image-go-nord-1.0.2.tar.gz` & `tmp/image-go-nord-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image-go-nord-1.0.2.tar", last modified: Wed Apr 17 09:34:22 2024, max compression
+gzip compressed data, was "image-go-nord-1.1.0.tar", last modified: Fri Apr 26 08:33:48 2024, max compression
```

## Comparing `image-go-nord-1.0.2.tar` & `image-go-nord-1.1.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 09:34:22.247226 image-go-nord-1.0.2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 09:34:22.243226 image-go-nord-1.0.2/ImageGoNord/
--rwxr-xr-x   0 root         (0) root         (0)    24849 2024-04-17 09:34:07.000000 image-go-nord-1.0.2/ImageGoNord/GoNord.py
--rw-r--r--   0 root         (0) root         (0)      768 2024-04-17 09:34:07.000000 image-go-nord-1.0.2/ImageGoNord/GoNord_test.py
--rwxr-xr-x   0 root         (0) root         (0)       72 2024-04-17 09:34:07.000000 image-go-nord-1.0.2/ImageGoNord/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 09:34:22.243226 image-go-nord-1.0.2/ImageGoNord/models/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 09:34:22.243226 image-go-nord-1.0.2/ImageGoNord/models/PaletteNet/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 09:34:07.000000 image-go-nord-1.0.2/ImageGoNord/models/PaletteNet/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 09:34:07.000000 image-go-nord-1.0.2/ImageGoNord/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 09:34:22.243226 image-go-nord-1.0.2/ImageGoNord/palettes/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 09:34:22.247226 image-go-nord-1.0.2/ImageGoNord/palettes/Nord/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 09:34:07.000000 image-go-nord-1.0.2/ImageGoNord/palettes/Nord/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 09:34:07.000000 image-go-nord-1.0.2/ImageGoNord/palettes/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 09:34:22.247226 image-go-nord-1.0.2/ImageGoNord/utility/
--rwxr-xr-x   0 root         (0) root         (0)     2330 2024-04-17 09:34:07.000000 image-go-nord-1.0.2/ImageGoNord/utility/ConvertUtility.py
--rwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 09:34:07.000000 image-go-nord-1.0.2/ImageGoNord/utility/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5947 2024-04-17 09:34:07.000000 image-go-nord-1.0.2/ImageGoNord/utility/model.py
--rw-r--r--   0 root         (0) root         (0)     3368 2024-04-17 09:34:07.000000 image-go-nord-1.0.2/ImageGoNord/utility/palette_loader.py
--rw-r--r--   0 root         (0) root         (0)      962 2024-04-17 09:34:07.000000 image-go-nord-1.0.2/ImageGoNord/utility/quantize.py
--rw-r--r--   0 root         (0) root         (0)    34522 2024-04-17 09:34:07.000000 image-go-nord-1.0.2/LICENSE
--rwxr-xr-x   0 root         (0) root         (0)       31 2024-04-17 09:34:07.000000 image-go-nord-1.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     7009 2024-04-17 09:34:22.247226 image-go-nord-1.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5861 2024-04-17 09:34:07.000000 image-go-nord-1.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 09:34:22.247226 image-go-nord-1.0.2/image_go_nord.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7009 2024-04-17 09:34:22.000000 image-go-nord-1.0.2/image_go_nord.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      608 2024-04-17 09:34:22.000000 image-go-nord-1.0.2/image_go_nord.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 09:34:22.000000 image-go-nord-1.0.2/image_go_nord.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       58 2024-04-17 09:34:22.000000 image-go-nord-1.0.2/image_go_nord.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-04-17 09:34:22.000000 image-go-nord-1.0.2/image_go_nord.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-17 09:34:22.247226 image-go-nord-1.0.2/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1756 2024-04-17 09:34:07.000000 image-go-nord-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 08:33:48.153412 image-go-nord-1.1.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 08:33:48.149412 image-go-nord-1.1.0/ImageGoNord/
+-rwxr-xr-x   0 root         (0) root         (0)    25929 2024-04-26 08:33:34.000000 image-go-nord-1.1.0/ImageGoNord/GoNord.py
+-rw-r--r--   0 root         (0) root         (0)      768 2024-04-26 08:33:34.000000 image-go-nord-1.1.0/ImageGoNord/GoNord_test.py
+-rwxr-xr-x   0 root         (0) root         (0)       72 2024-04-26 08:33:34.000000 image-go-nord-1.1.0/ImageGoNord/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 08:33:48.149412 image-go-nord-1.1.0/ImageGoNord/models/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 08:33:48.149412 image-go-nord-1.1.0/ImageGoNord/models/PaletteNet/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-26 08:33:34.000000 image-go-nord-1.1.0/ImageGoNord/models/PaletteNet/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-26 08:33:34.000000 image-go-nord-1.1.0/ImageGoNord/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 08:33:48.149412 image-go-nord-1.1.0/ImageGoNord/palettes/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 08:33:48.149412 image-go-nord-1.1.0/ImageGoNord/palettes/Nord/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-26 08:33:34.000000 image-go-nord-1.1.0/ImageGoNord/palettes/Nord/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-26 08:33:34.000000 image-go-nord-1.1.0/ImageGoNord/palettes/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 08:33:48.153412 image-go-nord-1.1.0/ImageGoNord/utility/
+-rwxr-xr-x   0 root         (0) root         (0)     2330 2024-04-26 08:33:34.000000 image-go-nord-1.1.0/ImageGoNord/utility/ConvertUtility.py
+-rwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 08:33:34.000000 image-go-nord-1.1.0/ImageGoNord/utility/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5947 2024-04-26 08:33:34.000000 image-go-nord-1.1.0/ImageGoNord/utility/model.py
+-rw-r--r--   0 root         (0) root         (0)     3368 2024-04-26 08:33:34.000000 image-go-nord-1.1.0/ImageGoNord/utility/palette_loader.py
+-rw-r--r--   0 root         (0) root         (0)      962 2024-04-26 08:33:34.000000 image-go-nord-1.1.0/ImageGoNord/utility/quantize.py
+-rw-r--r--   0 root         (0) root         (0)    34522 2024-04-26 08:33:34.000000 image-go-nord-1.1.0/LICENSE
+-rwxr-xr-x   0 root         (0) root         (0)       31 2024-04-26 08:33:34.000000 image-go-nord-1.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7028 2024-04-26 08:33:48.153412 image-go-nord-1.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5861 2024-04-26 08:33:34.000000 image-go-nord-1.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 08:33:48.153412 image-go-nord-1.1.0/image_go_nord.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7028 2024-04-26 08:33:48.000000 image-go-nord-1.1.0/image_go_nord.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      608 2024-04-26 08:33:48.000000 image-go-nord-1.1.0/image_go_nord.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-26 08:33:48.000000 image-go-nord-1.1.0/image_go_nord.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-26 08:33:48.000000 image-go-nord-1.1.0/image_go_nord.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-04-26 08:33:48.000000 image-go-nord-1.1.0/image_go_nord.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-26 08:33:48.153412 image-go-nord-1.1.0/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1665 2024-04-26 08:33:34.000000 image-go-nord-1.1.0/setup.py
```

### Comparing `image-go-nord-1.0.2/ImageGoNord/GoNord.py` & `image-go-nord-1.1.0/ImageGoNord/GoNord.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,34 +8,43 @@
 
 from PIL import Image, ImageFilter
 
 import numpy as np
 import ffmpeg
 import uuid
 import shutil
+import requests
 
-import torch
-import skimage.io as io
-import skimage.color as convertor
-import torchvision.transforms as transforms
+try:
+    import torch
+    import skimage.color as convertor
+    import torchvision.transforms as transforms
+except ImportError:
+    # AI feature disabled
+    pass
 
 
 try:
     import importlib.resources as pkg_resources
 except ImportError:
     # Try backported to PY<37 `importlib_resources`.
     import importlib_resources as pkg_resources
 
 from .palettes import Nord as nord_palette
 from .models import PaletteNet as palette_net
 
 from ImageGoNord.utility.quantize import quantize_to_palette
 import ImageGoNord.utility.palette_loader as pl
 from ImageGoNord.utility.ConvertUtility import ConvertUtility
-from ImageGoNord.utility.model import FeatureEncoder,RecoloringDecoder
+
+try:
+    from ImageGoNord.utility.model import FeatureEncoder,RecoloringDecoder
+except ImportError:
+    # AI feature disabled
+    pass
 
 
 class NordPaletteFile:
     """
     A class used to map the nord color-scheme into files.
     Each file contains the hex of colors
 
@@ -154,14 +163,16 @@
     PALETTE_LOOKUP_PATH = DEFAULT_PALETTE_PATH
     USE_GAUSSIAN_BLUR = False
     USE_AVG_COLOR = False
     AVG_BOX_DATA = {"w": -2, "h": 3}
     TRANSPARENCY_TOLERANCE = 190
     MAX_THREADS = 10
 
+    PALETTE_NET_REPO_FOLDER = 'https://github.com/Schrodinger-Hat/ImageGoNord-pip/raw/master/ImageGoNord/models/PaletteNet/'
+
     AVAILABLE_PALETTE = []
     PALETTE_DATA = {}
 
     def __init__(self):
         """Constructor: init variables & config"""
         self.set_default_nord_palette()
         self.set_avg_box_data()
@@ -421,14 +432,24 @@
                 colors_list = self.PALETTE_DATA[difference]
                 if (is_rgba and len(colors_list) == 3):
                     colors_list.append(color_to_check[3])
 
                 pixels[row, col] = tuple(colors_list)
         return pixels
 
+    def load_and_save_models(self):
+        rd_model = requests.get(self.PALETTE_NET_REPO_FOLDER + 'RD.state_dict.pt')
+        fe_model = requests.get(self.PALETTE_NET_REPO_FOLDER + 'FE.state_dict.pt')
+
+        with open(os.path.dirname(palette_net.__file__) + '/FE.state_dict.pt', "wb") as f:
+            f.write(fe_model.content)
+        
+        with open(os.path.dirname(palette_net.__file__) + '/RD.state_dict.pt', "wb") as f:
+            f.write(rd_model.content)
+
     def convert_image_by_model(self, image, use_model_cpu=False):
         """
         Process a Pillow image by using a PyTorch model "PaletteNet" for recoloring the image
 
         Parameters
         ----------
         image : pillow image
@@ -440,16 +461,22 @@
         -------
         pillow image
             processed image
         """
         FE = FeatureEncoder() # torch.Size([64, 3, 3, 3])
         RD = RecoloringDecoder() # torch.Size([530, 256, 3, 3])
 
-        FE.load_state_dict(torch.load(pkg_resources.open_binary(palette_net, "FE.state_dict.pt")))
-        RD.load_state_dict(torch.load(pkg_resources.open_binary(palette_net, "RD.state_dict.pt")))
+        if (
+            os.path.exists(os.path.dirname(palette_net.__file__) + '/FE.state_dict.pt')
+            and os.path.exists(os.path.dirname(palette_net.__file__) + '/RD.state_dict.pt')
+        ):
+            FE.load_state_dict(torch.load(pkg_resources.open_binary(palette_net, "FE.state_dict.pt")))
+            RD.load_state_dict(torch.load(pkg_resources.open_binary(palette_net, "RD.state_dict.pt")))
+        else:
+            self.load_and_save_models()
 
         if use_model_cpu:
             FE.to("cpu")
             RD.to("cpu")
 
         lab_image = ((convertor.rgb2lab(np.array(image))) - [50,0,0] ) / [50,127,127]
 
@@ -468,15 +495,16 @@
             for j in [2,4,6]:
                 a.append(int(hex[j-2:j],16))
             palette.append(a)
 
         try:
             pal_np = np.array(palette).reshape(1,6,3)/255
         except:
-            print("You have too many colors in your palette for the model, this feature is limited to 6 colours, now you have: ", len(palette), "! I'll take the first 6!")
+            # this feature is limited to 6 colours
+            # we're taking the first six
             pal_np = np.array(palette[0:6]).reshape(1,6,3)/255
 
         pal = torch.Tensor((convertor.rgb2lab(pal_np) - [50,0,0] ) / [50,128,128]).unsqueeze(0)
 
         image = img
         palette = pal
         illu = image[:,0:1,:,:]
@@ -514,15 +542,18 @@
         original_image = image.copy()
         original_pixels = self.load_pixel_image(original_image)
         original_image.close()
         pixels = self.load_pixel_image(image)
         is_rgba = (image.mode == 'RGBA')
 
         if use_model:
-            image = self.convert_image_by_model(image, use_model_cpu)
+            if torch != None:
+                image = self.convert_image_by_model(image, use_model_cpu)
+            else:
+                print('Please install the dependencies required for the AI feature: pip install image-go-nord[AI]')
         else:
             if not parallel_threading:
                 self.converted_loop(is_rgba, pixels, original_pixels, image.size[0], image.size[1])
             else:
                 step = ceil(image.size[0] / self.MAX_THREADS)
                 threads = []
                 for row in range(step, image.size[0] + step, step):
```

### Comparing `image-go-nord-1.0.2/ImageGoNord/GoNord_test.py` & `image-go-nord-1.1.0/ImageGoNord/GoNord_test.py`

 * *Files identical despite different names*

### Comparing `image-go-nord-1.0.2/ImageGoNord/utility/ConvertUtility.py` & `image-go-nord-1.1.0/ImageGoNord/utility/ConvertUtility.py`

 * *Files identical despite different names*

### Comparing `image-go-nord-1.0.2/ImageGoNord/utility/model.py` & `image-go-nord-1.1.0/ImageGoNord/utility/model.py`

 * *Files identical despite different names*

### Comparing `image-go-nord-1.0.2/ImageGoNord/utility/palette_loader.py` & `image-go-nord-1.1.0/ImageGoNord/utility/palette_loader.py`

 * *Files identical despite different names*

### Comparing `image-go-nord-1.0.2/ImageGoNord/utility/quantize.py` & `image-go-nord-1.1.0/ImageGoNord/utility/quantize.py`

 * *Files identical despite different names*

### Comparing `image-go-nord-1.0.2/LICENSE` & `image-go-nord-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `image-go-nord-1.0.2/PKG-INFO` & `image-go-nord-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image-go-nord
-Version: 1.0.2
+Version: 1.1.0
 Summary: A tool to convert any RGB image or video to any theme or color palette input by the user
 Home-page: https://github.com/Schrodinger-Hat/ImageGoNord-pip
 Author: Schrodinger Hat
 Author-email: schrodinger.hat.show@gmail.com
 License: AGPL-3.0
 Download-URL: https://github.com/Schrodinger-Hat/ImageGoNord-pip/releases
 Project-URL: Homepage, https://ign.schrodinger-hat.it
@@ -16,14 +16,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+Provides-Extra: AI
 License-File: LICENSE
 
 # ImageGoNord - RGB image and video to any kind of palette or theme
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/image-go-nord)
 [![PyPI](https://img.shields.io/pypi/v/image-go-nord)](https://pypi.org/project/image-go-nord/)
 [![license](https://img.shields.io/badge/license-MIT-green)](https://github.com/Schrodinger-Hat/ImageGoNord-pip/blob/master/LICENSE)
```

### Comparing `image-go-nord-1.0.2/README.md` & `image-go-nord-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `image-go-nord-1.0.2/image_go_nord.egg-info/PKG-INFO` & `image-go-nord-1.1.0/image_go_nord.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image-go-nord
-Version: 1.0.2
+Version: 1.1.0
 Summary: A tool to convert any RGB image or video to any theme or color palette input by the user
 Home-page: https://github.com/Schrodinger-Hat/ImageGoNord-pip
 Author: Schrodinger Hat
 Author-email: schrodinger.hat.show@gmail.com
 License: AGPL-3.0
 Download-URL: https://github.com/Schrodinger-Hat/ImageGoNord-pip/releases
 Project-URL: Homepage, https://ign.schrodinger-hat.it
@@ -16,14 +16,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+Provides-Extra: AI
 License-File: LICENSE
 
 # ImageGoNord - RGB image and video to any kind of palette or theme
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/image-go-nord)
 [![PyPI](https://img.shields.io/pypi/v/image-go-nord)](https://pypi.org/project/image-go-nord/)
 [![license](https://img.shields.io/badge/license-MIT-green)](https://github.com/Schrodinger-Hat/ImageGoNord-pip/blob/master/LICENSE)
```

### Comparing `image-go-nord-1.0.2/image_go_nord.egg-info/SOURCES.txt` & `image-go-nord-1.1.0/image_go_nord.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `image-go-nord-1.0.2/setup.py` & `image-go-nord-1.1.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,36 +2,39 @@
 from setuptools import setup, find_packages
 
 ROOT = pathlib.Path('.')
 README = (ROOT / "README.md").read_text()
 
 setup(
     name="image-go-nord",
-    version="1.0.2",
+    version="1.1.0",
     description="A tool to convert any RGB image or video to any theme or color palette input by the user",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/Schrodinger-Hat/ImageGoNord-pip",
     download_url = 'https://github.com/Schrodinger-Hat/ImageGoNord-pip/releases',
     keywords = ['nordtheme', 'pillow', 'image', 'conversion', 'rgb', 'color-scheme', 'color-palette', 'linux-rice', 'gruvbox', 'catpuccin'], 
     author="Schrodinger Hat",
     author_email="schrodinger.hat.show@gmail.com",
     license="AGPL-3.0",
     classifiers=[
-        'Development Status :: 5 - Production/Stable',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
+        'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
         "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7"
     ],
     project_urls={
         "Homepage": "https://ign.schrodinger-hat.it",
         "Source": "https://github.com/Schrodinger-Hat/ImageGoNord-pip",
         "Bug Reports": "https://github.com/Schrodinger-Hat/ImageGoNord-pip/issues",
     },
     packages=find_packages(),
-    package_data={'': ['*.txt', 'palettes/*.txt', 'models/*.pt', '*.pt', '*.state_dict.*']},
+    package_data={'': ['*.txt', 'palettes/*.txt']},
     include_package_data=True,
-    install_requires=["Pillow", "ffmpeg-python", "numpy", "torch", "scikit-image", "torchvision"],
+    install_requires=["Pillow", "ffmpeg-python", "numpy", "requests"],
+    extras_require = {
+        'AI':  ["torch", "scikit-image", "torchvision"]
+    },
     python_requires=">=3.5"
 )
```

