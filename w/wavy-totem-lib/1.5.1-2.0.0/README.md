# Comparing `tmp/wavy_totem_lib-1.5.1.tar.gz` & `tmp/wavy_totem_lib-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wavy_totem_lib-1.5.1.tar", max compression
+gzip compressed data, was "wavy_totem_lib-2.0.0.tar", max compression
```

## Comparing `wavy_totem_lib-1.5.1.tar` & `wavy_totem_lib-2.0.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     1338 2024-03-09 14:30:15.194590 wavy_totem_lib-1.5.1/LICENSE
--rw-r--r--   0        0        0     4965 2024-03-09 14:30:15.194590 wavy_totem_lib-1.5.1/README.md
--rw-r--r--   0        0        0      570 2024-03-09 14:30:23.622574 wavy_totem_lib-1.5.1/pyproject.toml
--rw-r--r--   0        0        0      524 2024-03-09 14:30:23.622574 wavy_totem_lib-1.5.1/wavy_totem_lib/__init__.py
--rw-r--r--   0        0        0     3736 2024-03-09 14:30:15.194590 wavy_totem_lib-1.5.1/wavy_totem_lib/aio.py
--rw-r--r--   0        0        0      596 2024-03-09 14:30:15.194590 wavy_totem_lib-1.5.1/wavy_totem_lib/exceptions.py
--rw-r--r--   0        0        0     1319 2024-03-09 14:30:15.194590 wavy_totem_lib-1.5.1/wavy_totem_lib/options.py
--rw-r--r--   0        0        0     1059 2024-03-09 14:30:15.194590 wavy_totem_lib-1.5.1/wavy_totem_lib/styles/abstract.py
--rw-r--r--   0        0        0     4542 2024-03-09 14:30:15.194590 wavy_totem_lib-1.5.1/wavy_totem_lib/styles/soul.py
--rw-r--r--   0        0        0     4020 2024-03-09 14:30:15.194590 wavy_totem_lib-1.5.1/wavy_totem_lib/styles/wavy.py
--rw-r--r--   0        0        0     4208 2024-03-09 14:30:15.194590 wavy_totem_lib-1.5.1/wavy_totem_lib/sync.py
--rw-r--r--   0        0        0     5777 1970-01-01 00:00:00.000000 wavy_totem_lib-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1338 2024-04-26 03:31:15.595946 wavy_totem_lib-2.0.0/LICENSE
+-rw-r--r--   0        0        0     4123 2024-04-26 03:31:15.595946 wavy_totem_lib-2.0.0/README.md
+-rw-r--r--   0        0        0      617 2024-04-26 03:31:23.340039 wavy_totem_lib-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0      550 2024-04-26 03:31:23.344039 wavy_totem_lib-2.0.0/wavy_totem_lib/__init__.py
+-rw-r--r--   0        0        0     1623 2024-04-26 03:31:15.599946 wavy_totem_lib-2.0.0/wavy_totem_lib/builder.py
+-rw-r--r--   0        0        0      386 2024-04-26 03:31:15.599946 wavy_totem_lib-2.0.0/wavy_totem_lib/exceptions.py
+-rw-r--r--   0        0        0      525 2024-04-26 03:31:15.599946 wavy_totem_lib-2.0.0/wavy_totem_lib/options.py
+-rw-r--r--   0        0        0    10783 2024-04-26 03:31:15.599946 wavy_totem_lib-2.0.0/wavy_totem_lib/skin.py
+-rw-r--r--   0        0        0      966 2024-04-26 03:31:15.599946 wavy_totem_lib-2.0.0/wavy_totem_lib/styles/abstract.py
+-rw-r--r--   0        0        0     4542 2024-04-26 03:31:15.599946 wavy_totem_lib-2.0.0/wavy_totem_lib/styles/soul.py
+-rw-r--r--   0        0        0     3881 2024-04-26 03:31:15.599946 wavy_totem_lib-2.0.0/wavy_totem_lib/styles/wavy.py
+-rw-r--r--   0        0        0     1218 2024-04-26 03:31:15.599946 wavy_totem_lib-2.0.0/wavy_totem_lib/totem.py
+-rw-r--r--   0        0        0     4945 1970-01-01 00:00:00.000000 wavy_totem_lib-2.0.0/PKG-INFO
```

### Comparing `wavy_totem_lib-1.5.1/LICENSE` & `wavy_totem_lib-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wavy_totem_lib-1.5.1/README.md` & `wavy_totem_lib-2.0.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,135 +1,157 @@
+Metadata-Version: 2.1
+Name: wavy-totem-lib
+Version: 2.0.0
+Summary: A library for generating the texture of Minecraft's Totem of Undying
+Home-page: https://github.com/wavy-cat/wavy-totem-lib
+License: BSL-1.0
+Author: WavyCat
+Author-email: unknown@wavycat.ru
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: Boost Software License 1.0 (BSL-1.0)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: pillow (>=10.0.0,<11.0.0)
+Project-URL: Issue tracker, https://github.com/wavy-cat/wavy-totem-lib/issues
+Description-Content-Type: text/markdown
+
 # wavy-totem-lib
 
-![GitHub repo size](https://img.shields.io/github/repo-size/wavy-cat/wavy-totem-lib?style=for-the-badge&logo=github&logoColor=white&labelColor=1A222E&color=242B36&cacheSeconds=0)
-![GitHub License](https://img.shields.io/github/license/wavy-cat/wavy-totem-lib?style=for-the-badge&labelColor=1A222E&color=242B36)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/wavy-totem-lib?style=for-the-badge&logo=Python&logoColor=white&label=Version&labelColor=1A222E&color=242B36&cacheSeconds=0)
+![GitHub License](https://img.shields.io/github/license/wavy-cat/wavy-totem-lib?style=for-the-badge&labelColor=1A222E&color=242B36)
+![GitHub repo size](https://img.shields.io/github/repo-size/wavy-cat/wavy-totem-lib?style=for-the-badge&logo=github&logoColor=white&labelColor=1A222E&color=242B36&cacheSeconds=0)
 
 Python library to generate totems of undying for Minecraft.
 
 ## Features
 
 * Support 64x32 skins
 * Zoning 2 layers and rounding the head
 * Lossless scaling image size
 * Asynchrony support
-* Built-in CLI [beta]
 * Supports PyPy
 * Supports different styles
 
 ## Requirements
 
 * python >= 3.8
 * Pillow >= 10.0.0
 
 ## Installing
 
 * Using poetry: `poetry add wavy-totem-lib`
 * Using pip: `pip install wavy-totem-lib`
 
-## Using CLI
-
-You can use the library without writing code, from the terminal.
-For help, enter the argument `--help` or `-h` (`python3 cli.py --help`).
-
-```
-usage: cli.py [-h] [--skin-type [{wide,slim,auto}]]
-              [--top-layers [{nothing,all,only_head,only_torso,only_hands,head_and_torso,head_and_hands}]]
-              [--round-head [ROUND_HEAD]] [--scale [FACTOR]]
-              skin_path totem_path
-```
-
-To give an example, the following command opens the skin file **my_skin.png** and creates a totem by **rounding its head**
-and saves it to the file **totem.png** at 64×64 resolution (**4x scaling**):
-
-```bash
-python3 cli.py my_skin.png totem.png --round-head true --scale 4
-```
-
-### Parameters
-
-| Name         | Required? | Valid values                    | Default | Description                                |
-|--------------|-----------|---------------------------------|---------|--------------------------------------------|
-| skin_path    | ✔         | string                          |         | Path to the skin file                      |
-| totem_path   | ✔         | string                          |         | Path where to save the finished totem file |
-| --skin-type  | ✖         | string (wide, slim, auto)       | auto    | Indication of what type of skin is used    |
-| --top-layers | ✖         | string (see Enum values in CLI) | all     | Indication of zoning 2 layers              |
-| --round-head | ✖         | bool                            | false   | Should the head be rounded                 |
-| --scale      | ✖         | integer (>0)                    | 1       | Image scaling multiplier                   |
-
 ## Examples
 
 * Quick generation:
 
 ```python
-from wavy_totem_lib import TotemBuilder, TopLayers
+from wavy_totem_lib import TotemBuilder, Skin, Totem, TopLayers
 
-totem = TotemBuilder('my_skin.png', top_layers=TopLayers.ONLY_HEAD, round_head=True)
-# top_layers=TopLayers.ONLY_HEAD – the outer layer will be applied only to the head
-# round_head=True – the head will be rounded at the corners
+builder = TotemBuilder(
+    Skin('my_skin.png'),
+    top_layers=[TopLayers.HEAD],  # the second layer will be applied only to the head
+    round_head=True  # the head will be rounded at the corners
+)
 
-totem_image = totem.generate()  # Returns a PIL.Image.Image object
-totem_image.save('totem.png')
+totem: Totem = builder.build()
+totem.image.save('totem.png')  # .image is Pillow image
 ```
 
 * Generation and scaling:
 
 ```python
-from wavy_totem_lib import TotemBuilder, SkinType
+from wavy_totem_lib import TotemBuilder, Skin, Totem, TopLayers
 
-totem = TotemBuilder('my_skin.png', skin_type=SkinType.WIDE)
-# skin_type allows you to set the skin type (slim or wide, default auto)
+builder = TotemBuilder(Skin('my_skin.png', slim=True))
 
-totem.generate()
-totem.scale(factor=8) # Scaling from 16×16 to 128×128
-totem.raw.show() # Image available in the `raw` variable
+totem: Totem = builder.build()
+scaled = totem.scale(factor=8)  # Scaling from 16×16 to 128×128
+scaled.save('totem.png')
 ```
 
 > [!NOTE]
 > To scale up, use the built-in `scale` method instead of `raw.resize` from Pillow, because it may blur the image.
 
 * Asynchronous generation:
 
 ```python
 import asyncio
-from wavy_totem_lib import AsyncTotemBuilder, SkinType, TopLayers
+import aiofiles  # This package must be installed
+from io import BytesIO
+from wavy_totem_lib import TotemBuilder, Skin, Totem, TopLayers
+
 
 async def main():
-    # Using AsyncTotemBuilder class instead of TotemBuilder
-    totem = AsyncTotemBuilder('my_skin.png', skin_type=SkinType.SLIM, top_layers=TopLayers.HEAD_AND_HANDS)
-    await totem.generate()
-    await totem.scale(factor=4) # 64×64
-    await totem.save('totem.png') # save() is only available in AsyncTotemBuilder
+    builder = TotemBuilder(Skin('my_skin.png', slim=False),
+                           top_layers=[TopLayers.HEAD, TopLayers.HANDS],
+                           round_head=True)
+    totem: Totem = await builder.build_async()
+    temp = BytesIO()
+    totem.image.save(temp, format='png')
+
+    async with aiofiles.open('totem.png', 'wb') as f:
+        await f.write(temp.getvalue())
+
 
 asyncio.run(main())
 ```
 
-> [!NOTE]
-> Although the methods `generate()`, `scale()` and the variable `raw` return values of type `PIL.Image.Image`, suitable for saving a file, it's advisable to use the built-in asynchronous save method instead.
-
 * Specifying a style
 
 ```python
-from wavy_totem_lib import TotemBuilder, STTStyle
+from wavy_totem_lib import TotemBuilder, Skin, Totem, STTStyle
 
-# WavyStyle (default), STTStyle available
-totem = TotemBuilder('my_skin.png', style=STTStyle)
-totem.generate()
-totem.raw.save('totem.png')
+# WavyStyle (default), STTStyle available built-in
+builder = TotemBuilder(Skin('my_skin.png'), style=STTStyle)
+totem: Totem = builder.build()
+totem.image.save('totem.png')
 ```
 
 > [!NOTE]
-> The `generate()` method accepts **kwargs, which will be passed on to the style class. None of the built-in styles support them.
+> The `generate()` method accepts **kwargs, which will be passed on to the style class. None of the built-in styles
+> support them.
 
 > STTStyle taken from https://github.com/UnFamousSoul/STT
 
-## Enum values
+## Styles
+
+> [!IMPORTANT]
+> You can create your own styles by inheriting the `AbstractStyle` class and implementing the `image` property.
+
+### Wavy
+
+Created by @wavy-cat.
+Class name: `WavyStyle`.
+This is the default style in TotemBuilder.
 
-**SkinType**: `WIDE`, `SLIM`, `AUTO`
+| Basil                           | Sylphiette                           | PWGood                           |
+|---------------------------------|--------------------------------------|----------------------------------|
+| ![Image](assets/basil_wavy.png) | ![Image](assets/sylphiette_wavy.png) | ![Image](assets/pwgood_wavy.png) |
 
-**TopLayers**: `NOTHING`, `ALL`, `ONLY_HEAD`, `ONLY_TORSO`, `ONLY_HANDS`, `HEAD_AND_TORSO`, `HEAD_AND_HANDS`
+```python
+from wavy_totem_lib import TotemBuilder, WavyStyle
+
+TotemBuilder(style=WavyStyle)
+# You can also not specify style at all, because WavyStyle - default style
+```
+
+### STT
 
-### In CLI
+Created by @UnFamousSoul.
+The code is taken from the [UnFamousSoul/STT](https://github.com/UnFamousSoul/STT) repository.
+Class name: `STTStyle`.
 
-**skin-type**: `wide`, `slim`, `auto`
+| Basil                          | Sylphiette                          | PWGood                          |
+|--------------------------------|-------------------------------------|---------------------------------|
+| ![Image](assets/basil_stt.png) | ![Image](assets/sylphiette_stt.png) | ![Image](assets/pwgood_stt.png) |
 
-**top-layers**: `nothing`, `all`, `only_head`, `only_torso`, `only_hands`, `head_and_torso`, `head_and_hands`
+```python
+from wavy_totem_lib import TotemBuilder, STTStyle
+
+TotemBuilder(style=STTStyle)
+```
```

### Comparing `wavy_totem_lib-1.5.1/pyproject.toml` & `wavy_totem_lib-2.0.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "wavy-totem-lib"
-version = "1.5.1"
-description = "Python library to generate totems of undying for Minecraft"
+version = "2.0.0"
+description = "A library for generating the texture of Minecraft's Totem of Undying"
 authors = ["WavyCat <unknown@wavycat.ru>"]
 readme = "README.md"
 license = "BSL-1.0"
 homepage = "https://github.com/wavy-cat/wavy-totem-lib"
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -17,7 +17,10 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.urls]
 "Issue tracker" = "https://github.com/wavy-cat/wavy-totem-lib/issues"
 
 [tool.ruff.lint.per-file-ignores]
 "__init__.py" = ["F401"]
+
+[tool.ruff]
+target-version = "py38"
```

### Comparing `wavy_totem_lib-1.5.1/wavy_totem_lib/styles/abstract.py` & `wavy_totem_lib-2.0.0/wavy_totem_lib/styles/abstract.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,35 @@
-#          Copyright WavyCat 2024 - 2025.
-# Distributed under the Boost Software License, Version 1.0.
-#        (See accompanying file LICENSE or copy at
-#          https://www.boost.org/LICENSE_1_0.txt)
+#                  Copyright WavyCat 2024.
+#  Distributed under the Boost Software License, Version 1.0.
+#         (See accompanying file LICENSE or copy at
+#           https://www.boost.org/LICENSE_1_0.txt)
 
 from abc import ABC, abstractmethod
 
 from PIL import Image
 
-from ..options import SkinType, TopLayers
+from ..options import TopLayers
+from ..skin import Skin
 
 
 class AbstractStyle(ABC):
     """Abstract style class. Use to create other styles."""
 
     @abstractmethod
-    def __init__(self, skin: Image.Image, skin_type: SkinType, top_layers: TopLayers, **kwargs):
+    def __init__(self, skin: Skin, top_layers: list[TopLayers], **kwargs):
         """
         Initializing method.
 
         Args:
             skin: PIL.Image.Image
-            skin_type: SkinType
-            top_layers: TopLayers
-            **_kwargs - extra options
+            top_layers: list[TopLayers]
+            **kwargs - extra options
         """
-        self._source = skin  # Skin Image object
-        self._skin_type = skin_type
-        self._top_layers = top_layers
-        self._kwargs = kwargs
+        self.skin = skin
+        self.top_layers = top_layers
+        self.kwargs = kwargs
         self._canvas = Image.new("RGBA", (16, 16))
 
     @property
     @abstractmethod
     def image(self) -> Image.Image:
         raise "This is an abstract method, don't try to use it."
```

### Comparing `wavy_totem_lib-1.5.1/wavy_totem_lib/styles/soul.py` & `wavy_totem_lib-2.0.0/wavy_totem_lib/styles/soul.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,30 @@
+#                  Copyright WavyCat 2024.
+#  Distributed under the Boost Software License, Version 1.0.
+#         (See accompanying file LICENSE or copy at
+#           https://www.boost.org/LICENSE_1_0.txt)
+
 from PIL import Image, ImageOps
 
 from .abstract import AbstractStyle
-from ..options import SkinType, TopLayers
+from ..skin import Skin
+from ..options import TopLayers
 
 
 class STTStyle(AbstractStyle):
     """Style taken from the UnFamousSoul/STT project (https://github.com/UnFamousSoul/STT)"""
 
-    def __init__(self, skin: Image.Image, skin_type: SkinType, top_layers: TopLayers, **kwargs):
-        super().__init__(skin, skin_type, top_layers, **kwargs)
+    def __init__(self, skin: Skin, top_layers: list[TopLayers], **kwargs):
+        super().__init__(skin, top_layers, **kwargs)
 
-    @staticmethod
-    def _head(skin, uol):
-        head = Image.new("RGBA", (8, 8))
+    def _add_head(self):
+        self._canvas.paste(self.skin.head_front, (4, 1))
 
-        head.paste(skin.crop((8, 8, 16, 16)), (0, 0))
-        if uol:
-            l21 = skin.crop((40, 8, 48, 9))
-            l22 = skin.crop((40, 9, 48, 16))
-            head.paste(l21, (0, 0), l21)
-            head.paste(l22, (0, 1), l22)
-        return head
+        if self.skin.available_second and TopLayers.HEAD in self.top_layers:
+            self._canvas.alpha_composite(self.skin.head_second_front, (4, 1))
 
     @staticmethod
     def _body(skin, uol):
         body = Image.new("RGBA", (8, 4))
 
         body.paste(skin.crop((20, 21, 28, 22)), (0, 0))
         body.paste(skin.crop((20, 23, 28, 24)), (0, 1))
@@ -71,19 +71,19 @@
             legs.paste(l25, (1, 2), l25)
             legs.paste(l26, (2, 2), l26)
             legs.paste(l27, (3, 2), l27)
             legs.paste(l28, (4, 2), l28)
         return legs
 
     @staticmethod
-    def _arms(skin, uol):
+    def _arms(skin, uol, slim):
         arms = Image.new("RGBA", (14, 3))
 
-        arms.paste(skin.crop((37, 52, 40, 54)).rotate(90, expand=True), (11, 0))
-        arms.paste(skin.crop((44, 20, 47, 22)).rotate(-90, expand=True), (1, 0))
+        arms.paste(skin.crop((37, 52, 39, 54) if slim else (37, 52, 40, 54)).rotate(90, expand=True), (11, 0))
+        arms.paste(skin.crop((44, 20, 46, 22) if slim else (44, 20, 47, 22)).rotate(-90, expand=True), (1, 0))
         arms.paste(skin.crop((39, 63, 40, 64)), (13, 0))
         arms.paste(skin.crop((36, 63, 37, 64)), (13, 1))
         arms.paste(skin.crop((44, 31, 45, 32)), (0, 0))
         arms.paste(skin.crop((47, 31, 48, 32)), (0, 1))
 
         if uol:
             l21 = skin.crop((53, 52, 56, 54)).rotate(90, expand=True)
@@ -100,22 +100,21 @@
             arms.paste(l25, (0, 0), l25)
             arms.paste(l26, (0, 1), l26)
 
         return arms
 
     @property
     def image(self) -> Image.Image:
-        torso = self._body(self._source, True if self._top_layers.value in (1, 3, 5) else False)
-        head = self._head(self._source, True if self._top_layers.value in (1, 2, 5, 6) else False)
-        legs = self._legs(self._source, True if self._top_layers.value in (1, 3, 5) else False)
-        arms = self._arms(self._source, True if self._top_layers.value in (1, 4, 6) else False)
+        torso = self._body(self.skin.image, TopLayers.TORSO in self.top_layers)
+        legs = self._legs(self.skin.image, TopLayers.LEGS in self.top_layers)
+        arms = self._arms(self.skin.image, TopLayers.HANDS in self.top_layers, self.skin.is_slim)
 
         self._canvas.paste(arms, (1, 8))
         self._canvas.paste(legs, (5, 13))
 
-        if self._source.height == 32:
+        if self.skin.version == 'old':
             self._canvas.paste(ImageOps.mirror(self._canvas.crop((0, 0, 8, 16))), (8, 0))
 
         self._canvas.paste(torso, (4, 9))
-        self._canvas.paste(head, (4, 1))
+        self._add_head()
 
         return self._canvas
```

