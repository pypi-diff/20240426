# Comparing `tmp/nhl_api_py-2.5.1.tar.gz` & `tmp/nhl_api_py-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nhl_api_py-2.5.1.tar", max compression
+gzip compressed data, was "nhl_api_py-2.6.0.tar", max compression
```

## Comparing `nhl_api_py-2.5.1.tar` & `nhl_api_py-2.6.0.tar`

### file list

```diff
@@ -1,36 +1,37 @@
--rw-r--r--   0        0        0    10405 2024-02-21 21:55:14.804094 nhl_api_py-2.5.1/README.md
--rw-r--r--   0        0        0       48 2023-11-21 00:18:26.510111 nhl_api_py-2.5.1/nhlpy/__init__.py
--rw-r--r--   0        0        0      135 2024-04-21 16:25:45.476047 nhl_api_py-2.5.1/nhlpy/_version.py
--rw-r--r--   0        0        0        0 2024-02-15 22:28:54.670055 nhl_api_py-2.5.1/nhlpy/api/__init__.py
--rw-r--r--   0        0        0     2586 2024-03-30 14:21:16.927747 nhl_api_py-2.5.1/nhlpy/api/game_center.py
--rw-r--r--   0        0        0    10934 2023-11-22 20:23:27.214283 nhl_api_py-2.5.1/nhlpy/api/helpers.py
--rw-r--r--   0        0        0     1525 2024-02-07 23:53:57.475920 nhl_api_py-2.5.1/nhlpy/api/misc.py
--rw-r--r--   0        0        0       54 2024-02-15 22:28:54.670254 nhl_api_py-2.5.1/nhlpy/api/query/__init__.py
--rw-r--r--   0        0        0     1683 2024-02-15 22:28:54.670371 nhl_api_py-2.5.1/nhlpy/api/query/builder.py
--rw-r--r--   0        0        0      235 2024-02-15 22:28:54.670502 nhl_api_py-2.5.1/nhlpy/api/query/filters/__init__.py
--rw-r--r--   0        0        0      789 2024-02-15 22:28:54.670605 nhl_api_py-2.5.1/nhlpy/api/query/filters/decision.py
--rw-r--r--   0        0        0      738 2024-02-15 22:28:54.670704 nhl_api_py-2.5.1/nhlpy/api/query/filters/draft.py
--rw-r--r--   0        0        0      540 2024-02-15 22:28:54.670802 nhl_api_py-2.5.1/nhlpy/api/query/filters/experience.py
--rw-r--r--   0        0        0      389 2024-02-15 22:28:54.670895 nhl_api_py-2.5.1/nhlpy/api/query/filters/franchise.py
--rw-r--r--   0        0        0      375 2024-02-15 22:28:54.670987 nhl_api_py-2.5.1/nhlpy/api/query/filters/game_type.py
--rw-r--r--   0        0        0      472 2024-02-15 22:28:54.671078 nhl_api_py-2.5.1/nhlpy/api/query/filters/home_road.py
--rw-r--r--   0        0        0      948 2024-02-15 22:28:54.671170 nhl_api_py-2.5.1/nhlpy/api/query/filters/nationality.py
--rw-r--r--   0        0        0      531 2024-02-15 22:28:54.671265 nhl_api_py-2.5.1/nhlpy/api/query/filters/opponent.py
--rw-r--r--   0        0        0      904 2024-02-15 22:28:54.671356 nhl_api_py-2.5.1/nhlpy/api/query/filters/position.py
--rw-r--r--   0        0        0      719 2024-02-15 22:28:54.671448 nhl_api_py-2.5.1/nhlpy/api/query/filters/season.py
--rw-r--r--   0        0        0      520 2024-02-15 22:28:54.671540 nhl_api_py-2.5.1/nhlpy/api/query/filters/shoot_catch.py
--rw-r--r--   0        0        0     1052 2024-02-15 22:28:54.671646 nhl_api_py-2.5.1/nhlpy/api/query/filters/status.py
--rw-r--r--   0        0        0        0 2024-02-15 22:28:54.671681 nhl_api_py-2.5.1/nhlpy/api/query/sorting/__init__.py
--rw-r--r--   0        0        0     4910 2024-02-15 22:28:54.671800 nhl_api_py-2.5.1/nhlpy/api/query/sorting/sorting_options.py
--rw-r--r--   0        0        0     2875 2024-02-13 02:14:59.762848 nhl_api_py-2.5.1/nhlpy/api/schedule.py
--rw-r--r--   0        0        0     2511 2023-11-26 16:03:46.687429 nhl_api_py-2.5.1/nhlpy/api/standings.py
--rw-r--r--   0        0        0     9662 2024-02-15 22:28:54.671967 nhl_api_py-2.5.1/nhlpy/api/stats.py
--rw-r--r--   0        0        0     2090 2024-02-07 23:53:57.476406 nhl_api_py-2.5.1/nhlpy/api/teams.py
--rw-r--r--   0        0        0      461 2024-02-21 21:55:14.804604 nhl_api_py-2.5.1/nhlpy/config.py
--rw-r--r--   0        0        0    31916 2023-11-21 00:18:26.511169 nhl_api_py-2.5.1/nhlpy/data/seasonal_information_manifest.json
--rw-r--r--   0        0        0     4749 2024-02-08 00:48:32.228772 nhl_api_py-2.5.1/nhlpy/data/team_stat_ids.json
--rw-r--r--   0        0        0     2299 2023-11-22 20:23:27.217165 nhl_api_py-2.5.1/nhlpy/data/teams_20232024.json
--rw-r--r--   0        0        0     1487 2024-03-30 13:49:01.322575 nhl_api_py-2.5.1/nhlpy/http_client.py
--rw-r--r--   0        0        0     1772 2024-02-21 21:55:14.805037 nhl_api_py-2.5.1/nhlpy/nhl_client.py
--rw-r--r--   0        0        0     1873 2024-04-21 16:25:45.473300 nhl_api_py-2.5.1/pyproject.toml
--rw-r--r--   0        0        0    11725 1970-01-01 00:00:00.000000 nhl_api_py-2.5.1/PKG-INFO
+-rw-r--r--   0        0        0    10405 2024-02-21 21:55:14.804094 nhl_api_py-2.6.0/README.md
+-rw-r--r--   0        0        0       48 2023-11-21 00:18:26.510111 nhl_api_py-2.6.0/nhlpy/__init__.py
+-rw-r--r--   0        0        0      135 2024-04-26 12:50:36.018428 nhl_api_py-2.6.0/nhlpy/_version.py
+-rw-r--r--   0        0        0        0 2024-02-15 22:28:54.670055 nhl_api_py-2.6.0/nhlpy/api/__init__.py
+-rw-r--r--   0        0        0     2586 2024-03-30 14:21:16.927747 nhl_api_py-2.6.0/nhlpy/api/game_center.py
+-rw-r--r--   0        0        0    10934 2023-11-22 20:23:27.214283 nhl_api_py-2.6.0/nhlpy/api/helpers.py
+-rw-r--r--   0        0        0     1525 2024-02-07 23:53:57.475920 nhl_api_py-2.6.0/nhlpy/api/misc.py
+-rw-r--r--   0        0        0     1365 2024-04-26 12:50:36.018680 nhl_api_py-2.6.0/nhlpy/api/playoffs.py
+-rw-r--r--   0        0        0       54 2024-02-15 22:28:54.670254 nhl_api_py-2.6.0/nhlpy/api/query/__init__.py
+-rw-r--r--   0        0        0     1683 2024-02-15 22:28:54.670371 nhl_api_py-2.6.0/nhlpy/api/query/builder.py
+-rw-r--r--   0        0        0      235 2024-02-15 22:28:54.670502 nhl_api_py-2.6.0/nhlpy/api/query/filters/__init__.py
+-rw-r--r--   0        0        0      789 2024-02-15 22:28:54.670605 nhl_api_py-2.6.0/nhlpy/api/query/filters/decision.py
+-rw-r--r--   0        0        0      738 2024-02-15 22:28:54.670704 nhl_api_py-2.6.0/nhlpy/api/query/filters/draft.py
+-rw-r--r--   0        0        0      540 2024-02-15 22:28:54.670802 nhl_api_py-2.6.0/nhlpy/api/query/filters/experience.py
+-rw-r--r--   0        0        0      389 2024-02-15 22:28:54.670895 nhl_api_py-2.6.0/nhlpy/api/query/filters/franchise.py
+-rw-r--r--   0        0        0      375 2024-02-15 22:28:54.670987 nhl_api_py-2.6.0/nhlpy/api/query/filters/game_type.py
+-rw-r--r--   0        0        0      472 2024-02-15 22:28:54.671078 nhl_api_py-2.6.0/nhlpy/api/query/filters/home_road.py
+-rw-r--r--   0        0        0      948 2024-02-15 22:28:54.671170 nhl_api_py-2.6.0/nhlpy/api/query/filters/nationality.py
+-rw-r--r--   0        0        0      531 2024-02-15 22:28:54.671265 nhl_api_py-2.6.0/nhlpy/api/query/filters/opponent.py
+-rw-r--r--   0        0        0      904 2024-02-15 22:28:54.671356 nhl_api_py-2.6.0/nhlpy/api/query/filters/position.py
+-rw-r--r--   0        0        0      719 2024-02-15 22:28:54.671448 nhl_api_py-2.6.0/nhlpy/api/query/filters/season.py
+-rw-r--r--   0        0        0      520 2024-02-15 22:28:54.671540 nhl_api_py-2.6.0/nhlpy/api/query/filters/shoot_catch.py
+-rw-r--r--   0        0        0     1052 2024-02-15 22:28:54.671646 nhl_api_py-2.6.0/nhlpy/api/query/filters/status.py
+-rw-r--r--   0        0        0        0 2024-02-15 22:28:54.671681 nhl_api_py-2.6.0/nhlpy/api/query/sorting/__init__.py
+-rw-r--r--   0        0        0     4910 2024-02-15 22:28:54.671800 nhl_api_py-2.6.0/nhlpy/api/query/sorting/sorting_options.py
+-rw-r--r--   0        0        0     2875 2024-02-13 02:14:59.762848 nhl_api_py-2.6.0/nhlpy/api/schedule.py
+-rw-r--r--   0        0        0     2511 2023-11-26 16:03:46.687429 nhl_api_py-2.6.0/nhlpy/api/standings.py
+-rw-r--r--   0        0        0     9662 2024-02-15 22:28:54.671967 nhl_api_py-2.6.0/nhlpy/api/stats.py
+-rw-r--r--   0        0        0     2090 2024-02-07 23:53:57.476406 nhl_api_py-2.6.0/nhlpy/api/teams.py
+-rw-r--r--   0        0        0      461 2024-02-21 21:55:14.804604 nhl_api_py-2.6.0/nhlpy/config.py
+-rw-r--r--   0        0        0    31916 2023-11-21 00:18:26.511169 nhl_api_py-2.6.0/nhlpy/data/seasonal_information_manifest.json
+-rw-r--r--   0        0        0     4749 2024-02-08 00:48:32.228772 nhl_api_py-2.6.0/nhlpy/data/team_stat_ids.json
+-rw-r--r--   0        0        0     2299 2023-11-22 20:23:27.217165 nhl_api_py-2.6.0/nhlpy/data/teams_20232024.json
+-rw-r--r--   0        0        0     1487 2024-03-30 13:49:01.322575 nhl_api_py-2.6.0/nhlpy/http_client.py
+-rw-r--r--   0        0        0     1855 2024-04-26 12:50:36.018929 nhl_api_py-2.6.0/nhlpy/nhl_client.py
+-rw-r--r--   0        0        0     1873 2024-04-26 12:50:36.019170 nhl_api_py-2.6.0/pyproject.toml
+-rw-r--r--   0        0        0    11725 1970-01-01 00:00:00.000000 nhl_api_py-2.6.0/PKG-INFO
```

### Comparing `nhl_api_py-2.5.1/README.md` & `nhl_api_py-2.6.0/README.md`

 * *Files identical despite different names*

### Comparing `nhl_api_py-2.5.1/nhlpy/api/game_center.py` & `nhl_api_py-2.6.0/nhlpy/api/game_center.py`

 * *Files identical despite different names*

### Comparing `nhl_api_py-2.5.1/nhlpy/api/helpers.py` & `nhl_api_py-2.6.0/nhlpy/api/helpers.py`

 * *Files identical despite different names*

### Comparing `nhl_api_py-2.5.1/nhlpy/api/misc.py` & `nhl_api_py-2.6.0/nhlpy/api/misc.py`

 * *Files identical despite different names*

### Comparing `nhl_api_py-2.5.1/nhlpy/api/query/builder.py` & `nhl_api_py-2.6.0/nhlpy/api/query/builder.py`

 * *Files identical despite different names*

### Comparing `nhl_api_py-2.5.1/nhlpy/api/query/filters/decision.py` & `nhl_api_py-2.6.0/nhlpy/api/query/filters/decision.py`

 * *Files identical despite different names*

### Comparing `nhl_api_py-2.5.1/nhlpy/api/query/filters/draft.py` & `nhl_api_py-2.6.0/nhlpy/api/query/filters/draft.py`

 * *Files identical despite different names*

### Comparing `nhl_api_py-2.5.1/nhlpy/api/query/filters/experience.py` & `nhl_api_py-2.6.0/nhlpy/api/query/filters/experience.py`

 * *Files identical despite different names*

### Comparing `nhl_api_py-2.5.1/nhlpy/api/query/filters/nationality.py` & `nhl_api_py-2.6.0/nhlpy/api/query/filters/nationality.py`

 * *Files identical despite different names*

### Comparing `nhl_api_py-2.5.1/nhlpy/api/query/filters/opponent.py` & `nhl_api_py-2.6.0/nhlpy/api/query/filters/opponent.py`

 * *Files identical despite different names*

### Comparing `nhl_api_py-2.5.1/nhlpy/api/query/filters/position.py` & `nhl_api_py-2.6.0/nhlpy/api/query/filters/position.py`

 * *Files identical despite different names*

### Comparing `nhl_api_py-2.5.1/nhlpy/api/query/filters/season.py` & `nhl_api_py-2.6.0/nhlpy/api/query/filters/season.py`

 * *Files identical despite different names*

### Comparing `nhl_api_py-2.5.1/nhlpy/api/query/filters/shoot_catch.py` & `nhl_api_py-2.6.0/nhlpy/api/query/filters/shoot_catch.py`

 * *Files identical despite different names*

### Comparing `nhl_api_py-2.5.1/nhlpy/api/query/filters/status.py` & `nhl_api_py-2.6.0/nhlpy/api/query/filters/status.py`

 * *Files identical despite different names*

### Comparing `nhl_api_py-2.5.1/nhlpy/api/query/sorting/sorting_options.py` & `nhl_api_py-2.6.0/nhlpy/api/query/sorting/sorting_options.py`

 * *Files identical despite different names*

### Comparing `nhl_api_py-2.5.1/nhlpy/api/schedule.py` & `nhl_api_py-2.6.0/nhlpy/api/schedule.py`

 * *Files identical despite different names*

### Comparing `nhl_api_py-2.5.1/nhlpy/api/standings.py` & `nhl_api_py-2.6.0/nhlpy/api/standings.py`

 * *Files identical despite different names*

### Comparing `nhl_api_py-2.5.1/nhlpy/api/stats.py` & `nhl_api_py-2.6.0/nhlpy/api/stats.py`

 * *Files identical despite different names*

### Comparing `nhl_api_py-2.5.1/nhlpy/api/teams.py` & `nhl_api_py-2.6.0/nhlpy/api/teams.py`

 * *Files identical despite different names*

### Comparing `nhl_api_py-2.5.1/nhlpy/data/seasonal_information_manifest.json` & `nhl_api_py-2.6.0/nhlpy/data/seasonal_information_manifest.json`

 * *Files identical despite different names*

### Comparing `nhl_api_py-2.5.1/nhlpy/data/team_stat_ids.json` & `nhl_api_py-2.6.0/nhlpy/data/team_stat_ids.json`

 * *Files identical despite different names*

### Comparing `nhl_api_py-2.5.1/nhlpy/data/teams_20232024.json` & `nhl_api_py-2.6.0/nhlpy/data/teams_20232024.json`

 * *Files identical despite different names*

### Comparing `nhl_api_py-2.5.1/nhlpy/http_client.py` & `nhl_api_py-2.6.0/nhlpy/http_client.py`

 * *Files identical despite different names*

### Comparing `nhl_api_py-2.5.1/nhlpy/nhl_client.py` & `nhl_api_py-2.6.0/nhlpy/nhl_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from nhlpy.api import teams, standings, schedule, game_center, stats, misc
+from nhlpy.api import teams, standings, schedule, game_center, stats, misc, playoffs
 from nhlpy.http_client import HttpClient
 from nhlpy.config import ClientConfig
 
 
 class NHLClient:
     """
     This is the main class that is used to access the NHL API.
@@ -31,7 +31,8 @@
 
         self.teams = teams.Teams(http_client=self._http_client)
         self.standings = standings.Standings(http_client=self._http_client)
         self.schedule = schedule.Schedule(http_client=self._http_client)
         self.game_center = game_center.GameCenter(http_client=self._http_client)
         self.stats = stats.Stats(http_client=self._http_client)
         self.misc = misc.Misc(http_client=self._http_client)
+        self.playoffs = playoffs.Playoffs(http_client=self._http_client)
```

### Comparing `nhl_api_py-2.5.1/pyproject.toml` & `nhl_api_py-2.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "nhl-api-py"
-version = "2.5.1"
+version = "2.6.0"
 description = "NHL API.  For standings, team stats, outcomes, player information.  Contains each individual API endpoint as well as convience methods for easy data loading in Pandas or any ML applications."
 authors = ["Corey Schaf <cschaf@gmail.com>"]
 readme = "README.md"
 packages = [{include = "nhlpy"}]
 license = "GPL-3.0-or-later"
 homepage = "https://github.com/coreyjs/nhl-api-py"
 repository = "https://github.com/coreyjs/nhl-api-py"
```

### Comparing `nhl_api_py-2.5.1/PKG-INFO` & `nhl_api_py-2.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nhl-api-py
-Version: 2.5.1
+Version: 2.6.0
 Summary: NHL API.  For standings, team stats, outcomes, player information.  Contains each individual API endpoint as well as convience methods for easy data loading in Pandas or any ML applications.
 Home-page: https://github.com/coreyjs/nhl-api-py
 License: GPL-3.0-or-later
 Keywords: nhl,api,wrapper,hockey,sports
 Author: Corey Schaf
 Author-email: cschaf@gmail.com
 Requires-Python: >=3.9,<4.0
```

