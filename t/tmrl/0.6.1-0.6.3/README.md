# Comparing `tmp/tmrl-0.6.1.tar.gz` & `tmp/tmrl-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmrl-0.6.1.tar", last modified: Wed Jan 17 23:52:55 2024, max compression
+gzip compressed data, was "tmrl-0.6.3.tar", last modified: Fri Apr 26 07:50:12 2024, max compression
```

## Comparing `tmrl-0.6.1.tar` & `tmrl-0.6.3.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxrwxrwx   0        0        0        0 2024-01-17 23:52:55.539212 tmrl-0.6.1/
--rw-rw-rw-   0        0        0     1089 2024-01-17 23:49:09.000000 tmrl-0.6.1/LICENSE
--rw-rw-rw-   0        0        0       43 2024-01-17 23:49:09.000000 tmrl-0.6.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2052 2024-01-17 23:52:55.539212 tmrl-0.6.1/PKG-INFO
--rw-rw-rw-   0        0        0    31109 2024-01-17 23:49:09.000000 tmrl-0.6.1/README.md
-drwxrwxrwx   0        0        0        0 2024-01-17 23:52:55.036609 tmrl-0.6.1/readme/
--rw-rw-rw-   0        0        0     1067 2024-01-17 23:49:09.000000 tmrl-0.6.1/readme/pypi.md
--rw-rw-rw-   0        0        0       42 2024-01-17 23:52:55.539212 tmrl-0.6.1/setup.cfg
--rw-rw-rw-   0        0        0     6169 2024-01-17 23:49:09.000000 tmrl-0.6.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-01-17 23:52:55.192617 tmrl-0.6.1/tmrl/
--rw-rw-rw-   0        0        0     1502 2024-01-17 23:49:09.000000 tmrl-0.6.1/tmrl/__init__.py
--rw-rw-rw-   0        0        0     4092 2024-01-17 23:49:09.000000 tmrl-0.6.1/tmrl/__main__.py
--rw-rw-rw-   0        0        0     5386 2024-01-17 23:49:09.000000 tmrl-0.6.1/tmrl/actor.py
-drwxrwxrwx   0        0        0        0 2024-01-17 23:52:55.224179 tmrl-0.6.1/tmrl/config/
--rw-rw-rw-   0        0        0        0 2024-01-17 23:49:09.000000 tmrl-0.6.1/tmrl/config/__init__.py
--rw-rw-rw-   0        0        0     6003 2024-01-17 23:49:09.000000 tmrl-0.6.1/tmrl/config/config_constants.py
--rw-rw-rw-   0        0        0     8564 2024-01-17 23:49:09.000000 tmrl-0.6.1/tmrl/config/config_objects.py
-drwxrwxrwx   0        0        0        0 2024-01-17 23:52:55.333774 tmrl-0.6.1/tmrl/custom/
--rw-rw-rw-   0        0        0        0 2024-01-17 23:49:09.000000 tmrl-0.6.1/tmrl/custom/__init__.py
--rw-rw-rw-   0        0        0    18803 2024-01-17 23:49:09.000000 tmrl-0.6.1/tmrl/custom/custom_algorithms.py
--rw-rw-rw-   0        0        0     9431 2024-01-17 23:49:09.000000 tmrl-0.6.1/tmrl/custom/custom_checkpoints.py
--rw-rw-rw-   0        0        0    12796 2024-01-17 23:49:09.000000 tmrl-0.6.1/tmrl/custom/custom_gym_interfaces.py
--rw-rw-rw-   0        0        0    23958 2024-01-17 23:49:09.000000 tmrl-0.6.1/tmrl/custom/custom_memories.py
--rw-rw-rw-   0        0        0    29938 2024-01-17 23:49:09.000000 tmrl-0.6.1/tmrl/custom/custom_models.py
--rw-rw-rw-   0        0        0     1387 2024-01-17 23:49:09.000000 tmrl-0.6.1/tmrl/custom/custom_preprocessors.py
-drwxrwxrwx   0        0        0        0 2024-01-17 23:52:55.476377 tmrl-0.6.1/tmrl/custom/utils/
--rw-rw-rw-   0        0        0        0 2024-01-17 23:49:09.000000 tmrl-0.6.1/tmrl/custom/utils/__init__.py
--rw-rw-rw-   0        0        0     5463 2024-01-17 23:49:09.000000 tmrl-0.6.1/tmrl/custom/utils/compute_reward.py
--rw-rw-rw-   0        0        0     2248 2024-01-17 23:49:09.000000 tmrl-0.6.1/tmrl/custom/utils/control_gamepad.py
--rw-rw-rw-   0        0        0     3981 2024-01-17 23:49:09.000000 tmrl-0.6.1/tmrl/custom/utils/control_keyboard.py
--rw-rw-rw-   0        0        0     1710 2024-01-17 23:49:09.000000 tmrl-0.6.1/tmrl/custom/utils/control_mouse.py
--rw-rw-rw-   0        0        0     9041 2024-01-17 23:49:09.000000 tmrl-0.6.1/tmrl/custom/utils/nn.py
--rw-rw-rw-   0        0        0     5019 2024-01-17 23:49:09.000000 tmrl-0.6.1/tmrl/custom/utils/tools.py
--rw-rw-rw-   0        0        0     9247 2024-01-17 23:49:09.000000 tmrl-0.6.1/tmrl/custom/utils/window.py
--rw-rw-rw-   0        0        0     1291 2024-01-17 23:49:09.000000 tmrl-0.6.1/tmrl/envs.py
--rw-rw-rw-   0        0        0     9555 2024-01-17 23:49:09.000000 tmrl-0.6.1/tmrl/memory.py
--rw-rw-rw-   0        0        0    41597 2024-01-17 23:49:09.000000 tmrl-0.6.1/tmrl/networking.py
-drwxrwxrwx   0        0        0        0 2024-01-17 23:52:55.510002 tmrl-0.6.1/tmrl/tools/
--rw-rw-rw-   0        0        0        0 2024-01-17 23:49:09.000000 tmrl-0.6.1/tmrl/tools/__init__.py
--rw-rw-rw-   0        0        0     2828 2024-01-17 23:49:09.000000 tmrl-0.6.1/tmrl/tools/check_environment.py
-drwxrwxrwx   0        0        0        0 2024-01-17 23:52:55.523548 tmrl-0.6.1/tmrl/tools/init_package/
--rw-rw-rw-   0        0        0        0 2024-01-17 23:49:09.000000 tmrl-0.6.1/tmrl/tools/init_package/__init__.py
--rw-rw-rw-   0        0        0    27288 2024-01-17 23:49:09.000000 tmrl-0.6.1/tmrl/tools/init_package/init_pywin32.py
--rw-rw-rw-   0        0        0     2867 2024-01-17 23:49:09.000000 tmrl-0.6.1/tmrl/tools/record.py
--rw-rw-rw-   0        0        0     1279 2024-01-17 23:49:09.000000 tmrl-0.6.1/tmrl/tools/save_replays.py
--rw-rw-rw-   0        0        0     1390 2024-01-17 23:49:09.000000 tmrl-0.6.1/tmrl/training.py
--rw-rw-rw-   0        0        0    10895 2024-01-17 23:49:09.000000 tmrl-0.6.1/tmrl/training_offline.py
--rw-rw-rw-   0        0        0    10255 2024-01-17 23:49:09.000000 tmrl-0.6.1/tmrl/util.py
--rw-rw-rw-   0        0        0     2031 2024-01-17 23:49:09.000000 tmrl-0.6.1/tmrl/wrappers.py
-drwxrwxrwx   0        0        0        0 2024-01-17 23:52:55.209168 tmrl-0.6.1/tmrl.egg-info/
--rw-rw-rw-   0        0        0     2052 2024-01-17 23:52:54.000000 tmrl-0.6.1/tmrl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1103 2024-01-17 23:52:54.000000 tmrl-0.6.1/tmrl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-17 23:52:54.000000 tmrl-0.6.1/tmrl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      159 2024-01-17 23:52:54.000000 tmrl-0.6.1/tmrl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-01-17 23:52:54.000000 tmrl-0.6.1/tmrl.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-26 07:50:12.138832 tmrl-0.6.3/
+-rw-rw-rw-   0        0        0     1089 2024-04-08 03:24:28.000000 tmrl-0.6.3/LICENSE
+-rw-rw-rw-   0        0        0       43 2024-04-08 03:28:54.000000 tmrl-0.6.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2052 2024-04-26 07:50:12.138832 tmrl-0.6.3/PKG-INFO
+-rw-rw-rw-   0        0        0    31154 2024-04-08 03:28:54.000000 tmrl-0.6.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-26 07:50:11.652002 tmrl-0.6.3/readme/
+-rw-rw-rw-   0        0        0     1067 2024-04-08 03:28:54.000000 tmrl-0.6.3/readme/pypi.md
+-rw-rw-rw-   0        0        0       42 2024-04-26 07:50:12.138832 tmrl-0.6.3/setup.cfg
+-rw-rw-rw-   0        0        0     6314 2024-04-26 07:47:33.000000 tmrl-0.6.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 07:50:11.761878 tmrl-0.6.3/tmrl/
+-rw-rw-rw-   0        0        0     1590 2024-04-23 05:21:02.000000 tmrl-0.6.3/tmrl/__init__.py
+-rw-rw-rw-   0        0        0     4262 2024-04-23 05:21:02.000000 tmrl-0.6.3/tmrl/__main__.py
+-rw-rw-rw-   0        0        0     5386 2024-04-08 03:24:28.000000 tmrl-0.6.3/tmrl/actor.py
+drwxrwxrwx   0        0        0        0 2024-04-26 07:50:11.812741 tmrl-0.6.3/tmrl/config/
+-rw-rw-rw-   0        0        0        0 2024-04-08 03:24:28.000000 tmrl-0.6.3/tmrl/config/__init__.py
+-rw-rw-rw-   0        0        0     6165 2024-04-23 05:21:02.000000 tmrl-0.6.3/tmrl/config/config_constants.py
+-rw-rw-rw-   0        0        0     8564 2024-04-08 03:28:54.000000 tmrl-0.6.3/tmrl/config/config_objects.py
+drwxrwxrwx   0        0        0        0 2024-04-26 07:50:11.918994 tmrl-0.6.3/tmrl/custom/
+-rw-rw-rw-   0        0        0        0 2024-04-08 03:24:28.000000 tmrl-0.6.3/tmrl/custom/__init__.py
+-rw-rw-rw-   0        0        0    18803 2024-04-08 03:28:54.000000 tmrl-0.6.3/tmrl/custom/custom_algorithms.py
+-rw-rw-rw-   0        0        0     9431 2024-04-08 03:28:54.000000 tmrl-0.6.3/tmrl/custom/custom_checkpoints.py
+-rw-rw-rw-   0        0        0    12796 2024-04-08 03:28:54.000000 tmrl-0.6.3/tmrl/custom/custom_gym_interfaces.py
+-rw-rw-rw-   0        0        0    23958 2024-04-08 03:28:54.000000 tmrl-0.6.3/tmrl/custom/custom_memories.py
+-rw-rw-rw-   0        0        0    29938 2024-04-08 03:28:54.000000 tmrl-0.6.3/tmrl/custom/custom_models.py
+-rw-rw-rw-   0        0        0     1387 2024-04-08 03:24:28.000000 tmrl-0.6.3/tmrl/custom/custom_preprocessors.py
+drwxrwxrwx   0        0        0        0 2024-04-26 07:50:12.075773 tmrl-0.6.3/tmrl/custom/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-08 03:24:28.000000 tmrl-0.6.3/tmrl/custom/utils/__init__.py
+-rw-rw-rw-   0        0        0     5463 2024-04-08 03:28:54.000000 tmrl-0.6.3/tmrl/custom/utils/compute_reward.py
+-rw-rw-rw-   0        0        0     2248 2024-04-08 03:24:28.000000 tmrl-0.6.3/tmrl/custom/utils/control_gamepad.py
+-rw-rw-rw-   0        0        0     3981 2024-04-08 03:24:28.000000 tmrl-0.6.3/tmrl/custom/utils/control_keyboard.py
+-rw-rw-rw-   0        0        0     1710 2024-04-08 03:24:28.000000 tmrl-0.6.3/tmrl/custom/utils/control_mouse.py
+-rw-rw-rw-   0        0        0     9041 2024-04-08 03:28:54.000000 tmrl-0.6.3/tmrl/custom/utils/nn.py
+-rw-rw-rw-   0        0        0     5019 2024-04-08 03:24:28.000000 tmrl-0.6.3/tmrl/custom/utils/tools.py
+-rw-rw-rw-   0        0        0     9247 2024-04-08 03:24:28.000000 tmrl-0.6.3/tmrl/custom/utils/window.py
+-rw-rw-rw-   0        0        0     1291 2024-04-08 03:28:54.000000 tmrl-0.6.3/tmrl/envs.py
+-rw-rw-rw-   0        0        0     9555 2024-04-08 03:28:54.000000 tmrl-0.6.3/tmrl/memory.py
+-rw-rw-rw-   0        0        0    41597 2024-04-08 03:28:54.000000 tmrl-0.6.3/tmrl/networking.py
+drwxrwxrwx   0        0        0        0 2024-04-26 07:50:12.091343 tmrl-0.6.3/tmrl/tools/
+-rw-rw-rw-   0        0        0        0 2024-04-08 03:24:28.000000 tmrl-0.6.3/tmrl/tools/__init__.py
+-rw-rw-rw-   0        0        0     2922 2024-04-26 07:47:33.000000 tmrl-0.6.3/tmrl/tools/check_environment.py
+drwxrwxrwx   0        0        0        0 2024-04-26 07:50:12.124322 tmrl-0.6.3/tmrl/tools/init_package/
+-rw-rw-rw-   0        0        0        0 2024-04-08 03:24:28.000000 tmrl-0.6.3/tmrl/tools/init_package/__init__.py
+-rw-rw-rw-   0        0        0    27288 2024-04-23 05:21:02.000000 tmrl-0.6.3/tmrl/tools/init_package/init_pywin32.py
+-rw-rw-rw-   0        0        0     4882 2024-04-23 05:21:02.000000 tmrl-0.6.3/tmrl/tools/init_package/init_tmrl.py
+-rw-rw-rw-   0        0        0     3238 2024-04-26 07:13:45.000000 tmrl-0.6.3/tmrl/tools/record.py
+-rw-rw-rw-   0        0        0     1279 2024-04-08 03:24:28.000000 tmrl-0.6.3/tmrl/tools/save_replays.py
+-rw-rw-rw-   0        0        0     1390 2024-04-08 03:24:28.000000 tmrl-0.6.3/tmrl/training.py
+-rw-rw-rw-   0        0        0    10895 2024-04-08 03:24:28.000000 tmrl-0.6.3/tmrl/training_offline.py
+-rw-rw-rw-   0        0        0    10255 2024-04-08 03:24:28.000000 tmrl-0.6.3/tmrl/util.py
+-rw-rw-rw-   0        0        0     2031 2024-04-08 03:24:28.000000 tmrl-0.6.3/tmrl/wrappers.py
+drwxrwxrwx   0        0        0        0 2024-04-26 07:50:11.793131 tmrl-0.6.3/tmrl.egg-info/
+-rw-rw-rw-   0        0        0     2052 2024-04-26 07:50:11.000000 tmrl-0.6.3/tmrl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1140 2024-04-26 07:50:11.000000 tmrl-0.6.3/tmrl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 07:50:11.000000 tmrl-0.6.3/tmrl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      159 2024-04-26 07:50:11.000000 tmrl-0.6.3/tmrl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-26 07:50:11.000000 tmrl-0.6.3/tmrl.egg-info/top_level.txt
```

### Comparing `tmrl-0.6.1/LICENSE` & `tmrl-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.1/PKG-INFO` & `tmrl-0.6.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tmrl
-Version: 0.6.1
+Version: 0.6.3
 Summary: Network-based framework for real-time robot learning
 Home-page: https://github.com/trackmania-rl/tmrl
-Download-URL: https://github.com/trackmania-rl/tmrl/archive/refs/tags/v0.6.1.tar.gz
+Download-URL: https://github.com/trackmania-rl/tmrl/archive/refs/tags/v0.6.3.tar.gz
 Author: Yann Bouteiller, Edouard Geze
 Author-email: yann.bouteiller@polymtl.ca, edouard.geze@hotmail.fr
 License: MIT
 Keywords: reinforcement learning,robot learning,trackmania,self driving,roborace
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `tmrl-0.6.1/README.md` & `tmrl-0.6.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -107,15 +107,15 @@
 In particular, [rtgym](https://github.com/yannbouteiller/rtgym) enables implementing Gymnasium environments in real-time applications,
 [vgamepad](https://github.com/yannbouteiller/vgamepad) enables emulating virtual game controllers,
 and [tlspyo](https://github.com/MISTLab/tls-python-object) enables transferring python object over the Internet in a secure fashion.
 
 ### TMRL in the media:
 - In the french show [Underscore_ (2022-06-08)](https://www.youtube.com/watch?v=c1xq7iJ3f9E), we used a vision-based (LIDAR) policy to play against the TrackMania world champions. Spoiler: our policy lost by far (expectedly :smile:); the superhuman target was set to about 32s on the `tmrl-test` track, while the trained policy had a mean performance of about 45.5s. The Gymnasium environment that we used for the show is available [here](#lidar-with-track-progress).
 
-- In 2023, we were invited at Ubisoft Montreal to talk about how video games could become simulators for vision-based autonomous driving in the future. Recording of the talk coming soon!
+- In 2023, we were [invited at Ubisoft Montreal](https://youtu.be/Nm71G0-wnFU?feature=shared&t=4317) to give a talk describing how video games could serve as visual simulators for vision-based autonomous driving in the near future.
 
 ## Installation
 
 Detailed instructions for installation are provided at [this link](readme/Install.md).
 
 ## Getting started
```

### Comparing `tmrl-0.6.1/readme/pypi.md` & `tmrl-0.6.3/readme/pypi.md`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.1/setup.py` & `tmrl-0.6.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 import urllib.error
 import socket
 
 if sys.version_info < (3, 7):
     sys.exit('Sorry, Python < 3.7 is not supported.')
 
 
+# NB: the following code is duplicated under tmrl.tools.init_package.init_tmrl,
+# don't forget to update both whenever changing RESOURCES_URL.
+
+
 RESOURCES_URL = "https://github.com/trackmania-rl/tmrl/releases/download/v0.6.0/resources.zip"
 
 
 def url_retrieve(url: str, outfile: Path, overwrite: bool = False):
     """
     Adapted from https://www.scivision.dev/python-switch-urlretrieve-requests-timeout/
     """
@@ -129,21 +133,21 @@
 HERE = os.path.abspath(os.path.dirname(__file__))
 README_FOLDER = os.path.join(HERE, "readme")
 with open(os.path.join(README_FOLDER, "pypi.md")) as fid:
     README = fid.read()
 
 setup(
     name='tmrl',
-    version='0.6.1',
+    version='0.6.3',
     description='Network-based framework for real-time robot learning',
     long_description=README,
     long_description_content_type='text/markdown',
     keywords='reinforcement learning, robot learning, trackmania, self driving, roborace',
     url='https://github.com/trackmania-rl/tmrl',
-    download_url='https://github.com/trackmania-rl/tmrl/archive/refs/tags/v0.6.1.tar.gz',
+    download_url='https://github.com/trackmania-rl/tmrl/archive/refs/tags/v0.6.3.tar.gz',
     author='Yann Bouteiller, Edouard Geze',
     author_email='yann.bouteiller@polymtl.ca, edouard.geze@hotmail.fr',
     license='MIT',
     install_requires=install_req,
     classifiers=[
             'Development Status :: 4 - Beta',
             'Intended Audience :: Developers',
```

### Comparing `tmrl-0.6.1/tmrl/__init__.py` & `tmrl-0.6.3/tmrl/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,16 @@
             import win32con
         except ImportError as e2:
             logging.error(f"tmrl could not fix pywin32 on your system. The following exceptions were raised:\
             \n=== Exception 1 ===\n{str(e1)}\n=== Exception 2 ===\n{str(e2)}\
             \nPlease install pywin32 manually.")
             raise RuntimeError("Please install pywin32 manually: https://github.com/mhammond/pywin32")
 
+# TMRL folder initialization:
+from tmrl.tools.init_package.init_tmrl import TMRL_FOLDER
 
 # do not remove this
 from dataclasses import dataclass
 
 from tmrl.envs import GenericGymEnv
 from tmrl.config.config_objects import CONFIG_DICT
```

### Comparing `tmrl-0.6.1/tmrl/__main__.py` & `tmrl-0.6.3/tmrl/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,20 +59,23 @@
     elif args.record_reward:
         record_reward_dist(path_reward=cfg.REWARD_PATH)
     elif args.check_env:
         if cfg.PRAGMA_LIDAR:
             check_env_tm20lidar()
         else:
             check_env_tm20full()
+    elif args.install:
+        logging.info(f"TMRL folder: {cfg.TMRL_FOLDER}")
     else:
         raise ArgumentTypeError('Enter a valid argument')
 
 
 if __name__ == "__main__":
     parser = ArgumentParser()
+    parser.add_argument('--install', action='store_true', help='checks TMRL installation')
     parser.add_argument('--server', action='store_true', help='launches the server')
     parser.add_argument('--trainer', action='store_true', help='launches the trainer')
     parser.add_argument('--worker', action='store_true', help='launches a rollout worker')
     parser.add_argument('--expert', action='store_true', help='launches an expert rollout worker (no model update)')
     parser.add_argument('--test', action='store_true', help='runs inference without training')
     parser.add_argument('--benchmark', action='store_true', help='runs a benchmark of the environment')
     parser.add_argument('--record-reward', dest='record_reward', action='store_true', help='utility to record a reward function in TM20')
```

### Comparing `tmrl-0.6.1/tmrl/actor.py` & `tmrl-0.6.3/tmrl/actor.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.1/tmrl/config/config_constants.py` & `tmrl-0.6.3/tmrl/config/config_constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 # standard library imports
+
+import logging
+
 import os
 from pathlib import Path
-import logging
 import json
 import platform
 from packaging import version
 
 
 __compatibility__ = "0.6.0"
 
+# TMRL FOLDER: =======================================================
+
 SYSTEM = platform.system()
 RTGYM_VERSION = "real-time-gym-v1" if SYSTEM == "Windows" else "real-time-gym-ts-v1"
 
 TMRL_FOLDER = Path.home() / "TmrlData"
+
+if not TMRL_FOLDER.exists():
+    raise RuntimeError(f"Missing folder: {TMRL_FOLDER}")
+
 CHECKPOINTS_FOLDER = TMRL_FOLDER / "checkpoints"
 DATASET_FOLDER = TMRL_FOLDER / "dataset"
 REWARD_FOLDER = TMRL_FOLDER / "reward"
 WEIGHTS_FOLDER = TMRL_FOLDER / "weights"
 CONFIG_FOLDER = TMRL_FOLDER / "config"
 
 CONFIG_FILE = TMRL_FOLDER / "config" / "config.json"
```

### Comparing `tmrl-0.6.1/tmrl/config/config_objects.py` & `tmrl-0.6.3/tmrl/config/config_objects.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.1/tmrl/custom/custom_algorithms.py` & `tmrl-0.6.3/tmrl/custom/custom_algorithms.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.1/tmrl/custom/custom_checkpoints.py` & `tmrl-0.6.3/tmrl/custom/custom_checkpoints.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.1/tmrl/custom/custom_gym_interfaces.py` & `tmrl-0.6.3/tmrl/custom/custom_gym_interfaces.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.1/tmrl/custom/custom_memories.py` & `tmrl-0.6.3/tmrl/custom/custom_memories.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.1/tmrl/custom/custom_models.py` & `tmrl-0.6.3/tmrl/custom/custom_models.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.1/tmrl/custom/custom_preprocessors.py` & `tmrl-0.6.3/tmrl/custom/custom_preprocessors.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.1/tmrl/custom/utils/compute_reward.py` & `tmrl-0.6.3/tmrl/custom/utils/compute_reward.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.1/tmrl/custom/utils/control_gamepad.py` & `tmrl-0.6.3/tmrl/custom/utils/control_gamepad.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.1/tmrl/custom/utils/control_keyboard.py` & `tmrl-0.6.3/tmrl/custom/utils/control_keyboard.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.1/tmrl/custom/utils/control_mouse.py` & `tmrl-0.6.3/tmrl/custom/utils/control_mouse.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.1/tmrl/custom/utils/nn.py` & `tmrl-0.6.3/tmrl/custom/utils/nn.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.1/tmrl/custom/utils/tools.py` & `tmrl-0.6.3/tmrl/custom/utils/tools.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.1/tmrl/custom/utils/window.py` & `tmrl-0.6.3/tmrl/custom/utils/window.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.1/tmrl/envs.py` & `tmrl-0.6.3/tmrl/envs.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.1/tmrl/memory.py` & `tmrl-0.6.3/tmrl/memory.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.1/tmrl/networking.py` & `tmrl-0.6.3/tmrl/networking.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.1/tmrl/tools/check_environment.py` & `tmrl-0.6.3/tmrl/tools/check_environment.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 from tmrl.custom.utils.tools import Lidar
 import tmrl.config.config_constants as cfg
 import logging
 
 
 def check_env_tm20lidar():
     window_interface = WindowInterface("Trackmania")
+    if cfg.SYSTEM != "Windows":
+        window_interface.move_and_resize()  # needed on Linux
     lidar = Lidar(window_interface.screenshot())
     env_config = DEFAULT_CONFIG_DICT.copy()
     env_config["interface"] = TM2020InterfaceLidar
     env_config["wait_on_done"] = True
     env_config["interface_kwargs"] = {"img_hist_len": 1, "gamepad": False}
     env = gymnasium.make(cfg.RTGYM_VERSION, config=env_config)
     o, i = env.reset()
```

### Comparing `tmrl-0.6.1/tmrl/tools/init_package/init_pywin32.py` & `tmrl-0.6.3/tmrl/tools/init_package/init_pywin32.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Adapted from https://github.com/mhammond/pywin32/blob/main/pywin32_postinstall.py
 
-# May have to be adapted in the future if becomming incompatible with new version of pywin32.
+# May have to be adapted in the future if becoming incompatible with new versions of pywin32.
 
 # postinstall script for pywin32
 #
 # copies PyWinTypesxx.dll and PythonCOMxx.dll into the system directory,
 # and creates a pth file
 import os
 import sys
```

### Comparing `tmrl-0.6.1/tmrl/tools/record.py` & `tmrl-0.6.3/tmrl/tools/record.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,52 @@
 # standard library imports
 import pickle
 import time
 
 # third-party imports
-import keyboard
 import numpy as np
 
 # local imports
 import tmrl.config.config_constants as cfg
 from tmrl.custom.utils.tools import TM2020OpenPlanetClient
 import logging
 
 
 PATH_REWARD = cfg.REWARD_PATH
 DATASET_PATH = cfg.DATASET_PATH
+SYSTEM = cfg.SYSTEM
+
+if SYSTEM == "Windows":
+    import keyboard
 
 
 def record_reward_dist(path_reward=PATH_REWARD):
     positions = []
     client = TM2020OpenPlanetClient()
     path = path_reward
 
     is_recording = False
     while True:
-        if keyboard.is_pressed('e'):
-            logging.info(f"start recording")
-            is_recording = True
+        if not is_recording:
+            if SYSTEM == "Windows":
+                if keyboard.is_pressed('e'):
+                    logging.info(f"start recording")
+                    is_recording = True
+            else:
+                logging.info(f"start recording")
+                is_recording = True
+
         if is_recording:
             data = client.retrieve_data(sleep_if_empty=0.01)  # we need many points to build a smooth curve
             terminated = bool(data[8])
-            if keyboard.is_pressed('q') or terminated:
+            if SYSTEM == "Windows":
+                early_stop = keyboard.is_pressed('q')
+            else:
+                early_stop = False
+            if early_stop or terminated:
                 logging.info(f"Computing reward function checkpoints from captured positions...")
                 logging.info(f"Initial number of captured positions: {len(positions)}")
                 positions = np.array(positions)
 
                 final_positions = [positions[0]]
                 dist_between_points = 0.1
                 j = 1
```

### Comparing `tmrl-0.6.1/tmrl/tools/save_replays.py` & `tmrl-0.6.3/tmrl/tools/save_replays.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.1/tmrl/training.py` & `tmrl-0.6.3/tmrl/training.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.1/tmrl/training_offline.py` & `tmrl-0.6.3/tmrl/training_offline.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.1/tmrl/util.py` & `tmrl-0.6.3/tmrl/util.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.1/tmrl/wrappers.py` & `tmrl-0.6.3/tmrl/wrappers.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.1/tmrl.egg-info/PKG-INFO` & `tmrl-0.6.3/tmrl.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tmrl
-Version: 0.6.1
+Version: 0.6.3
 Summary: Network-based framework for real-time robot learning
 Home-page: https://github.com/trackmania-rl/tmrl
-Download-URL: https://github.com/trackmania-rl/tmrl/archive/refs/tags/v0.6.1.tar.gz
+Download-URL: https://github.com/trackmania-rl/tmrl/archive/refs/tags/v0.6.3.tar.gz
 Author: Yann Bouteiller, Edouard Geze
 Author-email: yann.bouteiller@polymtl.ca, edouard.geze@hotmail.fr
 License: MIT
 Keywords: reinforcement learning,robot learning,trackmania,self driving,roborace
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `tmrl-0.6.1/tmrl.egg-info/SOURCES.txt` & `tmrl-0.6.3/tmrl.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -37,8 +37,9 @@
 tmrl/custom/utils/tools.py
 tmrl/custom/utils/window.py
 tmrl/tools/__init__.py
 tmrl/tools/check_environment.py
 tmrl/tools/record.py
 tmrl/tools/save_replays.py
 tmrl/tools/init_package/__init__.py
-tmrl/tools/init_package/init_pywin32.py
+tmrl/tools/init_package/init_pywin32.py
+tmrl/tools/init_package/init_tmrl.py
```

