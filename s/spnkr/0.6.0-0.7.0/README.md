# Comparing `tmp/spnkr-0.6.0.tar.gz` & `tmp/spnkr-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spnkr-0.6.0.tar", last modified: Fri Feb 23 19:14:45 2024, max compression
+gzip compressed data, was "spnkr-0.7.0.tar", last modified: Fri Apr 26 03:20:46 2024, max compression
```

## Comparing `spnkr-0.6.0.tar` & `spnkr-0.7.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2024-02-23 19:14:45.697992 spnkr-0.6.0/
--rw-rw-rw-   0        0        0     1056 2023-08-17 20:38:12.000000 spnkr-0.6.0/LICENSE
--rw-rw-rw-   0        0        0     3684 2024-02-23 19:14:45.695993 spnkr-0.6.0/PKG-INFO
--rw-rw-rw-   0        0        0     1541 2023-12-07 02:48:08.000000 spnkr-0.6.0/README.md
--rw-rw-rw-   0        0        0     1019 2024-02-23 19:07:57.000000 spnkr-0.6.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-23 19:14:45.697992 spnkr-0.6.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-02-23 19:14:45.433121 spnkr-0.6.0/spnkr/
--rw-rw-rw-   0        0        0       64 2023-08-24 18:33:58.000000 spnkr-0.6.0/spnkr/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-23 19:14:45.529045 spnkr-0.6.0/spnkr/auth/
--rw-rw-rw-   0        0        0      389 2023-08-24 18:33:58.000000 spnkr-0.6.0/spnkr/auth/__init__.py
--rw-rw-rw-   0        0        0      714 2023-08-24 18:33:58.000000 spnkr-0.6.0/spnkr/auth/app.py
--rw-rw-rw-   0        0        0     2771 2023-08-24 18:33:58.000000 spnkr-0.6.0/spnkr/auth/core.py
--rw-rw-rw-   0        0        0     2772 2023-12-01 18:09:06.000000 spnkr-0.6.0/spnkr/auth/halo.py
--rw-rw-rw-   0        0        0     3156 2023-08-24 18:33:58.000000 spnkr-0.6.0/spnkr/auth/oauth.py
--rw-rw-rw-   0        0        0     1051 2023-08-24 18:33:58.000000 spnkr-0.6.0/spnkr/auth/player.py
--rw-rw-rw-   0        0        0     3446 2023-08-24 18:33:58.000000 spnkr-0.6.0/spnkr/auth/xbox.py
--rw-rw-rw-   0        0        0     2637 2024-01-03 04:20:45.000000 spnkr-0.6.0/spnkr/client.py
--rw-rw-rw-   0        0        0      234 2023-12-01 03:28:26.000000 spnkr-0.6.0/spnkr/errors.py
-drwxrwxrwx   0        0        0        0 2024-02-23 19:14:45.620610 spnkr-0.6.0/spnkr/models/
--rw-rw-rw-   0        0        0       56 2023-12-07 02:48:08.000000 spnkr-0.6.0/spnkr/models/__init__.py
--rw-rw-rw-   0        0        0      908 2023-12-15 14:00:09.000000 spnkr-0.6.0/spnkr/models/base.py
--rw-rw-rw-   0        0        0    15383 2023-12-17 19:54:08.000000 spnkr-0.6.0/spnkr/models/discovery_ugc.py
--rw-rw-rw-   0        0        0     9696 2023-12-17 19:55:04.000000 spnkr-0.6.0/spnkr/models/gamecms_hacs.py
--rw-rw-rw-   0        0        0      711 2023-12-15 14:02:33.000000 spnkr-0.6.0/spnkr/models/profile.py
--rw-rw-rw-   0        0        0    10677 2024-02-23 18:26:17.000000 spnkr-0.6.0/spnkr/models/refdata.py
--rw-rw-rw-   0        0        0     5529 2024-02-23 18:26:14.000000 spnkr-0.6.0/spnkr/models/skill.py
--rw-rw-rw-   0        0        0    26305 2024-02-23 18:26:14.000000 spnkr-0.6.0/spnkr/models/stats.py
--rw-rw-rw-   0        0        0      932 2023-12-17 19:53:12.000000 spnkr-0.6.0/spnkr/models/types.py
-drwxrwxrwx   0        0        0        0 2024-02-23 19:14:45.691993 spnkr-0.6.0/spnkr/services/
--rw-rw-rw-   0        0        0      499 2023-12-04 03:29:58.000000 spnkr-0.6.0/spnkr/services/__init__.py
--rw-rw-rw-   0        0        0     2213 2024-01-03 04:20:45.000000 spnkr-0.6.0/spnkr/services/base.py
--rw-rw-rw-   0        0        0     7711 2023-12-27 20:34:37.000000 spnkr-0.6.0/spnkr/services/discovery_ugc.py
--rw-rw-rw-   0        0        0     2455 2023-12-21 01:58:28.000000 spnkr-0.6.0/spnkr/services/gamecms_hacs.py
--rw-rw-rw-   0        0        0     1944 2023-12-21 01:58:28.000000 spnkr-0.6.0/spnkr/services/profile.py
--rw-rw-rw-   0        0        0     3099 2023-12-21 19:48:37.000000 spnkr-0.6.0/spnkr/services/skill.py
--rw-rw-rw-   0        0        0     6856 2023-12-21 19:48:37.000000 spnkr-0.6.0/spnkr/services/stats.py
--rw-rw-rw-   0        0        0      942 2024-01-03 04:20:45.000000 spnkr-0.6.0/spnkr/session.py
--rw-rw-rw-   0        0        0     5335 2023-12-07 02:48:08.000000 spnkr-0.6.0/spnkr/tools.py
--rw-rw-rw-   0        0        0     2434 2023-12-01 03:28:26.000000 spnkr-0.6.0/spnkr/xuid.py
-drwxrwxrwx   0        0        0        0 2024-02-23 19:14:45.693994 spnkr-0.6.0/spnkr.egg-info/
--rw-rw-rw-   0        0        0     3684 2024-02-23 19:14:45.000000 spnkr-0.6.0/spnkr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      817 2024-02-23 19:14:45.000000 spnkr-0.6.0/spnkr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-23 19:14:45.000000 spnkr-0.6.0/spnkr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      179 2024-02-23 19:14:45.000000 spnkr-0.6.0/spnkr.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-02-23 19:14:45.000000 spnkr-0.6.0/spnkr.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-26 03:20:46.545469 spnkr-0.7.0/
+-rw-rw-rw-   0        0        0     1056 2023-08-17 20:38:12.000000 spnkr-0.7.0/LICENSE
+-rw-rw-rw-   0        0        0     3684 2024-04-26 03:20:46.544482 spnkr-0.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1541 2023-12-07 02:48:08.000000 spnkr-0.7.0/README.md
+-rw-rw-rw-   0        0        0     1023 2024-04-26 03:00:59.000000 spnkr-0.7.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-26 03:20:46.545469 spnkr-0.7.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-26 03:20:46.327065 spnkr-0.7.0/spnkr/
+-rw-rw-rw-   0        0        0       64 2023-08-24 18:33:58.000000 spnkr-0.7.0/spnkr/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 03:20:46.417865 spnkr-0.7.0/spnkr/auth/
+-rw-rw-rw-   0        0        0      389 2023-08-24 18:33:58.000000 spnkr-0.7.0/spnkr/auth/__init__.py
+-rw-rw-rw-   0        0        0      714 2023-08-24 18:33:58.000000 spnkr-0.7.0/spnkr/auth/app.py
+-rw-rw-rw-   0        0        0     2771 2023-08-24 18:33:58.000000 spnkr-0.7.0/spnkr/auth/core.py
+-rw-rw-rw-   0        0        0     2772 2023-12-01 18:09:06.000000 spnkr-0.7.0/spnkr/auth/halo.py
+-rw-rw-rw-   0        0        0     3279 2024-04-26 03:13:49.000000 spnkr-0.7.0/spnkr/auth/oauth.py
+-rw-rw-rw-   0        0        0     1051 2023-08-24 18:33:58.000000 spnkr-0.7.0/spnkr/auth/player.py
+-rw-rw-rw-   0        0        0     3446 2023-08-24 18:33:58.000000 spnkr-0.7.0/spnkr/auth/xbox.py
+-rw-rw-rw-   0        0        0     2637 2024-01-03 04:20:45.000000 spnkr-0.7.0/spnkr/client.py
+-rw-rw-rw-   0        0        0      450 2024-04-26 02:56:28.000000 spnkr-0.7.0/spnkr/errors.py
+drwxrwxrwx   0        0        0        0 2024-04-26 03:20:46.484225 spnkr-0.7.0/spnkr/models/
+-rw-rw-rw-   0        0        0       56 2023-12-07 02:48:08.000000 spnkr-0.7.0/spnkr/models/__init__.py
+-rw-rw-rw-   0        0        0      908 2023-12-15 14:00:09.000000 spnkr-0.7.0/spnkr/models/base.py
+-rw-rw-rw-   0        0        0    15383 2023-12-17 19:54:08.000000 spnkr-0.7.0/spnkr/models/discovery_ugc.py
+-rw-rw-rw-   0        0        0     9696 2023-12-17 19:55:04.000000 spnkr-0.7.0/spnkr/models/gamecms_hacs.py
+-rw-rw-rw-   0        0        0      711 2023-12-15 14:02:33.000000 spnkr-0.7.0/spnkr/models/profile.py
+-rw-rw-rw-   0        0        0    10730 2024-04-26 02:31:17.000000 spnkr-0.7.0/spnkr/models/refdata.py
+-rw-rw-rw-   0        0        0     5529 2024-02-23 18:26:14.000000 spnkr-0.7.0/spnkr/models/skill.py
+-rw-rw-rw-   0        0        0    26305 2024-02-23 18:26:14.000000 spnkr-0.7.0/spnkr/models/stats.py
+-rw-rw-rw-   0        0        0      932 2023-12-17 19:53:12.000000 spnkr-0.7.0/spnkr/models/types.py
+drwxrwxrwx   0        0        0        0 2024-04-26 03:20:46.540465 spnkr-0.7.0/spnkr/services/
+-rw-rw-rw-   0        0        0      499 2023-12-04 03:29:58.000000 spnkr-0.7.0/spnkr/services/__init__.py
+-rw-rw-rw-   0        0        0     2213 2024-01-03 04:20:45.000000 spnkr-0.7.0/spnkr/services/base.py
+-rw-rw-rw-   0        0        0     7711 2023-12-27 20:34:37.000000 spnkr-0.7.0/spnkr/services/discovery_ugc.py
+-rw-rw-rw-   0        0        0     2455 2023-12-21 01:58:28.000000 spnkr-0.7.0/spnkr/services/gamecms_hacs.py
+-rw-rw-rw-   0        0        0     1944 2023-12-21 01:58:28.000000 spnkr-0.7.0/spnkr/services/profile.py
+-rw-rw-rw-   0        0        0     3099 2023-12-21 19:48:37.000000 spnkr-0.7.0/spnkr/services/skill.py
+-rw-rw-rw-   0        0        0     6856 2023-12-21 19:48:37.000000 spnkr-0.7.0/spnkr/services/stats.py
+-rw-rw-rw-   0        0        0      942 2024-01-03 04:20:45.000000 spnkr-0.7.0/spnkr/session.py
+-rw-rw-rw-   0        0        0     5335 2023-12-07 02:48:08.000000 spnkr-0.7.0/spnkr/tools.py
+-rw-rw-rw-   0        0        0     2434 2023-12-01 03:28:26.000000 spnkr-0.7.0/spnkr/xuid.py
+drwxrwxrwx   0        0        0        0 2024-04-26 03:20:46.542463 spnkr-0.7.0/spnkr.egg-info/
+-rw-rw-rw-   0        0        0     3684 2024-04-26 03:20:46.000000 spnkr-0.7.0/spnkr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      817 2024-04-26 03:20:46.000000 spnkr-0.7.0/spnkr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 03:20:46.000000 spnkr-0.7.0/spnkr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      179 2024-04-26 03:20:46.000000 spnkr-0.7.0/spnkr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-26 03:20:46.000000 spnkr-0.7.0/spnkr.egg-info/top_level.txt
```

### Comparing `spnkr-0.6.0/LICENSE` & `spnkr-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spnkr-0.6.0/PKG-INFO` & `spnkr-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spnkr
-Version: 0.6.0
+Version: 0.7.0
 Summary: Python API for retrieving Halo Infinite multiplayer data.
 Author: Andy Curtis
 License: Copyright 2022 Andy Curtis
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `spnkr-0.6.0/README.md` & `spnkr-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `spnkr-0.6.0/pyproject.toml` & `spnkr-0.7.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ['setuptools>=61.0.0', 'wheel']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'spnkr'
-version = '0.6.0'
+version = '0.7.0'
 description = 'Python API for retrieving Halo Infinite multiplayer data.'
 readme = 'README.md'
-authors = [{name = 'Andy Curtis'}]
-license = {file = 'LICENSE'}
+authors = [{ name = 'Andy Curtis' }]
+license = { file = 'LICENSE' }
 classifiers = [
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python',
     'Programming Language :: Python :: 3',
 ]
 keywords = ['halo', 'infinite', 'api']
 dependencies = ['aiohttp>=3', 'aiolimiter>=1', 'pydantic>=2']
```

### Comparing `spnkr-0.6.0/spnkr/auth/app.py` & `spnkr-0.7.0/spnkr/auth/app.py`

 * *Files identical despite different names*

### Comparing `spnkr-0.6.0/spnkr/auth/core.py` & `spnkr-0.7.0/spnkr/auth/core.py`

 * *Files identical despite different names*

### Comparing `spnkr-0.6.0/spnkr/auth/halo.py` & `spnkr-0.7.0/spnkr/auth/halo.py`

 * *Files identical despite different names*

### Comparing `spnkr-0.6.0/spnkr/auth/oauth.py` & `spnkr-0.7.0/spnkr/auth/oauth.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 import urllib.parse
 from dataclasses import dataclass
 from typing import Any
 
 from aiohttp import ClientSession
 
-from .app import AzureApp
+from spnkr.auth.app import AzureApp
+from spnkr.errors import OAuth2Error
 
 DEFAULT_SCOPES = ["Xboxlive.signin", "Xboxlive.offline_access"]
 
 
 @dataclass(frozen=True)
 class OAuth2Token:
     """Response resulting from a request for an OAuth2 token.
@@ -105,8 +106,10 @@
     url = "https://login.live.com/oauth20_token.srf"
     request_data = {
         **data,
         "client_id": app.client_id,
         "client_secret": app.client_secret,
     }
     response = await session.post(url, data=request_data)
+    if not response.ok:
+        raise OAuth2Error(await response.json())
     return OAuth2Token(await response.json())
```

### Comparing `spnkr-0.6.0/spnkr/auth/player.py` & `spnkr-0.7.0/spnkr/auth/player.py`

 * *Files identical despite different names*

### Comparing `spnkr-0.6.0/spnkr/auth/xbox.py` & `spnkr-0.7.0/spnkr/auth/xbox.py`

 * *Files identical despite different names*

### Comparing `spnkr-0.6.0/spnkr/client.py` & `spnkr-0.7.0/spnkr/client.py`

 * *Files identical despite different names*

### Comparing `spnkr-0.6.0/spnkr/models/base.py` & `spnkr-0.7.0/spnkr/models/base.py`

 * *Files identical despite different names*

### Comparing `spnkr-0.6.0/spnkr/models/discovery_ugc.py` & `spnkr-0.7.0/spnkr/models/discovery_ugc.py`

 * *Files identical despite different names*

### Comparing `spnkr-0.6.0/spnkr/models/gamecms_hacs.py` & `spnkr-0.7.0/spnkr/models/gamecms_hacs.py`

 * *Files identical despite different names*

### Comparing `spnkr-0.6.0/spnkr/models/profile.py` & `spnkr-0.7.0/spnkr/models/profile.py`

 * *Files identical despite different names*

### Comparing `spnkr-0.6.0/spnkr/models/refdata.py` & `spnkr-0.7.0/spnkr/models/refdata.py`

 * *Files 1% similar despite different names*

```diff
@@ -327,14 +327,16 @@
     """Arena playlists. Typically 4v4."""
     BIG_TEAM_BATTLE = 3
     """Big team battle playlists. Typically 12v12."""
     PVE = 4
     """Player vs. bots playlists."""
     FEATURED = 5
     """Featured playlists. Rotates frequently."""
+    FIREFIGHT = 6
+    """Firefight PvE playlist"""
 
 
 class SkillResultCode(IntEnum):
     """Result codes for skill requests."""
 
     SUCCESS = 0
     """Skill request was successful."""
```

### Comparing `spnkr-0.6.0/spnkr/models/skill.py` & `spnkr-0.7.0/spnkr/models/skill.py`

 * *Files identical despite different names*

### Comparing `spnkr-0.6.0/spnkr/models/stats.py` & `spnkr-0.7.0/spnkr/models/stats.py`

 * *Files identical despite different names*

### Comparing `spnkr-0.6.0/spnkr/models/types.py` & `spnkr-0.7.0/spnkr/models/types.py`

 * *Files identical despite different names*

### Comparing `spnkr-0.6.0/spnkr/services/base.py` & `spnkr-0.7.0/spnkr/services/base.py`

 * *Files identical despite different names*

### Comparing `spnkr-0.6.0/spnkr/services/discovery_ugc.py` & `spnkr-0.7.0/spnkr/services/discovery_ugc.py`

 * *Files identical despite different names*

### Comparing `spnkr-0.6.0/spnkr/services/gamecms_hacs.py` & `spnkr-0.7.0/spnkr/services/gamecms_hacs.py`

 * *Files identical despite different names*

### Comparing `spnkr-0.6.0/spnkr/services/profile.py` & `spnkr-0.7.0/spnkr/services/profile.py`

 * *Files identical despite different names*

### Comparing `spnkr-0.6.0/spnkr/services/skill.py` & `spnkr-0.7.0/spnkr/services/skill.py`

 * *Files identical despite different names*

### Comparing `spnkr-0.6.0/spnkr/services/stats.py` & `spnkr-0.7.0/spnkr/services/stats.py`

 * *Files identical despite different names*

### Comparing `spnkr-0.6.0/spnkr/session.py` & `spnkr-0.7.0/spnkr/session.py`

 * *Files identical despite different names*

### Comparing `spnkr-0.6.0/spnkr/tools.py` & `spnkr-0.7.0/spnkr/tools.py`

 * *Files identical despite different names*

### Comparing `spnkr-0.6.0/spnkr/xuid.py` & `spnkr-0.7.0/spnkr/xuid.py`

 * *Files identical despite different names*

### Comparing `spnkr-0.6.0/spnkr.egg-info/PKG-INFO` & `spnkr-0.7.0/spnkr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spnkr
-Version: 0.6.0
+Version: 0.7.0
 Summary: Python API for retrieving Halo Infinite multiplayer data.
 Author: Andy Curtis
 License: Copyright 2022 Andy Curtis
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `spnkr-0.6.0/spnkr.egg-info/SOURCES.txt` & `spnkr-0.7.0/spnkr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

