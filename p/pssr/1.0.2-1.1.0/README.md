# Comparing `tmp/pssr-1.0.2.tar.gz` & `tmp/pssr-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pssr-1.0.2.tar", max compression
+gzip compressed data, was "pssr-1.1.0.tar", max compression
```

## Comparing `pssr-1.0.2.tar` & `pssr-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1070 2024-04-16 23:21:24.739071 pssr-1.0.2/LICENSE
--rw-r--r--   0        0        0     1135 2024-04-18 21:41:53.895012 pssr-1.0.2/README.md
--rw-r--r--   0        0        0     4098 2024-04-20 03:36:20.880209 pssr-1.0.2/_pssr.py
--rw-r--r--   0        0        0        0 2024-03-07 21:39:47.125640 pssr-1.0.2/pssr/__init__.py
--rw-r--r--   0        0        0     2823 2024-04-19 21:36:59.885172 pssr-1.0.2/pssr/crappifiers.py
--rw-r--r--   0        0        0    23918 2024-04-17 21:06:33.049096 pssr-1.0.2/pssr/data.py
--rw-r--r--   0        0        0     2606 2024-04-18 23:21:37.910893 pssr-1.0.2/pssr/loss.py
--rw-r--r--   0        0        0       60 2024-04-16 23:21:24.747072 pssr-1.0.2/pssr/models/__init__.py
--rw-r--r--   0        0        0     1538 2024-03-07 21:39:47.125640 pssr-1.0.2/pssr/models/_blocks.py
--rw-r--r--   0        0        0     3167 2024-04-16 23:21:24.747072 pssr-1.0.2/pssr/models/resunet.py
--rw-r--r--   0        0        0     5394 2024-04-16 23:21:24.747072 pssr-1.0.2/pssr/models/resuneta.py
--rw-r--r--   0        0        0    11172 2024-04-20 01:31:13.287411 pssr-1.0.2/pssr/predict.py
--rw-r--r--   0        0        0    12859 2024-04-19 22:26:27.237887 pssr-1.0.2/pssr/train.py
--rw-r--r--   0        0        0     1111 2024-04-20 03:02:24.140545 pssr-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     2481 1970-01-01 00:00:00.000000 pssr-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-16 23:21:24.739071 pssr-1.1.0/LICENSE
+-rw-r--r--   0        0        0     1135 2024-04-18 21:41:53.895012 pssr-1.1.0/README.md
+-rw-r--r--   0        0        0     4388 2024-04-26 16:18:41.417948 pssr-1.1.0/_pssr.py
+-rw-r--r--   0        0        0        0 2024-03-07 21:39:47.125640 pssr-1.1.0/pssr/__init__.py
+-rw-r--r--   0        0        0     4510 2024-04-26 04:19:02.573621 pssr-1.1.0/pssr/crappifiers.py
+-rw-r--r--   0        0        0    32538 2024-04-26 16:07:25.348267 pssr-1.1.0/pssr/data.py
+-rw-r--r--   0        0        0     2610 2024-04-26 03:52:46.726742 pssr-1.1.0/pssr/loss.py
+-rw-r--r--   0        0        0       60 2024-04-16 23:21:24.747072 pssr-1.1.0/pssr/models/__init__.py
+-rw-r--r--   0        0        0     1531 2024-04-23 03:43:56.881543 pssr-1.1.0/pssr/models/_blocks.py
+-rw-r--r--   0        0        0     3449 2024-04-23 03:55:21.307775 pssr-1.1.0/pssr/models/resunet.py
+-rw-r--r--   0        0        0     6143 2024-04-23 03:46:26.643939 pssr-1.1.0/pssr/models/resuneta.py
+-rw-r--r--   0        0        0    11102 2024-04-26 16:28:39.578874 pssr-1.1.0/pssr/predict.py
+-rw-r--r--   0        0        0    13012 2024-04-26 03:53:11.755078 pssr-1.1.0/pssr/train.py
+-rw-r--r--   0        0        0     1125 2024-04-26 04:20:30.130972 pssr-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2517 1970-01-01 00:00:00.000000 pssr-1.1.0/PKG-INFO
```

### Comparing `pssr-1.0.2/LICENSE` & `pssr-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pssr-1.0.2/README.md` & `pssr-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pssr-1.0.2/_pssr.py` & `pssr-1.1.0/_pssr.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import torch, argparse, sys
 from torch.nn import MSELoss
 from pssr.models import ResUNet, ResUNetA
 from pssr.data import ImageDataset, SlidingDataset, PairedImageDataset, PairedSlidingDataset
-from pssr.crappifiers import AdditiveGaussian, Poisson
+from pssr.crappifiers import MultiCrappifier, Poisson, AdditiveGaussian, SaltPepper
 from pssr.loss import SSIMLoss
 from pssr.train import train_paired
 from pssr.predict import predict_images, test_metrics
 
 def _handle_declaration(arg, defaults, req=None):
     req = ", ".join(req)+", " if req is not None else ""
 
@@ -28,22 +28,23 @@
     parser.add_argument("-mp", "--model-path", type=str, default="model.pth", help="specify model path")
 
     parser.add_argument("-e", "--epochs", type=int, default=10, help="specify number of training epochs")
     parser.add_argument("-b", "--batch-size", type=int, default=16, help="specify batch size")
     parser.add_argument("-lr", "--lr", type=float, default=1e-3, help="specify learning rate")
     parser.add_argument("-p", "--patience", type=int, default=3, help="specify learning rate decay patience")
     parser.add_argument("-mse", "--mse", action="store_true", help="use MSE loss instead of SSIM loss")
+    parser.add_argument("-sl", "--save-losses", action="store_true", help="save training losses")
 
     return parser
 
 def run():
     parser = parse()
     if len(sys.argv) == 1:
         parser.print_help(sys.stderr)
-        sys.exit(1)
+        return
     args = parser.parse_args()
 
     if "Paired" not in args.data_type and args.data_path is None:
         print("--data-path(-dp) must be provided for semi-synthetic datasets")
         return
 
     model = _handle_declaration(args.model_type, ["ResUNet", "ResUNetA"])
@@ -81,22 +82,28 @@
             dataloader_kwargs=kwargs,
         )
         print("\nTraining complete!")
 
         torch.save(model, args.model_path)
         print(f"Saved trained model to {args.model_path}")
 
+        if args.save_losses:
+            with open("train_loss.txt", "w") as file:
+                for loss in losses:
+                    file.write(f"{loss}\n")
+
     else:
         model.load_state_dict(torch.load(args.model_path))
 
         print("\nPredicting images from low resolution...")
-        predict_images(model, dataset, device, "preds", norm=not dataset.is_lr)
+        predict_images(model, dataset, device, norm=not dataset.is_lr, out_dir="preds")
 
         if not dataset.is_lr:
-            metrics = test_metrics(model, dataset, args.batch_size, device=device, dataloader_kwargs=kwargs)
+            print("\nCalculating metrics...")
+            metrics = test_metrics(model, dataset, device)
 
             print("\nMetrics:")
             for metric in metrics:
                 print(f"{metric}: {metrics[metric]}")
     
     print("\n")
```

### Comparing `pssr-1.0.2/pssr/crappifiers.py` & `pssr-1.1.0/pssr/crappifiers.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import numpy as np
 from abc import ABC, abstractmethod
+from skimage.util import random_noise
 
 class Crappifier(ABC):
     r"""Crappifier base class for custom crappifiers. Override the :meth:`crappify` method for logic.
     """
     @abstractmethod
     def crappify(self, image : np.ndarray):
         r"""An abstract function for degrading a low resolution image to simulate undersampling.
@@ -12,51 +13,87 @@
 
         Args:
             image (np.ndarray) : Low resolution image to crappify.
 
         Returns:
             crap (np.ndarray) : The low resolution image, only now has it been crappified.
         """
-        raise NotImplementedError("Crappify method not implemented")
+        raise NotImplementedError('"crappify" method not implemented.')
+    
+    def __call__(self, image : np.ndarray):
+        return self.crappify(image)
+
+class MultiCrappifier(Crappifier):
+    def __init__(self, crappifiers : list[Crappifier]):
+        r"""Chains multiple crappifiers sequentially for degrading low resolution images.
+
+        Args:
+            crappifiers (list[Crappifier]) : Crappifiers to be applied in order from first to last.
+        """
+        self.crappifiers = list(crappifiers) if type(crappifiers) is not list else crappifiers
+    
+    def crappify(self, image : np.ndarray):
+        for crappifier in self.crappifiers:
+            image = crappifier.crappify(image)
+        return image
 
 class AdditiveGaussian(Crappifier):
     def __init__(self, intensity : float = 13, gain : float = 0, spread : float = 0):
         r"""Crappifier using additive Gaussian noise sampling (normally distributed noise). Adds additive Gaussian noise to a low resolution image.
 
         Approximates :class:`Poisson` noise at high samples.
 
         Args:
             intensity (float) : Standard deviation of Gaussian distribution. Higher values will introduce more noise to the image. Default is 13.
 
             gain (float) : Mean of Gaussian distribution. Higher or lower values will raise the mean image value higher or lower respectively. Default is 0.
 
-            spread (float) : Standard deviation of crappifier intensity for training on a range of crappifications. Default is 0. 
+            spread (float) : Standard deviation of crappifier intensity for training on a range of crappifications. Default is 0.
         """
         self.intensity = intensity
         self.gain = gain
         self.spread = spread
 
     def crappify(self, image : np.ndarray):
         intensity = max(np.random.normal(self.intensity, self.spread), 0) if self.spread > 0 else self.intensity
         return image + np.random.normal(self.gain, intensity, image.shape)
     
 class Poisson(Crappifier):
     def __init__(self, intensity : float = 1, gain : float = 0, spread : float = 0):
         r"""Crappifier using Poisson noise sampling (shot noise). Adds Poisson noise to a low resolution image.
 
         Args:
-            intensity (float) : Interpolated mix of generated Poisson image. 1 is full noise, 0 is none. Default is 1.
+            intensity (float) : Interpolated mix of generated Poisson image. 1 is standard distribution, 0 is none, larger values amplify noise. Default is 1.
 
-            gain (float) : Value gain added to the output.
+            gain (float) : Value gain added to the output. Default is 0.
 
-            spread (float) : Standard deviation of crappifier intensity for training on a range of crappifications. Default is 0. 
+            spread (float) : Standard deviation of crappifier intensity for training on a range of crappifications. Default is 0.
         """
         self.intensity = intensity
         self.gain = gain
         self.spread = spread
         
     def crappify(self, image : np.ndarray):
         return self._interpolate(image, np.random.poisson(image)) + self.gain
     
     def _interpolate(self, x, y):
         intensity = max(np.random.normal(self.intensity, self.spread), 0) if self.spread > 0 else self.intensity
         return x * (1 - intensity) + y * intensity
+    
+class SaltPepper(Crappifier):
+    def __init__(self, intensity : float = 0.5, gain : float = 0, spread : float = 0):
+        r"""Crappifier using salt and pepper noise (full value addition/deletion). Adds salt and pepper noise to a low resolution image.
+
+        Args:
+            intensity (float) : Percent of values to replace with salt and pepper noise. Default is 0.5.
+
+            gain (float) : Value gain added to the output. Default is 0.
+
+            spread (float) : Standard deviation of crappifier intensity for training on a range of crappifications. Default is 0.
+        """
+        self.intensity = intensity / 100
+        self.gain = gain
+        self.spread = spread
+        
+    def crappify(self, image : np.ndarray):
+        intensity = max(np.random.normal(self.intensity, self.spread), 0) if self.spread > 0 else self.intensity
+        return random_noise(image/255, mode="s&p", amount=intensity) * 255 + self.gain
```

### Comparing `pssr-1.0.2/pssr/data.py` & `pssr-1.1.0/pssr/data.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,240 +1,272 @@
-import torch, glob, os, random, czifile, warnings
+import torch, glob, os, random, czifile, tifffile, psutil, warnings
 import numpy as np
 from torch.utils.data import Dataset
 from pathlib import Path
+from tqdm import tqdm
 from PIL import Image
 from .crappifiers import Crappifier, Poisson
 
 class ImageDataset(Dataset):
-    def __init__(self, path : Path, hr_res : int = 512, lr_scale : int = 4, crappifier : Crappifier = Poisson(), val_split : float = 0.1, extension : str = "tif", mode : str = "L", rotation : bool = True, split_seed : int = 0, transforms : list[torch.nn.Module] = None):
+    def __init__(self, path : Path, hr_res : int = 512, lr_scale : int = 4, crappifier : Crappifier = Poisson(), n_frames : int = None, mode : str = "L", extension : str = "tif", val_split : float = 0.1, rotation : bool = True, split_seed : int = 0, transforms : list[torch.nn.Module] = None):
         r"""Training dataset for loading high-resolution images from individual files and returning high-low-resolution pairs, the latter receiving crappification.
 
         Dataset used for pre-tiled image files. For image sheets (e.g. .czi files), use :class:`SlidingDataset`.
 
-        LR mode for predictions (dataset loads only unmodified low-resolution images) can be enabled by
-        either inputting images less than or equal to LR size (`hr_res`/`lr_scale`) or by setting `lr_scale` = 1 and `hr_res` = LR resolution.
+        LR mode (dataset loads only unmodified low-resolution images for prediction) can be enabled by
+        either inputting images less than or equal to LR size (``hr_res``/``lr_scale``) or by setting ``lr_scale`` = 1 and ``hr_res`` = LR resolution.
 
         Args:
             path (Path) : Path to folder containing high-resolution images. Can also be a str.
 
             hr_res (int) : Resolution of high-resolution images. Images larger than this will be downscaled to this resolution. Images smaller will be padded. Default is 512.
 
             lr_scale (int) : Downscaling factor for low-resolution images to simulate undersampling. Choose a power of 2 for best results. Default is 4.
 
             crappifier (Crappifier) : Crappifier for degrading low-resolution images to simulate undersampling. Not used in LR mode. Default is :class:`Poisson`.
 
-            val_split (float) : Fraction of images to be held out for evaluation. Default is 0.1.
+            n_frames (int) : Amount of stacked frames per image, disregarding color channels. Can also be list of low-resolution and high-resolution stack amounts respectively. A value of None uses all stacked image frames. Default is None.
+
+            mode (str) : Color mode for loading images, e.g. "L" for grayscale, "RGB" for color. Default is "L".
 
             extension (str) : File extension of images. Default is "tif".
 
-            mode (str) : PIL image mode for loading images, e.g. "L" for grayscale, "RGB" for color. Default is "L".
+            val_split (float) : Proportion of images to be held out for evaluation/prediction. Default is 0.1.
 
-            rotation (bool) : Whether to randomly rotate images when loading data. Automatically set to False during evaluation if `val_split` is not less than 1, or in LR mode. Default is True.
+            rotation (bool) : Whether to randomly rotate and/or flip images when loading data. Only used during training if applicable. Default is True.
 
             split_seed (int) : Seed for random train/evaluation data splitting. A value of None splits the last images as evaluation. Default is 0.
 
             transforms (list[nn.Module]) : Additional final data transforms to apply. Default is None.
         """
         super().__init__()
         self.path = Path(path) if type(path) is str else path
-        assert self.path.exists(), f"Path {self.path} does not exist."
+        if not self.path.exists(): raise FileNotFoundError(f'Path "{self.path}" does not exist.')
 
         self.hr_files = sorted(glob.glob(f"*.{extension}", root_dir=self.path))
-        assert len(self.hr_files) > 0, f"No {extension} files exist in {self.path}."
+        if not len(self.hr_files) > 0: raise FileNotFoundError(f'No .{extension} files exist in path "{self.path}".')
 
-        self.val_idx = _get_val_idx(len(self.hr_files), val_split, split_seed)
+        self.mode = mode.upper()
+        self.n_frames = _get_n_frames(n_frames, self.mode)
 
-        self.is_lr = all([size <= hr_res//lr_scale for size in Image.open(Path(self.path, self.hr_files[0])).size]) or (lr_scale == 1)
-        self.crop_res = min(hr_res, max(Image.open(Path(self.path, self.hr_files[0])).size)) * (lr_scale if self.is_lr else 1)
+        self.slices, max_size = [], 0
+        for image_idx in range(len(self.hr_files)):
+            image = Image.open(Path(self.path, self.hr_files[image_idx]))
+            self.slices.append(1 if self.n_frames is None else image.n_frames // self.n_frames[0])
+            max_size = max(max(image.size), max_size)
+
+        self.val_idx = _get_val_idx(self.slices, val_split, split_seed)
+        self.is_lr = max_size <= hr_res//lr_scale or (lr_scale == 1)
+        if self.is_lr: print("LR mode is enabled, dataset will load only unmodified low-resolution images.")
+        self.crop_res = min(hr_res, max_size) * (lr_scale if self.is_lr else 1)
 
         self.hr_res = hr_res
         self.lr_scale = lr_scale
         self.crappifier = crappifier
-        self.mode = mode
-        self.rotation = rotation if val_split < 1 else False
+        self.rotation = rotation
         self.transforms = transforms
 
-    def __len__(self):
-        return len(self.hr_files)
-    
-    def __getitem__(self, idx):
-        assert idx < len(self), "Tried to retrieve invalid image."
+    def __getitem__(self, idx, pp=False):
+        if idx >= len(self): raise IndexError(f"Tried to retrieve invalid image. Index {idx} is not less than {len(self)} total image frame slices.")
 
-        hr = Image.open(Path(self.path, self.hr_files[idx]))
+        is_val = idx in self.val_idx or pp
+        image_idx, idx = _get_image_idx(idx, self.slices)
 
-        hr = _frame_channel(hr, self.mode)
+        hr = _load_image(self.path, self.hr_files[image_idx], self.mode, self.n_frames[0] if self.n_frames is not None else None, self.slices[image_idx], idx)
         
         if self.is_lr:
             # Rotation and crappifier is disabled in lr mode
             return _ready_lr(hr, self.hr_res//self.lr_scale, self.transforms)
 
-        return _gen_pair(hr, self.hr_res, self.lr_scale, self.rotation, self.crappifier, self.transforms)
+        return _gen_pair(hr, self.hr_res, self.lr_scale, False if is_val else self.rotation, self.crappifier, self.transforms, self.n_frames)
     
+    def __len__(self):
+        return sum(self.slices)
+    
+    def __repr__(self):
+        return f'ImageDataset from path "{self.path}"\n{len(self.hr_files)} files with {len(self)} total frame slices\nLR mode {"enabled" if self.is_lr else "disabled"}'
+
     def _get_name(self, idx):
-        return self.hr_files[idx].split('.')[0]
+        image_idx, idx = _get_image_idx(idx, self.slices)
+        return self.hr_files[image_idx].split('.')[0] + (f"_{idx}" if self.n_frames is not None else "")
 
-# TODO: Optimize dataloading
 class SlidingDataset(Dataset):
-    def __init__(self, path : Path, hr_res : int = 512, lr_scale : int = 4, crappifier : Crappifier = Poisson(), overlap : int = 128, val_split : float = 0.1, extension : str = "czi", mode : str = "L", rotation : bool = True, split_seed : int = 0, transforms : list[torch.nn.Module] = None):
+    def __init__(self, path : Path, hr_res : int = 512, lr_scale : int = 4, crappifier : Crappifier = Poisson(), overlap : int = 128, n_frames : int = None, stack : str = "TZ", mode : str = "L", extension : str = "czi", preload : bool = True, val_split : float = 0.1, rotation : bool = True, split_seed : int = 0, transforms : list[torch.nn.Module] = None):
         r"""Training dataset for loading high-resolution image tiles from image sheets and returning high-low-resolution pairs, the latter receiving crappification.
 
         Dataset used for image sheets (e.g. .czi files). For pre-tiled image files, use :class:`ImageDataset`.
 
-        LR mode for predictions (dataset loads only unmodified low-resolution images) can be enabled by setting `lr_scale` = 1 and `hr_res` = LR resolution.
+        LR mode (dataset loads only unmodified low-resolution images for prediction) can be enabled by setting ``lr_scale`` = 1 and ``hr_res`` = LR resolution.
 
         Args:
             path (Path) : Path to folder containing high-resolution images. Can also be a str.
 
             hr_res (int) : Resolution of high-resolution images. Images larger than this will be downscaled to this resolution. Images smaller will be padded. Default is 512.
 
             lr_scale (int) : Downscaling factor for low-resolution images to simulate undersampling. Choose a power of 2 for best results. Default is 4.
 
             crappifier (Crappifier) : Crappifier for degrading low-resolution images to simulate undersampling. Not used in LR mode. Default is :class:`Poisson`.
 
             overlap (int) : Overlapping pixels between neighboring tiles to increase effective dataset size. Default is 128.
 
-            val_split (float) : Fraction of images to be held out for evaluation. Default is 0.1.
+            n_frames (int) : Amount of stacked frames per image, disregarding color channels. Can also be list of low-resolution and high-resolution stack amounts respectively. A value of None uses all stacked image frames. Default is None.
+
+            stack (str) : Multiframe stack handling mode, e.g "T" for time stack, "Z" for z dimension stack, "TZ" or "ZT" for both, determining flattenting order. Only applicable if loading from czi. Default is "TZ".
+
+            mode (str) : Color mode for loading images, e.g. "L" for grayscale, "RGB" for color. Default is "L".
 
             extension (str) : File extension of images. Default is "czi".
 
-            mode (str) : PIL image mode for loading images, e.g. "L" for grayscale, "RGB" for color. Not applicable if loading from czi. Default is "L".
+            preload (bool) : Whether to preload images in memory (not VRAM) for faster dataloading. Default is True.
+
+            val_split (float) : Proportion of images to be held out for evaluation/prediction. Default is 0.1.
 
-            rotation (bool) : Whether to randomly rotate images when loading data. Automatically set to False during evaluation if `val_split` is not less than 1, or in LR mode. Default is True.
+            rotation (bool) : Whether to randomly rotate and/or flip images when loading data. Only used during training if applicable. Default is True.
 
             split_seed (int) : Seed for random train/evaluation data splitting. A value of None splits the last images as evaluation. Default is 0.
 
             transforms (list[nn.Module]) : Additional final data transforms to apply. Default is None.
         """
         super().__init__()
         self.path = Path(path) if type(path) is str else path
-        assert self.path.exists(), f"Path {self.path} does not exist."
+        if not self.path.exists(): raise FileNotFoundError(f'Path "{self.path}" does not exist.')
         
         self.hr_files = sorted(glob.glob(f"*.{extension}", root_dir=self.path))
-        assert len(self.hr_files) > 0, f"No {extension} files exist in {self.path}."
+        if not len(self.hr_files) > 0: raise FileNotFoundError(f'No .{extension} files exist in path "{self.path}".')
 
+        if not hr_res > overlap: raise ValueError(f"hr_res must be greater than overlap. Given values are {hr_res} and {overlap} respectively.")
         self.stride = hr_res - overlap
-        self.tiles = []
-        for file in self.hr_files:
-            image = _load_sheet(self.path, file, mode)
+        self.stack = stack.upper()
+        self.mode = mode.upper()
+        self.n_frames = _get_n_frames(n_frames, self.mode)
+        
+        self.preload = _preload(preload, [self.path], [self.hr_files], self.mode, self.stack)
+
+        self.tiles, self.slices = [], []
+        for image_idx in range(len(self.hr_files)):
+            image = self.preload[image_idx] if self.preload else _load_sheet(self.path, self.hr_files[image_idx], self.stack, self.mode)
             tiles_x, tiles_y = _n_tiles(image, hr_res, self.stride)
             self.tiles.append(tiles_x * tiles_y)
+            self.slices.append(1 if self.n_frames is None else image.shape[0] // self.n_frames[0])
 
-        self.val_idx = _get_val_idx(sum(self.tiles), val_split, split_seed)
-        
+        self.val_idx = _get_val_idx(self.slices, val_split, split_seed, self.tiles)
         self.is_lr = (lr_scale == 1)
+        if self.is_lr: print("LR mode is enabled, dataset will load only unmodified low-resolution images.")
         self.crop_res = hr_res * (lr_scale if self.is_lr else 1)
 
         self.hr_res = hr_res
         self.lr_scale = lr_scale
         self.crappifier = crappifier
-        self.mode = mode
-        self.rotation = rotation if val_split < 1 else False
+        self.rotation = rotation
         self.transforms = transforms
-        
-    def __len__(self):
-        return sum(self.tiles)
     
-    def __getitem__(self, idx):
-        assert idx < len(self), "Tried to retrieve invalid tile."
+    def __getitem__(self, idx, pp=False):
+        if idx >= len(self): raise IndexError(f"Tried to retrieve invalid image. Index {idx} is not less than {len(self)} total image frame slices.")
 
-        # Find idx tile across all tiles
-        image_idx = 0
-        for size in self.tiles:
-            if idx < size:
-                image = _sliding_window(_load_sheet(self.path, self.hr_files[image_idx], self.mode), self.hr_res, self.stride, idx)
-                break
-            else:
-                idx -= size
-                image_idx += 1
+        is_val = idx in self.val_idx or pp
+        image_idx, idx = _get_image_idx(idx, self.slices, self.tiles)
+
+        hr = _sliding_window(self.preload[image_idx] if self.preload else _load_sheet(self.path, self.hr_files[image_idx], self.stack, self.mode), self.hr_res, self.stride, self.n_frames[0], self.slices[image_idx], idx)
 
         if self.is_lr:
-            return _ready_lr(image, self.hr_res, self.transforms)
+            return _ready_lr(hr, self.hr_res, self.transforms)
 
-        return _gen_pair(image, self.hr_res, self.lr_scale, self.rotation, self.crappifier, self.transforms)
+        return _gen_pair(hr, self.hr_res, self.lr_scale, False if is_val else self.rotation, self.crappifier, self.transforms, self.n_frames)
+    
+    def __len__(self):
+        return sum([self.tiles[idx] * self.slices[idx] for idx in range(len(self.hr_files))])
+    
+    def __repr__(self):
+        return f'SlidingDataset from path "{self.path}"\n{len(self.hr_files)} files with {len(self)} total frame slices\nLR mode {"enabled" if self.is_lr else "disabled"}'
     
     def _get_name(self, idx):
-        image_idx = 0
-        for size in self.tiles:
-            if idx < size:
-                break
-            else:
-                idx -= size
-                image_idx += 1
-
+        image_idx, idx = _get_image_idx(idx, self.slices, self.tiles)
         return f"{self.hr_files[image_idx].split('.')[0]}_{idx}"
 
 class PairedImageDataset(Dataset):
-    def __init__(self, hr_path : Path, lr_path : Path, hr_res : int = 512, lr_scale : int = 4, val_split : float = 1, extension : str = "tif", mode : str = "L", rotation : bool = False, split_seed : int = None, transforms : list[torch.nn.Module] = None):
+    def __init__(self, hr_path : Path, lr_path : Path, hr_res : int = 512, lr_scale : int = 4, n_frames : int = None, mode : str = "L", extension : str = "tif", val_split : float = 1, rotation : bool = True, split_seed : int = None, transforms : list[torch.nn.Module] = None):
         r"""Testing dataset for loading paired high-low-resolution images without using crappification. Can also be used for approximating :class:`Crappifier` parameters.
 
         Args:
             hr_path (Path) : Path to folder containing high-resolution images. Can also be a str.
 
             lr_path (Path) : Path to folder containing low-resolution images. Can also be a str.
 
             hr_res (int) : Resolution of high-resolution images. Images larger than this will be downscaled to this resolution. Images smaller will be padded. Default is 512.
 
             lr_scale (int) : Downscaling factor for low-resolution images to simulate undersampling. Choose a power of 2 for best results. Default is 4.
 
-            val_split (float) : Fraction of images to be held out for evaluation. Default is 1.
+            n_frames (int) : Amount of stacked frames per image, disregarding color channels. Can also be list of low-resolution and high-resolution stack amounts respectively. A value of None uses all stacked image frames. Default is None.
+
+            mode (str) : Color mode for loading images, e.g. "L" for grayscale, "RGB" for color. Default is "L".
 
             extension (str) : File extension of images. Default is "tif".
 
-            mode (str) : PIL image mode for loading images, e.g. "L" for grayscale, "RGB" for color. Default is "L".
+            val_split (float) : Proportion of images to be held out for evaluation/prediction. Default is 1.
 
-            rotation (bool) : Whether to randomly rotate images when loading data. Default is False.
+            rotation (bool) : Whether to randomly rotate and/or flip images when loading data. Only used during training if applicable. Default is True.
 
             split_seed (int) : Seed for random train/evaluation data splitting. A value of None splits the last images as evaluation. Default is None.
 
             transforms (list[nn.Module]) : Additional final data transforms to apply. Default is None.
         """
         super().__init__()
         self.hr_path = Path(hr_path) if type(hr_path) is str else hr_path
         self.lr_path = Path(lr_path) if type(lr_path) is str else lr_path
-        assert self.hr_path.exists() and self.lr_path.exists(), f"One path {self.hr_path} or {self.lr_path} does not exist."
-        if self.hr_path == self.lr_path:
-            warnings.warn("hr_path is equal to lr_path, this should not be done except for testing purposes. Consider using ImageDataset instead.")
+        for path in [self.hr_path, self.lr_path]:
+            if not path.exists(): raise FileNotFoundError(f'Path "{path}" does not exist.')
+        if self.hr_path == self.lr_path: warnings.warn("hr_path is equal to lr_path! Consider using ImageDataset instead.", stacklevel=2)
 
         self.hr_files = sorted(glob.glob(f"*.{extension}", root_dir=self.hr_path))
         self.lr_files = sorted(glob.glob(f"*.{extension}", root_dir=self.lr_path))
         for files, path in zip([self.hr_files, self.lr_files], [self.hr_path, self.lr_path]):
-            assert len(files) > 0, f"No {extension} files exist in {path}."
-        assert len(self.hr_files) == len(self.lr_files), "Length mismatch between high-low-resolution images."
+            if not len(files) > 0: raise FileNotFoundError(f'No .{extension} files exist in path "{path}".')
+        if len(self.hr_files) != len(self.lr_files): raise FileNotFoundError(f"Mismatch between amounts of high-low-resolution images. Found {len(self.hr_files)} high-resolution and {len(self.lr_files)} low-resolution images.")
+
+        self.mode = mode.upper()
+        self.n_frames = _get_n_frames(n_frames, self.mode)
 
-        self.val_idx = _get_val_idx(len(self.hr_files), val_split, split_seed)
+        self.slices, max_size = [], 0
+        for image_idx in range(len(self.hr_files)):
+            image = Image.open(Path(self.hr_path, self.hr_files[image_idx]))
+            self.slices.append(1 if self.n_frames is None else image.n_frames // self.n_frames[0])
+            max_size = max(max(image.size), max_size)
 
+        self.val_idx = _get_val_idx(self.slices, val_split, split_seed)
         self.is_lr = False
-        self.crop_res = min(hr_res, max(Image.open(Path(self.hr_path, self.hr_files[0])).size))
+        self.crop_res = min(hr_res, max_size)
 
         self.hr_res = hr_res
         self.lr_scale = lr_scale
-        self.mode = mode
         self.rotation = rotation
         self.transforms = transforms
-
-    def __len__(self):
-        return len(self.hr_files)
     
-    def __getitem__(self, idx):
-        assert idx < len(self), "Tried to retrieve invalid image."
+    def __getitem__(self, idx, pp=False):
+        if idx >= len(self): raise IndexError(f"Tried to retrieve invalid image. Index {idx} is not less than {len(self)} total image frame slices.")
 
-        hr = Image.open(Path(self.hr_path, self.hr_files[idx]))
-        lr = Image.open(Path(self.lr_path, self.lr_files[idx]))
+        is_val = idx in self.val_idx or pp
+        image_idx, idx = _get_image_idx(idx, self.slices)
 
-        hr = _frame_channel(hr, self.mode)
-        lr = _frame_channel(lr, self.mode)
+        hr = _load_image(self.hr_path, self.hr_files[image_idx], self.mode, self.n_frames[0] if self.n_frames is not None else None, self.slices[image_idx], idx)
+        lr = _load_image(self.lr_path, self.lr_files[image_idx], self.mode, self.n_frames[0] if self.n_frames is not None else None, self.slices[image_idx], idx)
 
-        return _transform_pair(hr, lr, self.hr_res, self.hr_res//self.lr_scale, self.rotation, self.transforms)
+        return _transform_pair(hr, lr, self.hr_res, self.hr_res//self.lr_scale, False if is_val else self.rotation, self.transforms, self.n_frames)
+    
+    def __len__(self):
+        return sum(self.slices)
+    
+    def __repr__(self):
+        return f'PairedImageDataset from paths "{self.hr_path}" and "{self.lr_path}"\n{len(self.hr_files)+len(self.lr_files)} files with {len(self)} total frame slices'
 
     def _get_name(self, idx):
-        return self.lr_files[idx].split('.')[0]
+        image_idx, idx = _get_image_idx(idx, self.slices)
+        return self.lr_files[image_idx].split('.')[0] + (f"_{idx}" if self.n_frames is not None else "")
 
 class PairedSlidingDataset(Dataset):
-    def __init__(self, hr_path : Path, lr_path : Path, hr_res : int = 512, lr_scale : int = 4, overlap : int = 128, val_split : float = 1, extension : str = "czi", mode : str = "L", rotation : bool = False, split_seed : int = None, transforms : list[torch.nn.Module] = None):
+    def __init__(self, hr_path : Path, lr_path : Path, hr_res : int = 512, lr_scale : int = 4, overlap : int = 128, n_frames : int = None, stack : str = "TZ", mode : str = "L", extension : str = "czi", preload : bool = True, val_split : float = 1, rotation : bool = True, split_seed : int = None, transforms : list[torch.nn.Module] = None):
         r"""Testing dataset for loading high-low-resolution image tiles from image sheets without crappification. Can also be used for approximating :class:`Crappifier` parameters.
 
         Dataset used for image sheets (e.g. .czi files). For pre-tiled image files, use :class:`ImageDataset`.
 
         Args:
             hr_path (Path) : Path to folder containing high-resolution images. Can also be a str.
 
@@ -242,274 +274,374 @@
 
             hr_res (int) : Resolution of high-resolution images. Images larger than this will be downscaled to this resolution. Images smaller will be padded. Default is 512.
 
             lr_scale (int) : Downscaling factor for low-resolution images to simulate undersampling. Choose a power of 2 for best results. Default is 4.
 
             overlap (int) : Overlapping pixels between neighboring tiles to increase effective dataset size. Default is 128.
 
-            val_split (float) : Fraction of images to be held out for evaluation. Default is 1.
+            n_frames (int) : Amount of stacked frames per image, disregarding color channels. Can also be list of low-resolution and high-resolution stack amounts respectively. A value of None uses all stacked image frames. Default is None.
+
+            stack (str) : Multiframe stack handling mode, e.g "T" for time stack, "Z" for z dimension stack, "TZ" or "ZT" for both, determining flattenting order. Only applicable if loading from czi. Default is "TZ".
+
+            mode (str) : Color mode for loading images, e.g. "L" for grayscale, "RGB" for color. Default is "L".
 
             extension (str) : File extension of images. Default is "czi".
 
-            mode (str) : PIL image mode for loading images, e.g. "L" for grayscale, "RGB" for color. Not applicable if loading from czi. Default is "L".
+            preload (bool) : Whether to preload images in memory (not VRAM) for faster dataloading. Default is True.
+
+            val_split (float) : Proportion of images to be held out for evaluation/prediction. Default is 1.
 
-            rotation (bool) : Whether to randomly rotate images when loading data. Default is False.
+            rotation (bool) : Whether to randomly rotate and/or flip images when loading data. Only used during training if applicable. Default is True.
 
             split_seed (int) : Seed for random train/evaluation data splitting. A value of None splits the last images as evaluation. Default is None.
 
             transforms (list[nn.Module]) : Additional final data transforms to apply. Default is None.
         """
         super().__init__()
         self.hr_path = Path(hr_path) if type(hr_path) is str else hr_path
         self.lr_path = Path(lr_path) if type(lr_path) is str else lr_path
-        assert self.hr_path.exists() and self.lr_path.exists(), f"One path {self.hr_path} or {self.lr_path} does not exist."
-        if self.hr_path == self.lr_path:
-            warnings.warn("hr_path is equal to lr_path, this should not be done except for testing purposes. Consider using SlidingDataset instead.")
+        for path in [self.hr_path, self.lr_path]:
+            if not path.exists(): raise FileNotFoundError(f'Path "{path}" does not exist.')
+        if self.hr_path == self.lr_path: warnings.warn("hr_path is equal to lr_path! Consider using SlidingDataset instead.", stacklevel=2)
         
         self.hr_files = sorted(glob.glob(f"*.{extension}", root_dir=self.hr_path))
         self.lr_files = sorted(glob.glob(f"*.{extension}", root_dir=self.lr_path))
         for files, path in zip([self.hr_files, self.lr_files], [self.hr_path, self.lr_path]):
-            assert len(files) > 0, f"No {extension} files exist in {path}."
-        assert len(self.hr_files) == len(self.lr_files), "Length mismatch between high-low-resolution images."
+            if not len(files) > 0: raise FileNotFoundError(f'No .{extension} files exist in path "{path}".')
+        if len(self.hr_files) != len(self.lr_files): raise FileNotFoundError(f"Mismatch between amounts of high-low-resolution images. Found {len(self.hr_files)} high-resolution and {len(self.lr_files)} low-resolution images.")
 
+        if not hr_res > overlap: raise ValueError(f"hr_res must be greater than overlap. Given values are {hr_res} and {overlap} respectively.")
         self.stride = hr_res - overlap
-
-        self.tiles = []
-        for file in self.hr_files:
-            image = _load_sheet(self.hr_path, file, mode)
+        self.stack = stack.upper()
+        self.mode = mode.upper()
+        self.n_frames = _get_n_frames(n_frames, self.mode)
+
+        self.preload = _preload(preload, [self.hr_path, self.lr_path], [self.hr_files, self.lr_files], self.mode, self.stack)
+
+        self.tiles, self.slices = [], []
+        for image_idx in range(len(self.hr_files)):
+            image = self.preload[0][image_idx] if self.preload else _load_sheet(self.hr_path, self.hr_files[image_idx], self.stack, self.mode)
             tiles_x, tiles_y = _n_tiles(image, hr_res, self.stride)
             self.tiles.append(tiles_x * tiles_y)
+            self.slices.append(1 if self.n_frames is None else image.shape[0] // self.n_frames[0])
 
-        self.val_idx = _get_val_idx(sum(self.tiles), val_split, split_seed)
-        
+        self.val_idx = _get_val_idx(self.slices, val_split, split_seed, self.tiles)
         self.is_lr = False
         self.crop_res = hr_res
 
         self.hr_res = hr_res
         self.lr_scale = lr_scale
-        self.mode = mode
         self.rotation = rotation
         self.transforms = transforms
-
-    def __len__(self):
-        return sum(self.tiles)
     
-    def __getitem__(self, idx):
-        assert idx < len(self), "Tried to retrieve invalid tile."
+    def __getitem__(self, idx, pp=False):
+        if idx >= len(self): raise IndexError(f"Tried to retrieve invalid image. Index {idx} is not less than {len(self)} total image frame slices.")
 
-        # Find idx tile across all tiles
-        image_idx = 0
-        for size in self.tiles:
-            if idx < size:
-                hr = _sliding_window(_load_sheet(self.hr_path, self.hr_files[image_idx], self.mode), self.hr_res, self.stride, idx)
-                lr = _sliding_window(_load_sheet(self.lr_path, self.lr_files[image_idx], self.mode), self.hr_res//self.lr_scale, self.stride//self.lr_scale, idx)
-                break
-            else:
-                idx -= size
-                image_idx += 1
+        is_val = idx in self.val_idx or pp
+        image_idx, idx = _get_image_idx(idx, self.slices, self.tiles)
+
+        hr = _sliding_window(self.preload[0][image_idx] if self.preload else _load_sheet(self.hr_path, self.hr_files[image_idx], self.stack, self.mode), self.hr_res, self.stride, self.n_frames[0], self.slices[image_idx], idx)
+        lr = _sliding_window(self.preload[1][image_idx] if self.preload else _load_sheet(self.lr_path, self.lr_files[image_idx], self.stack, self.mode), self.hr_res//self.lr_scale, self.stride//self.lr_scale, self.n_frames[0], self.slices[image_idx], idx)
 
-        return _transform_pair(hr, lr, self.hr_res, self.hr_res//self.lr_scale, self.rotation, self.transforms)
+        return _transform_pair(hr, lr, self.hr_res, self.hr_res//self.lr_scale, False if is_val else self.rotation, self.transforms, self.n_frames)
+    
+    def __len__(self):
+        return sum([self.tiles[idx] * self.slices[idx] for idx in range(len(self.hr_files))])
+    
+    def __repr__(self):
+        return f'PairedSlidingDataset from paths "{self.hr_path}" and "{self.lr_path}"\n{len(self.hr_files)+len(self.lr_files)} files with {len(self)} total frame slices'
     
     def _get_name(self, idx):
-        image_idx = 0
-        for size in self.tiles:
-            if idx < size:
-                break
-            else:
-                idx -= size
-                image_idx += 1
-
+        image_idx, idx = _get_image_idx(idx, self.slices, self.tiles)
         return f"{self.lr_files[image_idx].split('.')[0]}_{idx}"
 
-# TODO: preprocess_dataset
-def preprocess_hr(path : Path, hr_res : int = 512, lr_scale : int = 4, crappifier : Crappifier = Poisson(), extension : str = "tif", mode : str = "L"):
-    r"""Preprocesses and crappifies low-resolution images from high-resolution images.
-    However, it is better for most use cases to process data at runtime using a dataset such as :class:`ImageDataset` to save disk space at the cost of negligible CPU usage.
-
+def preprocess_dataset(dataset : Dataset, preprocess_hr : bool = False, out_dir : str = "preprocess"):
+    r"""Saves processed frame slices from a given dataset, including processes such as crappification or cropping/padding.
+    
     Args:
-        path (Path) : Path to folder containing high-resolution images. Can also be a str.
+        dataset (Dataset) : Dataset to load images from. Preprocessing is determined by the dataloading procedure as specified in dataset arguments. Rotation is disabled.
 
-        hr_res (int) : Resolution of high-resolution images. Images larger than this will be downscaled to this resolution. Default is 512.
+        preprocess_hr (bool) : Whether to save preprocessed high-resolution images in addition to preprocessed low-resolution images. Default is False.
 
-        lr_scale (int) : Downscaling factor for low-resolution images to simulate undersampling. Choose a power of 2 for best results. Default is 4.
-
-        crappifier (Crappifier) : Crappifier for degrading low-resolution images to simulate undersampling. Default is :class:`Poisson`.
-
-        extension (str) : File extension of images. Default is "tif".
-
-        mode (str) : PIL image mode for loading images, e.g. "L" for grayscale, "RGB" for color. Default is "L".
+        out_dir (str) : Directory to save preprocessed images. Default is "preprocess".
     """
-    path = Path(path) if type(path) is str else path
-    assert path.exists(), f"Path {path} does not exist."
-
-    lr_path = Path(path.parent, "pp/lr")
-    os.makedirs(lr_path, exist_ok=True)
-
-    hr_files = sorted(glob.glob(f"*.{extension}", root_dir=path))
-
-    if Image.open(Path(path, hr_files[0])).size != (hr_res, hr_res):
-        print("High-resolution image dimensions are not square and/or do not match hr_res, cropped hr files will be saved in addition to lr.")
-
-        differing = True
-        hr_path = Path(path.parent, "pp/hr")
-        os.makedirs(hr_path, exist_ok=True)
-    else:
-        differing = False
-
-    for file in hr_files:
-        hr = Image.open(Path(path, file))
-
-        hr = _frame_channel(hr, mode)
-
-        hr, lr = _gen_pair(hr, hr_res, lr_scale, False, crappifier, None)
+    os.makedirs(f"{out_dir}/lr", exist_ok=True)
+    if preprocess_hr:
+        os.makedirs(f"{out_dir}/hr", exist_ok=True)
+
+    progress = tqdm(range(len(dataset)))
+    for idx in progress:
+        hr, lr = dataset.__getitem__(idx, pp=True)
+        hr, lr = np.asarray(hr, dtype=np.uint8), np.asarray(lr, dtype=np.uint8)
+        
+        tifffile.imwrite(f"{out_dir}/lr/{dataset._get_name(idx)}.tif", lr)
+        if preprocess_hr:
+            tifffile.imwrite(f"{out_dir}/hr/{dataset._get_name(idx)}.tif", hr)
 
-        # TODO: Save multiframe images
-        Image.fromarray(np.moveaxis(np.asarray(lr, dtype=np.uint8), 0, -1).squeeze()).save(Path(lr_path, file))
-        if differing:
-            Image.fromarray(np.moveaxis(np.asarray(hr, dtype=np.uint8), 0, -1).squeeze()).save(Path(hr_path, file))
+# TODO: crappify_images
 
-def _gen_pair(hr, hr_res, lr_scale, rotation, crappifier, transforms):
+def _gen_pair(hr, hr_res, lr_scale, rotation, crappifier, transforms, n_frames):
     r"""Creates training ready pair of images from a single high-resolution image.
     """
-    # Square crop
-    hr = np.stack([_square_crop(channel, hr_res) for channel in hr])
-
-    # Ensure image has hr_res
-    if hr.shape[1] < hr_res:
-        hr = np.stack([np.pad(channel, pad_width=[[0,hr_res-hr.shape[1]]]*2, mode="reflect") for channel in hr])
-    # if hr.shape[1] > hr_res:
-    #     hr = np.stack([Image.fromarray(channel).resize(([hr_res]*2), Image.Resampling.BILINEAR) for channel in hr])
+    hr = _square_crop(hr, hr_res)
+    hr = _pad_image(hr, hr_res)
     
     # Set random rotation and flip in xy axis
     if rotation:
         hr = np.rot90(hr, axes=(1,2)) if bool(random.getrandbits(1)) else hr
         hr = np.flip(hr, axis=random.choice((1,2,(1,2))))
 
     # Crappification
     lr = np.stack([Image.fromarray(channel).resize(([hr_res//lr_scale]*2), Image.Resampling.BILINEAR) for channel in hr])
     if crappifier is not None:
-        # Allows either Crappifier or nn.Module to be used as a crappifier
+        # Allows either Crappifier or nn.Module (or any callable function) to be used as a crappifier
         lr = crappifier.crappify(lr) if issubclass(type(crappifier), Crappifier) else crappifier(lr)
         lr = np.clip(lr.round(), 0, 255)
 
+    hr = _slice_center(hr, n_frames)
+
     return _tensor_ready(hr, transforms), _tensor_ready(lr, transforms)
 
-def _transform_pair(hr, lr, hr_res, lr_res, rotation, transforms):
+def _transform_pair(hr, lr, hr_res, lr_res, rotation, transforms, n_frames):
     r"""Same as _gen_pair, but uses paired high-low-resolution images with no crappifier.
     """
-    hr = np.stack([_square_crop(channel, hr_res) for channel in hr])
-    lr = np.stack([_square_crop(channel, lr_res) for channel in lr])
+    hr = _square_crop(hr, hr_res)
+    lr = _square_crop(lr, lr_res)
 
-    if hr.shape[1] < hr_res:
-        hr = np.stack([np.pad(channel, pad_width=[[0,hr_res-hr.shape[1]]]*2, mode="reflect") for channel in hr])
-        lr = np.stack([np.pad(channel, pad_width=[[0,lr_res-lr.shape[1]]]*2, mode="reflect") for channel in lr])
+    hr = _pad_image(hr, hr_res)
+    lr = _pad_image(lr, lr_res)
 
     if rotation:
         choice = bool(random.getrandbits(1)), random.choice((0,1,(0,1)))
 
         hr, lr = np.rot90(hr, axes=(1,2)) if choice[0] else hr, np.rot90(lr, axes=(1,2)) if choice[0] else lr
         hr, lr = np.flip(hr, axis=choice[1]), np.flip(lr, axis=choice[1])
+    
+    hr = _slice_center(hr, n_frames)
 
     return _tensor_ready(hr, transforms), _tensor_ready(lr, transforms)
 
 def _ready_lr(lr, lr_res, transforms):
     r"""Processes lr images for prediction. Same as transform pair but without rotation.
     """
-    lr = np.stack([_square_crop(channel, lr_res) for channel in lr])
-
-    if lr.shape[1] < lr_res:
-        lr = np.stack([np.pad(channel, pad_width=[[0,lr_res-lr.shape[1]]]*2, mode="reflect") for channel in lr])
+    lr = _square_crop(lr, lr_res)
+    lr = _pad_image(lr, lr_res)
 
     return _tensor_ready(lr, transforms)
 
-def _frame_channel(image, mode):
-    # Create frame dimension
-    if image.n_frames > 1:
-        image = np.stack([np.asarray(image.seek(frame).convert(mode), dtype=np.uint8) for frame in range(image.n_frames)])
-    else:
-        image = np.asarray(image.convert(mode), dtype=np.uint8)[np.newaxis, :, :]
-
-    # Merge channel into frame dimension
-    if len(image.shape) > 3:
-        image = np.reshape(np.moveaxis(image, -1, 0), [-1, *image.shape[1:3]])
-    
-    return image
-
 def _tensor_ready(image, transforms):
-    r"""nn.Module ready axes.
-    """
     image = torch.tensor(image.copy(), dtype=torch.float)
 
     # Additional nn.Module user transforms
     if transforms is not None:
         for transform in transforms:
             image = transform(image)
     
     return image
 
 def _square_crop(image, max_res):
-    if list(image.shape) == [max_res]*2:
-        return image
+    height, width = image.shape[-2:]
 
-    height, width = image.shape
-    size = min(height, width, max_res)
+    if [height, width] == [max_res]*2:
+        return image
     
-    start_row = (height - size) // 2
-    start_col = (width - size) // 2
+    size = min(height, width, max_res)
+    start_x = (height - size) // 2
+    start_y = (width - size) // 2
     
-    return image[start_row:start_row + size, start_col:start_col + size]
+    return image[:, start_x:start_x + size, start_y:start_y + size]
+
+def _pad_image(image, res):
+    if image.shape[-1] < res:
+        return np.stack([np.pad(channel, pad_width=[[0,res-image.shape[-1]]]*2, mode="reflect") for channel in image])
+    return image
+
+def _preload(preload, path, files, mode, stack):
+    if not preload:
+        return False
+    
+    size = sum([sum([os.stat(Path(idx_path, file)).st_size for file in idx_files]) for idx_path, idx_files in zip(path, files)]) / 10**9
+    memory = psutil.virtual_memory().available / 10**9
+    if size > memory:
+        warnings.warn(f"Total dataset size {size:.2f}GB is greater than available memory of {memory:.2f}GB. Consider disabling preloading to avoid potential slowdowns.", stacklevel=2)
+
+    print(f"Preloading {sum([len(item) for item in files])} images into memory...")
+    preload = [[_load_sheet(idx_path, file, stack, mode) for file in idx_files] for idx_path, idx_files in zip(path, files)]
+    return preload[0] if len(preload) == 1 else preload
+
+def _load_image(path, file, mode, n_frames, slices, idx):
+    hr = Image.open(Path(path, file))
+
+    hr = _frame_channel(hr, mode)
+    return _slice_image(hr, n_frames, slices, idx)
 
-# TODO: T stacking option
-def _load_sheet(path, file, mode):
+def _load_sheet(path, file, stack, mode):
     extension = file.split(".")[-1]
     if extension == "czi":
-        image = czifile.imread(Path(path, file))[0,0,0,:,:,:,:,0] # Only CZYX, disregard T?
-        image = np.reshape(np.moveaxis(image, [0,2], [1,3]), [-1, image.shape[3], image.shape[2]]) # CZYX to ZCXY to CXY
+        # Retrieve same channel information from czi regardless of channel order
+        image = czifile.CziFile(Path(path, file))
+        out_axes = "TZCXY"
+
+        # Get info only from out_axes axes
+        slice_idx, slice_axes = [], []
+        for axis in image.axes:
+            if axis not in out_axes:
+                slice_idx.append(0)
+            else:
+                slice_idx.append(slice(None))
+                slice_axes.append(axis)
+        image = image.asarray()[tuple(slice_idx)]
+
+        # Rearrange axes to out_axes order
+        axes_idx = [out_axes.rfind(axis) for axis in slice_axes]
+        image = np.moveaxis(image, range(len(image.shape)), axes_idx)
+
+        # TODO: Assumes images must have all out_axes?
+        # Disregard additional channels and/or reorder
+        if mode == "L":
+            image = np.mean(image, axis=2)
+        match stack:
+            case "T":
+                image = image[:,0]
+            case "Z":
+                image = image[0]
+            case "ZT":
+                image = np.moveaxis(image, 0, 1)
+            case "TZ":
+                pass
+            case _:
+                raise ValueError(f"Stack type {stack} is not valid.")
+        
+        # Flatten channel dimensions
+        image = np.reshape(image, [-1, image.shape[-2], image.shape[-1]])
         if image.max() != 0:
-            image = image / image.max() * 255
+            image = image / (image.max() / 255)
         return image.astype(np.uint8)
     else:
         image = Image.open(Path(path, file))
         return _frame_channel(image, mode)
 
-def _sliding_window(image, size, stride, idx):
+def _sliding_window(image, size, stride, n_frames, n_slices, idx):
     tiles_x, tiles_y = _n_tiles(image, size, stride)
-    if idx > tiles_x * tiles_y:
-        return tiles_x * tiles_y
+    tile_idx = idx // n_slices
 
-    start_x = idx // tiles_y * stride
-    start_y = idx % tiles_y * stride
+    start_x = tile_idx // tiles_y * stride
+    start_y = tile_idx % tiles_y * stride
 
-    return image[:, start_x:start_x + size, start_y:start_y + size]
+    image = image[..., start_x:start_x + size, start_y:start_y + size]
+
+    return _slice_image(image, n_frames, n_slices, idx)
+
+def _frame_channel(image, mode):
+    # Create frame dimension
+    if image.n_frames > 1:
+        image = np.stack([np.asarray(_seek_channel(image, frame).convert(mode), dtype=np.uint8) for frame in range(image.n_frames)])
+    else:
+        image = np.asarray(image.convert(mode), dtype=np.uint8)[np.newaxis, :, :]
+    
+    return image
+
+def _slice_image(image, n_frames, n_slices, idx):
+    if n_frames == None:
+        return image
+    
+    # Only need to calculate residual idx of specific tile
+    idx = idx % n_slices
+    idx *= n_frames
+    return image[idx:idx+n_frames]
+
+def _slice_center(image, n_frames):
+    if n_frames is None or n_frames[0] == n_frames[1] or n_frames[1] > image.shape[-3]:
+        return image
+
+    center = image.shape[-3] // 2
+    half = n_frames[1] // 2
+    if n_frames[1] % 2 == 0:
+        return image[...,center - half:center + half,:,:]
+    else:
+        return image[...,center - half:center + half + 1,:,:]
+
+def _seek_channel(image, idx):
+    # Because we can't have nice things...
+    image.seek(idx)
+    return image
 
 def _n_tiles(image, size, stride):
-    x, y = image.shape[1:]
+    x, y = image.shape[-2:]
 
     tiles_x = max(0, (x - size) // stride + 1)
     tiles_y = max(0, (y - size) // stride + 1)
     return tiles_x, tiles_y
 
-def _get_val_idx(idx_len, split, seed):
-    val_idx = list(range(idx_len))
+def _get_n_frames(n_frames, mode):
+    if n_frames is None:
+        return n_frames
+    
+    n_frames = _force_list(n_frames)
+    n_frames = n_frames*2 if len(n_frames) == 1 else n_frames
+    n_frames = [item*3 for item in n_frames] if mode == "RGB" else n_frames
+    return n_frames # [in (low-resolution), out (high-resolution)]
+
+def _force_list(item):
+    # Because we still can't have nice things...
+    if type(item) is int:
+        return [item]
+    elif type(item) is not list:
+        return list(item)
+    return item
+
+def _get_image_idx(idx, slices, tiles=None):
+    tiles = [1]*len(slices) if tiles is None else tiles
+
+    image_idx = 0
+    for slice, tile in zip(slices, tiles):
+        if idx < slice * tile:
+            return image_idx, idx
+        else:
+            idx -= slice * tile
+            image_idx += 1
+
+def _get_val_idx(slices, split, seed, tiles=None):
+    # Tiles are individual images
+    if tiles is not None:
+        tile_slices = []
+        for slice, tile in zip(slices, tiles):
+            tile_slices.extend([slice]*tile)
+        slices = tile_slices
 
+    # Select random image indexes as validation
+    val_slices = list(range(len(slices)))
     if seed is not None and split < 1:
         np.random.seed(seed)
-        np.random.shuffle(val_idx)
+        np.random.shuffle(val_slices)
+    val_slices = val_slices[-max(1,int(split*len(slices))):]
     
-    return val_idx[-int(split*idx_len):]
+    # Convert image indexes to frame indexes for dataloading
+    val_idx, idx = [], 0
+    for slice_idx, slice in enumerate(slices):
+        if slice_idx in val_slices:
+            val_idx.extend(range(idx,idx+slice))
+        idx += slice
+
+    return val_idx
 
 def _invert_idx(idx, idx_len):
     idx_range = np.arange(idx_len)
     inverse = np.logical_not(np.isin(idx_range, idx))
     return idx_range[inverse]
 
 class _RandomIterIdx:
-    def __init__(self, idx):
+    def __init__(self, idx, seed=False):
         self.idx = idx
+        self.seed = seed
         
     def __iter__(self):
         random_idx = self.idx.copy()
-        random.shuffle(random_idx)
+        if self.seed:
+            np.random.seed(0)
+            np.random.shuffle(random_idx)
+        else:
+            random.shuffle(random_idx)
         yield from random_idx
     
     def __len__(self):
         return len(self.idx)
```

### Comparing `pssr-1.0.2/pssr/loss.py` & `pssr-1.1.0/pssr/loss.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
             win_size (int) : Size of Gaussian window. Must be odd. Default is 11.
 
             win_sigma (float) : Sigma for distribution of Gaussian window. Default is 1.5.
 
             ms (bool) : Whether to use MS-SSIM over basic SSIM. Default is True.
 
-            kwargs (dict[str, Any]) : Keyword arguments for pytorch_msssim.
+            kwargs (dict[str, Any]) : Keyword arguments for ``pytorch_msssim``.
         """
         super().__init__()
 
         kwargs = {} if kwargs is None else kwargs
         self.ssim = MS_SSIM(channel=channels, win_size=win_size, win_sigma=win_sigma, data_range=1, **kwargs) if ms else SSIM(channel=channels, win_size=win_size, win_sigma=win_sigma, data_range=1, **kwargs)
 
         if mix < 1:
```

### Comparing `pssr-1.0.2/pssr/models/_blocks.py` & `pssr-1.1.0/pssr/models/_blocks.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 import numpy as np
 
 class Reconstruction(nn.Module):
-    def __init__(self, channels : int, hidden : int, scale : int = 4):
+    def __init__(self, in_channels : int, out_channels : int, hidden : int, scale : int = 4):
         super().__init__()
 
-        self.pre = nn.Conv2d(in_channels=hidden + channels, out_channels=scale**2 * hidden, kernel_size=3, padding=1)
-        self.conv = nn.Conv2d(in_channels=hidden, out_channels=channels, kernel_size=3, padding=1)
+        self.pre = nn.Conv2d(in_channels=hidden + in_channels, out_channels=scale**2 * hidden, kernel_size=3, padding=1)
+        self.conv = nn.Conv2d(in_channels=hidden, out_channels=out_channels, kernel_size=3, padding=1)
 
         self.scale = scale
 
     def forward(self, x):
         x = F.relu(self.pre(x), inplace=True)
         x = self.conv(F.pixel_shuffle(x, self.scale))
         return x
@@ -31,9 +31,8 @@
     def forward(self, x):
         batch, size = x.shape[0], np.prod(x.shape[2:])
         x = x.flatten(start_dim=1)[:, np.newaxis, :] - self.centers[:, np.newaxis].to(device=x.device)
         x = torch.sigmoid(x * self.sigma)
         diff = torch.cat([torch.ones((batch, 1, size), device=x.device), x], dim=1) - torch.cat([x, torch.zeros((batch, 1, size), device=x.device)], dim=1)
 
         diff = diff.sum(dim=-1)
-        # diff[:, -2] += diff[:, -1]
         return diff[:, :-1]
```

### Comparing `pssr-1.0.2/pssr/models/resunet.py` & `pssr-1.1.0/pssr/models/resunet.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from ._blocks import Reconstruction
+from ..data import _force_list
 
 class ResUNet(nn.Module):
     def __init__(self, channels : int = 1, hidden : list[int] = [64, 128, 256, 512, 1024], scale : int = 4, depth : int = 3):
         r"""A modified Residual UNet as detailed in Zhang et al., 2017 with an additional image upscaling block.
 
         Args:
-            channels (int) : Number of channels in image data.
+            channels (int) : Number of channels in image data. Can also be a list of in channels and out channels respectively.
 
             hidden (list[int]) : Elementwise list of hidden layer channels controlling width and length of model.
 
             scale (int) : Upscaling factor for predictions. Choose a power of 2 for best results. Default is 4.
 
             depth (int) : Number of hidden layers per residual block. Default is 3.
         """
         super().__init__()
+        channels = _force_list(channels)
+        channels = channels*2 if len(channels) == 1 else channels
         
-        self.norm = nn.BatchNorm2d(channels)
+        self.norm = nn.BatchNorm2d(channels[0])
         
         self.encoder, self.decoder, self.upscale = nn.ModuleList(), nn.ModuleList(), nn.ModuleList()
-        layers = [channels, *hidden]
+        layers = [channels[0], *hidden]
         n_layers = len(layers) - 1
         for layer_idx in range(n_layers):
             self.encoder.append(_ResBlock(in_channels=layers[layer_idx], out_channels=layers[layer_idx+1], depth=depth))
             if layer_idx + 1 < n_layers:
                 self.decoder.append(_ResBlock(in_channels=layers[-layer_idx-1] - int(layers[-layer_idx-2]/2), out_channels=layers[-layer_idx-2], depth=depth))
                 self.upscale.append(nn.PixelShuffle(2))
 
-        self.reconstuction = Reconstruction(channels, hidden[0], scale)
+        self.reconstuction = Reconstruction(channels[0], channels[1], hidden[0], scale)
 
     def forward(self, x):
         x = x / 128 - 1 # Scale input approx from [0, 255] to [-1, 1]
         x = self.norm(x)
 
         skips = [x]
         for idx, layer in enumerate(self.encoder):
@@ -46,15 +49,15 @@
         for idx, layer in enumerate(self.decoder):
             x = self.upscale[idx](x) # Upscale
 
             x = torch.cat([x, skips.pop()], dim=1) # ResBlock
             x = layer(x)
 
         x = torch.cat([x, skips.pop()], dim=1) # Final skip connection before reconstruction
-        assert len(skips) == 0, "Skip connection mismatch between encoder and decoder."
+        if len(skips) != 0: raise IndexError(f"Skip connection mismatch between encoder and decoder. {len(skips)} skip connections are unused.")
 
         x = self.reconstuction(x)
 
         x = x * 128 + 128 # Scale output approx from [-1, 1] to [0, 255]
         return x
     
 class _ResBlock(nn.Module):
```

### Comparing `pssr-1.0.2/pssr/models/resuneta.py` & `pssr-1.1.0/pssr/models/resuneta.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,53 +1,58 @@
-import torch
+import torch, warnings
 import torch.nn as nn
 import torch.nn.functional as F
 from ._blocks import Reconstruction
+from ..data import _force_list
 
 class ResUNetA(nn.Module):
     def __init__(self, channels : int = 1, hidden : list[int] = [64, 128, 256, 512, 1024], scale : int = 4, depth : int = 3, dilations : list[list[int]] = [[1,3,15,31],[1,3,15],[1,3],[1],[1]], pool_sizes : list[int] = [1, 2, 4, 8], encoder_pool : bool = False):
         r"""A modified Atrous Residual UNet as detailed in Diakogiannis et al., 2019 with an additional image upscaling block.
 
-        Channel sizes hidden[0] (and hidden[-1] if encoder_pool) should be divisible by len(pool_sizes).
+        Channel sizes hidden[0] (and hidden[-1] if encoder_pool is True) must be divisible by len(pool_sizes).
 
         Args:
-            channels (int) : Number of channels in image data.
+            channels (int) : Number of channels in image data. Can also be a list of in channels and out channels respectively.
 
             hidden (list[int]) : Elementwise list of hidden layer channels controlling width and length of model.
 
             scale (int) : Upscaling factor for predictions. Choose a power of 2 for best results. Default is 4.
 
             depth (int) : Number of hidden layers per residual block. Default is 3.
 
-            dilations (list[list[int]]) : List of dilation values per layer.
+            dilations (list[list[int]]) : List of dilation values per layer. If value is none, atrous convolutions will not be used.
 
             pool_sizes (list[int]) : Pooling ratios for PSP pooling.
 
             encoder_pool (bool) : Whether to include PSP pooling layer at end of encoder. Should not be used if last layer has a size of less than 16 pixels. Default is False.
         """
         super().__init__()
+        channels = _force_list(channels)
+        channels = channels*2 if len(channels) == 1 else channels
 
         if dilations is None:
-            print("dilations is None, atrous convolutions will not be used.")
+            warnings.warn("dilations is None, atrous convolutions will not be used.", stacklevel=2)
             dilations = [1]*len(hidden)
-        assert len(dilations) == len(hidden), f"len(dilations) must equal len(hidden), lengths are {len(dilations)} and {len(hidden)}."
+        if len(dilations) != len(hidden): raise ValueError(f"len(dilations) must equal len(hidden). Lengths are {len(dilations)} and {len(hidden)}.")
+        if hidden[0] % len(pool_sizes) != 0: raise ValueError(f"hidden[0] must be divisible by len(pool_sizes). Sizes are {hidden[0]} and {len(pool_sizes)}.")
+        if hidden[-1] % len(pool_sizes) != 0 and encoder_pool: raise ValueError(f"hidden[-1] must be divisible by len(pool_sizes) if encoder_pool is True. Sizes are {hidden[-1]} and {len(pool_sizes)}.")
         
         self.encoder, self.decoder, self.upscale = nn.ModuleList(), nn.ModuleList(), nn.ModuleList()
-        layers = [channels, *hidden]
+        layers = [channels[0], *hidden]
         n_layers = len(layers) - 1
         for layer_idx in range(n_layers):
             self.encoder.append(_ResBlockA(in_channels=layers[layer_idx], out_channels=layers[layer_idx+1], dilations=dilations[layer_idx], depth=depth))
             if layer_idx + 1 < n_layers:
                 self.decoder.append(_ResBlockA(in_channels=layers[-layer_idx-1] - int(layers[-layer_idx-2]/2), out_channels=layers[-layer_idx-2], dilations=dilations[-layer_idx-1], depth=depth))
                 self.upscale.append(nn.PixelShuffle(2))
 
         self.encoder_pool = _PSP_Pooling(hidden[-1], pool_sizes) if encoder_pool else None
         self.reconstuction_pool = _PSP_Pooling(hidden[0], pool_sizes)
 
-        self.reconstuction = Reconstruction(channels, hidden[0], scale)
+        self.reconstuction = Reconstruction(channels[0], channels[1], hidden[0], scale)
 
     def forward(self, x):
         x = x / 128 - 1 # Scale input approx from [0, 255] to [-1, 1]
 
         skips = [x]
         for idx, layer in enumerate(self.encoder):
             x = layer(x) # ResBlock
@@ -64,15 +69,15 @@
 
             x = torch.cat([x, skips.pop()], dim=1) # ResBlock
             x = layer(x)
 
         x = self.reconstuction_pool(x)
 
         x = torch.cat([x, skips.pop()], dim=1) # Final skip connection before reconstruction
-        assert len(skips) == 0, "Skip connection mismatch between encoder and decoder."
+        if len(skips) != 0: raise IndexError(f"Skip connection mismatch between encoder and decoder. {len(skips)} skip connections are unused.")
 
         x = self.reconstuction(x)
 
         x = x * 128 + 128 # Scale output approx from [-1, 1] to [0, 255]
         return x
 
 class _ResBlockA(nn.Module):
```

### Comparing `pssr-1.0.2/pssr/predict.py` & `pssr-1.1.0/pssr/predict.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,40 @@
-import torch, os, cv2
+import torch, os, tifffile
 import torch.nn as nn
 import numpy as np
 from torch.utils.data import DataLoader, Dataset
 from skimage.metrics import peak_signal_noise_ratio, structural_similarity
+from skimage.transform import resize
 from tqdm import tqdm
 from PIL import Image
+from .data import _RandomIterIdx, _slice_center
 from .loss import pixel_metric
 
-def predict_images(model : nn.Module, dataset : Dataset, device : str = "cpu", out_dir : str = None, norm : bool = False):
+def predict_images(model : nn.Module, dataset : Dataset, device : str = "cpu", norm : bool = False, prefix : str = None, out_dir : str = "preds"):
     r"""Predicts high-resolution images from low-resolution images using a given model.
     
-    Only predicts evaluation images if applicable. Set `val_split=1` in dataset to use all images.
+    Only uses evaluation images if applicable. Set ``val_split=1`` in dataset to use all images.
 
     Args:
-        model (nn.Module) : Model recieve low-resolution images.
+        model (nn.Module) : Model to recieve low-resolution images.
 
-        dataset (Dataset) : Single image dataset to load data from.
+        dataset (Dataset) : Dataset to load low-resolution images from.
 
         device (str) : Device to train model on. Default is "cpu".
 
-        out_dir (str) : Set to a path to automatically save images, otherwise return images. Default is None.
-
         norm (bool) : Whether to normalize prediction image intensities to ground truth, which must be provided by a paired dataset. Default is False.
+
+        prefix (str) : Prefix to append at the beginning the output file name. Default is None.
+
+        out_dir (str) : Directory to save images. A value of None returns images. Default is "preds".
     
     Returns:
-        images (list[Image]) : Returns predicted images if `out_dir` is None.
+        images (list[np.ndarray]) : Returns predicted images if ``out_dir`` is None.
     """
-    if norm:
-        assert not dataset.is_lr, "Dataset must be paired with high-low-resolution images for normalization."
+    if norm and dataset.is_lr: raise ValueError("Dataset must be paired with high-low-resolution images for normalization.")
 
     model.to(device)
     model.eval()
 
     progress = tqdm(dataset.val_idx)
     outs = []
     with torch.no_grad():
@@ -39,113 +42,103 @@
             lr = dataset[idx] if dataset.is_lr else dataset[idx][1]
             lr = lr.to(device).unsqueeze(0)
 
             hr_hat = model(lr)
             hr_hat = _pred_array(hr_hat).squeeze(0)
             
             if norm:
-                _, hr_hat = normalize_preds(np.mean(_pred_array(dataset[idx][0]), axis=0), np.mean(hr_hat, axis=0))
-
-            hr_hat = Image.fromarray(hr_hat.astype(np.uint8).squeeze())
-            hr_hat = hr_hat.crop([0,0,dataset.crop_res,dataset.crop_res])
+                _, hr_hat = normalize_preds(_pred_array(dataset[idx][0]), hr_hat)
 
+            hr_hat = hr_hat[:,:dataset.crop_res,:dataset.crop_res]
             outs.append(hr_hat)
 
     if out_dir:
         os.makedirs(out_dir, exist_ok=True)
         for idx, hr_hat in enumerate(outs):
-            cv2.imwrite(out_dir + f"/{dataset._get_name(idx)}_pred.png", np.asarray(hr_hat))
+            tifffile.imwrite(f"{out_dir}/{prefix+'_' if prefix else ''}{dataset._get_name(idx)}.tif", np.asarray(hr_hat))
     else:
         return outs
 
-def predict_collage(model : nn.Module, dataset : Dataset, batch_size : int, device : str = "cpu", norm : bool = True, n_images : int = None, prefix : str = None, dataloader_kwargs = None):
+def predict_collage(model : nn.Module, dataset : Dataset, device : str = "cpu", norm : bool = True, n_images : int = None, prefix : str = None, out_dir : str = "preds"):
     r"""Saves to file an image collage of vertically stacked instances of horizontally aligned low-resolution, PSSR upscaled, and high-resolution images in that order.
+    Only the center frame of each slice is displayed.
 
-    Only predicts evaluation images if applicable. Set `val_split=1` in dataset to use all images.
+    Only uses evaluation images if applicable. Set ``val_split=1`` in dataset to use all images.
 
     Args:
-        model (nn.Module) : Model recieve low-resolution images.
+        model (nn.Module) : Model to recieve low-resolution images.
 
         dataset (Dataset) : Paired image dataset to load data from.
 
-        batch_size (int) : Batch size for dataloader.
-
         device (str) : Device to train model on. Default is "cpu".
 
         norm (bool) : Whether to normalize prediction image intensities to ground truth. Default is True.
 
         n_images (int) : Number of images to concatenate. Set to None to use all validation images, maximum 50. Default is None.
 
         prefix (str) : Prefix to append at the beginning the output file name. Default is None.
 
-        dataloader_kwargs (dict[str, Any]) : Keyword arguments for pytorch Dataloader. Default is None.
+        out_dir (str) : Directory to save collage. Default is "preds".
     """
-    prefix = "" if prefix is None else prefix
-    dataloader_kwargs = {} if dataloader_kwargs is None else dataloader_kwargs
-    val_dataloader = DataLoader(dataset, batch_size, sampler=dataset.val_idx, **dataloader_kwargs)
     n_images = min(50, len(dataset)) if n_images is None else n_images
 
     model.to(device)
     model.eval()
 
     collage = Image.new("L", (dataset.crop_res*3, dataset.crop_res*n_images))
-    remaining = n_images
     with torch.no_grad():
-        for idx, (hr, lr) in enumerate(val_dataloader):
-            hr, lr = hr.to(device), lr.to(device)
+        for idx, data_idx in enumerate(_RandomIterIdx(dataset.val_idx, seed=True)):
+            hr, lr = dataset[data_idx]
+            hr, lr = hr.to(device).unsqueeze(0), lr.to(device).unsqueeze(0)
 
             hr_hat = model(lr)
 
-            collage.paste(_collage_preds(lr, hr_hat, hr, norm, min(remaining, batch_size), dataset.crop_res), (0, dataset.crop_res*batch_size*idx))
+            collage.paste(_collage_preds(lr, hr_hat, hr, norm, 1, dataset.crop_res), (0, dataset.crop_res*idx))
 
-            remaining -= batch_size
-            if remaining <= 0:
+            if idx >= n_images:
                 break
 
-    os.makedirs("preds", exist_ok=True)
-    collage.save(f"preds/{prefix+'_' if prefix else ''}collage_{n_images}.png")
+    os.makedirs(out_dir, exist_ok=True)
+    collage.save(f"{out_dir}/{prefix+'_' if prefix else ''}collage_{n_images}.png")
 
-def test_metrics(model : nn.Module, dataset : Dataset, batch_size : int, device : str = "cpu", metrics : list[str] = ["mse", "pixel", "psnr", "ssim"], avg : bool = True, norm : bool = True, dataloader_kwargs = None):
+def test_metrics(model : nn.Module, dataset : Dataset, device : str = "cpu", metrics : list[str] = ["mse", "pixel", "psnr", "ssim"], avg : bool = True, norm : bool = True):
     r"""Computes image restoration metrics of predicted vs ground truth images.
 
+    Only uses evaluation images if applicable. Set ``val_split=1`` in dataset to use all images.
+
     Args:
-        model (nn.Module) : Model recieve low-resolution images.
+        model (nn.Module) : Model to recieve low-resolution images.
 
         dataset (Dataset) : Paired image dataset to load data from.
 
-        batch_size (int) : Batch size for dataloader.
-
         device (str) : Device to train model on. Default is "cpu".
 
         metrics (list[str]) : Metrics to calculate out of "mse", "pixel", "psnr", and "ssim". Default is all.
 
         avg (bool) : Whether to return a single averaged value per metric. Default is True.
 
         norm (bool) : Whether to normalize prediction image intensities to ground truth. Default is True.
-
-        dataloader_kwargs (dict[str, Any]) : Keyword arguments for pytorch Dataloader. Default is None.
     
     Returns:
         metrics (dict[str, Any]) : Dictionary of metric names and outputs.
     """
-    dataloader_kwargs = {} if dataloader_kwargs is None else dataloader_kwargs
-    val_dataloader = DataLoader(dataset, batch_size, sampler=dataset.val_idx, **dataloader_kwargs)
     image_range = 255
 
     metrics = [metrics] if type(metrics) is str else metrics
     metrics = {metric:[] for metric in metrics}
     use_mse = True if any(x in metrics.keys() for x in ["mse", "pixel"]) else False
 
     model.to(device)
     model.eval()
 
-    progress = tqdm(val_dataloader)
+    progress = tqdm(dataset.val_idx)
     with torch.no_grad():
-        for hr, lr in progress:
-            hr, lr = hr.to(device), lr.to(device)
+        for idx in progress:
+            hr, lr = dataset[0]
+            hr, lr = hr.to(device).unsqueeze(0), lr.to(device).unsqueeze(0)
 
             hr_hat = model(lr)
 
             hr, hr_hat = _pred_array(hr)[:,:,:dataset.crop_res,:dataset.crop_res], _pred_array(hr_hat)[:,:,:dataset.crop_res,:dataset.crop_res]
 
             if norm:
                 hr, hr_hat = normalize_preds(hr, hr_hat)
@@ -158,16 +151,15 @@
                 if "pixel" in metrics:
                     metrics["pixel"].append(pixel_metric(mse, image_range))
                 if "psnr" in metrics:
                     metrics["psnr"].append(peak_signal_noise_ratio(hr[idx], hr_hat[idx], data_range=image_range))
                 if "ssim" in metrics:
                     metrics["ssim"].append(structural_similarity(hr[idx].squeeze(), hr_hat[idx].squeeze(), data_range=image_range))
 
-    metrics = {metric:(sum(values)/len(values) if avg else values) for metric, values in metrics.items()}
-    return metrics
+    return {metric:(sum(values)/len(values) if avg else values) for metric, values in metrics.items()}
 
 def normalize_preds(hr : np.ndarray, hr_hat : np.ndarray, pmin : float = 0.1, pmax : float = 99.9):
     r"""Normalizes prediction image intensities to ground truth for fair benchmarking.
 
     Args:
         hr (ndarray) : High-resolution ground truth images as array.
 
@@ -178,22 +170,22 @@
         pmax (float) : Percentile maximum image intensity. Default is 99.9.
     
     Returns:
         hr_norm (ndarray) : Normalized high-resolution ground truth image.
 
         hr_hat_norm (ndarray) : Normalized high-resolution prediction image.
     """
-    assert len(hr.shape) == len(hr_hat.shape), "hr and hr_hat must have the same number of dimensions."
+    if len(hr.shape) != len(hr_hat.shape): raise ValueError(f"hr and hr_hat must have the same number of dimensions. Dimension lengths are {hr.shape} and {hr_hat.shape} respectively.")
     hr_shape = hr.shape
     hr_hat_shape = hr_hat.shape
 
     if len(hr.shape) < 3:
         hr, hr_hat = hr[np.newaxis, ...], hr_hat[np.newaxis, ...]
     hr, hr_hat = hr.reshape(-1, *hr.shape[-2:]), hr_hat.reshape(-1, *hr_hat.shape[-2:])
-    assert len(hr) == len(hr_hat), "hr and hr_hat must have the same number of images."
+    if len(hr) != len(hr_hat): raise ValueError(f"hr and hr_hat must have the same number of images. Received {len(hr)} and {len(hr_hat)} images respectively.")
 
     hr_norms, hr_hat_norms = [], []
     for idx in range(len(hr)):
         # Same procedure as in intial PSSR implementation
         hr_norm = hr[idx].astype(np.float32)
         hr_hat_norm = hr_hat[idx].astype(np.float32)
 
@@ -201,27 +193,27 @@
         base_mean = np.mean(hr_norm)
 
         hr_norm = _normalize_minmax(hr_norm, pmin, pmax)
 
         hr_hat_norm = hr_hat_norm - np.mean(hr_hat_norm)
         hr_norm = hr_norm - np.mean(hr_norm)
 
-        scale = np.cov(cv2.resize(hr_hat_norm, hr_norm.shape).flatten(), hr_norm.flatten())[0, 1] / np.var(hr_hat_norm.flatten())
-        hr_hat_norm = scale * hr_hat_norm
+        scaled = resize(hr_hat_norm, hr_norm.shape) if hr_hat_norm.shape != hr_norm.shape else hr_hat_norm
+        amp = np.cov(scaled.flatten(), hr_norm.flatten())[0, 1] / np.var(hr_hat_norm.flatten())
+        hr_hat_norm = amp * hr_hat_norm
         
         # Rescale to initial image intensity
         hr_norm, hr_hat_norm = (hr_norm-hr_norm.min())*base_max, (hr_hat_norm-hr_norm.min())*base_max
         hr_norm, hr_hat_norm = hr_norm/(hr_norm.mean()/base_mean), hr_hat_norm/(hr_hat_norm.mean()/base_mean)
 
         hr_norms.append(hr_norm)
         hr_hat_norms.append(hr_hat_norm)
     
     hr, hr_hat = np.asarray(hr_norms).clip(0, 255), np.asarray(hr_hat_norms).clip(0, 255)
-    return hr.reshape(hr_shape), hr_hat.reshape(hr_hat_shape)
-    
+    return hr.reshape(hr_shape).astype(np.uint8), hr_hat.reshape(hr_hat_shape).astype(np.uint8)
 
 def _collage_preds(lr, hr_hat, hr, norm : bool = True, max_images : int = 5, crop_res : int = None):
     crop_res = hr.shape[-1] if crop_res is None else crop_res
     lr, hr_hat, hr = _pred_array(lr)[:,:,:crop_res//4,:crop_res//4], _pred_array(hr_hat)[:,:,:crop_res,:crop_res], _pred_array(hr)[:,:,:crop_res,:crop_res]
 
     if norm:
         hr, hr_hat = normalize_preds(hr, hr_hat)
@@ -258,9 +250,10 @@
     x_max = dtype(x_max) if np.isscalar(x_max) else x_max.astype(dtype,copy=False)
     eps = dtype(eps)
 
     x = (x - x_min) / (x_max - x_min + eps)
 
     return x
 
-def _pred_array(data):
-    return np.clip(data.detach().cpu().numpy(), 0, 255).astype(np.uint8)
+def _pred_array(data, n_frames=1):
+    n_frames = [0, n_frames]
+    return _slice_center(np.clip(data.detach().cpu().numpy(), 0, 255).astype(np.uint8), n_frames)
```

### Comparing `pssr-1.0.2/pssr/train.py` & `pssr-1.1.0/pssr/train.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,22 +48,22 @@
 
         scheduler (LRScheduler) : Optional learning rate scheduler for training. Default is None.
 
         clamp (bool) : Whether to clamp model image output before weight calculation. Default is False.
 
         log_frequency (int) : Frequency to log losses and recalculate metrics in steps. Default is 50.
 
-        dataloader_kwargs (dict[str, Any]) : Keyword arguments for pytorch Dataloader. Default is None.
+        dataloader_kwargs (dict[str, Any]) : Keyword arguments for pytorch ``Dataloader``. Default is None.
 
     Returns:
         losses (list[float]) : List of losses during training.
     """
     dataloader_kwargs = {} if dataloader_kwargs is None else dataloader_kwargs
     train_dataloader = DataLoader(dataset, batch_size, sampler=_RandomIterIdx(_invert_idx(dataset.val_idx, len(dataset))), **dataloader_kwargs)
-    val_dataloader = DataLoader(dataset, batch_size, sampler=dataset.val_idx, **dataloader_kwargs)
+    val_dataloader = DataLoader(dataset, batch_size, sampler=_RandomIterIdx(dataset.val_idx, seed=True), **dataloader_kwargs)
     include_metric = True if type(scheduler) == torch.optim.lr_scheduler.ReduceLROnPlateau else False
     image_range = 255
 
     model.to(device)
 
     losses = []
     for epoch in range(epochs):
@@ -79,15 +79,15 @@
                 hr_hat = torch.clamp(hr_hat, 0, image_range)
 
             loss = loss_fn(hr_hat/image_range, hr/image_range)
             loss.backward()
             optim.step()
             optim.zero_grad()
 
-            if batch_idx % log_frequency == 0:
+            if batch_idx % log_frequency == 0 or batch_idx == len(progress) - 1:
                 losses.append(loss.item())
 
                 mse = nn.functional.mse_loss(hr_hat/image_range, hr/image_range)
                 progress.set_description(f"pixel[{pixel_metric(mse, image_range):.2f}], psnr[{_psnr_metric(mse, hr.max()/image_range):.2f}], ssim[{ssim(hr_hat, hr, data_range=image_range):.3f}]")
 
         # Validation
         model.eval()
@@ -161,22 +161,22 @@
 
         scheduler (LRScheduler) : Optional learning rate scheduler for training. Default is None.
 
         clamp (bool) : Whether to clamp model image output before weight calculation. Default is False.
 
         log_frequency (int) : Frequency to log losses and recalculate metrics in steps. Default is 50.
 
-        dataloader_kwargs (dict[str, Any]) : Keyword arguments for pytorch Dataloader. Default is None.
+        dataloader_kwargs (dict[str, Any]) : Keyword arguments for pytorch ``Dataloader``. Default is None.
 
     Returns:
         losses (list[float]) : List of losses during training.
     """
     dataloader_kwargs = {} if dataloader_kwargs is None else dataloader_kwargs
     train_dataloader = DataLoader(dataset, batch_size, sampler=_RandomIterIdx(_invert_idx(dataset.val_idx, len(dataset))), **dataloader_kwargs)
-    val_dataloader = DataLoader(dataset, batch_size, sampler=dataset.val_idx, **dataloader_kwargs)
+    val_dataloader = DataLoader(dataset, batch_size, sampler=_RandomIterIdx(dataset.val_idx, seed=True), **dataloader_kwargs)
     include_metric = True if type(scheduler) == torch.optim.lr_scheduler.ReduceLROnPlateau else False
 
     model.to(device)
     model.train()
 
     # Leave on cpu?
     hist_fn = GradHist(sigma=sigma)
@@ -202,15 +202,15 @@
 
             if clip is not None and clip > 0:
                 nn.utils.clip_grad_value_(model.parameters(), clip)
 
             optim.step()
             optim.zero_grad()
 
-            if batch_idx % log_frequency == 0:
+            if batch_idx % log_frequency == 0 or batch_idx == len(progress) - 1:
                 losses.append(loss.item())
 
                 progress.set_description(f"loss[{loss.item():.5f}]")
 
         # Validation
         model.eval()
 
@@ -236,15 +236,15 @@
 
         if scheduler:
             if include_metric:
                 scheduler.step(val_loss)
             else:
                 scheduler.step()
 
-        collage = _collage_preds(lr, lr_hat, hr)
+        collage = _collage_preds(lr, lr_hat, hr, crop_res=dataset.crop_res)
         os.makedirs("preds", exist_ok=True)
         collage.save(f"preds/pred{epoch}_loss{val_loss:.3f}.png")
     return losses
 
 def approximate_crappifier(crappifier : Crappifier, space : list[Dimension], dataset : Dataset, max_images = None, opt_kwargs = None):
     r"""Approximates :class:`Crappifier` parameters from ground truth paired images. Uses Bayesian optimization because Crappifier functions are not differentiable.
 
@@ -253,15 +253,15 @@
 
         space (list[Dimension]) : List of parameter spaces for each crappifier parameter.
 
         dataset (Dataset) : Paired image dataset to load data from.
 
         max_images (int) : Number of image samples to average computations over for each optimization step. Default is None, using all images in dataset.
 
-        opt_kwargs (dict[str, Any]) : Keyword arguments for skopt :meth:`gp_minimize`. Default is None
+        opt_kwargs (dict[str, Any]) : Keyword arguments for skopt ``gp_minimize``. Default is None
     """
     space = [space] if type(space) is not list else space
     n_samples = len(dataset) if max_images is None else min(max_images, len(dataset))
     opt_kwargs = {} if opt_kwargs is None else opt_kwargs
 
     objective = _Crappifier_Objective(crappifier, dataset, n_samples).sample
```

### Comparing `pssr-1.0.2/pyproject.toml` & `pssr-1.1.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pssr"
-version = "1.0.2"
+version = "1.1.0"
 description = "Point-Scanning Super-Resolution"
 authors = ["Hayden Stites"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/haydenstites/PSSR"
 documentation = "https://haydenstites.github.io/PSSR/"
 classifiers = [
@@ -22,19 +22,20 @@
 
 [tool.poetry.dependencies]
 python = "^3.11"
 torch = "^2.0.0"
 numpy = "^1.26.4"
 pillow = "^10.2.0"
 czifile = "^2019.7.2"
-opencv-python = "^4.9.0.80"
+tifffile = "^2024.4.24"
 scikit-image = "^0.23.1"
 scikit-optimize = "^0.9.0"
 tqdm = "^4.66.2"
 pytorch-msssim = "^1.0.0"
+psutil = "^5.9.8"
 
 [tool.poetry.scripts]
 pssr = "_pssr:run"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pssr-1.0.2/PKG-INFO` & `pssr-1.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pssr
-Version: 1.0.2
+Version: 1.1.0
 Summary: Point-Scanning Super-Resolution
 Home-page: https://github.com/haydenstites/PSSR
 License: MIT
 Author: Hayden Stites
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: GPU :: NVIDIA CUDA
@@ -15,19 +15,20 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Requires-Dist: czifile (>=2019.7.2,<2020.0.0)
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
-Requires-Dist: opencv-python (>=4.9.0.80,<5.0.0.0)
 Requires-Dist: pillow (>=10.2.0,<11.0.0)
+Requires-Dist: psutil (>=5.9.8,<6.0.0)
 Requires-Dist: pytorch-msssim (>=1.0.0,<2.0.0)
 Requires-Dist: scikit-image (>=0.23.1,<0.24.0)
 Requires-Dist: scikit-optimize (>=0.9.0,<0.10.0)
+Requires-Dist: tifffile (>=2024.4.24,<2025.0.0)
 Requires-Dist: torch (>=2.0.0,<3.0.0)
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Project-URL: Documentation, https://haydenstites.github.io/PSSR/
 Project-URL: Repository, https://github.com/haydenstites/PSSR
 Description-Content-Type: text/markdown
 
 # Point-Scanning Super-Resolution (**PSSR**)
```

