# Comparing `tmp/buffalo_gym-0.0.2.tar.gz` & `tmp/buffalo_gym-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buffalo_gym-0.0.2.tar", last modified: Sun Apr 14 21:17:09 2024, max compression
+gzip compressed data, was "buffalo_gym-0.0.3.tar", last modified: Fri Apr 26 02:48:05 2024, max compression
```

## Comparing `buffalo_gym-0.0.2.tar` & `buffalo_gym-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:17:09.959032 buffalo_gym-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-14 21:17:09.955032 buffalo_gym-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-04-14 21:17:06.000000 buffalo_gym-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:17:09.955032 buffalo_gym-0.0.2/buffalo_gym/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-14 21:17:06.000000 buffalo_gym-0.0.2/buffalo_gym/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:17:09.955032 buffalo_gym-0.0.2/buffalo_gym/envs/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-14 21:17:06.000000 buffalo_gym-0.0.2/buffalo_gym/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-14 21:17:06.000000 buffalo_gym-0.0.2/buffalo_gym/envs/buffalo_gym.py
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-14 21:17:06.000000 buffalo_gym-0.0.2/buffalo_gym/envs/multibuffalo_gym.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:17:09.955032 buffalo_gym-0.0.2/buffalo_gym.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-14 21:17:09.000000 buffalo_gym-0.0.2/buffalo_gym.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-14 21:17:09.000000 buffalo_gym-0.0.2/buffalo_gym.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 21:17:09.000000 buffalo_gym-0.0.2/buffalo_gym.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-14 21:17:09.000000 buffalo_gym-0.0.2/buffalo_gym.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-14 21:17:09.000000 buffalo_gym-0.0.2/buffalo_gym.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 21:17:09.959032 buffalo_gym-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-14 21:17:06.000000 buffalo_gym-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:17:09.955032 buffalo_gym-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-14 21:17:06.000000 buffalo_gym-0.0.2/tests/test_buffalo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-14 21:17:06.000000 buffalo_gym-0.0.2/tests/test_multibuffalo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:48:05.267831 buffalo_gym-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-04-26 02:48:05.267831 buffalo_gym-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-04-26 02:48:01.000000 buffalo_gym-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:48:05.267831 buffalo_gym-0.0.3/buffalo_gym/
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-26 02:48:01.000000 buffalo_gym-0.0.3/buffalo_gym/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:48:05.267831 buffalo_gym-0.0.3/buffalo_gym/envs/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-26 02:48:01.000000 buffalo_gym-0.0.3/buffalo_gym/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-26 02:48:01.000000 buffalo_gym-0.0.3/buffalo_gym/envs/buffalo_gym.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-26 02:48:01.000000 buffalo_gym-0.0.3/buffalo_gym/envs/buffalotrail_gym.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-26 02:48:01.000000 buffalo_gym-0.0.3/buffalo_gym/envs/multibuffalo_gym.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:48:05.267831 buffalo_gym-0.0.3/buffalo_gym.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-04-26 02:48:05.000000 buffalo_gym-0.0.3/buffalo_gym.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-26 02:48:05.000000 buffalo_gym-0.0.3/buffalo_gym.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 02:48:05.000000 buffalo_gym-0.0.3/buffalo_gym.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-26 02:48:05.000000 buffalo_gym-0.0.3/buffalo_gym.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-26 02:48:05.000000 buffalo_gym-0.0.3/buffalo_gym.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-26 02:48:01.000000 buffalo_gym-0.0.3/license.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 02:48:05.267831 buffalo_gym-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-26 02:48:01.000000 buffalo_gym-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:48:05.267831 buffalo_gym-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-26 02:48:01.000000 buffalo_gym-0.0.3/tests/test_buffalo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-26 02:48:01.000000 buffalo_gym-0.0.3/tests/test_buffalotrail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-26 02:48:01.000000 buffalo_gym-0.0.3/tests/test_multibuffalo.py
```

### Comparing `buffalo_gym-0.0.2/PKG-INFO` & `buffalo_gym-0.0.3/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: buffalo_gym
-Version: 0.0.2
-Summary: Buffalo Gym environment
-Author: foreverska
-Project-URL: Github:, https://github.com/foreverska/buffalo-gym
-Keywords: gymnasium,gym
-Description-Content-Type: text/markdown
-Requires-Dist: gymnasium>=0.26.0
-Requires-Dist: numpy
-
 # Buffalo Gym
 
 A multi-armed bandit (MAB) environment for the gymnasium API.
 One-armed Bandit is a reference to slot machines, and Buffalo 
 is a reference to one such slot machine that I am fond 
 of.  MABs are an excellent playground for theoretical exercise and 
 debugging of RL agents as they provide an environment that 
@@ -41,17 +30,28 @@
 
 This module had an extra parameter, pace.  By default (None), a 
 new state is chosen for every step of the environment.  It can 
 be set to any integer to determine how many steps between randomly 
 choosing a new state.  Of course, transitioning to a new state is 
 not guaranteed as the next state is random.
 
+## Buffalo Trail ("BuffaloTrail-v0")
+
+There is a pervasive rumor that slot machine manufacturers put in 
+a secret sequence of bets which trigger a large reward or the 
+jackpot.  It is almost certainly not true in the real world but 
+it is here.  A sequence of actions gives the max reward.  The 
+sequence is randomly chosen on environment setup and indicated 
+in the info of reset.  Not all sequences are aliased and this 
+may be an important thing to check in an implementation.  Therefore, 
+there is a rudimentary algorithm to force aliasing included.
+
 ## Using
 
 Install via pip and import buffalo_gym along with gymnasium.
 
 ```
 import gymnasium  
 import buffalo_gym
 
 env = gym.make("Buffalo-v0")
-```
+```
```

### Comparing `buffalo_gym-0.0.2/buffalo_gym/envs/buffalo_gym.py` & `buffalo_gym-0.0.3/buffalo_gym/envs/buffalo_gym.py`

 * *Files identical despite different names*

### Comparing `buffalo_gym-0.0.2/buffalo_gym/envs/multibuffalo_gym.py` & `buffalo_gym-0.0.3/buffalo_gym/envs/multibuffalo_gym.py`

 * *Files identical despite different names*

### Comparing `buffalo_gym-0.0.2/buffalo_gym.egg-info/PKG-INFO` & `buffalo_gym-0.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: buffalo_gym
-Version: 0.0.2
+Version: 0.0.3
 Summary: Buffalo Gym environment
 Author: foreverska
 Project-URL: Github:, https://github.com/foreverska/buffalo-gym
 Keywords: gymnasium,gym
 Description-Content-Type: text/markdown
+License-File: license.txt
 Requires-Dist: gymnasium>=0.26.0
 Requires-Dist: numpy
 
 # Buffalo Gym
 
 A multi-armed bandit (MAB) environment for the gymnasium API.
 One-armed Bandit is a reference to slot machines, and Buffalo 
@@ -41,14 +42,25 @@
 
 This module had an extra parameter, pace.  By default (None), a 
 new state is chosen for every step of the environment.  It can 
 be set to any integer to determine how many steps between randomly 
 choosing a new state.  Of course, transitioning to a new state is 
 not guaranteed as the next state is random.
 
+## Buffalo Trail ("BuffaloTrail-v0")
+
+There is a pervasive rumor that slot machine manufacturers put in 
+a secret sequence of bets which trigger a large reward or the 
+jackpot.  It is almost certainly not true in the real world but 
+it is here.  A sequence of actions gives the max reward.  The 
+sequence is randomly chosen on environment setup and indicated 
+in the info of reset.  Not all sequences are aliased and this 
+may be an important thing to check in an implementation.  Therefore, 
+there is a rudimentary algorithm to force aliasing included.
+
 ## Using
 
 Install via pip and import buffalo_gym along with gymnasium.
 
 ```
 import gymnasium  
 import buffalo_gym
```

### Comparing `buffalo_gym-0.0.2/tests/test_multibuffalo.py` & `buffalo_gym-0.0.3/tests/test_multibuffalo.py`

 * *Files identical despite different names*

