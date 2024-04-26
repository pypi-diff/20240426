# Comparing `tmp/bbo-calibcam-2.3.1.tar.gz` & `tmp/bbo-calibcam-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbo-calibcam-2.3.1.tar", last modified: Wed Dec 20 15:02:36 2023, max compression
+gzip compressed data, was "bbo-calibcam-2.4.1.tar", last modified: Fri Apr 26 05:46:51 2024, max compression
```

## Comparing `bbo-calibcam-2.3.1.tar` & `bbo-calibcam-2.4.1.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxrwxr-x   0 voit     (86501) voit     (86501)        0 2023-12-20 15:02:36.694481 bbo-calibcam-2.3.1/
--rw-rw-r--   0 voit     (86501) voit     (86501)    25314 2023-11-13 15:21:57.000000 bbo-calibcam-2.3.1/LICENSE
--rw-rw-r--   0 voit     (86501) voit     (86501)     3448 2023-12-20 15:02:36.694481 bbo-calibcam-2.3.1/PKG-INFO
--rw-rw-r--   0 voit     (86501) voit     (86501)     2965 2023-11-13 15:21:57.000000 bbo-calibcam-2.3.1/README.md
-drwxrwxr-x   0 voit     (86501) voit     (86501)        0 2023-12-20 15:02:36.690481 bbo-calibcam-2.3.1/bbo_calibcam.egg-info/
--rw-rw-r--   0 voit     (86501) voit     (86501)     3448 2023-12-20 15:02:36.000000 bbo-calibcam-2.3.1/bbo_calibcam.egg-info/PKG-INFO
--rw-rw-r--   0 voit     (86501) voit     (86501)      701 2023-12-20 15:02:36.000000 bbo-calibcam-2.3.1/bbo_calibcam.egg-info/SOURCES.txt
--rw-rw-r--   0 voit     (86501) voit     (86501)        1 2023-12-20 15:02:36.000000 bbo-calibcam-2.3.1/bbo_calibcam.egg-info/dependency_links.txt
--rw-rw-r--   0 voit     (86501) voit     (86501)       82 2023-12-20 15:02:36.000000 bbo-calibcam-2.3.1/bbo_calibcam.egg-info/requires.txt
--rw-rw-r--   0 voit     (86501) voit     (86501)        9 2023-12-20 15:02:36.000000 bbo-calibcam-2.3.1/bbo_calibcam.egg-info/top_level.txt
-drwxrwxr-x   0 voit     (86501) voit     (86501)        0 2023-12-20 15:02:36.694481 bbo-calibcam-2.3.1/calibcam/
--rw-rw-r--   0 voit     (86501) voit     (86501)       21 2023-11-13 15:21:57.000000 bbo-calibcam-2.3.1/calibcam/__init__.py
--rwxrwxr-x   0 voit     (86501) voit     (86501)     5716 2023-11-13 15:21:57.000000 bbo-calibcam-2.3.1/calibcam/__main__.py
--rw-rw-r--   0 voit     (86501) voit     (86501)     1778 2023-11-13 15:21:57.000000 bbo-calibcam-2.3.1/calibcam/board.py
--rw-rw-r--   0 voit     (86501) voit     (86501)     5185 2023-12-20 15:01:17.000000 bbo-calibcam-2.3.1/calibcam/calibrator_opts.py
--rw-rw-r--   0 voit     (86501) voit     (86501)    25053 2023-11-13 15:21:57.000000 bbo-calibcam-2.3.1/calibcam/camcalibrator.py
--rw-rw-r--   0 voit     (86501) voit     (86501)     7375 2023-12-20 15:01:17.000000 bbo-calibcam-2.3.1/calibcam/camfunctions.py
--rw-rw-r--   0 voit     (86501) voit     (86501)     3413 2023-11-13 15:21:57.000000 bbo-calibcam-2.3.1/calibcam/camfunctions_ag.py
--rw-rw-r--   0 voit     (86501) voit     (86501)     1500 2023-11-13 15:21:57.000000 bbo-calibcam-2.3.1/calibcam/compatibility.py
--rw-rw-r--   0 voit     (86501) voit     (86501)     6860 2023-11-13 15:21:57.000000 bbo-calibcam-2.3.1/calibcam/detection.py
--rw-rw-r--   0 voit     (86501) voit     (86501)      110 2023-11-13 15:21:57.000000 bbo-calibcam-2.3.1/calibcam/exceptions.py
--rw-rw-r--   0 voit     (86501) voit     (86501)     5561 2023-11-13 15:21:57.000000 bbo-calibcam-2.3.1/calibcam/helper.py
--rw-rw-r--   0 voit     (86501) voit     (86501)     2128 2023-11-13 15:21:57.000000 bbo-calibcam-2.3.1/calibcam/helper_ag.py
-drwxrwxr-x   0 voit     (86501) voit     (86501)        0 2023-12-20 15:02:36.694481 bbo-calibcam-2.3.1/calibcam/opt_jacfwd/
--rw-rw-r--   0 voit     (86501) voit     (86501)        0 2023-11-13 15:21:57.000000 bbo-calibcam-2.3.1/calibcam/opt_jacfwd/__init__.py
--rw-rw-r--   0 voit     (86501) voit     (86501)     4283 2023-12-20 15:01:17.000000 bbo-calibcam-2.3.1/calibcam/opt_jacfwd/optfunctions.py
--rw-rw-r--   0 voit     (86501) voit     (86501)     2067 2023-11-13 15:21:57.000000 bbo-calibcam-2.3.1/calibcam/opt_jacfwd/optfunctions_ag.py
--rw-rw-r--   0 voit     (86501) voit     (86501)     7496 2023-12-20 15:01:17.000000 bbo-calibcam-2.3.1/calibcam/optimization.py
--rw-rw-r--   0 voit     (86501) voit     (86501)     5724 2023-11-13 15:21:57.000000 bbo-calibcam-2.3.1/calibcam/pose_estimation.py
--rw-rw-r--   0 voit     (86501) voit     (86501)     3665 2023-11-13 15:21:57.000000 bbo-calibcam-2.3.1/calibcam/single_camcalibration.py
--rw-rw-r--   0 voit     (86501) voit     (86501)       38 2023-12-20 15:02:36.694481 bbo-calibcam-2.3.1/setup.cfg
--rw-rw-r--   0 voit     (86501) voit     (86501)     1024 2023-12-20 15:02:32.000000 bbo-calibcam-2.3.1/setup.py
-drwxrwxr-x   0 voit     (86501) voit     (86501)        0 2023-12-20 15:02:36.694481 bbo-calibcam-2.3.1/test/
--rw-rw-r--   0 voit     (86501) voit     (86501)     4011 2023-12-20 15:01:17.000000 bbo-calibcam-2.3.1/test/test_detection.py
+drwxrwxr-x   0 voit     (86501) voit     (86501)        0 2024-04-26 05:46:51.825947 bbo-calibcam-2.4.1/
+-rw-rw-r--   0 voit     (86501) voit     (86501)    25314 2023-11-13 15:21:57.000000 bbo-calibcam-2.4.1/LICENSE
+-rw-rw-r--   0 voit     (86501) voit     (86501)     3448 2024-04-26 05:46:51.825947 bbo-calibcam-2.4.1/PKG-INFO
+-rw-rw-r--   0 voit     (86501) voit     (86501)     2965 2023-11-13 15:21:57.000000 bbo-calibcam-2.4.1/README.md
+drwxrwxr-x   0 voit     (86501) voit     (86501)        0 2024-04-26 05:46:51.813946 bbo-calibcam-2.4.1/bbo_calibcam.egg-info/
+-rw-rw-r--   0 voit     (86501) voit     (86501)     3448 2024-04-26 05:46:51.000000 bbo-calibcam-2.4.1/bbo_calibcam.egg-info/PKG-INFO
+-rw-rw-r--   0 voit     (86501) voit     (86501)      725 2024-04-26 05:46:51.000000 bbo-calibcam-2.4.1/bbo_calibcam.egg-info/SOURCES.txt
+-rw-rw-r--   0 voit     (86501) voit     (86501)        1 2024-04-26 05:46:51.000000 bbo-calibcam-2.4.1/bbo_calibcam.egg-info/dependency_links.txt
+-rw-rw-r--   0 voit     (86501) voit     (86501)       82 2024-04-26 05:46:51.000000 bbo-calibcam-2.4.1/bbo_calibcam.egg-info/requires.txt
+-rw-rw-r--   0 voit     (86501) voit     (86501)        9 2024-04-26 05:46:51.000000 bbo-calibcam-2.4.1/bbo_calibcam.egg-info/top_level.txt
+drwxrwxr-x   0 voit     (86501) voit     (86501)        0 2024-04-26 05:46:51.825947 bbo-calibcam-2.4.1/calibcam/
+-rw-rw-r--   0 voit     (86501) voit     (86501)       21 2023-11-13 15:21:57.000000 bbo-calibcam-2.4.1/calibcam/__init__.py
+-rwxrwxr-x   0 voit     (86501) voit     (86501)     6939 2024-04-03 11:11:24.000000 bbo-calibcam-2.4.1/calibcam/__main__.py
+-rw-rw-r--   0 voit     (86501) voit     (86501)     2177 2024-04-03 11:11:24.000000 bbo-calibcam-2.4.1/calibcam/board.py
+-rw-rw-r--   0 voit     (86501) voit     (86501)     6562 2024-04-03 11:11:24.000000 bbo-calibcam-2.4.1/calibcam/calibrator_opts.py
+-rw-rw-r--   0 voit     (86501) voit     (86501)    28418 2024-04-03 12:49:17.000000 bbo-calibcam-2.4.1/calibcam/camcalibrator.py
+-rw-rw-r--   0 voit     (86501) voit     (86501)     7387 2024-02-21 09:07:16.000000 bbo-calibcam-2.4.1/calibcam/camfunctions.py
+-rw-rw-r--   0 voit     (86501) voit     (86501)     3413 2023-11-13 15:21:57.000000 bbo-calibcam-2.4.1/calibcam/camfunctions_ag.py
+-rw-rw-r--   0 voit     (86501) voit     (86501)     1500 2023-11-13 15:21:57.000000 bbo-calibcam-2.4.1/calibcam/compatibility.py
+-rw-rw-r--   0 voit     (86501) voit     (86501)     7828 2024-03-08 12:23:55.000000 bbo-calibcam-2.4.1/calibcam/detection.py
+-rw-rw-r--   0 voit     (86501) voit     (86501)      110 2023-11-13 15:21:57.000000 bbo-calibcam-2.4.1/calibcam/exceptions.py
+-rw-rw-r--   0 voit     (86501) voit     (86501)     8574 2024-02-21 09:07:16.000000 bbo-calibcam-2.4.1/calibcam/helper.py
+-rw-rw-r--   0 voit     (86501) voit     (86501)     2128 2023-11-13 15:21:57.000000 bbo-calibcam-2.4.1/calibcam/helper_ag.py
+drwxrwxr-x   0 voit     (86501) voit     (86501)        0 2024-04-26 05:46:51.825947 bbo-calibcam-2.4.1/calibcam/opt_jacfwd/
+-rw-rw-r--   0 voit     (86501) voit     (86501)        0 2023-11-13 15:21:57.000000 bbo-calibcam-2.4.1/calibcam/opt_jacfwd/__init__.py
+-rw-rw-r--   0 voit     (86501) voit     (86501)     4283 2023-12-20 15:01:17.000000 bbo-calibcam-2.4.1/calibcam/opt_jacfwd/optfunctions.py
+-rw-rw-r--   0 voit     (86501) voit     (86501)     2067 2023-11-13 15:21:57.000000 bbo-calibcam-2.4.1/calibcam/opt_jacfwd/optfunctions_ag.py
+-rw-rw-r--   0 voit     (86501) voit     (86501)     7496 2023-12-20 15:01:17.000000 bbo-calibcam-2.4.1/calibcam/optimization.py
+-rw-rw-r--   0 voit     (86501) voit     (86501)     5724 2023-11-13 15:21:57.000000 bbo-calibcam-2.4.1/calibcam/pose_estimation.py
+-rw-rw-r--   0 voit     (86501) voit     (86501)     3731 2024-03-11 13:54:23.000000 bbo-calibcam-2.4.1/calibcam/single_camcalibration.py
+-rw-rw-r--   0 voit     (86501) voit     (86501)      749 2024-04-03 12:26:54.000000 bbo-calibcam-2.4.1/calibcam/yaml_helper.py
+-rw-rw-r--   0 voit     (86501) voit     (86501)       38 2024-04-26 05:46:51.825947 bbo-calibcam-2.4.1/setup.cfg
+-rw-rw-r--   0 voit     (86501) voit     (86501)     1024 2024-04-26 05:46:03.000000 bbo-calibcam-2.4.1/setup.py
+drwxrwxr-x   0 voit     (86501) voit     (86501)        0 2024-04-26 05:46:51.825947 bbo-calibcam-2.4.1/test/
+-rw-rw-r--   0 voit     (86501) voit     (86501)     3290 2024-02-21 15:41:26.000000 bbo-calibcam-2.4.1/test/test_detection.py
```

### Comparing `bbo-calibcam-2.3.1/LICENSE` & `bbo-calibcam-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bbo-calibcam-2.3.1/PKG-INFO` & `bbo-calibcam-2.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbo-calibcam
-Version: 2.3.1
+Version: 2.4.1
 Summary: Calibrate intrinsic and extrinsic parameters of cameras with charuco boards
 Home-page: https://github.com/bbo-lab/calibcam
 Author: BBO-lab @ caesar
 Author-email: kay-michael.voit@mpinb.mpg.de
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bbo-calibcam-2.3.1/README.md` & `bbo-calibcam-2.4.1/README.md`

 * *Files identical despite different names*

### Comparing `bbo-calibcam-2.3.1/bbo_calibcam.egg-info/PKG-INFO` & `bbo-calibcam-2.4.1/bbo_calibcam.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbo-calibcam
-Version: 2.3.1
+Version: 2.4.1
 Summary: Calibrate intrinsic and extrinsic parameters of cameras with charuco boards
 Home-page: https://github.com/bbo-lab/calibcam
 Author: BBO-lab @ caesar
 Author-email: kay-michael.voit@mpinb.mpg.de
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bbo-calibcam-2.3.1/bbo_calibcam.egg-info/SOURCES.txt` & `bbo-calibcam-2.4.1/bbo_calibcam.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -17,11 +17,12 @@
 calibcam/detection.py
 calibcam/exceptions.py
 calibcam/helper.py
 calibcam/helper_ag.py
 calibcam/optimization.py
 calibcam/pose_estimation.py
 calibcam/single_camcalibration.py
+calibcam/yaml_helper.py
 calibcam/opt_jacfwd/__init__.py
 calibcam/opt_jacfwd/optfunctions.py
 calibcam/opt_jacfwd/optfunctions_ag.py
 test/test_detection.py
```

### Comparing `bbo-calibcam-2.3.1/calibcam/__main__.py` & `bbo-calibcam-2.4.1/calibcam/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,109 +1,139 @@
 #!/usr/bin/env python3
 import argparse
 import yaml
 import numpy as np
+from pathlib import Path
 
-from calibcam import calibrator_opts, helper
+from calibcam import calibrator_opts, helper, yaml_helper
 from calibcam.camcalibrator import CamCalibrator
 import timeit
 
 
 def main():
     print("Starting")
     tic = timeit.default_timer()
     # PArse command line arguments
     parser = argparse.ArgumentParser(description="Calibrate set of cameras")
+    # Input videos. Could probably also be a driect input (no flag) now
     parser.add_argument('--videos', type=str, required=False, nargs='*', default=None, help="")
-    parser.add_argument('--pipelines', type=str, required=False, nargs='*', default=None,
-                        help="Add pipeline readable by bbo-svidreader. "
-                             "The final output of the pipeline is used for calibration.")
-    parser.add_argument('--config', type=str, required=False, nargs=1, default=[None], help="")
+    # Process parameters, control if steps are performed or read from file
+    parser.add_argument('--detection', type=str, required=False, nargs='*', default=False)
+    parser.add_argument('--calibration_single', type=str, required=False, nargs='*', default=False)
+    parser.add_argument('--calibration_multi', required=False, default=False, action='store_true')
+    # Options
+    parser.add_argument('--opts', type=str, required=False, nargs='*', default=[],
+                        help="List of options files to include. Later files supersede earlier files, "
+                             "commandline arguments supersede files")
     parser.add_argument('--board', type=str, required=False, nargs=1, default=[None], help="")
-    parser.add_argument('--model', type=str, required=False, nargs=1, default=["pinhole"], help="")
+    parser.add_argument('--model', type=str, required=False, nargs='*', default=False, help="")
     parser.add_argument('--frame_step', type=int, required=False, nargs=1, default=[None], help="")
     parser.add_argument('--start_frame_indexes', type=int, required=False, nargs='*', default=None, help="")
-    parser.add_argument('--frames_masks', type=str, required=False, nargs=1, default=[None], help="A .npy file")
+    parser.add_argument('--stop_frame_indexes', type=int, required=False, nargs='*', default=None, help="")
+    parser.add_argument('--frames_masks', type=str, required=False, nargs=1, default=[None],
+                        help="A .npy file. The frames_masks start from the start_frame_indexes and end at "
+                             "the stop_frame_indexes if they are provided.")
     parser.add_argument('--optimize_only', required=False, default=None, action="store_true", help="")
     parser.add_argument('--numerical_jacobian', required=False, default=None, action="store_true", help="")
+    # Other
+    parser.add_argument('--pipelines', type=str, required=False, nargs='*', default=None,
+                        help="Add pipeline readable by bbo-svidreader. "
+                             "The final output of the pipeline is used for calibration.")
     parser.add_argument('--write_opts', type=str, required=False, nargs=1, default=[None], help="")
     parser.add_argument('--data_path', type=str, required=False, nargs=1, default=[None], help="")
 
     args = parser.parse_args()
 
-    # Fill options. These options supersede everything (defaults, saved file)
-    opts = {}
+    n_cams = len(args.videos)
+
+    # Build options from defaults and --opts parameters TODO: Currently not functional for yml, implement helpers!
+    opts = calibrator_opts.get_default_opts(n_cams)
+    for opts_file in args.opts:
+        opts_file = Path(opts_file)
+        if opts_file.suffix == ".yml":
+            with open(opts_file, "r") as file:
+                file_opts = yaml_helper.load_opts(yaml.safe_load(file))
+        elif opts_file.suffix == ".npy":
+            file_opts = np.load(opts_file, allow_pickle=True)[()]
+        else:
+            raise FileNotFoundError(f"{opts_file} is not supported")
+        opts = helper.deepmerge_dicts(file_opts, opts)
+
+    # Deal with process parameters
+    if not any([args.detection, args.calibration_single, args.calibration_multi]):
+        # No parameter has been set, which is interpreted as all desired
+        args.detection, args.calibration_single, args.calibration_multi = (True, True, True)
+    # Parameter with empty list means True
+    for param in ["detection", "calibration_single", "calibration_multi"]:
+        if isinstance(getattr(args, param), list):
+            if len(getattr(args, param)) == 0:
+                opts[param] = True
+            else:
+                opts[param] = getattr(args, param)
+        elif getattr(args, param):
+            opts[param] = True
+
+    # Fill commandline options
     if args.optimize_only is not None:
         opts['optimize_only'] = args.optimize_only
     if args.numerical_jacobian is not None:
         opts['numerical_jacobian'] = args.numerical_jacobian
-    if args.frame_step[0] is not None:
-        opts['frame_step'] = args.frame_step[0]
+    if args.model:
+        opts['models'] = args.model
 
-    # It is necessary for the videos to be in sync to perform multicalibration. If some videos lag behind other videos,
+    # It is necessary for the videos to be in sync to perform multi calibration. If some videos lag behind other videos,
     # start_frames_indexes should be provided to adjust for the lag.
     if args.start_frame_indexes is not None:
-        assert len(args.videos) == len(args.start_frame_indexes), "number of start_frame_indexes " \
+        assert len(args.start_frame_indexes) == n_cams, "number of start_frame_indexes " \
                                                                   "does not match number of videos!"
-        opts['start_frame_indexes'] = args.start_frame_indexes
-    # Use frames_masks together with start_frames_indexes only after fully understanding their use!
+        opts['start_frame_indexes'] = np.array(args.start_frame_indexes)
+
+    if args.frame_step[0] is not None:
+        opts['frame_step'] = args.frame_step[0]
+
+    # Sometimes, it is better to use only certain portion of the video for calibration.
+    # start_frame_indexes and stop_frame_indexes can be used to specify the frames to be used for calibration.
+    if args.stop_frame_indexes is not None:
+        assert len(args.stop_frame_indexes) == n_cams, "number of stop_frame_indexes " \
+                                                                 "does not match number of videos!"
+        opts['stop_frame_indexes'] = np.array(args.stop_frame_indexes)
+
+    # Use frames_masks together with start_frames_indexes to provide the frames to be used for calibration.
+    # TODO: EXPLAIN USE!!!
     if args.frames_masks[0] is not None:
         opts['init_frames_masks'] = args.frames_masks[0]
 
-    # Load details from config file
-    if isinstance(args.config[0], str):
-        with open(args.config[0], "r") as file:
-            config_dict = yaml.safe_load(file)
-            assert len(args.videos) == len(config_dict["cameras"]), "Number of cameras provided in the config file " \
-                                                                    "does not match the number of videos!"
-    else:
-        config_dict = {'cameras':
-                           [{'model': args.model[0]} for _ in args.videos]
-                       }
+    # Fill defaults for opts that depend on other opts
+    calibrator_opts.fill(opts)
 
-    # Write options to file for later editing. File in data_path will be automatically included and supersedes defaults
+    # Write options to file for later editing.
     if isinstance(args.write_opts[0], str):
-        cameras = config_dict['cameras']
-        save_opts = helper.deepmerge_dicts(opts, calibrator_opts.get_default_opts([cam['model'] for cam in cameras]))
-        np.save(args.write_opts[0] + "/opts.npy", save_opts, allow_pickle=True)
-        print(f"Options written to {args.write_opts[0] + '/opts.npy'}")
-
-    # Run calibration
-    if isinstance(args.videos[0], str):
-        recFileNames = sorted(args.videos)
-
-        if args.pipelines is None:
-            recPipelines = None
-        elif len(args.pipelines) == len(recFileNames):
-            recPipelines = [args.pipelines[args.videos.index(rec)] for rec in recFileNames]
-        elif len(args.pipelines) == 1:
-            recPipelines = args.pipelines * len(recFileNames)
-        else:
-            print("Sorry, the number of pipelines does not match the number of videos!")
-            raise RuntimeError
-
-        cameras = config_dict['cameras']
-        opts = helper.deepmerge_dicts(opts, calibrator_opts.get_default_opts([cam['model'] for cam in cameras]))
+        write_path = Path(args.write_opts[0])
+        with open(write_path / "opts.yml", "w") as file:
+            yaml.dump(yaml_helper.numpy_collection_to_list(opts), file)
+        np.save(write_path / "opts.npy", opts, allow_pickle=True)
+        print(f"Options written to {write_path / 'opts.{npy/yml}'}")
+
+    recFileNames = args.videos
+
+    if args.pipelines is None:
+        recPipelines = None
+    elif len(args.pipelines) == len(recFileNames):
+        recPipelines = args.pipelines
+    elif len(args.pipelines) == 1:
+        recPipelines = args.pipelines * len(recFileNames)
+    else:
+        print("Sorry, the number of pipelines does not match the number of videos!")
+        raise RuntimeError
 
-        # 'internals' will be deleted from the opts dictionary later.
-        opts['internals'] = [None for _ in cameras]
-        for i_cam, cam in enumerate(cameras):
-            if 'calibration_file' in cam.get('internals', {}):
-                idx_2get = cam['internals']['calibration_cam_idx']
-                opts['internals'][i_cam] = np.load(cam['internals']['calibration_file'],
-                                                   allow_pickle=True).item()['calibs'][idx_2get]
-            if not cam.get('internals', {}).get('optimize', True):
-                opts['free_vars'][i_cam]['A'][:] = False
-                opts['free_vars'][i_cam]['xi'] = False
-                opts['free_vars'][i_cam]['k'][:] = False
-
-        print(f"Camera models: {[cam['model'] for cam in cameras]}")
-        calibrator = CamCalibrator(recFileNames, pipelines=recPipelines, board_name=args.board[0], opts=opts, data_path=args.data_path[0])
-        calibrator.perform_multi_calibration()
-        print("Camera calibrated")
+    calibrator = CamCalibrator(recFileNames, pipelines=recPipelines, board_name=args.board[0], opts=opts,
+                               data_path=args.data_path[0])
+    calibrator.perform_multi_calibration()
+    print("Camera calibrated")
+    calibrator.close_readers()
 
     toc = timeit.default_timer()
 
     print(f"Overall procedure took {toc - tic} s")
 
     return
```

### Comparing `bbo-calibcam-2.3.1/calibcam/board.py` & `bbo-calibcam-2.4.1/calibcam/board.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 import os
 import numpy as np
 import pathlib
 import cv2
+from pathlib import Path
 
 
 def get_board_params(board_source):
-    if isinstance(board_source, pathlib.Path):
+    board_source = Path(board_source)
+    if board_source.is_file():
+        board_path = board_source.as_posix()
+    elif board_source.is_dir():
         board_path = board_source / 'board.npy'
     else:
-        board_path = os.path.join(os.path.dirname(os.path.abspath(__file__)), '../boards', board_source + '.npy')
+        board_path = os.path.join(os.path.dirname(os.path.abspath(__file__)), '../boards', board_source.as_posix() + '.npy')
 
     board_params = np.load(os.path.expanduser(board_path), allow_pickle=True).item()
 
     if board_params is not None:
         board_params['marker_size_real'] = board_params['square_size_real'] * board_params['marker_size']  # noqa
 
     return board_params
@@ -25,21 +29,27 @@
                                           board_params['marker_size'] * board_params['square_size_real'],
                                           cv2.aruco.getPredefinedDictionary(  # noqa
                                               board_params['dictionary_type']))
 
     return board
 
 
-def make_board_points(board_params):
+def make_board_points(board_params, exact=False):
     board_width = board_params['boardWidth']
     board_height = board_params['boardHeight']
-    square_size = board_params['square_size_real']
+    if exact:
+        square_size_x = board_params['square_size_real_x']
+        square_size_y = board_params['square_size_real_y']
+    else:
+        square_size_x = board_params['square_size_real']
+        square_size_y = board_params['square_size_real']
 
     n_corners = (board_width - 1) * (board_height - 1)
 
     board_0 = np.repeat(np.arange(1, board_width).reshape(1, board_width - 1), board_height - 1,
                         axis=0).ravel().reshape(n_corners, 1)
     board_1 = np.repeat(np.arange(1, board_height), board_width - 1, axis=0).reshape(n_corners, 1)
     board_2 = np.zeros(n_corners).reshape(n_corners, 1)
-    board = np.concatenate([board_0, board_1, board_2], 1) * square_size
+    board = np.concatenate([board_0 * square_size_x, board_1 * square_size_y,
+                            board_2], 1)
 
     return board  # n_corners x 3
```

### Comparing `bbo-calibcam-2.3.1/calibcam/calibrator_opts.py` & `bbo-calibcam-2.4.1/calibcam/calibrator_opts.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,82 +1,127 @@
 import cv2
 import numpy as np
 
 
-def get_default_opts(models=["pinhole"]):
-
+def get_default_opts(ncams=0, do_fill=False):
     default_opts = {
-        'debug': True,  # Will enable advanced tests and outputs
-        'jax_backend': 'cpu',  # GPU regularly runs out of memory for these problems
-        'coord_cam': 0,  # Reference camera that defines the multicam coordinate system
-        'frame_step': 1,  # Skip frames in recording
-        'allow_unequal_n_frame': True,  # Sometimes last frame is cut, so this may be okay.
-        'common_pose_r_err': 0.1,  # Iteratively exclude poses with higher rotation deviation from mean
-        'color_convert': False,  # Set to cv2.COLOR_RGB2GRAY to convert rgb images to grayscale for corner detection
-        'detect_cpu_divisor': 6,  # use N_CPU/detect_cpu_divisor threads for feature detection
-        'optimize_only': False,
+        # === Program function control ===
+        # If True, calibcam will perform detections. If list of yml files, these files will be used instead
+        'detection': False,
+        # If True, calibcam will perform single cam calibrations. If list of yml files, these files will be used instead
+        'calibration_single': False,
+        # If True, calibcam will perform multi cam calibration.
+        'calibration_multi': False,
+
+        # === Camera system description
+        # Number of cams
+        'n_cams': ncams,
+        # Camera models. Will be filled with opts["n_cams"]*["pinhole"] if left False
+        'models': False,
+        # Free variables. Will be filled with get_free_vars() if left False
+        'free_vars': False,
+
+        # === Settings ===
+        # Will enable advanced tests and outputs
+        'debug': True,
+        # GPU regularly runs out of memory for these problems
+        'jax_backend': 'cpu',
+        # Reference camera that defines the multicam coordinate system
+        'coord_cam': 0,
+        # Skip frames in recording
+        'frame_step': 1,
+        # Sometimes last frame is cut, so this may be okay.
+        'allow_unequal_n_frame': True,
+        # Iteratively exclude poses with higher rotation deviation from mean
+        'common_pose_r_err': 0.1,
+        # Set to cv2.COLOR_RGB2GRAY to convert rgb images to grayscale for corner detection
+        'color_convert': False,
+        # use N_CPU/detect_cpu_divisor threads for feature detection
+        'detect_cpu_divisor': 6,
+        # Use radial contrast value for rejecting corners, check rejection params below in detection_opts
+        'RC_reject_corners': False,
+        # DEPRECATED
         # Do not perform detection and single cam calibration. (Disable mostly for development.)
-        'numerical_jacobian': False,  # Use 2-point numerical jacobian instead of jax.jacobian
+        'optimize_only': False,
+        # Use 2-point numerical jacobian instead of jax.jacobian
+        'numerical_jacobian': False,
         # Optimise individual cameras immediately after performing opencv single calibration
         'optimize_ind_cams': False,
-
         # Optimize individual board poses then all params again.
         # In a test, optimality was already reached after a first general optimization
         'optimize_board_poses': False,
-        'max_allowed_res': 2.0,  # In pixels. replace the pose with higher error and insert 'nearby' pose with lower
+        # In pixels. replace the pose with higher error and insert 'nearby' pose with lower
         # error while optimizing individual board poses.
+        'max_allowed_res': 5.0,
 
-        'reject_corners': False,  # Reject corners with high zscore, check rejection params below
-
-        'free_vars': [get_free_vars(model) for model in models],
-        'detection': {
+        'detection_opts': {
             'inter_frame_dist': 1.0,  # In pixels
+            'min_corners': 5,  # Minimum number of corners to detect in a frame
             'aruco_detect': {
                 'parameters': get_detector_parameters_opts(),
             },
             'aruco_refine': {
                 'minRepDistance': 3.0,
                 'errorCorrectionRate': 1.0,
                 'checkAllOrders': True,
                 'parameters': get_detector_parameters_opts(),
             },
             'aruco_interpolate': {
                 'minMarkers': 2,
             },
+            'radial_contrast_reject': {
+                'options': {'lib': 'np'},
+                'width': 20,
+                'normalize': 50,
+                'norm_mean': 0.311,
+            }
         },
-        'aruco_calibration': [{
-            'flags': get_flags(model),
-            'criteria': (cv2.TermCriteria_COUNT + cv2.TermCriteria_EPS,
-                         30,
-                         float(np.finfo(np.float32).eps)),
-        } for model in models],
+        'aruco_calibration': False,
         'pose_estimation': {
             'use_required_corners': True,
         },
         'optimization': {
             'method': 'trf',
             'ftol': 1e-9,
             'xtol': 1e-9,
             'gtol': 1e-9,
             'x_scale': 'jac',
             'loss': 'linear',
             'tr_solver': 'exact',
             'max_nfev': 120,
             'verbose': 2,
-        },
-        'rejection': {
-            'max_zscore': 3.0,
-            'max_res': 2.0,  # in pixels, only reject corners with high residual (rep. error) and zscore
-            'reject_poses': True  # Reject degenerate poses
         }
     }
 
+    if do_fill:
+        fill(default_opts)
+
     return default_opts
 
 
+def fill(opts):
+    if not opts["models"]:
+        opts["models"] = opts["n_cams"] * ["pinhole"]
+    if len(opts["models"]) == 1:
+        opts["models"] *= opts["n_cams"]
+
+    if not opts["free_vars"]:
+        opts["free_vars"] = [get_free_vars(model) for model in opts["models"]]
+
+    if not opts["aruco_calibration"]:
+        opts['aruco_calibration'] = [{
+            'flags': get_flags(model),
+            'criteria': (cv2.TermCriteria_COUNT + cv2.TermCriteria_EPS,
+                         30,
+                         float(np.finfo(np.float32).eps)),
+        } for model in opts["models"]]
+
+    return opts  # not necessarily required due to pass by reference
+
+
 def get_free_vars(model: str):
     free_vars = {
         'cam_pose': True,
         'board_poses': True,
         'A': np.asarray([[True, False, True],  # a   c   u   (c is skew and should not be necessary)
                          [False, True, True],  # 0   b   v
                          [False, False, False],  # 0   0   1
@@ -105,15 +150,15 @@
 
     return flags
 
 
 def get_detector_parameters_opts():
     detector_parameters = {  # SPOT for detector params
         'adaptiveThreshWinSizeMin': 15,
-        'adaptiveThreshWinSizeMax': 30,
+        'adaptiveThreshWinSizeMax': 45,
         'adaptiveThreshWinSizeStep': 5,
 
         'cornerRefinementMethod': cv2.aruco.CORNER_REFINE_SUBPIX,
         'cornerRefinementWinSize': 3,
         'cornerRefinementMaxIterations': 60,
         'cornerRefinementMinAccuracy': 0.05,
```

### Comparing `bbo-calibcam-2.3.1/calibcam/camcalibrator.py` & `bbo-calibcam-2.4.1/calibcam/camcalibrator.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-import copy
 import os
 from copy import deepcopy
 
 import numpy as np
 from scipy.io import savemat as scipy_io_savemat
 import cv2
+import matplotlib.pyplot as plt
 
 from pathlib import Path
+import yaml
 
 from ccvtools import rawio  # noqa
 from svidreader import filtergraph
 
 import multiprocessing
 from joblib import Parallel, delayed
 
@@ -19,24 +20,27 @@
 from calibcam.exceptions import *
 from calibcam import helper, camfunctions, board, compatibility
 
 from calibcam.calibrator_opts import get_default_opts
 from calibcam.pose_estimation import estimate_cam_poses
 from calibcam.single_camcalibration import calibrate_single_camera
 
+from calibcam import yaml_helper
+
 
 class CamCalibrator:
     def __init__(self, recordings, pipelines=None, board_name=None, data_path=None, calibs_init=None, opts=None):
         if opts is None:
             opts = {}
 
         self.board_name = board_name  # Currently, recordings are needed to determine the board path in most cases
 
         if data_path is not None:
             self.data_path = data_path
+            os.makedirs(self.data_path, exist_ok=True)
         else:
             self.data_path = os.path.expanduser(os.path.dirname(recordings[0]))
 
         # Board
         self.board_params = None
 
         # Videos
@@ -63,35 +67,36 @@
             board_params = board.get_board_params(board_name)
         else:
             board_params = board.get_board_params(Path(self.rec_file_names[0]).parent)
         return board_params
 
     @staticmethod
     def load_calibs_init(calibs_init, data_path=None):
-        calib_init_path = data_path + "/multicam_calibration.npy"
+        # TODO Remove this in favor of a commandline option
+        calib_init_path = data_path + "/multicam_calibration_init.npy"
         if calibs_init is None and data_path is not None and os.path.isfile(calib_init_path):
             print(f"Loading initialization from {calib_init_path}")
             calibs_init = np.load(calib_init_path, allow_pickle=True).item()["calibs"]
 
         return calibs_init
 
     @staticmethod
     def load_opts(opts, data_path=None):
         if data_path is not None and os.path.isfile(data_path + "/opts.npy"):
             fileopts = np.load(data_path + "/opts.npy", allow_pickle=True).item()
             opts = helper.deepmerge_dicts(opts, fileopts)
 
-        return helper.deepmerge_dicts(opts, get_default_opts())
+        return helper.deepmerge_dicts(opts, get_default_opts(0))
 
     def load_recordings(self, recordings, pipelines=None):
         # check if input files are valid files
         try:
             self.readers = []
             for irec, rec in enumerate(recordings):
-                reader = filtergraph.get_reader(rec, backend="iio")
+                reader = filtergraph.get_reader(rec, backend="iio", cache=False)
                 if pipelines is not None:
                     fg = filtergraph.create_filtergraph_from_string([reader], pipelines[irec])
                     reader = fg['out']
                 self.readers.append(reader)
         except ValueError:
             print('At least one unsupported format supplied')
             raise UnsupportedFormatException
@@ -117,147 +122,193 @@
                 self.n_frames = np.int64(np.min(n_frames))
             else:
                 # raise exception for outside confirmation
                 raise UnequalFrameCountException
 
         self.board_params = self.get_board_params_from_name(self.board_name)
 
+    def close_readers(self):
+        if not self.readers:
+            return
+        for reader in self.readers:
+            reader.close()
+
     def perform_multi_calibration(self):
         n_corners = (self.board_params["boardWidth"] - 1) * (self.board_params["boardHeight"] - 1)
         required_corner_idxs = [0,
                                 self.board_params["boardWidth"] - 2,
                                 (self.board_params["boardWidth"] - 1) * (self.board_params["boardHeight"] - 2),
                                 (self.board_params["boardWidth"] - 1) * (self.board_params["boardHeight"] - 1) - 1,
                                 ]  # Corners that we require to be detected for pose estimation
-        if self.opts["optimize_only"]:  # We expect that detections and single cam calibs are already present
-            preoptim = np.load(self.data_path + '/preoptim.npy', allow_pickle=True)[()]
-            preoptim = compatibility.update_preoptim(preoptim, n_corners)
-
-            del self.opts['internals']
-            calibs_single = preoptim['info']['other']['calibs_single']
-            used_frames_ids = preoptim['info']['used_frames_ids']
-            corners = preoptim['info']['corners']
 
-            # We just redo this since it is fast and the output may help
-            calibs_multi = estimate_cam_poses(calibs_single, self.opts, corners=corners,
-                                              required_corner_idxs=required_corner_idxs)
-        else:
+        # === Detection ===
+        if isinstance(self.opts["detection"], list):
+            # TODO: Support True in the list instead of strings to only detect individual cams
+            assert len(self.opts["detection"]) == self.opts["n_cams"], ("Number of detection files must be equal "
+                                                                        "to number of cameras")
+
+            corners = []
+            used_frames_ids = []
+            for detection_file in self.opts["detection"]:
+                detection_file = Path(detection_file)
+                if detection_file.suffix == ".yml":
+                    with open(detection_file, "r") as file:
+                        detection = yaml.safe_load(file)
+                elif detection_file.suffix == ".npy":
+                    detection = np.load(detection_file, allow_pickle=True)[()]
+                else:
+                    raise FileNotFoundError(f"{detection_file} is not supported")
+
+                # For multicam_calibration files
+                if ("corners" not in detection) and ("info" in detection):
+                    detection = detection["info"]
+
+                corners.append(np.squeeze(detection["corners"]))
+                used_frames_ids.append(np.array(detection["used_frames_ids"]))
+
+            used_frames_ids = used_frames_ids[0]
+            corners = np.array(corners)
+        elif self.opts["detection"]:
             # detect corners
             # Corners are originally detected by cv2 as ragged lists with additional id lists (to determine which
             # corners the values refer to) and frame masks (to determine which frames the list elements refer to).
             # This saves memory, but significantly increases complexity of code as we might index into camera frames,
             # used frames or global frames. For simplification, corners are returned as a single matrix of shape
             #  n_cams x n_timepoints_with_used_detections x n_corners x 2
-            # Memory footprint at this stage is al but critical.
-            corners, used_frames_ids = \
-                detect_corners(self.rec_file_names, self.n_frames, self.board_params, self.opts,
-                               rec_pipelines=self.rec_pipelines)
-
-            calibs_single = self.obtain_single_cam_calibrations(calibs_single=self.opts.pop('internals'),
-                                                                corners=corners)
+            # Memory footprint at this stage is not critical.
+            corners, used_frames_ids = detect_corners(self.rec_file_names, self.n_frames, self.board_params, self.opts,
+                                                      rec_pipelines=self.rec_pipelines)
+
+            for i_cam, (rfn, c) in enumerate(zip(self.rec_file_names, corners)):
+                detection = {
+                    "rec_file_name": rfn,  # Not used in readout, only for reference
+                    "corners": c.tolist(),
+                    "used_frames_ids": used_frames_ids.tolist()
+                }
+                with open(Path(self.data_path) / f"detection_{i_cam:03d}.yml", "w") as file:
+                    yaml.dump(detection, file, default_flow_style=True)
+        else:
+            print("Cannot proceed without detections. Exiting.")
+            return
 
+        # === Single cam calibration ===
+        if isinstance(self.opts["calibration_single"], list):
+            # TODO: Support True in the list instead of strings to only detect individual cams
+            assert len(self.opts["calibration_single"]) == self.opts["n_cams"], ("Number of calibration_single files "
+                                                                                 "must be equal to number of cameras")
+            calibs_single = []
+            for calibration_single_file in self.opts["calibration_single"]:
+                calibration_single_file = Path(calibration_single_file)
+                if calibration_single_file.suffix == ".yml":
+                    with open(calibration_single_file, "r") as file:
+                        calibs_single.append(yaml_helper.load_calib(yaml.safe_load(file)))
+                elif calibration_single_file.suffix == ".npy":
+                    calib = np.load(calibration_single_file, allow_pickle=True)[()]
+                    # For multicam_calibration files
+                    if "calibs" in calib:
+                        calib = calib["calibs"][0]
+                    calibs_single.append(calib)
+                else:
+                    raise FileNotFoundError(f"{calibration_single_file} is not supported")
+            calibs_single = self.obtain_single_cam_calibrations(corners=corners, calibs_single=calibs_single)
+        elif self.opts["calibration_single"]:
+            calibs_single = self.obtain_single_cam_calibrations(corners=corners)
             if self.opts['optimize_ind_cams']:
                 for i_cam, calib in enumerate(calibs_single):
                     # analytically estimate initial camera poses
+                    # Although we don't have camera poses at this step, we use this function to correctly structure the
+                    # calibs_single to optimize poses.
                     calibs_interim = estimate_cam_poses([calib], self.opts, corners=corners[[i_cam]],
                                                         required_corner_idxs=required_corner_idxs)
 
                     calibs_fit_single, rvecs_boards, tvecs_boards, _, _ = self.optimize_poses(corners[[i_cam]],
                                                                                               calibs_interim)
                     calibs_single[i_cam].update(
                         helper.combine_calib_with_board_params(calibs_fit_single, rvecs_boards, tvecs_boards)[0])
                     calibs_single[i_cam]['frames_mask'] = np.sum(~np.isnan(corners[i_cam][:, :, 1]), axis=1) > 0
+        else:
+            print("Cannot proceed without single cam calbrations. Exiting.")
+            return
 
+        for i_cam, calib_single in enumerate(calibs_single):
+            save_path = Path(self.data_path) / f"calibration_single_{i_cam:03d}.yml"
+            with open(save_path, "w") as file:
+                yaml.dump(yaml_helper.numpy_collection_to_list(calib_single), file, default_flow_style=True)
+            # np.save(save_path.with_suffix(".npy"), calib_single, allow_pickle=True)
+
+        # === Multi cam calibration ===
+        if self.opts["calibration_multi"]:
             # analytically estimate initial camera poses
             calibs_multi = estimate_cam_poses(calibs_single, self.opts, corners=corners,
                                               required_corner_idxs=required_corner_idxs)
 
-            # Save intermediate result, for dev purposes on optimization (quote code above and unquote code below)
-            # pose_params = optimization.make_common_pose_params(calibs_multi, corners)
-            result = self.build_result(calibs_multi,
-                                       corners=corners, used_frames_ids=used_frames_ids,
-                                       # rvecs_boards=pose_params[0], tvecs_boards=pose_params[1],
-                                       other={'calibs_single': calibs_single})
-            self.save_multicalibration(result, 'preoptim')
-
-        if self.opts['debug']:
-            args, vars_free = make_optim_input(self.board_params, calibs_multi, corners, self.opts)
-            test_objective_function(calibs_multi, vars_free, args, corners, self.board_params,
-                                    individual_poses=True)
-
-        print('OPTIMIZING ALL POSES')
-        # self.plot(calibs_single, corners, used_frames_ids, self.board_params, 3, 35)
-        calibs_fit, rvecs_boards, tvecs_boards, min_result, args = self.optimize_poses(corners, calibs_multi)
-
-        if self.opts['debug']:
-            calibs_fit = helper.combine_calib_with_board_params(calibs_fit, rvecs_boards, tvecs_boards)
-            test_objective_function(calibs_fit, min_result.x, args, corners, self.board_params,
-                                    individual_poses=True)
+            if self.opts['debug']:
+                args, vars_free = make_optim_input(self.board_params, calibs_multi, corners, self.opts)
+                test_objective_function(calibs_multi, vars_free, args, corners, self.board_params,
+                                        individual_poses=True)
 
-        print('OPTIMIZING ALL PARAMETERS I')
-        calibs_fit, rvecs_boards, tvecs_boards, min_result, args = self.optimize_calibration(corners, calibs_fit)
+            print('OPTIMIZING ALL POSES')
+            # self.plot(calibs_single, corners, used_frames_ids, self.board_params, 3, 35)
+            calibs_fit, rvecs_boards, tvecs_boards, min_result, args = self.optimize_poses(corners, calibs_multi)
 
-        # According to tests with good calibration recordings, the following steps are unnecessary and optimality was
-        #  already reached in the previous step
-        if self.opts["optimize_board_poses"]:
             if self.opts['debug']:
                 calibs_fit = helper.combine_calib_with_board_params(calibs_fit, rvecs_boards, tvecs_boards)
                 test_objective_function(calibs_fit, min_result.x, args, corners, self.board_params,
                                         individual_poses=True)
 
-            print('OPTIMIZING BOARD POSES')
-            calibs_fit, rvecs_boards, tvecs_boards, _, _ = self.optimize_board_poses(corners, calibs_fit,
-                                                                                                 prev_fun=min_result.fun)
-            calibs_fit = helper.combine_calib_with_board_params(calibs_fit, rvecs_boards, tvecs_boards)
-
-            print('OPTIMIZING ALL PARAMETERS II')
+            print('OPTIMIZING ALL PARAMETERS I')
             calibs_fit, rvecs_boards, tvecs_boards, min_result, args = self.optimize_calibration(corners, calibs_fit)
 
-        if self.opts["reject_corners"]:
+            # According to tests with good calibration recordings, the following steps are unnecessary and optimality
+            # was already reached in the previous step
+            if self.opts["optimize_board_poses"]:
+                if self.opts['debug']:
+                    calibs_fit = helper.combine_calib_with_board_params(calibs_fit, rvecs_boards, tvecs_boards)
+                    test_objective_function(calibs_fit, min_result.x, args, corners, self.board_params,
+                                            individual_poses=True)
+
+                print('OPTIMIZING BOARD POSES')
+                calibs_fit, rvecs_boards, tvecs_boards, _, _ = self.optimize_board_poses(corners, calibs_fit,
+                                                                                         prev_fun=min_result.fun)
+                calibs_fit = helper.combine_calib_with_board_params(calibs_fit, rvecs_boards, tvecs_boards)
+
+                print('OPTIMIZING ALL PARAMETERS II')
+                calibs_fit, rvecs_boards, tvecs_boards, min_result, args = self.optimize_calibration(corners, calibs_fit)
+
+            # No board poses in final calibration!
+            calibs_test = helper.combine_calib_with_board_params(calibs_fit, rvecs_boards, tvecs_boards, copy=True)
+            test_objective_function(calibs_test, min_result.x, args, corners, self.board_params,
+                                    individual_poses=True)
+
             result = self.build_result(calibs_fit,
                                        corners=corners, used_frames_ids=used_frames_ids,
                                        min_result=min_result, args=args,
                                        rvecs_boards=rvecs_boards, tvecs_boards=tvecs_boards,
                                        other={'calibs_single': calibs_single, 'calibs_multi': calibs_multi,
-                                                'board_coords_3d_0': board.make_board_points(self.board_params)})
-            self.save_multicalibration(result, 'prereject')
-
-            print('INSPECTING CORNERS')
-            corners, rejected_poses, rejected_corners = helper.reject_corners(corners, min_result.fun,
-                                                                              self.board_params,
-                                                                              self.opts["rejection"])
-            rvecs_boards = rvecs_boards[~rejected_poses]
-            tvecs_boards = tvecs_boards[~rejected_poses]
-            used_frames_ids = used_frames_ids[~rejected_poses]
-            calibs_fit = helper.combine_calib_with_board_params(calibs_fit, rvecs_boards, tvecs_boards)
+                                              'board_coords_3d_0': board.make_board_points(self.board_params)})
 
-            print('OPTIMIZING ALL PARAMETERS III')
-            calibs_fit, rvecs_boards, tvecs_boards, min_result, args = self.optimize_calibration(corners, calibs_fit)
-
-        # No board poses in final calibration!
-        calibs_test = helper.combine_calib_with_board_params(calibs_fit, rvecs_boards, tvecs_boards, copy=True)
-        test_objective_function(calibs_test, min_result.x, args, corners, self.board_params,
-                                individual_poses=True)
-
-        result = self.build_result(calibs_fit,
-                                   corners=corners, used_frames_ids=used_frames_ids,
-                                   min_result=min_result, args=args,
-                                   rvecs_boards=rvecs_boards, tvecs_boards=tvecs_boards,
-                                   other={'calibs_single': calibs_single, 'calibs_multi': calibs_multi,
-                                          'board_coords_3d_0': board.make_board_points(self.board_params)})
-
-        print('SAVE MULTI CAMERA CALIBRATION')
-        self.save_multicalibration(result)
-        # Builds a part of the v1 result that is necessary for other software
-        self.save_multicalibration(helper.build_v1_result(result), 'multicalibration_v1')
-
-        print('FINISHED MULTI CAMERA CALIBRATION')
+            print('SAVE MULTI CAMERA CALIBRATION')
+            self.save_multicalibration(result)
+            # Builds a part of the v1 result that is necessary for other software
+            self.save_multicalibration(helper.build_v1_result(result), 'multicalibration_v1')
+            print('SAVE FIUGRE WITH DETECTIONS')
+            rep_err = min_result.fun.reshape(corners.shape)
+            for i_cam, (i_reader, c, err) in enumerate(zip(self.readers, corners, rep_err)):
+                fig_cam = self.get_corners_cam_fig(camfunctions.get_header_from_reader(i_reader)['sensorsize'],
+                                                   c, err)
+                fig_cam.savefig(self.data_path + f"/detections_cam_{i_cam:03d}.svg", dpi=300, bbox_inches='tight')
+            print('FINISHED MULTI CAMERA CALIBRATION')
+        else:
+            return
+            
         return
 
-    def obtain_single_cam_calibrations(self, calibs_single, corners):
+    def obtain_single_cam_calibrations(self, corners, calibs_single=None):
+        if calibs_single is None:
+            calibs_single = len(corners)*[None]
 
         cams_2calibrate = []
         for i_cam, cam_calib in enumerate(calibs_single):
             if cam_calib is not None:
                 calibs_single[i_cam] = self.estimate_board_positions_in_single_cam(cam_calib, corners[i_cam])
             else:
                 cams_2calibrate.append(i_cam)
@@ -302,27 +353,27 @@
         calib['rvecs'] = np.full((corners_cam.shape[0], 3), np.nan)
         calib['tvecs'] = np.full((corners_cam.shape[0], 3), np.nan)
         calib['frames_mask'] = mask
 
         pose_idxs = np.where(mask)[0]
         for pose_idx, pos in zip(pose_idxs, board_positions):
             if pos[0]:
-                calib['rvecs'][pose_idx] = pos[1][:,0]
-                calib['tvecs'][pose_idx] = pos[2][:,0]
+                calib['rvecs'][pose_idx] = pos[1][:, 0]
+                calib['tvecs'][pose_idx] = pos[2][:, 0]
             else:
                 calib['frames_mask'][pose_idx] = False
 
         return calib
 
     @staticmethod
     def estimate_single_board_position(calib, corners, ids, board_params, opts):
         if len(ids) < 4:
             return 0, np.full((3,), np.nan), np.full((3,), np.nan)
 
-        retval, rvec, tvec = cv2.solvePnP(board.make_board_points(board_params)[ids].reshape((-1,3)),
+        retval, rvec, tvec = cv2.solvePnP(board.make_board_points(board_params)[ids].reshape((-1, 3)),
                                           corners.reshape((-1, 2)),
                                           calib["A"], calib["k"],
                                           flags=cv2.SOLVEPNP_IPPE)
         return retval, rvec, tvec
 
     def perform_single_cam_calibrations(self, corners, camera_indexes=None, calibs_init=None):
         print('PERFORM SINGLE CAMERA CALIBRATION')
@@ -376,17 +427,17 @@
     def optimize_board_poses(self, corners, calibs_multi, opts=None, board_params=None, prev_fun=None):
         if opts is None:
             opts = self.opts
         if board_params is None:
             board_params = self.board_params
 
         pose_opts = deepcopy(opts)
-        pose_opts['optimization']['ftol'] = 1e-13
-        pose_opts['optimization']['gtol'] = 1e-13
-        pose_opts['optimization']['xtol'] = 1e-13
+        pose_opts['optimization']['ftol'] = 1e-14
+        pose_opts['optimization']['gtol'] = 1e-14
+        pose_opts['optimization']['xtol'] = 1e-14
         free_vars = pose_opts['free_vars']
         for cam in free_vars:
             cam['cam_pose'] = False
             cam['A'][:] = False
             cam['k'][:] = False
             cam['xi'] = False
 
@@ -405,15 +456,16 @@
 
         print("Number of bad_poses:", len(calibs_multi[0]['rvecs']) - len(good_poses))
         print(f"Optimizing {len(calibs_multi[0]['rvecs'])} poses: ", end='')
         for i_pose in range(len(calibs_multi[0]["rvecs"])):
             print(".", end='', flush=True)
             corners_pose = corners[:, [i_pose]]
             for calib, calib_orig in zip(calibs_multi_pose, calibs_multi):
-                nearest_i_pose = helper.nearest_element(i_pose, good_poses)  # nearest_i_pose = i_pose if i_pose in good_poses
+                nearest_i_pose = helper.nearest_element(i_pose,
+                                                        good_poses)  # nearest_i_pose = i_pose if i_pose in good_poses
                 calib["rvecs"] = calib_orig["rvecs"][[nearest_i_pose]]
                 calib["tvecs"] = calib_orig["tvecs"][[nearest_i_pose]]
 
             # print(i_pose, rvecs_boards[i_pose])
             calibs_fit_pose, rvecs_boards[i_pose], tvecs_boards[i_pose], min_result, args = \
                 camfunctions.optimize_calib_parameters(corners_pose, calibs_multi_pose, board_params, opts=pose_opts,
                                                        verbose=0)
@@ -444,15 +496,15 @@
         if rvecs_boards is None:
             rvecs_boards = []
         if used_frames_ids is None:
             used_frames_ids = []
         if corners is None:
             corners = []
         result = {
-            'version': 2.2,  # Increase when this structure changes
+            'version': 2.3,  # Increase when this structure changes
             'calibs': calibs,
             # This field shall always hold all intrinsically necessary information to project and triangulate.
             'board_params': self.board_params,  # All parameters to recreate the board
             'rec_file_names': self.rec_file_names,  # Recording filenames, may be used for cam names
             'vid_headers': [camfunctions.get_header_from_reader(r) for r in self.readers],
             # Headers. No content structure guaranteed
             'info': {  # Additional nonessential info from the calibration process
@@ -475,18 +527,20 @@
             result['info']['cost_val_final'] = min_result.cost
             result['info']['optimality_final'] = min_result.optimality
 
         return result
 
     def save_multicalibration(self, result, filename="multicam_calibration"):
         # save
-        result_path = self.data_path + '/' + filename
-        np.save(result_path + '.npy', result)
-        scipy_io_savemat(result_path + '.mat', result)
-        print('Saved multi camera calibration to file {:s}'.format(result_path))
+        result_path = Path(self.data_path + '/' + filename)
+        np.save(result_path.with_suffix('.npy'), result)
+        scipy_io_savemat(result_path.with_suffix('.mat'), result)
+        with open(result_path.with_suffix('.yml'), "w") as yml_file:
+            yaml.dump(yaml_helper.numpy_collection_to_list(result), yml_file, default_flow_style=True)
+        print(f'Saved multi camera calibration to file {result_path}')
         return
 
     # Debug function
     def plot(self, calibs, corners, used_frames_ids, board_params, cidx, fidx):
         import matplotlib.pyplot as plt
         from scipy.spatial.transform import Rotation as R  # noqa
         import camfunctions_ag
@@ -514,7 +568,27 @@
         board_coords_3d_d = camfunctions_ag.distort(board_coords_3d, calibs[cidx]['k'])
         board_coords_3d_d = camfunctions_ag.ideal_to_sensor(board_coords_3d_d, calibs[cidx]['A'])
 
         plt.plot(board_coords_3d_d[(0, 4, 34), 0], board_coords_3d_d[(0, 4, 34), 1], 'r+')
         plt.plot(board_coords_3d_nd[(0, 4, 34), 0], board_coords_3d_nd[(0, 4, 34), 1], 'g+')
 
         plt.show()
+
+    @staticmethod
+    def get_corners_cam_fig(im_shape, corners_cam, repro_err_cam):
+
+        im_w, im_h = im_shape
+        corners_cam = corners_cam.reshape(-1, 2)
+        repro_err_cam = repro_err_cam.reshape(-1, 2)
+
+        fig, ax = plt.subplots()
+        ax.errorbar(corners_cam[:, 0], corners_cam[:, 1],
+                    fmt=".", ms=1.2,
+                    xerr=np.absolute(repro_err_cam[:, 0]), yerr=np.absolute(repro_err_cam[:, 0]),
+                    elinewidth=0.8, ecolor="red")
+        ax.set_xlim(0, im_w)
+        ax.set_ylim(0, im_h)
+        ax.set_xlabel("Image x (pix.)")
+        ax.set_ylabel("Image y (pix.)")
+        ax.invert_yaxis()
+
+        return fig
```

### Comparing `bbo-calibcam-2.3.1/calibcam/camfunctions.py` & `bbo-calibcam-2.4.1/calibcam/camfunctions.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import sys
 
 
 def optimize_calib_parameters(corners, calibs_multi, board_params, opts=None, verbose=None):
     if opts is None:
         opts = {}
 
-    defaultopts = calibrator_opts.get_default_opts()
+    defaultopts = calibrator_opts.get_default_opts(len(corners))
     opts = helper.deepmerge_dicts(opts, defaultopts)
 
     if verbose is None:
         verbose = opts['optimization']['verbose']
     else:
         opts['optimization']['verbose'] = verbose
```

### Comparing `bbo-calibcam-2.3.1/calibcam/camfunctions_ag.py` & `bbo-calibcam-2.4.1/calibcam/camfunctions_ag.py`

 * *Files identical despite different names*

### Comparing `bbo-calibcam-2.3.1/calibcam/compatibility.py` & `bbo-calibcam-2.4.1/calibcam/compatibility.py`

 * *Files identical despite different names*

### Comparing `bbo-calibcam-2.3.1/calibcam/detection.py` & `bbo-calibcam-2.4.1/calibcam/detection.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,28 +9,24 @@
 from calibcam import camfunctions, board, helper
 from calibcam.calibrator_opts import finalize_aruco_detector_opts
 
 
 def detect_corners(rec_file_names, n_frames, board_params, opts, rec_pipelines=None, return_matrix=True):
     print('DETECTING FEATURES')
 
-    if 'start_frame_indexes' in opts:
-        start_frm_indexes = opts['start_frame_indexes']
-        stop_frm_indexes = list(np.ones(len(rec_file_names), dtype='int')*(n_frames - np.max(start_frm_indexes))
-                            + np.asarray(start_frm_indexes))
-    else:
-        start_frm_indexes = [0]*len(rec_file_names)
-        stop_frm_indexes = [None]*len(rec_file_names)
-
+    start_frm_indexes = opts.get('start_frame_indexes', np.zeros(len(rec_file_names), dtype=int))
+    stop_frm_indexes = opts.get('stop_frame_indexes', np.full(len(rec_file_names), fill_value=n_frames, dtype=int))
     if rec_pipelines is None:
         rec_pipelines = [None] * len(rec_file_names)
+
     init_frames_masks = opts.get('init_frames_masks', [None] * len(rec_file_names))
     if isinstance(init_frames_masks, str):
         init_frames_masks = np.load(init_frames_masks)
-    fin_frames_masks = np.zeros(shape=(len(rec_file_names), n_frames - np.max(start_frm_indexes)), dtype=bool)
+
+    fin_frames_masks = np.zeros(shape=(len(rec_file_names), np.min(stop_frm_indexes - start_frm_indexes)), dtype=bool)
     corners_all = []
     ids_all = []
 
     # Empirically, detection seems to utilize about 6 cores
     detections = Parallel(n_jobs=int(np.floor(multiprocessing.cpu_count() // opts['detect_cpu_divisor'])))(
         delayed(detect_corners_cam)(rec_file_name, opts, board_params, start_frm_indexes[i_rec],
                                     stop_frm_indexes[i_rec], init_frames_masks[i_rec],
@@ -53,92 +49,117 @@
 def detect_corners_cam(video, opts, board_params, start_frm_idx=0, stop_frm_idx=None, init_frames_mask=None, rec_pipeline=None):
 
     reader = filtergraph.get_reader(video, backend="iio", cache=False)
     if rec_pipeline is not None:
         fg = filtergraph.create_filtergraph_from_string([reader], rec_pipeline)
         reader = fg['out']
 
+    # We take offset into consideration at corner detection level. This means that the calibration parameters always
+    # refer to the offset-free pixel positions and offsets do NOT have to be taken into account anywhere in
+    # this calibration procedure or when working with the
+    offset_x, offset_y = camfunctions.get_header_from_reader(reader)['offset']
+
+    if opts['RC_reject_corners']:
+        # Reject corners based on radial contrast value
+        RC_params = opts['detection_opts']['radial_contrast_reject']
+        RC_reader = helper.RadialContrast(reader, **RC_params)
+
     if stop_frm_idx is None:
         stop_frm_idx = camfunctions.get_n_frames_from_reader(reader)
 
     corners_cam = []
     ids_cam = []
     if init_frames_mask is None:
         init_frames_mask = np.ones(stop_frm_idx - start_frm_idx, dtype=bool)
     fin_frames_mask = np.zeros(stop_frm_idx - start_frm_idx, dtype=bool)
 
     # Detect corners over cams
     for (i_frame, frame) in enumerate(islice(reader, start_frm_idx, stop_frm_idx, opts["frame_step"])):
         i_frame = i_frame * opts["frame_step"]
 
+        if opts.get("gamma_correction", None) is not None: # TODO: Generalize this
+            frame -= np.min(frame)
+            frame = frame.astype(np.float64)
+            frame /= np.max(frame)
+            frame = np.sqrt(frame)
+            frame = (frame*255).astype(np.uint8)
+
         if not init_frames_mask[i_frame]:
             continue
 
         # color management
         if not isinstance(opts['color_convert'], bool) and len(frame.shape) > 2:
             frame = cv2.cvtColor(frame, opts['color_convert'])  # noqa
 
         # corner detection
         corners, ids, rejected_img_points = \
             cv2.aruco.detectMarkers(frame,  # noqa
                                     cv2.aruco.getPredefinedDictionary(board_params['dictionary_type']),  # noqa
-                                    **finalize_aruco_detector_opts(opts['detection']['aruco_detect']))
+                                    **finalize_aruco_detector_opts(opts['detection_opts']['aruco_detect']))
 
         if len(corners) == 0:
             continue
 
         # corner refinement
         corners_ref, ids_ref = \
             cv2.aruco.refineDetectedMarkers(frame,  # noqa
                                             board.make_board(board_params),
                                             corners,
                                             ids,
                                             rejected_img_points,
-                                            **finalize_aruco_detector_opts(opts['detection']['aruco_refine']))[0:2]
+                                            **finalize_aruco_detector_opts(opts['detection_opts']['aruco_refine']))[0:2]
 
         # corner interpolation
         retval, charuco_corners, charuco_ids = \
             cv2.aruco.interpolateCornersCharuco(corners_ref,  # noqa
                                                 ids_ref,
                                                 frame,
                                                 board.make_board(board_params),
-                                                **opts['detection']['aruco_interpolate'])
+                                                **opts['detection_opts']['aruco_interpolate'])
         if charuco_corners is None:
             continue
 
+        if opts['RC_reject_corners']:
+            # Reject corners based on radial contrast value
+            RC_frame = RC_reader.read(i_frame + start_frm_idx)
+            corners_frame = np.squeeze(charuco_corners).astype(int).T
+            RC_bool = RC_frame[tuple(corners_frame[::-1, np.newaxis])] > 0
+            charuco_ids = charuco_ids[RC_bool[0]]
+            charuco_corners = charuco_corners[RC_bool[0]]
+
         # check if the result is degenerated (all corners on a line)
-        if not helper.check_detections_nondegenerate(board_params['boardWidth'], charuco_ids):
+        if not helper.check_detections_nondegenerate(board_params['boardWidth'], charuco_ids,
+                                                     opts['detection_opts']['min_corners']):
             continue
 
         # add offset
-        # We take offset into consideration at corner detection level. This means that the calibration parameters always
-        # refer to the offset-free pixel positions and offsets do NOT have to be taken into account anywhere in
-        # this calibration procedure or when working with the 
-        offset_x, offset_y = camfunctions.get_header_from_reader(reader)['offset']
         charuco_corners[:, :, 0] = charuco_corners[:, :, 0] + offset_x
         charuco_corners[:, :, 1] = charuco_corners[:, :, 1] + offset_y
 
         # check against last used frame
         # TODO check functionality of this code and determine actual value for maxdist
         #  Also, this bears the danger that different cams get detections in different frames and pose estimation
         #  becomes impossible. If this is ever required, it has to be made sure that cameras get detections on the same
         #  frames, e.g. by determining sufficient movement only on the first cam.
         #  Alternatively, in videos with a too high framerate, we could just use a frameskip.
         used_frame_ids = np.where(fin_frames_mask)[0]
         if len(used_frame_ids) > 0:
             ids_common = np.intersect1d(ids_cam[-1], charuco_ids)
 
-            if helper.check_detections_nondegenerate(board_params['boardWidth'], ids_common):
+            if helper.check_detections_nondegenerate(board_params['boardWidth'], ids_common,
+                                                     opts['detection_opts']['min_corners']):
                 prev_mask = np.isin(ids_cam[-1], ids_common)
                 curr_mask = np.isin(charuco_ids, ids_common)
 
                 diff = corners_cam[-1][prev_mask] - charuco_corners[curr_mask]
                 dist = np.sqrt(np.sum(diff ** 2, 1))
 
-                if np.max(dist) < opts['detection']['inter_frame_dist']:
+                if np.max(dist) < opts['detection_opts']['inter_frame_dist']:
                     continue
 
         fin_frames_mask[i_frame] = True
         corners_cam.append(charuco_corners)
         ids_cam.append(charuco_ids)
 
+    reader.close()
+
     return corners_cam, ids_cam, fin_frames_mask
```

### Comparing `bbo-calibcam-2.3.1/calibcam/helper_ag.py` & `bbo-calibcam-2.4.1/calibcam/helper_ag.py`

 * *Files identical despite different names*

### Comparing `bbo-calibcam-2.3.1/calibcam/opt_jacfwd/optfunctions.py` & `bbo-calibcam-2.4.1/calibcam/opt_jacfwd/optfunctions.py`

 * *Files identical despite different names*

### Comparing `bbo-calibcam-2.3.1/calibcam/opt_jacfwd/optfunctions_ag.py` & `bbo-calibcam-2.4.1/calibcam/opt_jacfwd/optfunctions_ag.py`

 * *Files identical despite different names*

### Comparing `bbo-calibcam-2.3.1/calibcam/optimization.py` & `bbo-calibcam-2.4.1/calibcam/optimization.py`

 * *Files identical despite different names*

### Comparing `bbo-calibcam-2.3.1/calibcam/pose_estimation.py` & `bbo-calibcam-2.4.1/calibcam/pose_estimation.py`

 * *Files identical despite different names*

### Comparing `bbo-calibcam-2.3.1/calibcam/single_camcalibration.py` & `bbo-calibcam-2.4.1/calibcam/single_camcalibration.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,19 @@
         return {}
 
     corners_nn = corners_cam[mask]
     corners_use, ids_use = helper.corners_array_to_ragged(corners_nn)
 
     if calib_init is not None:
         A = calib_init['A']
-        xi = calib_init['xi'].reshape(1, -1)
         k = calib_init['k']
+        if "xi" in calib_init:
+            xi = calib_init['xi'].reshape(1, -1)
+        else:
+            xi=0
     else:
         A = None
         xi = None
         k = None
 
     if opts['free_vars']['xi']:
         # Omnidir camera model
```

### Comparing `bbo-calibcam-2.3.1/setup.py` & `bbo-calibcam-2.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 README = (HERE / "README.md").read_text()
 
 packages=find_packages()
 print(packages)
 # This call to setup() does all the work
 setup(
     name="bbo-calibcam",
-    version="2.3.1",
+    version="2.4.1",
     description="Calibrate intrinsic and extrinsic parameters of cameras with charuco boards",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/bbo-lab/calibcam",
     author="BBO-lab @ caesar",
     author_email="kay-michael.voit@mpinb.mpg.de",
     license="BSD",
```

