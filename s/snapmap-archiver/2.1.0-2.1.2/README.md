# Comparing `tmp/snapmap-archiver-2.1.0.tar.gz` & `tmp/snapmap_archiver-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snapmap-archiver-2.1.0.tar", last modified: Sat Jan 28 03:31:28 2023, max compression
+gzip compressed data, was "snapmap_archiver-2.1.2.tar", max compression
```

## Comparing `snapmap-archiver-2.1.0.tar` & `snapmap_archiver-2.1.2.tar`

### file list

```diff
@@ -1,20 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-01-28 03:31:28.245219 snapmap-archiver-2.1.0/
--rw-rw-rw-   0        0        0    35823 2022-12-23 12:52:31.000000 snapmap-archiver-2.1.0/LICENSE
--rw-rw-rw-   0        0        0     2562 2023-01-28 03:31:28.244220 snapmap-archiver-2.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2262 2023-01-28 03:13:07.000000 snapmap-archiver-2.1.0/README.md
--rw-rw-rw-   0        0        0      440 2023-01-28 02:55:18.000000 snapmap-archiver-2.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-01-28 03:31:28.245219 snapmap-archiver-2.1.0/setup.cfg
--rw-rw-rw-   0        0        0      778 2023-01-28 02:41:34.000000 snapmap-archiver-2.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-28 03:31:28.231220 snapmap-archiver-2.1.0/snapmap_archiver/
--rw-rw-rw-   0        0        0     9240 2023-01-28 03:28:20.000000 snapmap-archiver-2.1.0/snapmap_archiver/SnapmapArchiver.py
--rw-rw-rw-   0        0        0     1785 2023-01-09 05:15:51.000000 snapmap-archiver-2.1.0/snapmap_archiver/__init__.py
--rw-rw-rw-   0        0        0       84 2023-01-28 03:14:38.000000 snapmap-archiver-2.1.0/snapmap_archiver/__main__.py
--rw-rw-rw-   0        0        0      817 2023-01-09 05:15:51.000000 snapmap-archiver-2.1.0/snapmap_archiver/coordinates.py
--rw-rw-rw-   0        0        0      264 2023-01-28 02:37:25.000000 snapmap-archiver-2.1.0/snapmap_archiver/snap.py
-drwxrwxrwx   0        0        0        0 2023-01-28 03:31:28.242216 snapmap-archiver-2.1.0/snapmap_archiver.egg-info/
--rw-rw-rw-   0        0        0     2562 2023-01-28 03:31:27.000000 snapmap-archiver-2.1.0/snapmap_archiver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      434 2023-01-28 03:31:27.000000 snapmap-archiver-2.1.0/snapmap_archiver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-28 03:31:27.000000 snapmap-archiver-2.1.0/snapmap_archiver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-01-28 03:31:27.000000 snapmap-archiver-2.1.0/snapmap_archiver.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       38 2023-01-28 03:31:27.000000 snapmap-archiver-2.1.0/snapmap_archiver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-01-28 03:31:27.000000 snapmap-archiver-2.1.0/snapmap_archiver.egg-info/top_level.txt
+-rw-r--r--   0        0        0    35823 2024-04-26 12:55:26.451161 snapmap_archiver-2.1.2/LICENSE
+-rw-r--r--   0        0        0      440 2024-04-26 13:55:22.620365 snapmap_archiver-2.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2262 2024-04-26 12:55:26.451161 snapmap_archiver-2.1.2/README.md
+-rw-r--r--   0        0        0     2179 2024-04-26 13:35:15.422379 snapmap_archiver-2.1.2/snapmap_archiver/__init__.py
+-rw-r--r--   0        0        0       84 2024-04-26 12:55:26.455162 snapmap_archiver-2.1.2/snapmap_archiver/__main__.py
+-rw-r--r--   0        0        0      599 2024-04-26 13:31:54.392135 snapmap_archiver-2.1.2/snapmap_archiver/coordinates.py
+-rw-r--r--   0        0        0      283 2024-04-26 13:31:54.393136 snapmap_archiver-2.1.2/snapmap_archiver/snap.py
+-rw-r--r--   0        0        0     9360 2024-04-26 13:57:40.865489 snapmap_archiver-2.1.2/snapmap_archiver/SnapmapArchiver.py
+-rw-r--r--   0        0        0      520 2024-04-26 13:53:40.404385 snapmap_archiver-2.1.2/snapmap_archiver/time.py
+-rw-r--r--   0        0        0     2939 1970-01-01 00:00:00.000000 snapmap_archiver-2.1.2/setup.py
+-rw-r--r--   0        0        0     2744 1970-01-01 00:00:00.000000 snapmap_archiver-2.1.2/PKG-INFO
```

### Comparing `snapmap-archiver-2.1.0/LICENSE` & `snapmap_archiver-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `snapmap-archiver-2.1.0/PKG-INFO` & `snapmap_archiver-2.1.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: snapmap-archiver
-Version: 2.1.0
-Summary: Download all Snapmaps content from a specific location.
-Home-page: https://github.com/king-millez/snapmap-archiver
-Author: Miles Greenwark
-Author-email: millez.dev@gmail.com
-Requires-Python: >=3.10
-License-File: LICENSE
-
 # snapmap-archiver
 
 A tool written in Python **3.10** to download all Snapmaps content from a specific location.
 
 ## Install Python 3.10+
 
 Be sure to check that you're using a version of Python that is 3.10 or above. **This project will not work on Python 3.9 or below!**
```

### Comparing `snapmap-archiver-2.1.0/snapmap_archiver/SnapmapArchiver.py` & `snapmap_archiver-2.1.2/snapmap_archiver/SnapmapArchiver.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,241 +1,267 @@
+import json
 import os
 import re
 import sys
-import json
-import requests
-from time import sleep
-from typing import Iterable, Any
+import typing as t
 from datetime import datetime
+from time import sleep
+
+import requests
 
 from snapmap_archiver.coordinates import Coordinates
 from snapmap_archiver.snap import Snap, SnapJSONEncoder
+from snapmap_archiver.time import since_epoch
 
+DEFAULT_RADIUS = 10_000
+MAX_RADIUS = 85_000
+ISSUES_URL = "https://github.com/king-millez/snapmap-archiver/issues/new/choose"
+SNAP_PATTERN = re.compile(
+    r"(?:https?:\/\/map\.snapchat\.com\/ttp\/snap\/)?(W7_(?:[a-zA-Z0-9\-_\+]{56})(?:\/?@-?[0-9]{1,3}\.?[0-9]{0,},-?[0-9]{1,3}\.?[0-9]{0,}(?:,[0-9]{1,3}\.?[0-9]{0,}z))?)"
+)
 
-class SnapmapArchiver:
-    MAX_RADIUS = 85_000
-    ISSUES_URL = "https://github.com/king-millez/snapmap-archiver/issues/new/choose"
-    SNAP_PATTERN = re.compile(
-        r"(?:https?:\/\/map\.snapchat\.com\/ttp\/snap\/)?(W7_(?:[aA-zZ0-9\-_\+]{22})(?:[aA-zZ0-9-_\+]{28})AAAAA[AQ])(?:\/?@-?[0-9]{1,3}\.?[0-9]{0,},-?[0-9]{1,3}\.?[0-9]{0,}(?:,[0-9]{1,3}\.?[0-9]{0,}z))?"
-    )
 
-    def __init__(self, *args, **kwargs) -> None:
+class SnapmapArchiver:
+    def __init__(
+        self,
+        *args: str,
+        output_dir: str,
+        input_file: t.Optional[str] = None,
+        since_time: t.Optional[str] = None,
+        locations: list[str] = [],
+        radius: int = DEFAULT_RADIUS,
+        write_json: bool = False,
+        zoom_depth: int = 5,
+    ) -> None:
         if sys.version_info < (3, 10):
             raise RuntimeError(
                 "Python 3.10 or above is required to use snapmap-archiver!"
             )
 
-        self.write_json = kwargs.get("write_json")
-        self.all_snaps: dict[str, Snap] = {}
+        self.since_time = None
+        if since_time:
+            self.since_time = since_epoch(since_time.lower())
+            print(f"Skipping Snaps older than [{self.since_time}].")
+
+        self.input_file = input_file
         self.arg_snaps = args
-        self.coords_list = []
-        self.radius = 10_000
-        self.zoom_depth = (
-            kwargs.get("zoom_depth") or 5
-        )  # TODO change this 5 to a default const somewhere?
-        self.input_file = ""
 
-        if not kwargs["locations"] and not args and not kwargs["input_file"]:
+        self.write_json = write_json
+        self.zoom_depth = zoom_depth
+        self.all_snaps: dict[str, Snap] = {}
+
+        if not locations and not args and not input_file:
             raise ValueError(
-                "Some sort of input is required; location (-l), input file (-f), and raw Snap IDs are all valid options."
+                "Some sort of input is required. Run snapmap-archiver with [-h] to see a list of options."
             )
 
-        if not kwargs["output_dir"]:
-            raise ValueError("Output directory (-o) is required.")
+        self.output_dir = os.path.expanduser(output_dir)
+        if not os.path.isdir(self.output_dir):
+            os.makedirs(self.output_dir, exist_ok=True)
 
-        self.output_dir = os.path.expanduser(kwargs["output_dir"])
+        self.radius = MAX_RADIUS if radius > MAX_RADIUS else radius
+        self.coords_list = [Coordinates(latlon) for latlon in locations]
 
-        if not os.path.isdir(self.output_dir):
-            os.makedirs(
-                self.output_dir, exist_ok=True
-            )  # Python's exception handling has us covered here
-
-        if kwargs.get("radius"):
-            self.radius = (
-                self.MAX_RADIUS
-                if kwargs["radius"] > self.MAX_RADIUS
-                else kwargs["radius"]
-            )
-
-        # Query provided coordinates for Snaps
-        if kwargs.get("locations"):
-            self.coords_list = [
-                Coordinates(latlon[0]) for latlon in kwargs["locations"]
-            ]
-
-        # Check input file for Snap IDs
-        if kwargs.get("input_file"):
-            self.input_file = kwargs["input_file"]
-
-    def download_snaps(self, group: list[Snap] | Snap):
-        if isinstance(group, Snap):
-            group = [group]
+    def download_snaps(self, group: t.Iterable[Snap]):
         for snap in group:
             fpath = os.path.join(self.output_dir, f"{snap.snap_id}.{snap.file_type}")
+
             if os.path.isfile(fpath):
-                print(f" - {fpath} already exists.")
+                print(f" - [{fpath}] already exists.")
                 continue
+
             with open(fpath, "wb") as f:
                 f.write(requests.get(snap.url).content)
-            print(f" - Downloaded {fpath}.")
 
-    def query_snaps(self, snaps: str | Iterable[str]) -> list[Snap]:
-        if isinstance(snaps, str):
-            snaps = [
-                snaps
-            ]  # The Snap query endpoint can take multiple IDs, so here we can query 1 or more snaps with ease.
-        to_query = []
+            print(f" - Downloaded [{fpath}].")
+
+    def query_snaps(self, snaps: t.Iterable[str]) -> list[Snap]:
+        to_query: list[str] = []
         for snap_id in snaps:
             rgx_match = re.search(
-                self.SNAP_PATTERN,
+                SNAP_PATTERN,
                 snap_id,
             )
             if not rgx_match:
-                print(f"{snap_id} is not a valid Snap URL or ID.")
+                print(f" - [{snap_id}] is not a valid Snap URL or ID.")
                 continue
             to_query.append(rgx_match.group(1))
+
+        if not to_query:
+            return []
+
+        api_response = requests.post(
+            "https://ms.sc-jpl.com/web/getStoryElements",
+            json={"snapIds": to_query},
+        )
         try:
-            retl = []
-            for snap in requests.post(
-                "https://ms.sc-jpl.com/web/getStoryElements",
-                json={"snapIds": to_query},
-            ).json()["elements"]:
+            retl: list[Snap] = []
+            for snap in api_response.json().get("elements", []):
                 s = self._parse_snap(snap)
                 if s:
                     retl.append(s)
             return retl
-        except requests.exceptions.JSONDecodeError:
+        except requests.exceptions.JSONDecodeError as e:
+            print(
+                f"Encountered error while querying Snap IDs:\n[{e}]. API Response: [{api_response.text}]."
+            )
             return []
 
     def query_coords(self, coords: Coordinates):
         to_download: dict[str, Snap] = {}
         current_iteration = self.radius
         epoch = self._get_epoch()
         while current_iteration != 1:
-            print(f"Querying with radius {current_iteration}...")
-            while True:
+            print(f"Querying with radius [{current_iteration}]...")
+            json_data = None
+            while not json_data:
                 api_data = requests.post(
                     "https://ms.sc-jpl.com/web/getPlaylist",
                     headers={
                         "Content-Type": "application/json",
                     },
                     json={
                         "requestGeoPoint": {"lat": coords.lat, "lon": coords.long},
                         "zoomLevel": self.zoom_depth,
                         "tileSetId": {"flavor": "default", "epoch": epoch, "type": 1},
                         "radiusMeters": current_iteration,
                         "maximumFuzzRadius": 0,
                     },
                 ).text
+
                 if api_data:
                     if api_data.strip() == "Too many requests":
                         print("You have been rate limited. Sleeping for 1 minute.")
                         sleep(60)
                     else:
                         try:
                             json_data = json.loads(api_data)["manifest"]["elements"]
-                            break
                         except requests.exceptions.JSONDecodeError:
-                            print("You have been rate limited. Sleeping for 1 minute.")
+                            print(
+                                f"Unable to decode API response (likely a rate limit): [{api_data}] Sleeping for 1 minute."
+                            )
                             sleep(60)
 
             for snap in json_data:
                 if to_download.get(
                     snap["id"]
                 ):  # Avoids downloading duplicates. Faster than a list because the Snap ID is indexed
                     continue
+
                 parsed = self._parse_snap(snap)
+
                 if not parsed:
                     continue
+
                 to_download[snap["id"]] = parsed
 
             if current_iteration > 2000:
                 current_iteration -= 2000
             elif current_iteration > 1000:
                 current_iteration -= 100
             else:
                 current_iteration = 1
 
-        print(f"Found {len(list(to_download.keys()))} Snaps")
-        return self._transform_index(to_download)
+        print(f"Found [{len(list(to_download.keys()))}] Snaps.")
+        return to_download.values()
 
     def main(self):
         # Query provided coordinates
-        if self.coords_list:
-            for coords in self.coords_list:
-                self.download_snaps(self.query_coords(coords))
+        for coords in self.coords_list:
+            self.download_snaps(self.query_coords(coords))
+
+        snap_ids = []
 
         # Download Snaps from input file
         if self.input_file:
             if os.path.isfile(self.input_file):
                 with open(self.input_file, "r") as f:
-                    to_format = [ln for ln in f.read().split("\n") if ln.strip()]
-                self.download_snaps(self.query_snaps(to_format))
+                    snap_ids = [ln for ln in f.read().split("\n") if ln.strip()]
             else:
-                raise FileNotFoundError("Input file does not exist.")
+                raise FileNotFoundError(
+                    f"Input file [{self.input_file}] does not exist."
+                )
+
+        snap_ids.extend(self.arg_snaps)
 
         # Download Snaps provided from the command line
-        self.download_snaps(self.query_snaps(self.arg_snaps))
+        self.download_snaps(self.query_snaps(snap_ids))
 
         if self.write_json:
             with open(
                 os.path.join(
                     self.output_dir, f"archive_{int(datetime.now().timestamp())}.json"
                 ),
                 "w",
             ) as f:
-                f.write(
-                    json.dumps(
-                        self._transform_index(self.all_snaps),
-                        indent=2,
-                        cls=SnapJSONEncoder,
-                    )
+                json.dump(
+                    list(self.all_snaps.values()),
+                    f,
+                    indent=2,
+                    cls=SnapJSONEncoder,
                 )
 
-    def _transform_index(self, index: dict[str, Snap]):
-        return [v for v in index.values()]
-
     def _parse_snap(
         self,
         snap: dict[
-            str, Any
+            str, t.Any
         ],  # I don't like the Any type but this dict is so dynamic there isn't much point hinting it accurately.
     ) -> Snap | None:
-        data_dict = {
-            "create_time": round(int(snap["timestamp"]) * 10**-3, 3),
-            "snap_id": snap["id"],
-        }
-        if snap["snapInfo"].get("snapMediaType"):
-            data_dict["file_type"] = "mp4"
-        elif snap["snapInfo"].get("streamingMediaInfo"):
-            data_dict["file_type"] = "jpg"
-        else:
+        if self.all_snaps.get(snap["id"]):
+            return self.all_snaps[snap["id"]]
+
+        file_type = (
+            "mp4"
+            if snap["snapInfo"].get("snapMediaType")
+            else "jpg"
+            if snap["snapInfo"].get("streamingMediaInfo")
+            else "UNKNOWN"
+        )
+
+        url: str | None = snap["snapInfo"]["streamingMediaInfo"].get("mediaUrl")
+        if not url:
+            print(f'Media URL for snap [{snap["id"]}] could not be determined.')
+            return None
+
+        create_time = round(int(snap["timestamp"]) * 10**-3, 3)
+
+        if (self.since_time) and (create_time < self.since_time):
             print(
-                f'**Unknown Snap type detected!**\n\tID: {snap["id"]}\n\tSnap data: {json.dumps(snap)}\nPlease report this at {self.ISSUES_URL}\n'
+                f" - [{snap['id']}] is older than the specified time of [{self.since_time}]. Snap timestamp: [{int(create_time)}]. Skipping."
             )
             return None
-        url = snap["snapInfo"]["streamingMediaInfo"].get("mediaUrl")
-        if not url:
-            return None
-        data_dict["url"] = url
-        s = Snap(**data_dict)
-        if not self.all_snaps.get(snap["id"]):
-            self.all_snaps[snap["id"]] = s
+
+        s = Snap(
+            create_time=create_time,  # type: ignore
+            snap_id=snap["id"],
+            url=url,
+            file_type=file_type,
+            location=snap["snapInfo"]
+            .get("title", {})
+            .get(
+                "fallback",
+                snap["snapInfo"].get("localitySubtitle", {}).get("fallback", "UNKNOWN"),
+            ),
+        )
+
+        self.all_snaps[snap["id"]] = s
+
         return s
 
     def _get_epoch(self):
         epoch_endpoint = requests.post(
             "https://ms.sc-jpl.com/web/getLatestTileSet",
             headers={"Content-Type": "application/json"},
             json={},
         ).json()
+
         if epoch_endpoint:
             for entry in epoch_endpoint["tileSetInfos"]:
                 if entry["id"]["type"] == "HEAT":
                     return entry["id"]["epoch"]
         else:
             raise self.MissingEpochError(
-                f"The API epoch could not be obtained.\n\nPlease report this at {self.ISSUES_URL}"
+                f"The API epoch could not be obtained.\n\nPlease report this at [{ISSUES_URL}]."
             )
 
     class MissingEpochError(Exception):
         pass
```

### Comparing `snapmap-archiver-2.1.0/snapmap_archiver/__init__.py` & `snapmap_archiver-2.1.2/snapmap_archiver/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import argparse
 
 from snapmap_archiver.SnapmapArchiver import SnapmapArchiver
 
 
-USAGE_MSG = 'snapmap_archiver -o [OUTPUT DIR] -l="[LATITUDE],[LONGITUDE]"\n\nUse -h to display more options.'
-
-
 def main():
     parser = argparse.ArgumentParser(
-        description="Download content from Snapmaps", usage=USAGE_MSG
+        description="Download content from Snapmaps",
+        usage='snapmap_archiver -o [OUTPUT DIR] -l="[LATITUDE],[LONGITUDE]"\n\nUse -h to display more options.',
     )
     parser.add_argument(
         "-o",
         dest="output_dir",
         type=str,
         help="Output directory for downloaded content.",
     )
@@ -49,19 +47,28 @@
     parser.add_argument(
         "-f",
         "--file",
         dest="input_file",
         type=str,
         help="File containing line-separated Snap URLs or IDs",
     )
+    parser.add_argument(
+        "-t",
+        "--since-time",
+        dest="since_time",
+        type=str,
+        help="Remove any Snaps older than the passed time. Either a 10 digit UTC Unix timestamp or [n = number of][m = minutes | h = hours | d = days] (e.g., 1d, 15h, 30m).",
+        default=None,
+    )
     args, unknown = parser.parse_known_args()
 
     sm_archiver = SnapmapArchiver(
         *unknown,
         radius=args.radius,
         output_dir=args.output_dir,
-        locations=args.location,
+        locations=[location for location, in (args.location if args.location else [])],
         zoom_depth=args.zoom_depth,
         write_json=args.write_json,
         input_file=args.input_file,
+        since_time=args.since_time,
     )
     sm_archiver.main()
```

### Comparing `snapmap-archiver-2.1.0/snapmap_archiver/coordinates.py` & `snapmap_archiver-2.1.2/snapmap_archiver/coordinates.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,16 @@
 class Coordinates:
     def __init__(self, coord_str: str):
-        self.geo_msg = (
-            '\n\nUse comma seperated values for latitude/longitude, e.g: -l="35.0,67.0"'
-        )
-        if "," not in coord_str:
-            raise ValueError(
-                f"No comma is present in the provided coordinates.{self.geo_msg}"
-            )
         try:
             lat, long = coord_str.split(",", 1)
             self.lat = float(lat)
             self.long = float(long)
         except Exception:
             raise ValueError(
-                f"Provided coordinates could not be split to lat/long points.{self.geo_msg}"
+                f'Provided coordinates [{coord_str}] could not be split to lat/long points. Use comma seperated values for latitude/longitude, e.g: -l="35.0,67.0".'
             )
 
     def __str__(self) -> str:
         return f"Lat: {self.lat}, Lon: {self.long}"
 
     def __repr__(self) -> str:
         return f"({self.lat},{self.long})"
```

