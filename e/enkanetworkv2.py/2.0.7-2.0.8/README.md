# Comparing `tmp/enkanetworkv2.py-2.0.7.tar.gz` & `tmp/enkanetworkv2.py-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enkanetworkv2.py-2.0.7.tar", last modified: Thu Apr 25 10:22:25 2024, max compression
+gzip compressed data, was "enkanetworkv2.py-2.0.8.tar", last modified: Fri Apr 26 17:03:35 2024, max compression
```

## Comparing `enkanetworkv2.py-2.0.7.tar` & `enkanetworkv2.py-2.0.8.tar`

### file list

```diff
@@ -1,60 +1,59 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 10:22:25.002086 enkanetworkv2.py-2.0.7/
--rw-rw-rw-   0        0        0     1070 2024-02-24 18:53:52.000000 enkanetworkv2.py-2.0.7/LICENSE
--rw-rw-rw-   0        0        0       36 2024-02-24 18:58:13.000000 enkanetworkv2.py-2.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0    19341 2024-04-25 10:22:25.002086 enkanetworkv2.py-2.0.7/PKG-INFO
--rw-rw-rw-   0        0        0    18242 2024-02-24 19:02:02.000000 enkanetworkv2.py-2.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-04-25 10:22:24.952067 enkanetworkv2.py-2.0.7/enkanetwork/
--rw-rw-rw-   0        0        0     1462 2024-04-25 10:21:59.000000 enkanetworkv2.py-2.0.7/enkanetwork/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 10:22:24.935552 enkanetworkv2.py-2.0.7/enkanetwork/assets/
-drwxrwxrwx   0        0        0        0 2024-04-25 10:22:24.961575 enkanetworkv2.py-2.0.7/enkanetwork/assets/data/
--rw-rw-rw-   0        0        0    54223 2024-04-25 10:20:23.000000 enkanetworkv2.py-2.0.7/enkanetwork/assets/data/artifact_props.json
--rw-rw-rw-   0        0        0  1095132 2024-04-25 10:20:22.000000 enkanetworkv2.py-2.0.7/enkanetwork/assets/data/artifacts.json
--rw-rw-rw-   0        0        0    43649 2024-04-25 10:20:23.000000 enkanetworkv2.py-2.0.7/enkanetwork/assets/data/characters.json
--rw-rw-rw-   0        0        0    52516 2024-04-25 10:20:22.000000 enkanetworkv2.py-2.0.7/enkanetwork/assets/data/constellations.json
--rw-rw-rw-   0        0        0    12831 2024-04-25 10:20:22.000000 enkanetworkv2.py-2.0.7/enkanetwork/assets/data/costumes.json
--rw-rw-rw-   0        0        0  1316924 2024-04-25 10:20:22.000000 enkanetworkv2.py-2.0.7/enkanetwork/assets/data/fight_props.json
--rw-rw-rw-   0        0        0    57396 2024-04-25 10:20:21.000000 enkanetworkv2.py-2.0.7/enkanetwork/assets/data/namecards.json
--rw-rw-rw-   0        0        0     8862 2024-04-25 10:20:19.000000 enkanetworkv2.py-2.0.7/enkanetwork/assets/data/pfps.json
--rw-rw-rw-   0        0        0    87635 2024-04-25 10:20:22.000000 enkanetworkv2.py-2.0.7/enkanetwork/assets/data/skills.json
--rw-rw-rw-   0        0        0    41728 2024-04-25 10:20:21.000000 enkanetworkv2.py-2.0.7/enkanetwork/assets/data/weapons.json
-drwxrwxrwx   0        0        0        0 2024-04-25 10:22:24.970053 enkanetworkv2.py-2.0.7/enkanetwork/assets/langs/
--rw-rw-rw-   0        0        0   554994 2024-04-25 10:21:30.000000 enkanetworkv2.py-2.0.7/enkanetwork/assets/langs/artifact_sets.json
--rw-rw-rw-   0        0        0  2431947 2024-04-25 10:21:31.000000 enkanetworkv2.py-2.0.7/enkanetwork/assets/langs/artifacts.json
--rw-rw-rw-   0        0        0    33337 2024-04-25 10:21:31.000000 enkanetworkv2.py-2.0.7/enkanetwork/assets/langs/characters.json
--rw-rw-rw-   0        0        0   310851 2024-04-25 10:21:31.000000 enkanetworkv2.py-2.0.7/enkanetwork/assets/langs/constellations.json
--rw-rw-rw-   0        0        0    30562 2024-02-24 19:12:22.000000 enkanetworkv2.py-2.0.7/enkanetwork/assets/langs/fight_props.json
--rw-rw-rw-   0        0        0   122404 2024-04-25 10:21:31.000000 enkanetworkv2.py-2.0.7/enkanetwork/assets/langs/namecards.json
--rw-rw-rw-   0        0        0   309249 2024-04-25 10:21:32.000000 enkanetworkv2.py-2.0.7/enkanetwork/assets/langs/skills.json
--rw-rw-rw-   0        0        0   113312 2024-04-25 10:21:32.000000 enkanetworkv2.py-2.0.7/enkanetwork/assets/langs/weapons.json
--rw-rw-rw-   0        0        0     8268 2024-04-25 10:21:49.000000 enkanetworkv2.py-2.0.7/enkanetwork/assets.py
--rw-rw-rw-   0        0        0      645 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.7/enkanetwork/cache.py
--rw-rw-rw-   0        0        0    12474 2024-04-07 20:58:35.000000 enkanetworkv2.py-2.0.7/enkanetwork/client.py
--rw-rw-rw-   0        0        0      798 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.7/enkanetwork/config.py
--rw-rw-rw-   0        0        0     1099 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.7/enkanetwork/enum.py
--rw-rw-rw-   0        0        0     1925 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.7/enkanetwork/exception.py
--rw-rw-rw-   0        0        0     7345 2024-02-24 18:56:30.000000 enkanetworkv2.py-2.0.7/enkanetwork/http.py
-drwxrwxrwx   0        0        0        0 2024-04-25 10:22:24.979563 enkanetworkv2.py-2.0.7/enkanetwork/model/
--rw-rw-rw-   0        0        0      137 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.7/enkanetwork/model/__init__.py
--rw-rw-rw-   0        0        0     5029 2024-04-06 17:00:40.000000 enkanetworkv2.py-2.0.7/enkanetwork/model/assets.py
--rw-rw-rw-   0        0        0     1935 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.7/enkanetwork/model/base.py
--rw-rw-rw-   0        0        0     1403 2024-02-24 18:46:53.000000 enkanetworkv2.py-2.0.7/enkanetwork/model/build.py
--rw-rw-rw-   0        0        0     5183 2024-02-24 18:47:25.000000 enkanetworkv2.py-2.0.7/enkanetwork/model/character.py
--rw-rw-rw-   0        0        0     5634 2024-02-24 18:35:48.000000 enkanetworkv2.py-2.0.7/enkanetwork/model/equipments.py
--rw-rw-rw-   0        0        0      307 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.7/enkanetwork/model/hoyos.py
--rw-rw-rw-   0        0        0     4063 2024-04-06 17:07:07.000000 enkanetworkv2.py-2.0.7/enkanetwork/model/players.py
--rw-rw-rw-   0        0        0      346 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.7/enkanetwork/model/profile.py
--rw-rw-rw-   0        0        0     7763 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.7/enkanetwork/model/stats.py
--rw-rw-rw-   0        0        0      293 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.7/enkanetwork/model/utils.py
--rw-rw-rw-   0        0        0     1313 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.7/enkanetwork/tools.py
-drwxrwxrwx   0        0        0        0 2024-04-25 10:22:24.980563 enkanetworkv2.py-2.0.7/enkanetwork/types/
--rw-rw-rw-   0        0        0      157 2024-02-24 18:56:57.000000 enkanetworkv2.py-2.0.7/enkanetwork/types/__init__.py
--rw-rw-rw-   0        0        0     1157 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.7/enkanetwork/types/enkanetwork.py
--rw-rw-rw-   0        0        0     3450 2024-04-25 10:20:08.000000 enkanetworkv2.py-2.0.7/enkanetwork/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-25 10:22:25.001086 enkanetworkv2.py-2.0.7/enkanetworkv2.py.egg-info/
--rw-rw-rw-   0        0        0    19341 2024-04-25 10:22:24.000000 enkanetworkv2.py-2.0.7/enkanetworkv2.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1550 2024-04-25 10:22:24.000000 enkanetworkv2.py-2.0.7/enkanetworkv2.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 10:22:24.000000 enkanetworkv2.py-2.0.7/enkanetworkv2.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-04-25 10:22:24.000000 enkanetworkv2.py-2.0.7/enkanetworkv2.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-25 10:22:24.000000 enkanetworkv2.py-2.0.7/enkanetworkv2.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-25 10:22:25.002086 enkanetworkv2.py-2.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1105 2024-04-06 17:09:00.000000 enkanetworkv2.py-2.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 17:03:35.374206 enkanetworkv2.py-2.0.8/
+-rw-rw-rw-   0        0        0     1070 2024-02-24 18:53:52.000000 enkanetworkv2.py-2.0.8/LICENSE
+-rw-rw-rw-   0        0        0       36 2024-02-24 18:58:13.000000 enkanetworkv2.py-2.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0    19341 2024-04-26 17:03:35.373202 enkanetworkv2.py-2.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0    18242 2024-02-24 19:02:02.000000 enkanetworkv2.py-2.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-26 17:03:35.258993 enkanetworkv2.py-2.0.8/enkanetwork/
+-rw-rw-rw-   0        0        0     1462 2024-04-26 17:02:28.000000 enkanetworkv2.py-2.0.8/enkanetwork/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 17:03:35.244459 enkanetworkv2.py-2.0.8/enkanetwork/assets/
+drwxrwxrwx   0        0        0        0 2024-04-26 17:03:35.305090 enkanetworkv2.py-2.0.8/enkanetwork/assets/data/
+-rw-rw-rw-   0        0        0    54223 2024-04-26 16:59:15.000000 enkanetworkv2.py-2.0.8/enkanetwork/assets/data/artifact_props.json
+-rw-rw-rw-   0        0        0  1095132 2024-04-26 16:59:14.000000 enkanetworkv2.py-2.0.8/enkanetwork/assets/data/artifacts.json
+-rw-rw-rw-   0        0        0    43649 2024-04-26 16:59:15.000000 enkanetworkv2.py-2.0.8/enkanetwork/assets/data/characters.json
+-rw-rw-rw-   0        0        0    52516 2024-04-26 16:59:15.000000 enkanetworkv2.py-2.0.8/enkanetwork/assets/data/constellations.json
+-rw-rw-rw-   0        0        0    12831 2024-04-26 16:59:14.000000 enkanetworkv2.py-2.0.8/enkanetwork/assets/data/costumes.json
+-rw-rw-rw-   0        0        0  1316924 2024-04-26 16:59:15.000000 enkanetworkv2.py-2.0.8/enkanetwork/assets/data/fight_props.json
+-rw-rw-rw-   0        0        0    57396 2024-04-26 16:59:13.000000 enkanetworkv2.py-2.0.8/enkanetwork/assets/data/namecards.json
+-rw-rw-rw-   0        0        0     8862 2024-04-25 10:20:19.000000 enkanetworkv2.py-2.0.8/enkanetwork/assets/data/pfps.json
+-rw-rw-rw-   0        0        0    87635 2024-04-26 16:59:15.000000 enkanetworkv2.py-2.0.8/enkanetwork/assets/data/skills.json
+-rw-rw-rw-   0        0        0    41728 2024-04-26 16:59:13.000000 enkanetworkv2.py-2.0.8/enkanetwork/assets/data/weapons.json
+drwxrwxrwx   0        0        0        0 2024-04-26 17:03:35.345156 enkanetworkv2.py-2.0.8/enkanetwork/assets/langs/
+-rw-rw-rw-   0        0        0   554994 2024-04-26 17:00:26.000000 enkanetworkv2.py-2.0.8/enkanetwork/assets/langs/artifact_sets.json
+-rw-rw-rw-   0        0        0  2431947 2024-04-26 17:00:30.000000 enkanetworkv2.py-2.0.8/enkanetwork/assets/langs/artifacts.json
+-rw-rw-rw-   0        0        0    33337 2024-04-26 17:00:30.000000 enkanetworkv2.py-2.0.8/enkanetwork/assets/langs/characters.json
+-rw-rw-rw-   0        0        0   310851 2024-04-26 17:00:31.000000 enkanetworkv2.py-2.0.8/enkanetwork/assets/langs/constellations.json
+-rw-rw-rw-   0        0        0    30562 2024-02-24 19:12:22.000000 enkanetworkv2.py-2.0.8/enkanetwork/assets/langs/fight_props.json
+-rw-rw-rw-   0        0        0   122404 2024-04-26 17:00:31.000000 enkanetworkv2.py-2.0.8/enkanetwork/assets/langs/namecards.json
+-rw-rw-rw-   0        0        0   309249 2024-04-26 17:00:31.000000 enkanetworkv2.py-2.0.8/enkanetwork/assets/langs/skills.json
+-rw-rw-rw-   0        0        0   113312 2024-04-26 17:00:32.000000 enkanetworkv2.py-2.0.8/enkanetwork/assets/langs/weapons.json
+-rw-rw-rw-   0        0        0     8268 2024-04-25 10:21:49.000000 enkanetworkv2.py-2.0.8/enkanetwork/assets.py
+-rw-rw-rw-   0        0        0      645 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.8/enkanetwork/cache.py
+-rw-rw-rw-   0        0        0    12474 2024-04-07 20:58:35.000000 enkanetworkv2.py-2.0.8/enkanetwork/client.py
+-rw-rw-rw-   0        0        0      798 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.8/enkanetwork/config.py
+-rw-rw-rw-   0        0        0     1099 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.8/enkanetwork/enum.py
+-rw-rw-rw-   0        0        0     1925 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.8/enkanetwork/exception.py
+-rw-rw-rw-   0        0        0     7345 2024-02-24 18:56:30.000000 enkanetworkv2.py-2.0.8/enkanetwork/http.py
+drwxrwxrwx   0        0        0        0 2024-04-26 17:03:35.351665 enkanetworkv2.py-2.0.8/enkanetwork/model/
+-rw-rw-rw-   0        0        0      137 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.8/enkanetwork/model/__init__.py
+-rw-rw-rw-   0        0        0     5029 2024-04-06 17:00:40.000000 enkanetworkv2.py-2.0.8/enkanetwork/model/assets.py
+-rw-rw-rw-   0        0        0     1935 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.8/enkanetwork/model/base.py
+-rw-rw-rw-   0        0        0     1403 2024-02-24 18:46:53.000000 enkanetworkv2.py-2.0.8/enkanetwork/model/build.py
+-rw-rw-rw-   0        0        0     5183 2024-02-24 18:47:25.000000 enkanetworkv2.py-2.0.8/enkanetwork/model/character.py
+-rw-rw-rw-   0        0        0     5634 2024-02-24 18:35:48.000000 enkanetworkv2.py-2.0.8/enkanetwork/model/equipments.py
+-rw-rw-rw-   0        0        0      307 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.8/enkanetwork/model/hoyos.py
+-rw-rw-rw-   0        0        0     4063 2024-04-06 17:07:07.000000 enkanetworkv2.py-2.0.8/enkanetwork/model/players.py
+-rw-rw-rw-   0        0        0      346 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.8/enkanetwork/model/profile.py
+-rw-rw-rw-   0        0        0     7763 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.8/enkanetwork/model/stats.py
+-rw-rw-rw-   0        0        0      293 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.8/enkanetwork/model/utils.py
+-rw-rw-rw-   0        0        0     1313 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.8/enkanetwork/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-26 17:03:35.352169 enkanetworkv2.py-2.0.8/enkanetwork/types/
+-rw-rw-rw-   0        0        0     1157 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.8/enkanetwork/types/enkanetwork.py
+-rw-rw-rw-   0        0        0     3617 2024-04-26 17:01:35.000000 enkanetworkv2.py-2.0.8/enkanetwork/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-26 17:03:35.372697 enkanetworkv2.py-2.0.8/enkanetworkv2.py.egg-info/
+-rw-rw-rw-   0        0        0    19341 2024-04-26 17:03:35.000000 enkanetworkv2.py-2.0.8/enkanetworkv2.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1520 2024-04-26 17:03:35.000000 enkanetworkv2.py-2.0.8/enkanetworkv2.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 17:03:35.000000 enkanetworkv2.py-2.0.8/enkanetworkv2.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-04-26 17:03:35.000000 enkanetworkv2.py-2.0.8/enkanetworkv2.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-26 17:03:35.000000 enkanetworkv2.py-2.0.8/enkanetworkv2.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-26 17:03:35.374206 enkanetworkv2.py-2.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1105 2024-04-06 17:09:00.000000 enkanetworkv2.py-2.0.8/setup.py
```

### Comparing `enkanetworkv2.py-2.0.7/LICENSE` & `enkanetworkv2.py-2.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.7/PKG-INFO` & `enkanetworkv2.py-2.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enkanetworkv2.py
-Version: 2.0.7
+Version: 2.0.8
 Summary: Library for fetching JSON data from site https://enka.network/
 Home-page: https://github.com/DEViantUA/EnkaNetworkV2.py
 Author: DeviantUa
 Author-email: deviantapi@gmail.com
 Keywords: enkanetwork.py,enkanetwork,enka.network,genshinapi,enkanetworkV2,enkanetworkV2.py
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `enkanetworkv2.py-2.0.7/README.md` & `enkanetworkv2.py-2.0.8/README.md`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.7/enkanetwork/__init__.py` & `enkanetworkv2.py-2.0.8/enkanetwork/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE."""
 
 __title__ = 'enkanetworkV2.py'
 __author__ = 'DeviantUa'
-__version__ = '2.0.7'
+__version__ = '2.0.8'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2024-present DeviantUa'
 
 
 from .client import *
 from .exception import *
 from .model import *
```

### Comparing `enkanetworkv2.py-2.0.7/enkanetwork/assets/data/artifact_props.json` & `enkanetworkv2.py-2.0.8/enkanetwork/assets/data/artifact_props.json`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.7/enkanetwork/assets/data/artifacts.json` & `enkanetworkv2.py-2.0.8/enkanetwork/assets/data/artifacts.json`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.7/enkanetwork/assets/data/characters.json` & `enkanetworkv2.py-2.0.8/enkanetwork/assets/data/characters.json`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.7/enkanetwork/assets/data/constellations.json` & `enkanetworkv2.py-2.0.8/enkanetwork/assets/data/constellations.json`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.7/enkanetwork/assets/data/costumes.json` & `enkanetworkv2.py-2.0.8/enkanetwork/assets/data/costumes.json`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.7/enkanetwork/assets/data/fight_props.json` & `enkanetworkv2.py-2.0.8/enkanetwork/assets/data/fight_props.json`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.7/enkanetwork/assets/data/namecards.json` & `enkanetworkv2.py-2.0.8/enkanetwork/assets/data/namecards.json`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.7/enkanetwork/assets/data/pfps.json` & `enkanetworkv2.py-2.0.8/enkanetwork/assets/data/pfps.json`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.7/enkanetwork/assets/data/skills.json` & `enkanetworkv2.py-2.0.8/enkanetwork/assets/data/skills.json`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.7/enkanetwork/assets/data/weapons.json` & `enkanetworkv2.py-2.0.8/enkanetwork/assets/data/weapons.json`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.7/enkanetwork/assets/langs/artifact_sets.json` & `enkanetworkv2.py-2.0.8/enkanetwork/assets/langs/artifact_sets.json`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.7/enkanetwork/assets/langs/artifacts.json` & `enkanetworkv2.py-2.0.8/enkanetwork/assets/langs/artifacts.json`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.7/enkanetwork/assets/langs/characters.json` & `enkanetworkv2.py-2.0.8/enkanetwork/assets/langs/characters.json`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.7/enkanetwork/assets/langs/constellations.json` & `enkanetworkv2.py-2.0.8/enkanetwork/assets/langs/constellations.json`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.7/enkanetwork/assets/langs/fight_props.json` & `enkanetworkv2.py-2.0.8/enkanetwork/assets/langs/fight_props.json`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.7/enkanetwork/assets/langs/namecards.json` & `enkanetworkv2.py-2.0.8/enkanetwork/assets/langs/namecards.json`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.7/enkanetwork/assets/langs/skills.json` & `enkanetworkv2.py-2.0.8/enkanetwork/assets/langs/skills.json`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.7/enkanetwork/assets/langs/weapons.json` & `enkanetworkv2.py-2.0.8/enkanetwork/assets/langs/weapons.json`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.7/enkanetwork/assets.py` & `enkanetworkv2.py-2.0.8/enkanetwork/assets.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.7/enkanetwork/cache.py` & `enkanetworkv2.py-2.0.8/enkanetwork/cache.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.7/enkanetwork/client.py` & `enkanetworkv2.py-2.0.8/enkanetwork/client.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.7/enkanetwork/config.py` & `enkanetworkv2.py-2.0.8/enkanetwork/config.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.7/enkanetwork/enum.py` & `enkanetworkv2.py-2.0.8/enkanetwork/enum.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.7/enkanetwork/exception.py` & `enkanetworkv2.py-2.0.8/enkanetwork/exception.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.7/enkanetwork/http.py` & `enkanetworkv2.py-2.0.8/enkanetwork/http.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.7/enkanetwork/model/assets.py` & `enkanetworkv2.py-2.0.8/enkanetwork/model/assets.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.7/enkanetwork/model/base.py` & `enkanetworkv2.py-2.0.8/enkanetwork/model/base.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.7/enkanetwork/model/build.py` & `enkanetworkv2.py-2.0.8/enkanetwork/model/build.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.7/enkanetwork/model/character.py` & `enkanetworkv2.py-2.0.8/enkanetwork/model/character.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.7/enkanetwork/model/equipments.py` & `enkanetworkv2.py-2.0.8/enkanetwork/model/equipments.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.7/enkanetwork/model/players.py` & `enkanetworkv2.py-2.0.8/enkanetwork/model/players.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.7/enkanetwork/model/stats.py` & `enkanetworkv2.py-2.0.8/enkanetwork/model/stats.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.7/enkanetwork/tools.py` & `enkanetworkv2.py-2.0.8/enkanetwork/tools.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.7/enkanetwork/types/enkanetwork.py` & `enkanetworkv2.py-2.0.8/enkanetwork/types/enkanetwork.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.7/enkanetwork/utils.py` & `enkanetworkv2.py-2.0.8/enkanetwork/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -128,10 +128,13 @@
 
 async def update_pfps(path):
     async with aiohttp.ClientSession() as session:
         async with session.get("https://raw.githubusercontent.com/EnkaNetwork/API-docs/master/store/pfps.json") as response:
             data = await response.read()
             
     data = json.loads(data)
-    
-    with open(os.path.join(path, "data/pfps.json"), 'w',  encoding='utf-8') as file:
-        json.dump(data, file, indent=4)
+    try:
+        with open(os.path.join(path, "data/pfps.json"), 'w', encoding='utf-8') as file:
+            json.dump(data, file, indent=4)
+    except FileNotFoundError:
+        with open(os.path.join(path, "pfps.json"), 'w', encoding='utf-8') as file:
+            json.dump(data, file, indent=4)
```

### Comparing `enkanetworkv2.py-2.0.7/enkanetworkv2.py.egg-info/PKG-INFO` & `enkanetworkv2.py-2.0.8/enkanetworkv2.py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enkanetworkv2.py
-Version: 2.0.7
+Version: 2.0.8
 Summary: Library for fetching JSON data from site https://enka.network/
 Home-page: https://github.com/DEViantUA/EnkaNetworkV2.py
 Author: DeviantUa
 Author-email: deviantapi@gmail.com
 Keywords: enkanetwork.py,enkanetwork,enka.network,genshinapi,enkanetworkV2,enkanetworkV2.py
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `enkanetworkv2.py-2.0.7/enkanetworkv2.py.egg-info/SOURCES.txt` & `enkanetworkv2.py-2.0.8/enkanetworkv2.py.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,13 @@
 enkanetwork/model/character.py
 enkanetwork/model/equipments.py
 enkanetwork/model/hoyos.py
 enkanetwork/model/players.py
 enkanetwork/model/profile.py
 enkanetwork/model/stats.py
 enkanetwork/model/utils.py
-enkanetwork/types/__init__.py
 enkanetwork/types/enkanetwork.py
 enkanetworkv2.py.egg-info/PKG-INFO
 enkanetworkv2.py.egg-info/SOURCES.txt
 enkanetworkv2.py.egg-info/dependency_links.txt
 enkanetworkv2.py.egg-info/requires.txt
 enkanetworkv2.py.egg-info/top_level.txt
```

### Comparing `enkanetworkv2.py-2.0.7/setup.py` & `enkanetworkv2.py-2.0.8/setup.py`

 * *Files identical despite different names*

