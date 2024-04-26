# Comparing `tmp/bestdori-api-1.0.0.tar.gz` & `tmp/bestdori-api-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bestdori-api-1.0.0.tar", last modified: Thu Apr 25 16:09:35 2024, max compression
+gzip compressed data, was "bestdori-api-1.0.1.tar", last modified: Fri Apr 26 15:09:35 2024, max compression
```

## Comparing `bestdori-api-1.0.0.tar` & `bestdori-api-1.0.1.tar`

### file list

```diff
@@ -1,44 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:09:35.171573 bestdori-api-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-25 16:09:25.000000 bestdori-api-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5901 2024-04-25 16:09:35.171573 bestdori-api-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4356 2024-04-25 16:09:25.000000 bestdori-api-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:09:35.171573 bestdori-api-1.0.0/bestdori/
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-04-25 16:09:25.000000 bestdori-api-1.0.0/bestdori/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:09:35.171573 bestdori-api-1.0.0/bestdori/ayachan/
--rw-r--r--   0 runner    (1001) docker     (127)     7318 2024-04-25 16:09:25.000000 bestdori-api-1.0.0/bestdori/ayachan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-25 16:09:25.000000 bestdori-api-1.0.0/bestdori/ayachan/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:09:35.171573 bestdori-api-1.0.0/bestdori/ayachan/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-25 16:09:25.000000 bestdori-api-1.0.0/bestdori/ayachan/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12086 2024-04-25 16:09:25.000000 bestdori-api-1.0.0/bestdori/ayachan/utils/network.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-25 16:09:25.000000 bestdori-api-1.0.0/bestdori/ayachan/utils/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-25 16:09:25.000000 bestdori-api-1.0.0/bestdori/ayachan/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16496 2024-04-25 16:09:25.000000 bestdori-api-1.0.0/bestdori/cards.py
--rw-r--r--   0 runner    (1001) docker     (127)     8548 2024-04-25 16:09:25.000000 bestdori-api-1.0.0/bestdori/characters.py
--rw-r--r--   0 runner    (1001) docker     (127)    12046 2024-04-25 16:09:25.000000 bestdori-api-1.0.0/bestdori/charts.py
--rw-r--r--   0 runner    (1001) docker     (127)    12237 2024-04-25 16:09:25.000000 bestdori-api-1.0.0/bestdori/comics.py
--rw-r--r--   0 runner    (1001) docker     (127)    12181 2024-04-25 16:09:25.000000 bestdori-api-1.0.0/bestdori/costumes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6745 2024-04-25 16:09:25.000000 bestdori-api-1.0.0/bestdori/eventarchives.py
--rw-r--r--   0 runner    (1001) docker     (127)    20223 2024-04-25 16:09:25.000000 bestdori-api-1.0.0/bestdori/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     9306 2024-04-25 16:09:25.000000 bestdori-api-1.0.0/bestdori/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    12807 2024-04-25 16:09:25.000000 bestdori-api-1.0.0/bestdori/gacha.py
--rw-r--r--   0 runner    (1001) docker     (127)     9606 2024-04-25 16:09:25.000000 bestdori-api-1.0.0/bestdori/logincampaigns.py
--rw-r--r--   0 runner    (1001) docker     (127)     5817 2024-04-25 16:09:25.000000 bestdori-api-1.0.0/bestdori/miracleticket.py
--rw-r--r--   0 runner    (1001) docker     (127)     6545 2024-04-25 16:09:25.000000 bestdori-api-1.0.0/bestdori/missions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-25 16:09:25.000000 bestdori-api-1.0.0/bestdori/player.py
--rw-r--r--   0 runner    (1001) docker     (127)    34492 2024-04-25 16:09:25.000000 bestdori-api-1.0.0/bestdori/post.py
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-25 16:09:25.000000 bestdori-api-1.0.0/bestdori/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-25 16:09:25.000000 bestdori-api-1.0.0/bestdori/songmeta.py
--rw-r--r--   0 runner    (1001) docker     (127)    11219 2024-04-25 16:09:25.000000 bestdori-api-1.0.0/bestdori/songs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-04-25 16:09:25.000000 bestdori-api-1.0.0/bestdori/upload.py
--rw-r--r--   0 runner    (1001) docker     (127)    13044 2024-04-25 16:09:25.000000 bestdori-api-1.0.0/bestdori/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:09:35.171573 bestdori-api-1.0.0/bestdori/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     8249 2024-04-25 16:09:25.000000 bestdori-api-1.0.0/bestdori/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22048 2024-04-25 16:09:25.000000 bestdori-api-1.0.0/bestdori/utils/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     4116 2024-04-25 16:09:25.000000 bestdori-api-1.0.0/bestdori/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:09:35.171573 bestdori-api-1.0.0/bestdori_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5901 2024-04-25 16:09:34.000000 bestdori-api-1.0.0/bestdori_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-25 16:09:35.000000 bestdori-api-1.0.0/bestdori_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 16:09:34.000000 bestdori-api-1.0.0/bestdori_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-25 16:09:34.000000 bestdori-api-1.0.0/bestdori_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 16:09:35.171573 bestdori-api-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-25 16:09:25.000000 bestdori-api-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:09:35.922131 bestdori-api-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-26 15:09:28.000000 bestdori-api-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5901 2024-04-26 15:09:35.922131 bestdori-api-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4356 2024-04-26 15:09:28.000000 bestdori-api-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:09:35.918131 bestdori-api-1.0.1/bestdori/
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-04-26 15:09:28.000000 bestdori-api-1.0.1/bestdori/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:09:35.918131 bestdori-api-1.0.1/bestdori/ayachan/
+-rw-r--r--   0 runner    (1001) docker     (127)     7318 2024-04-26 15:09:28.000000 bestdori-api-1.0.1/bestdori/ayachan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-26 15:09:28.000000 bestdori-api-1.0.1/bestdori/ayachan/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:09:35.918131 bestdori-api-1.0.1/bestdori/ayachan/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-26 15:09:28.000000 bestdori-api-1.0.1/bestdori/ayachan/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12086 2024-04-26 15:09:28.000000 bestdori-api-1.0.1/bestdori/ayachan/utils/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-26 15:09:28.000000 bestdori-api-1.0.1/bestdori/ayachan/utils/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-26 15:09:28.000000 bestdori-api-1.0.1/bestdori/ayachan/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16496 2024-04-26 15:09:28.000000 bestdori-api-1.0.1/bestdori/cards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8548 2024-04-26 15:09:28.000000 bestdori-api-1.0.1/bestdori/characters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12046 2024-04-26 15:09:28.000000 bestdori-api-1.0.1/bestdori/charts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12237 2024-04-26 15:09:28.000000 bestdori-api-1.0.1/bestdori/comics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12181 2024-04-26 15:09:28.000000 bestdori-api-1.0.1/bestdori/costumes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6745 2024-04-26 15:09:28.000000 bestdori-api-1.0.1/bestdori/eventarchives.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20223 2024-04-26 15:09:28.000000 bestdori-api-1.0.1/bestdori/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9306 2024-04-26 15:09:28.000000 bestdori-api-1.0.1/bestdori/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12807 2024-04-26 15:09:28.000000 bestdori-api-1.0.1/bestdori/gacha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9606 2024-04-26 15:09:28.000000 bestdori-api-1.0.1/bestdori/logincampaigns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5817 2024-04-26 15:09:28.000000 bestdori-api-1.0.1/bestdori/miracleticket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6545 2024-04-26 15:09:28.000000 bestdori-api-1.0.1/bestdori/missions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:09:35.918131 bestdori-api-1.0.1/bestdori/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-26 15:09:28.000000 bestdori-api-1.0.1/bestdori/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-04-26 15:09:28.000000 bestdori-api-1.0.1/bestdori/models/content.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5139 2024-04-26 15:09:28.000000 bestdori-api-1.0.1/bestdori/models/note.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-26 15:09:28.000000 bestdori-api-1.0.1/bestdori/player.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34492 2024-04-26 15:09:28.000000 bestdori-api-1.0.1/bestdori/post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-26 15:09:28.000000 bestdori-api-1.0.1/bestdori/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-26 15:09:28.000000 bestdori-api-1.0.1/bestdori/songmeta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11219 2024-04-26 15:09:28.000000 bestdori-api-1.0.1/bestdori/songs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-04-26 15:09:28.000000 bestdori-api-1.0.1/bestdori/upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13044 2024-04-26 15:09:28.000000 bestdori-api-1.0.1/bestdori/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:09:35.918131 bestdori-api-1.0.1/bestdori/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     8249 2024-04-26 15:09:28.000000 bestdori-api-1.0.1/bestdori/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22048 2024-04-26 15:09:28.000000 bestdori-api-1.0.1/bestdori/utils/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4116 2024-04-26 15:09:28.000000 bestdori-api-1.0.1/bestdori/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:09:35.922131 bestdori-api-1.0.1/bestdori_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5901 2024-04-26 15:09:35.000000 bestdori-api-1.0.1/bestdori_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-26 15:09:35.000000 bestdori-api-1.0.1/bestdori_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 15:09:35.000000 bestdori-api-1.0.1/bestdori_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-26 15:09:35.000000 bestdori-api-1.0.1/bestdori_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 15:09:35.922131 bestdori-api-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-26 15:09:28.000000 bestdori-api-1.0.1/setup.py
```

### Comparing `bestdori-api-1.0.0/LICENSE` & `bestdori-api-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.0.0/PKG-INFO` & `bestdori-api-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bestdori-api
-Version: 1.0.0
+Version: 1.0.1
 Summary: Bestdori 的各种 API 调用整合，另外附带部分功能
 Home-page: https://github.com/WindowsSov8forUs/bestdori-api
 Author: WindowsSov8
 Author-email: qwertyuiop2333@hotmail.com
 License: MIT
 Description: <div align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bestdori-api Version: 1.0.0 Summary: Bestdori
+Metadata-Version: 2.1 Name: bestdori-api Version: 1.0.1 Summary: Bestdori
 çåç§ API è°ç¨æ´åï¼å¦å¤éå¸¦é¨ååè½ Home-page: https://
 github.com/WindowsSov8forUs/bestdori-api Author: WindowsSov8 Author-email:
 qwertyuiop2333@hotmail.com License: MIT Description:
   ![bestdori-api logo](https://github.com/WindowsSov8forUs/bestdori-api/blob/
 main/logo.png) # Bestdori-api _â¨ [Bestdori](https://bestdori.com/) çåç§
          API è°ç¨æ´åï¼å¦å¤éå¸¦é¨ååè½ â¨_ **:warning:
         è¯¥é¡¹ç®ä»ç¶æ¥éæ´æ°ä¸ Debug ï¼ä½¿ç¨æ¶è¥éå° Bug
```

### Comparing `bestdori-api-1.0.0/README.md` & `bestdori-api-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.0.0/bestdori/__init__.py` & `bestdori-api-1.0.1/bestdori/__init__.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.0.0/bestdori/ayachan/__init__.py` & `bestdori-api-1.0.1/bestdori/ayachan/__init__.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.0.0/bestdori/ayachan/exceptions.py` & `bestdori-api-1.0.1/bestdori/ayachan/exceptions.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.0.0/bestdori/ayachan/utils/network.py` & `bestdori-api-1.0.1/bestdori/ayachan/utils/network.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.0.0/bestdori/ayachan/utils/utils.py` & `bestdori-api-1.0.1/bestdori/ayachan/utils/utils.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.0.0/bestdori/cards.py` & `bestdori-api-1.0.1/bestdori/cards.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.0.0/bestdori/characters.py` & `bestdori-api-1.0.1/bestdori/characters.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.0.0/bestdori/charts.py` & `bestdori-api-1.0.1/bestdori/charts.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.0.0/bestdori/comics.py` & `bestdori-api-1.0.1/bestdori/comics.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.0.0/bestdori/costumes.py` & `bestdori-api-1.0.1/bestdori/costumes.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.0.0/bestdori/eventarchives.py` & `bestdori-api-1.0.1/bestdori/eventarchives.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.0.0/bestdori/events.py` & `bestdori-api-1.0.1/bestdori/events.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.0.0/bestdori/exceptions.py` & `bestdori-api-1.0.1/bestdori/exceptions.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.0.0/bestdori/gacha.py` & `bestdori-api-1.0.1/bestdori/gacha.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.0.0/bestdori/logincampaigns.py` & `bestdori-api-1.0.1/bestdori/logincampaigns.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.0.0/bestdori/miracleticket.py` & `bestdori-api-1.0.1/bestdori/miracleticket.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.0.0/bestdori/missions.py` & `bestdori-api-1.0.1/bestdori/missions.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.0.0/bestdori/player.py` & `bestdori-api-1.0.1/bestdori/player.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.0.0/bestdori/post.py` & `bestdori-api-1.0.1/bestdori/post.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.0.0/bestdori/settings.py` & `bestdori-api-1.0.1/bestdori/settings.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.0.0/bestdori/songmeta.py` & `bestdori-api-1.0.1/bestdori/songmeta.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.0.0/bestdori/songs.py` & `bestdori-api-1.0.1/bestdori/songs.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.0.0/bestdori/upload.py` & `bestdori-api-1.0.1/bestdori/upload.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.0.0/bestdori/user.py` & `bestdori-api-1.0.1/bestdori/user.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.0.0/bestdori/utils/__init__.py` & `bestdori-api-1.0.1/bestdori/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.0.0/bestdori/utils/network.py` & `bestdori-api-1.0.1/bestdori/utils/network.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.0.0/bestdori/utils/utils.py` & `bestdori-api-1.0.1/bestdori/utils/utils.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.0.0/bestdori_api.egg-info/PKG-INFO` & `bestdori-api-1.0.1/bestdori_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bestdori-api
-Version: 1.0.0
+Version: 1.0.1
 Summary: Bestdori 的各种 API 调用整合，另外附带部分功能
 Home-page: https://github.com/WindowsSov8forUs/bestdori-api
 Author: WindowsSov8
 Author-email: qwertyuiop2333@hotmail.com
 License: MIT
 Description: <div align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bestdori-api Version: 1.0.0 Summary: Bestdori
+Metadata-Version: 2.1 Name: bestdori-api Version: 1.0.1 Summary: Bestdori
 çåç§ API è°ç¨æ´åï¼å¦å¤éå¸¦é¨ååè½ Home-page: https://
 github.com/WindowsSov8forUs/bestdori-api Author: WindowsSov8 Author-email:
 qwertyuiop2333@hotmail.com License: MIT Description:
   ![bestdori-api logo](https://github.com/WindowsSov8forUs/bestdori-api/blob/
 main/logo.png) # Bestdori-api _â¨ [Bestdori](https://bestdori.com/) çåç§
          API è°ç¨æ´åï¼å¦å¤éå¸¦é¨ååè½ â¨_ **:warning:
         è¯¥é¡¹ç®ä»ç¶æ¥éæ´æ°ä¸ Debug ï¼ä½¿ç¨æ¶è¥éå° Bug
```

### Comparing `bestdori-api-1.0.0/bestdori_api.egg-info/SOURCES.txt` & `bestdori-api-1.0.1/bestdori_api.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -23,14 +23,17 @@
 bestdori/user.py
 bestdori/ayachan/__init__.py
 bestdori/ayachan/exceptions.py
 bestdori/ayachan/utils/__init__.py
 bestdori/ayachan/utils/network.py
 bestdori/ayachan/utils/settings.py
 bestdori/ayachan/utils/utils.py
+bestdori/models/__init__.py
+bestdori/models/content.py
+bestdori/models/note.py
 bestdori/utils/__init__.py
 bestdori/utils/network.py
 bestdori/utils/utils.py
 bestdori_api.egg-info/PKG-INFO
 bestdori_api.egg-info/SOURCES.txt
 bestdori_api.egg-info/dependency_links.txt
 bestdori_api.egg-info/top_level.txt
```

### Comparing `bestdori-api-1.0.0/setup.py` & `bestdori-api-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r') as readme:
     long_description = readme.read()
 
 setup(
     name='bestdori-api',
-    version='1.0.0',
+    version='1.0.1',
     author='WindowsSov8',
     author_email='qwertyuiop2333@hotmail.com',
     description='Bestdori 的各种 API 调用整合，另外附带部分功能',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/WindowsSov8forUs/bestdori-api',
     include_package_data=False,
```

