# Comparing `tmp/mov_cli_youtube-1.2.0a3.tar.gz` & `tmp/mov_cli_youtube-1.2.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mov_cli_youtube-1.2.0a3.tar", last modified: Thu Apr 25 18:01:44 2024, max compression
+gzip compressed data, was "mov_cli_youtube-1.2.0a4.tar", last modified: Fri Apr 26 01:05:44 2024, max compression
```

## Comparing `mov_cli_youtube-1.2.0a3.tar` & `mov_cli_youtube-1.2.0a4.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-25 18:01:44.839696 mov_cli_youtube-1.2.0a3/
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1064 2024-03-04 22:22:29.000000 mov_cli_youtube-1.2.0a3/LICENSE
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2990 2024-04-25 18:01:44.839696 mov_cli_youtube-1.2.0a3/PKG-INFO
--rw-r--r--   0 goldy     (1000) goldy     (1000)      674 2024-03-21 15:27:20.000000 mov_cli_youtube-1.2.0a3/README.md
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-25 18:01:44.839696 mov_cli_youtube-1.2.0a3/mov_cli_youtube/
--rw-r--r--   0 goldy     (1000) goldy     (1000)      335 2024-04-25 18:01:37.000000 mov_cli_youtube-1.2.0a3/mov_cli_youtube/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     4403 2024-04-25 18:01:37.000000 mov_cli_youtube-1.2.0a3/mov_cli_youtube/youtube.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-25 18:01:44.839696 mov_cli_youtube-1.2.0a3/mov_cli_youtube.egg-info/
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2990 2024-04-25 18:01:44.000000 mov_cli_youtube-1.2.0a3/mov_cli_youtube.egg-info/PKG-INFO
--rw-r--r--   0 goldy     (1000) goldy     (1000)      281 2024-04-25 18:01:44.000000 mov_cli_youtube-1.2.0a3/mov_cli_youtube.egg-info/SOURCES.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)        1 2024-04-25 18:01:44.000000 mov_cli_youtube-1.2.0a3/mov_cli_youtube.egg-info/dependency_links.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)       97 2024-04-25 18:01:44.000000 mov_cli_youtube-1.2.0a3/mov_cli_youtube.egg-info/requires.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)       16 2024-04-25 18:01:44.000000 mov_cli_youtube-1.2.0a3/mov_cli_youtube.egg-info/top_level.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1295 2024-04-16 20:20:33.000000 mov_cli_youtube-1.2.0a3/pyproject.toml
--rw-r--r--   0 goldy     (1000) goldy     (1000)       38 2024-04-25 18:01:44.839696 mov_cli_youtube-1.2.0a3/setup.cfg
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-26 01:05:44.834520 mov_cli_youtube-1.2.0a4/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1064 2024-03-04 22:22:29.000000 mov_cli_youtube-1.2.0a4/LICENSE
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2990 2024-04-26 01:05:44.834520 mov_cli_youtube-1.2.0a4/PKG-INFO
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      674 2024-03-21 15:27:20.000000 mov_cli_youtube-1.2.0a4/README.md
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-26 01:05:44.834520 mov_cli_youtube-1.2.0a4/mov_cli_youtube/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      656 2024-04-26 00:59:40.000000 mov_cli_youtube-1.2.0a4/mov_cli_youtube/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2526 2024-04-26 00:35:08.000000 mov_cli_youtube-1.2.0a4/mov_cli_youtube/pytube.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     3765 2024-04-26 01:01:35.000000 mov_cli_youtube-1.2.0a4/mov_cli_youtube/yt_dlp.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-26 01:05:44.834520 mov_cli_youtube-1.2.0a4/mov_cli_youtube.egg-info/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2990 2024-04-26 01:05:44.000000 mov_cli_youtube-1.2.0a4/mov_cli_youtube.egg-info/PKG-INFO
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      306 2024-04-26 01:05:44.000000 mov_cli_youtube-1.2.0a4/mov_cli_youtube.egg-info/SOURCES.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)        1 2024-04-26 01:05:44.000000 mov_cli_youtube-1.2.0a4/mov_cli_youtube.egg-info/dependency_links.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       97 2024-04-26 01:05:44.000000 mov_cli_youtube-1.2.0a4/mov_cli_youtube.egg-info/requires.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       16 2024-04-26 01:05:44.000000 mov_cli_youtube-1.2.0a4/mov_cli_youtube.egg-info/top_level.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1295 2024-04-26 00:34:40.000000 mov_cli_youtube-1.2.0a4/pyproject.toml
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       38 2024-04-26 01:05:44.834520 mov_cli_youtube-1.2.0a4/setup.cfg
```

### Comparing `mov_cli_youtube-1.2.0a3/LICENSE` & `mov_cli_youtube-1.2.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `mov_cli_youtube-1.2.0a3/PKG-INFO` & `mov_cli_youtube-1.2.0a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mov-cli-youtube
-Version: 1.2.0a3
+Version: 1.2.0a4
 Summary: A mov-cli v4 plugin for watching youtube.
 Author-email: Goldy <goldy@devgoldy.xyz>
 License: MIT License
         
         Copyright (c) 2024 mov-cli
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `mov_cli_youtube-1.2.0a3/README.md` & `mov_cli_youtube-1.2.0a4/README.md`

 * *Files identical despite different names*

### Comparing `mov_cli_youtube-1.2.0a3/mov_cli_youtube/youtube.py` & `mov_cli_youtube-1.2.0a4/mov_cli_youtube/yt_dlp.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,27 @@
     from typing import Optional, Dict, Generator, Any, List, Tuple
 
     from mov_cli import Config
     from mov_cli.http_client import HTTPClient
     from mov_cli.scraper import ScraperOptionsT
 
 import yt_dlp
-from pytube import YouTube
 
 from mov_cli.scraper import Scraper
-from mov_cli.utils import EpisodeSelector, what_platform
+from mov_cli.utils import EpisodeSelector
 from mov_cli import Single, Metadata, MetadataType
 
-__all__ = ("YouTubeScraper",)
+__all__ = ("YTDlpScraper",)
 
-class YouTubeScraper(Scraper):
+class YTDlpScraper(Scraper):
     def __init__(self, config: Config, http_client: HTTPClient, options: Optional[ScraperOptionsT] = None) -> None:
         super().__init__(config, http_client, options)
 
     def search(self, query: str, limit: Optional[int] = None) -> Generator[Metadata, Any, None]:
-        max_videos = 100 if limit is None else limit
+        max_videos = 70 if limit is None else limit
 
         yt_options = {
             "noplaylist": "True", 
             "default_search": "ytsearch", 
             "nocheckcertificate": True, 
             "geo_bypass": True, 
             "extract_flat": "in_playlist", 
@@ -58,37 +57,24 @@
         yt_options = {
             "format": "best", 
             "nocheckcertificate": True, 
             "geo_bypass": True, 
             "quiet": False if self.config.debug else True
         }
 
-        platform = what_platform()
-
         audio_url = None
 
-        if not platform == "Android" and not platform == "iOS":
-
-            with yt_dlp.YoutubeDL(yt_options) as ydl:
-                info = ydl.extract_info(watch_url, download = False)
-
-                if self.options.get("audio", False):
-                    url = self.__get_best_stream(info, audio = True)
-                else:
-                    url = self.__get_best_stream(info, video = True)
-                    audio_url = self.__get_best_stream(info, audio = True)
-
-        else: # Fall back to pytube on iOS and Android as their players can't take audio_url. 
-            # Sadly this will result in lower resolution as pytube doesn't seem to pick up higher resolutions well.
-            pytube_video = YouTube(watch_url)
+        with yt_dlp.YoutubeDL(yt_options) as ydl:
+            info = ydl.extract_info(watch_url, download = False)
 
             if self.options.get("audio", False):
-                url = pytube_video.streams.get_audio_only().url
+                url = self.__get_best_stream(info, audio = True)
             else:
-                url = pytube_video.streams.get_highest_resolution().url
+                url = self.__get_best_stream(info, video = True)
+                audio_url = self.__get_best_stream(info, audio = True)
 
         return Single(
             url = url, 
             audio_url = audio_url, 
             title = metadata.title, 
             year = metadata.year
         )
```

### Comparing `mov_cli_youtube-1.2.0a3/mov_cli_youtube.egg-info/PKG-INFO` & `mov_cli_youtube-1.2.0a4/mov_cli_youtube.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mov-cli-youtube
-Version: 1.2.0a3
+Version: 1.2.0a4
 Summary: A mov-cli v4 plugin for watching youtube.
 Author-email: Goldy <goldy@devgoldy.xyz>
 License: MIT License
         
         Copyright (c) 2024 mov-cli
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `mov_cli_youtube-1.2.0a3/pyproject.toml` & `mov_cli_youtube-1.2.0a4/pyproject.toml`

 * *Files identical despite different names*

