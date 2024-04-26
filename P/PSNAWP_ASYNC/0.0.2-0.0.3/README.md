# Comparing `tmp/psnawp_async-0.0.2.tar.gz` & `tmp/psnawp_async-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psnawp_async-0.0.2.tar", max compression
+gzip compressed data, was "psnawp_async-0.0.3.tar", max compression
```

## Comparing `psnawp_async-0.0.2.tar` & `psnawp_async-0.0.3.tar`

### file list

```diff
@@ -1,31 +1,32 @@
--rw-r--r--   0        0        0     5036 2023-12-26 13:33:00.089102 psnawp_async-0.0.2/LICENSE.md
--rw-r--r--   0        0        0    11361 2023-12-26 13:33:00.089238 psnawp_async-0.0.2/README.md
--rw-r--r--   0        0        0     1794 2024-01-14 14:46:22.962215 psnawp_async-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      103 2023-12-26 13:33:00.091388 psnawp_async-0.0.2/src/psnawp_api/__init__.py
--rw-r--r--   0        0        0        0 2023-12-26 13:33:00.091443 psnawp_async-0.0.2/src/psnawp_api/core/__init__.py
--rw-r--r--   0        0        0     5434 2023-12-26 17:23:25.116614 psnawp_async-0.0.2/src/psnawp_api/core/authenticator.py
--rw-r--r--   0        0        0     1054 2023-12-26 13:33:00.091597 psnawp_async-0.0.2/src/psnawp_api/core/psnawp_exceptions.py
--rw-r--r--   0        0        0        0 2023-12-26 13:33:00.091650 psnawp_async-0.0.2/src/psnawp_api/models/__init__.py
--rw-r--r--   0        0        0    17006 2024-01-14 13:54:28.004571 psnawp_async-0.0.2/src/psnawp_api/models/client.py
--rw-r--r--   0        0        0     5174 2024-01-10 02:42:18.185060 psnawp_async-0.0.2/src/psnawp_api/models/game_title.py
--rw-r--r--   0        0        0     7982 2024-01-09 00:39:35.484961 psnawp_async-0.0.2/src/psnawp_api/models/group.py
--rw-r--r--   0        0        0        0 2023-12-26 13:33:00.091943 psnawp_async-0.0.2/src/psnawp_api/models/listing/__init__.py
--rw-r--r--   0        0        0     2829 2023-12-26 13:33:00.092011 psnawp_async-0.0.2/src/psnawp_api/models/listing/listing_generator.py
--rw-r--r--   0        0        0      538 2023-12-26 13:33:00.092068 psnawp_async-0.0.2/src/psnawp_api/models/listing/pagination_arguments.py
--rw-r--r--   0        0        0     5152 2024-01-10 01:22:36.758031 psnawp_async-0.0.2/src/psnawp_api/models/search.py
--rw-r--r--   0        0        0     5976 2023-12-26 13:33:00.092238 psnawp_async-0.0.2/src/psnawp_api/models/title_stats.py
--rw-r--r--   0        0        0        0 2023-12-26 13:33:00.092288 psnawp_async-0.0.2/src/psnawp_api/models/trophies/__init__.py
--rw-r--r--   0        0        0    12552 2024-01-09 01:44:08.774835 psnawp_async-0.0.2/src/psnawp_api/models/trophies/trophy.py
--rw-r--r--   0        0        0      600 2023-12-26 13:33:00.092438 psnawp_async-0.0.2/src/psnawp_api/models/trophies/trophy_constants.py
--rw-r--r--   0        0        0    10560 2023-12-26 13:33:00.092508 psnawp_async-0.0.2/src/psnawp_api/models/trophies/trophy_group.py
--rw-r--r--   0        0        0     2047 2024-01-06 15:34:03.418465 psnawp_async-0.0.2/src/psnawp_api/models/trophies/trophy_summary.py
--rw-r--r--   0        0        0    10792 2024-01-09 03:07:43.352644 psnawp_async-0.0.2/src/psnawp_api/models/trophies/trophy_titles.py
--rw-r--r--   0        0        0      476 2023-12-26 13:33:00.092700 psnawp_async-0.0.2/src/psnawp_api/models/trophies/utility_functions.py
--rw-r--r--   0        0        0    15901 2024-01-07 14:28:18.830287 psnawp_async-0.0.2/src/psnawp_api/models/user.py
--rw-r--r--   0        0        0     7602 2024-01-14 13:44:30.674364 psnawp_async-0.0.2/src/psnawp_api/psnawp.py
--rw-r--r--   0        0        0        0 2023-12-26 13:33:00.092873 psnawp_async-0.0.2/src/psnawp_api/py.typed
--rw-r--r--   0        0        0        0 2023-12-26 13:33:00.092934 psnawp_async-0.0.2/src/psnawp_api/utils/__init__.py
--rw-r--r--   0        0        0     2532 2023-12-26 13:33:00.093004 psnawp_async-0.0.2/src/psnawp_api/utils/endpoints.py
--rw-r--r--   0        0        0     2396 2023-12-26 13:33:00.093059 psnawp_async-0.0.2/src/psnawp_api/utils/misc.py
--rw-r--r--   0        0        0     6717 2024-01-09 00:37:14.529223 psnawp_async-0.0.2/src/psnawp_api/utils/request_builder.py
--rw-r--r--   0        0        0    12206 1970-01-01 00:00:00.000000 psnawp_async-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      195 2023-12-26 13:33:00.088904 psnawp_async-0.0.3/AUTHORS.md
+-rw-r--r--   0        0        0     5036 2023-12-26 13:33:00.089102 psnawp_async-0.0.3/LICENSE.md
+-rw-r--r--   0        0        0    11361 2023-12-26 13:33:00.089238 psnawp_async-0.0.3/README.md
+-rw-r--r--   0        0        0     1795 2024-04-26 15:37:54.356138 psnawp_async-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      103 2023-12-26 13:33:00.091388 psnawp_async-0.0.3/src/psnawp_api/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-26 13:33:00.091443 psnawp_async-0.0.3/src/psnawp_api/core/__init__.py
+-rw-r--r--   0        0        0     5434 2023-12-26 17:23:25.116614 psnawp_async-0.0.3/src/psnawp_api/core/authenticator.py
+-rw-r--r--   0        0        0     1054 2023-12-26 13:33:00.091597 psnawp_async-0.0.3/src/psnawp_api/core/psnawp_exceptions.py
+-rw-r--r--   0        0        0        0 2023-12-26 13:33:00.091650 psnawp_async-0.0.3/src/psnawp_api/models/__init__.py
+-rw-r--r--   0        0        0    17021 2024-01-20 21:23:43.842260 psnawp_async-0.0.3/src/psnawp_api/models/client.py
+-rw-r--r--   0        0        0     5174 2024-01-10 02:42:18.185060 psnawp_async-0.0.3/src/psnawp_api/models/game_title.py
+-rw-r--r--   0        0        0     7982 2024-01-09 00:39:35.484961 psnawp_async-0.0.3/src/psnawp_api/models/group.py
+-rw-r--r--   0        0        0        0 2023-12-26 13:33:00.091943 psnawp_async-0.0.3/src/psnawp_api/models/listing/__init__.py
+-rw-r--r--   0        0        0     2829 2023-12-26 13:33:00.092011 psnawp_async-0.0.3/src/psnawp_api/models/listing/listing_generator.py
+-rw-r--r--   0        0        0      538 2023-12-26 13:33:00.092068 psnawp_async-0.0.3/src/psnawp_api/models/listing/pagination_arguments.py
+-rw-r--r--   0        0        0     5152 2024-01-10 01:22:36.758031 psnawp_async-0.0.3/src/psnawp_api/models/search.py
+-rw-r--r--   0        0        0     5976 2023-12-26 13:33:00.092238 psnawp_async-0.0.3/src/psnawp_api/models/title_stats.py
+-rw-r--r--   0        0        0        0 2023-12-26 13:33:00.092288 psnawp_async-0.0.3/src/psnawp_api/models/trophies/__init__.py
+-rw-r--r--   0        0        0    12552 2024-01-09 01:44:08.774835 psnawp_async-0.0.3/src/psnawp_api/models/trophies/trophy.py
+-rw-r--r--   0        0        0      600 2023-12-26 13:33:00.092438 psnawp_async-0.0.3/src/psnawp_api/models/trophies/trophy_constants.py
+-rw-r--r--   0        0        0    10560 2023-12-26 13:33:00.092508 psnawp_async-0.0.3/src/psnawp_api/models/trophies/trophy_group.py
+-rw-r--r--   0        0        0     2047 2024-01-06 15:34:03.418465 psnawp_async-0.0.3/src/psnawp_api/models/trophies/trophy_summary.py
+-rw-r--r--   0        0        0    10792 2024-01-09 03:07:43.352644 psnawp_async-0.0.3/src/psnawp_api/models/trophies/trophy_titles.py
+-rw-r--r--   0        0        0      476 2023-12-26 13:33:00.092700 psnawp_async-0.0.3/src/psnawp_api/models/trophies/utility_functions.py
+-rw-r--r--   0        0        0    15901 2024-01-07 14:28:18.830287 psnawp_async-0.0.3/src/psnawp_api/models/user.py
+-rw-r--r--   0        0        0     7602 2024-01-14 13:44:30.674364 psnawp_async-0.0.3/src/psnawp_api/psnawp.py
+-rw-r--r--   0        0        0        0 2023-12-26 13:33:00.092873 psnawp_async-0.0.3/src/psnawp_api/py.typed
+-rw-r--r--   0        0        0        0 2023-12-26 13:33:00.092934 psnawp_async-0.0.3/src/psnawp_api/utils/__init__.py
+-rw-r--r--   0        0        0     2532 2023-12-26 13:33:00.093004 psnawp_async-0.0.3/src/psnawp_api/utils/endpoints.py
+-rw-r--r--   0        0        0     2396 2023-12-26 13:33:00.093059 psnawp_async-0.0.3/src/psnawp_api/utils/misc.py
+-rw-r--r--   0        0        0     6717 2024-01-09 00:37:14.529223 psnawp_async-0.0.3/src/psnawp_api/utils/request_builder.py
+-rw-r--r--   0        0        0    12214 1970-01-01 00:00:00.000000 psnawp_async-0.0.3/PKG-INFO
```

### Comparing `psnawp_async-0.0.2/LICENSE.md` & `psnawp_async-0.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `psnawp_async-0.0.2/README.md` & `psnawp_async-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `psnawp_async-0.0.2/pyproject.toml` & `psnawp_async-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PSNAWP_ASYNC"
-version = "0.0.2"
+version = "0.0.3"
 description = "Async Python API Wrapper for PlayStation Network API"
 authors = ["jackjpowell <jackjpowell@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["PSN", "PlayStation"]
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -18,15 +18,15 @@
     "Programming Language :: Python :: 3.11",
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
 packages = [{ include = "psnawp_api", from = "src" }]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-attrs = "23.1.0"
+attrs = "^23.1.0"
 requests = "^2.31.0"
 
 [tool.poetry.group.typing.dependencies]
 mypy = "^1.4.0"
 types-requests = "^2.31.0.2"
 
 [tool.poetry.group.linting.dependencies]
```

### Comparing `psnawp_async-0.0.2/src/psnawp_api/core/authenticator.py` & `psnawp_async-0.0.3/src/psnawp_api/core/authenticator.py`

 * *Files identical despite different names*

### Comparing `psnawp_async-0.0.2/src/psnawp_api/core/psnawp_exceptions.py` & `psnawp_async-0.0.3/src/psnawp_api/core/psnawp_exceptions.py`

 * *Files identical despite different names*

### Comparing `psnawp_async-0.0.2/src/psnawp_api/models/client.py` & `psnawp_async-0.0.3/src/psnawp_api/models/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,15 +189,15 @@
 
         """
         response = await self._request_builder.get(url=f"{BASE_PATH['profile_uri']}{API_PATH['available_to_play']}")
         json = response.json()
         user_list = []
         
         for account_id_dict in json["settings"]:
-            user = await User.create(
+            user = await User.from_account_id(
                  request_builder=self._request_builder,
                  account_id=account_id_dict["accountId"],
              )
             user_list.append(user)
         return user_list
         
         # return (
@@ -412,15 +412,15 @@
             ).user_trophy_groups_summary(account_id="me", platform=platform)
         else:
             return TrophyGroupsSummaryBuilder(
                 request_builder=self._request_builder,
                 np_communication_id=np_communication_id,
             ).user_trophy_groups_summary_with_metadata(account_id="me", platform=platform)
 
-    def title_stats(self, *, limit: Optional[int] = None, offset: int = 0, page_size: int = 200) -> TitleStatsListing:
+    async def title_stats(self, *, limit: Optional[int] = None, offset: int = 0, page_size: int = 200) -> TitleStatsListing:
         """Retrieve a list of titles with their stats and basic meta-data
 
         :param limit: Limit of titles returned.
         :type limit: Optional[int]
         :param page_size: The number of items to receive per api request.
         :type page_size: int
         :param offset: Specifies the offset for paginator
```

### Comparing `psnawp_async-0.0.2/src/psnawp_api/models/game_title.py` & `psnawp_async-0.0.3/src/psnawp_api/models/game_title.py`

 * *Files identical despite different names*

### Comparing `psnawp_async-0.0.2/src/psnawp_api/models/group.py` & `psnawp_async-0.0.3/src/psnawp_api/models/group.py`

 * *Files identical despite different names*

### Comparing `psnawp_async-0.0.2/src/psnawp_api/models/listing/listing_generator.py` & `psnawp_async-0.0.3/src/psnawp_api/models/listing/listing_generator.py`

 * *Files identical despite different names*

### Comparing `psnawp_async-0.0.2/src/psnawp_api/models/listing/pagination_arguments.py` & `psnawp_async-0.0.3/src/psnawp_api/models/listing/pagination_arguments.py`

 * *Files identical despite different names*

### Comparing `psnawp_async-0.0.2/src/psnawp_api/models/search.py` & `psnawp_async-0.0.3/src/psnawp_api/models/search.py`

 * *Files identical despite different names*

### Comparing `psnawp_async-0.0.2/src/psnawp_api/models/title_stats.py` & `psnawp_async-0.0.3/src/psnawp_api/models/title_stats.py`

 * *Files identical despite different names*

### Comparing `psnawp_async-0.0.2/src/psnawp_api/models/trophies/trophy.py` & `psnawp_async-0.0.3/src/psnawp_api/models/trophies/trophy.py`

 * *Files identical despite different names*

### Comparing `psnawp_async-0.0.2/src/psnawp_api/models/trophies/trophy_constants.py` & `psnawp_async-0.0.3/src/psnawp_api/models/trophies/trophy_constants.py`

 * *Files identical despite different names*

### Comparing `psnawp_async-0.0.2/src/psnawp_api/models/trophies/trophy_group.py` & `psnawp_async-0.0.3/src/psnawp_api/models/trophies/trophy_group.py`

 * *Files identical despite different names*

### Comparing `psnawp_async-0.0.2/src/psnawp_api/models/trophies/trophy_summary.py` & `psnawp_async-0.0.3/src/psnawp_api/models/trophies/trophy_summary.py`

 * *Files identical despite different names*

### Comparing `psnawp_async-0.0.2/src/psnawp_api/models/trophies/trophy_titles.py` & `psnawp_async-0.0.3/src/psnawp_api/models/trophies/trophy_titles.py`

 * *Files identical despite different names*

### Comparing `psnawp_async-0.0.2/src/psnawp_api/models/user.py` & `psnawp_async-0.0.3/src/psnawp_api/models/user.py`

 * *Files identical despite different names*

### Comparing `psnawp_async-0.0.2/src/psnawp_api/psnawp.py` & `psnawp_async-0.0.3/src/psnawp_api/psnawp.py`

 * *Files identical despite different names*

### Comparing `psnawp_async-0.0.2/src/psnawp_api/utils/endpoints.py` & `psnawp_async-0.0.3/src/psnawp_api/utils/endpoints.py`

 * *Files identical despite different names*

### Comparing `psnawp_async-0.0.2/src/psnawp_api/utils/misc.py` & `psnawp_async-0.0.3/src/psnawp_api/utils/misc.py`

 * *Files identical despite different names*

### Comparing `psnawp_async-0.0.2/src/psnawp_api/utils/request_builder.py` & `psnawp_async-0.0.3/src/psnawp_api/utils/request_builder.py`

 * *Files identical despite different names*

### Comparing `psnawp_async-0.0.2/PKG-INFO` & `psnawp_async-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PSNAWP_ASYNC
-Version: 0.0.2
+Version: 0.0.3
 Summary: Async Python API Wrapper for PlayStation Network API
 License: MIT
 Keywords: PSN,PlayStation
 Author: jackjpowell
 Author-email: jackjpowell@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: attrs (==23.1.0)
+Requires-Dist: attrs (>=23.1.0,<24.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # <img src="docs/_static/psn_logo.png" height="35px"> PlayStation Network API Wrapper Python (PSNAWP)
 
 Retrieve User Information, Trophies, Game and Store data from the PlayStation Network
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: PSNAWP_ASYNC Version: 0.0.2 Summary: Async Python
+Metadata-Version: 2.1 Name: PSNAWP_ASYNC Version: 0.0.3 Summary: Async Python
 API Wrapper for PlayStation Network API License: MIT Keywords: PSN,PlayStation
 Author: jackjpowell Author-email: jackjpowell@gmail.com Requires-Python:
 >=3.8,<4.0 Classifier: Development Status :: 4 - Beta Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Classifier: Topic :: Software Development :: Libraries :: Python
-Modules Requires-Dist: attrs (==23.1.0) Requires-Dist: requests
+Modules Requires-Dist: attrs (>=23.1.0,<24.0.0) Requires-Dist: requests
 (>=2.31.0,<3.0.0) Description-Content-Type: text/markdown # [docs/_static/
 psn_logo.png]PlayStation Network API Wrapper Python (PSNAWP) Retrieve User
 Information, Trophies, Game and Store data from the PlayStation Network [![PyPI
 version](https://badge.fury.io/py/psnawp.svg)](https://badge.fury.io/py/psnawp)
 [![Downloads](https://static.pepy.tech/badge/psnawp)](https://pepy.tech/
 project/psnawp) [![python-logo](https://img.shields.io/badge/python-
 3.8_|_3.9_|_3.10_|_3.11-blue.svg)](https://www.python.org/) [![pytest](https://
```

