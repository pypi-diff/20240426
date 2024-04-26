# Comparing `tmp/mov-cli-files-1.0.3.tar.gz` & `tmp/mov_cli_files-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mov-cli-files-1.0.3.tar", last modified: Fri Apr  5 21:01:56 2024, max compression
+gzip compressed data, was "mov_cli_files-1.1.0.tar", last modified: Fri Apr 26 01:21:43 2024, max compression
```

## Comparing `mov-cli-files-1.0.3.tar` & `mov_cli_files-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 21:01:56.341027 mov-cli-files-1.0.3/
--rw-rw-rw-   0        0        0     1085 2024-04-05 05:34:53.000000 mov-cli-files-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     2970 2024-04-05 21:01:56.339026 mov-cli-files-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      574 2024-04-05 05:55:40.000000 mov-cli-files-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-05 21:01:56.308019 mov-cli-files-1.0.3/mov_cli_files/
--rw-rw-rw-   0        0        0      351 2024-04-05 21:01:29.000000 mov-cli-files-1.0.3/mov_cli_files/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 21:01:56.336026 mov-cli-files-1.0.3/mov_cli_files/files/
--rw-rw-rw-   0        0        0       22 2024-03-21 12:20:57.000000 mov-cli-files-1.0.3/mov_cli_files/files/__init__.py
--rw-rw-rw-   0        0        0     2419 2024-04-05 18:31:09.000000 mov-cli-files-1.0.3/mov_cli_files/files/scraper.py
-drwxrwxrwx   0        0        0        0 2024-04-05 21:01:56.337026 mov-cli-files-1.0.3/mov_cli_files.egg-info/
--rw-rw-rw-   0        0        0     2970 2024-04-05 21:01:56.000000 mov-cli-files-1.0.3/mov_cli_files.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2024-04-05 21:01:56.000000 mov-cli-files-1.0.3/mov_cli_files.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 21:01:56.000000 mov-cli-files-1.0.3/mov_cli_files.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       81 2024-04-05 21:01:56.000000 mov-cli-files-1.0.3/mov_cli_files.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-05 21:01:56.000000 mov-cli-files-1.0.3/mov_cli_files.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1377 2024-04-05 05:41:14.000000 mov-cli-files-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-05 21:01:56.341027 mov-cli-files-1.0.3/setup.cfg
+drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-04-26 01:21:43.863646 mov_cli_files-1.1.0/
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     1064 2024-04-26 01:21:34.000000 mov_cli_files-1.1.0/LICENSE
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     2921 2024-04-26 01:21:43.863646 mov_cli_files-1.1.0/PKG-INFO
+-rw-r--r--   0 ananas    (1000) ananas    (1000)      544 2024-04-26 01:21:34.000000 mov_cli_files-1.1.0/README.md
+drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-04-26 01:21:43.863646 mov_cli_files-1.1.0/mov_cli_files/
+-rw-r--r--   0 ananas    (1000) ananas    (1000)      296 2024-04-26 01:21:34.000000 mov_cli_files-1.1.0/mov_cli_files/__init__.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)      987 2024-04-26 01:21:34.000000 mov_cli_files-1.1.0/mov_cli_files/paths.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     3011 2024-04-26 01:21:34.000000 mov_cli_files-1.1.0/mov_cli_files/scraper.py
+drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-04-26 01:21:43.863646 mov_cli_files-1.1.0/mov_cli_files.egg-info/
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     2921 2024-04-26 01:21:43.000000 mov_cli_files-1.1.0/mov_cli_files.egg-info/PKG-INFO
+-rw-r--r--   0 ananas    (1000) ananas    (1000)      290 2024-04-26 01:21:43.000000 mov_cli_files-1.1.0/mov_cli_files.egg-info/SOURCES.txt
+-rw-r--r--   0 ananas    (1000) ananas    (1000)        1 2024-04-26 01:21:43.000000 mov_cli_files-1.1.0/mov_cli_files.egg-info/dependency_links.txt
+-rw-r--r--   0 ananas    (1000) ananas    (1000)       96 2024-04-26 01:21:43.000000 mov_cli_files-1.1.0/mov_cli_files.egg-info/requires.txt
+-rw-r--r--   0 ananas    (1000) ananas    (1000)       14 2024-04-26 01:21:43.000000 mov_cli_files-1.1.0/mov_cli_files.egg-info/top_level.txt
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     1349 2024-04-26 01:21:34.000000 mov_cli_files-1.1.0/pyproject.toml
+-rw-r--r--   0 ananas    (1000) ananas    (1000)       38 2024-04-26 01:21:43.863646 mov_cli_files-1.1.0/setup.cfg
```

### Comparing `mov-cli-files-1.0.3/PKG-INFO` & `mov_cli_files-1.1.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,79 +1,80 @@
-Metadata-Version: 2.1
-Name: mov-cli-files
-Version: 1.0.3
-Summary:  A mov-cli v4 plugin for watching files on your device.
-Author-email: Ananas <ananas@r3tr0ananas.lol>
-License: MIT License
-        
-        Copyright (c) 2024 mov-cli
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: GitHub, https://github.com/mov-cli/mov-cli-files
-Project-URL: BugTracker, https://github.com/mov-cli/mov-cli-files/issues
-Keywords: amazing mov-cli plugin
-Classifier: Operating System :: Microsoft :: Windows :: Windows 11
-Classifier: Operating System :: Microsoft :: Windows :: Windows 10
-Classifier: Operating System :: POSIX :: Linux
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests
-Requires-Dist: importlib-metadata; python_version < "3.8"
-Requires-Dist: mov-cli
-Provides-Extra: dev
-Requires-Dist: ruff; extra == "dev"
-Requires-Dist: build; extra == "dev"
-
-<div align="center">
-
-  # mov-cli-files 
-  <sub>A mov-cli v4 plugin for watching files on your device.</sub>
-  
-  ![grafik](https://github.com/mov-cli/mov-cli-files/assets/132799819/5f25ac19-de39-4b26-8121-c0f58f167c6b)
-
-</div>
-
-
-## Installation 🛠️
-Here's how to install and add the plugin to mov-cli.
-
-1. Install the pip package.
-```sh
-pip install mov-cli-files
-```
-2. Then add the plugin to your mov-cli config.
-```sh
-mov-cli -e
-```
-```toml
-[mov-cli.plugins]
-files = "mov-cli-files"
-```
-
-## Usage 🖱️
-```sh
-mov-cli -s files PATH
-```
+Metadata-Version: 2.1
+Name: mov-cli-files
+Version: 1.1.0
+Summary:  A mov-cli v4 plugin for watching files on your device.
+Author-email: Ananas <ananas@r3tr0ananas.lol>
+License: MIT License
+        
+        Copyright (c) 2024 mov-cli
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: GitHub, https://github.com/mov-cli/mov-cli-files
+Project-URL: BugTracker, https://github.com/mov-cli/mov-cli-files/issues
+Keywords: amazing mov-cli plugin
+Classifier: Operating System :: Microsoft :: Windows :: Windows 11
+Classifier: Operating System :: Microsoft :: Windows :: Windows 10
+Classifier: Operating System :: POSIX :: Linux
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: importlib-metadata; python_version < "3.8"
+Requires-Dist: mov-cli>=4.3.0
+Requires-Dist: thefuzz
+Provides-Extra: dev
+Requires-Dist: ruff; extra == "dev"
+Requires-Dist: build; extra == "dev"
+
+<div align="center">
+
+  # mov-cli-files 
+  <sub>A mov-cli v4 plugin for watching files on your device.</sub>
+  
+  ![grafik](https://github.com/mov-cli/mov-cli-files/assets/132799819/5f25ac19-de39-4b26-8121-c0f58f167c6b)
+
+</div>
+
+
+## Installation 🛠️
+Here's how to install and add the plugin to mov-cli.
+
+1. Install the pip package.
+```sh
+pip install mov-cli-files
+```
+2. Then add the plugin to your mov-cli config.
+```sh
+mov-cli -e
+```
+```toml
+[mov-cli.plugins]
+files = "mov-cli-files"
+```
+
+## Usage 🖱️
+```sh
+mov-cli -s files PATH
+```
```

### Comparing `mov-cli-files-1.0.3/mov_cli_files/files/scraper.py` & `mov_cli_files-1.1.0/mov_cli_files/scraper.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,54 +1,72 @@
-from __future__ import annotations
-from typing import TYPE_CHECKING
-
-if TYPE_CHECKING:
-    from typing import Generator, Any, Dict, Optional, List
-    from mov_cli import Config
-    from mov_cli.http_client import HTTPClient
-
-from mov_cli import utils
-from mov_cli.scraper import Scraper
-from mov_cli import Single, Metadata, MetadataType
-
-from datetime import datetime
-from pathlib import Path
-
-__all__ = ("FilesScraper", )
-
-video_extensions = [".3g2", ".3ga", ".3gp", ".3gpp", ".aac", ".ac3", ".adt", ".adts", ".aif", ".aifc", ".aiff", ".amr", ".asf", ".asx", ".av", ".avi", ".bmp", ".cue", ".dat", ".divx", ".dv", ".dvr-ms", ".eac3", ".evo", ".f4v", ".flac", ".flc", ".fli", ".flv", ".gif", ".gsm", ".ifo", ".ismv", ".ivf", ".m1v", ".m2p", ".m2t", ".m2ts", ".m2v", ".m3u", ".m4a", ".m4b", ".m4p", ".m4v", ".mk3d", ".mkv", ".mod", ".mov", ".mp2", ".mp2v", ".mp3", ".mp4", ".mp4v", ".mpe", ".mpeg", ".mpeg1", ".mpeg2", ".mpeg4", ".mpg", ".mpg2", ".mpv", ".mts", ".mxf", ".nsv", ".nuv", ".oga", ".ogg", ".ogm", ".ogv", ".ogx", ".oma", ".opus", ".pva", ".qt", ".ra", ".ram", ".rm", ".rmvb", ".s3m", ".sdp", ".spx", ".thd", ".tivo", ".tod", ".tp", ".ts", ".tta", ".vob", ".voc", ".vqf", ".w64", ".wav", ".webm", ".wma", ".wmv", ".wv", ".xesc", ".xspf"]
-
-class FilesScraper(Scraper):
-    def __init__(self, config: Config, http_client: HTTPClient) -> None:
-        self.base_url = None
-        super().__init__(config, http_client)
-
-    def search(self, query, **kwargs) -> Generator[Metadata, Any, None]:
-        query = Path(query)
-
-        for path in query.glob("**/*"):
-            if path.suffix not in video_extensions:
-                continue
-
-            st_ctime = path.stat().st_ctime
-
-            create_datetime = datetime.fromtimestamp(st_ctime)
-
-            year = create_datetime.strftime("%Y")
-
-            yield Metadata(
-                id = str(path), 
-                title = path.stem, 
-                type = MetadataType.MOVIE, 
-                year = year
-            )
-
-    def scrape(self, metadata: Metadata, episode: Optional[utils.EpisodeSelector] = None) -> Single:
-        return Single(
-            url = metadata.id, 
-            title = metadata.title, 
-            referrer = None, 
-            year = metadata.year 
-        )
-
-    def scrape_episodes(self, metadata: Metadata, **kwargs) -> Dict[None, int]:
+from __future__ import annotations
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from typing import Dict, Optional, Generator, Any
+    from mov_cli import Config
+
+    from mov_cli.utils import EpisodeSelector
+    from mov_cli.http_client import HTTPClient
+    from mov_cli.scraper import ScraperOptionsT
+
+from mov_cli.scraper import Scraper
+from mov_cli.utils import what_platform
+from mov_cli import Single, Metadata, MetadataType
+
+from thefuzz import fuzz
+from datetime import datetime
+
+from .paths import get_user_media_paths
+from pathlib import Path
+
+__all__ = ("FilesScraper",)
+
+video_extensions = [".3g2", ".3ga", ".3gp", ".3gpp", ".aac", ".ac3", ".adt", ".adts", ".aif", ".aifc", ".aiff", ".amr", ".asf", ".asx", ".av", ".avi", ".bmp", ".cue", ".dat", ".divx", ".dv", ".dvr-ms", ".eac3", ".evo", ".f4v", ".flac", ".flc", ".fli", ".flv", ".gif", ".gsm", ".ifo", ".ismv", ".ivf", ".m1v", ".m2p", ".m2t", ".m2ts", ".m2v", ".m3u", ".m4a", ".m4b", ".m4p", ".m4v", ".mk3d", ".mkv", ".mod", ".mov", ".mp2", ".mp2v", ".mp3", ".mp4", ".mp4v", ".mpe", ".mpeg", ".mpeg1", ".mpeg2", ".mpeg4", ".mpg", ".mpg2", ".mpv", ".mts", ".mxf", ".nsv", ".nuv", ".oga", ".ogg", ".ogm", ".ogv", ".ogx", ".oma", ".opus", ".pva", ".qt", ".ra", ".ram", ".rm", ".rmvb", ".s3m", ".sdp", ".spx", ".thd", ".tivo", ".tod", ".tp", ".ts", ".tta", ".vob", ".voc", ".vqf", ".w64", ".wav", ".webm", ".wma", ".wmv", ".wv", ".xesc", ".xspf"]
+
+class FilesScraper(Scraper):
+    def __init__(self, config: Config, http_client: HTTPClient, options: Optional[ScraperOptionsT] = None) -> None:
+        self.platform = what_platform()
+        super().__init__(config, http_client, options)
+
+    def search(self, query: str, _: int = 20) -> Generator[Metadata, Any, None]:
+        options_path = self.options.get("path", None)
+        media_paths = get_user_media_paths(self.platform)
+
+        if options_path is not None:
+            options_path = Path(options_path)
+
+            if options_path.exists():
+                media_paths = [options_path]
+
+        for media_path in media_paths:
+            paths = media_path.glob("**/*")
+
+            for path in paths:
+                if fuzz.token_set_ratio(path.name, query) < 30 and query != "*":
+                    continue
+
+                if path.suffix not in video_extensions:
+                    continue
+
+                st_ctime = path.stat().st_ctime
+
+                create_datetime = datetime.fromtimestamp(st_ctime)
+
+                year = create_datetime.strftime("%Y")
+
+                yield Metadata(
+                    id = str(path), 
+                    title = path.stem, 
+                    type = MetadataType.MOVIE, 
+                    year = year
+                )
+
+    def scrape(self, metadata: Metadata, _: EpisodeSelector) -> Single:
+        return Single(
+            url = metadata.id, 
+            title = metadata.title, 
+            year = metadata.year 
+        )
+
+    def scrape_episodes(self, _: Metadata) -> Dict[None, int]:
         return {None: 1}
```

### Comparing `mov-cli-files-1.0.3/mov_cli_files.egg-info/PKG-INFO` & `mov_cli_files-1.1.0/mov_cli_files.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,79 +1,80 @@
-Metadata-Version: 2.1
-Name: mov-cli-files
-Version: 1.0.3
-Summary:  A mov-cli v4 plugin for watching files on your device.
-Author-email: Ananas <ananas@r3tr0ananas.lol>
-License: MIT License
-        
-        Copyright (c) 2024 mov-cli
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: GitHub, https://github.com/mov-cli/mov-cli-files
-Project-URL: BugTracker, https://github.com/mov-cli/mov-cli-files/issues
-Keywords: amazing mov-cli plugin
-Classifier: Operating System :: Microsoft :: Windows :: Windows 11
-Classifier: Operating System :: Microsoft :: Windows :: Windows 10
-Classifier: Operating System :: POSIX :: Linux
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests
-Requires-Dist: importlib-metadata; python_version < "3.8"
-Requires-Dist: mov-cli
-Provides-Extra: dev
-Requires-Dist: ruff; extra == "dev"
-Requires-Dist: build; extra == "dev"
-
-<div align="center">
-
-  # mov-cli-files 
-  <sub>A mov-cli v4 plugin for watching files on your device.</sub>
-  
-  ![grafik](https://github.com/mov-cli/mov-cli-files/assets/132799819/5f25ac19-de39-4b26-8121-c0f58f167c6b)
-
-</div>
-
-
-## Installation 🛠️
-Here's how to install and add the plugin to mov-cli.
-
-1. Install the pip package.
-```sh
-pip install mov-cli-files
-```
-2. Then add the plugin to your mov-cli config.
-```sh
-mov-cli -e
-```
-```toml
-[mov-cli.plugins]
-files = "mov-cli-files"
-```
-
-## Usage 🖱️
-```sh
-mov-cli -s files PATH
-```
+Metadata-Version: 2.1
+Name: mov-cli-files
+Version: 1.1.0
+Summary:  A mov-cli v4 plugin for watching files on your device.
+Author-email: Ananas <ananas@r3tr0ananas.lol>
+License: MIT License
+        
+        Copyright (c) 2024 mov-cli
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: GitHub, https://github.com/mov-cli/mov-cli-files
+Project-URL: BugTracker, https://github.com/mov-cli/mov-cli-files/issues
+Keywords: amazing mov-cli plugin
+Classifier: Operating System :: Microsoft :: Windows :: Windows 11
+Classifier: Operating System :: Microsoft :: Windows :: Windows 10
+Classifier: Operating System :: POSIX :: Linux
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: importlib-metadata; python_version < "3.8"
+Requires-Dist: mov-cli>=4.3.0
+Requires-Dist: thefuzz
+Provides-Extra: dev
+Requires-Dist: ruff; extra == "dev"
+Requires-Dist: build; extra == "dev"
+
+<div align="center">
+
+  # mov-cli-files 
+  <sub>A mov-cli v4 plugin for watching files on your device.</sub>
+  
+  ![grafik](https://github.com/mov-cli/mov-cli-files/assets/132799819/5f25ac19-de39-4b26-8121-c0f58f167c6b)
+
+</div>
+
+
+## Installation 🛠️
+Here's how to install and add the plugin to mov-cli.
+
+1. Install the pip package.
+```sh
+pip install mov-cli-files
+```
+2. Then add the plugin to your mov-cli config.
+```sh
+mov-cli -e
+```
+```toml
+[mov-cli.plugins]
+files = "mov-cli-files"
+```
+
+## Usage 🖱️
+```sh
+mov-cli -s files PATH
+```
```

### Comparing `mov-cli-files-1.0.3/pyproject.toml` & `mov_cli_files-1.1.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,51 +1,52 @@
-[project]
-name = "mov-cli-files"
-description = " A mov-cli v4 plugin for watching files on your device."
-authors = [
-    {name = "Ananas", email = "ananas@r3tr0ananas.lol"}
-]
-readme = {file = "README.md", content-type = "text/markdown"}
-requires-python = ">=3.8"
-license = { file = "LICENSE" }
-keywords = [
-    "amazing mov-cli plugin"
-]
-classifiers = [
-	'Operating System :: Microsoft :: Windows :: Windows 11',
-    'Operating System :: Microsoft :: Windows :: Windows 10',
-    'Operating System :: POSIX :: Linux',
-    'License :: OSI Approved :: MIT License',
-    'Programming Language :: Python :: 3.8',
-    'Programming Language :: Python :: 3.9',
-    'Programming Language :: Python :: 3.10',
-	'Programming Language :: Python :: 3.11',
-    "Programming Language :: Python :: 3.12"
-]
-dependencies = [
-    "requests",
-    "importlib-metadata; python_version<'3.8'",
-
-    "mov-cli"
-]
-
-dynamic = ["version"]
-
-[project.optional-dependencies]
-dev = [
-    "ruff",
-    "build"
-]
-
-[project.urls]
-GitHub = "https://github.com/mov-cli/mov-cli-files"
-BugTracker = "https://github.com/mov-cli/mov-cli-files/issues"
-
-[tool.setuptools.dynamic]
-version = { attr = "mov_cli_files.__version__" }
-
-[build-system]
-requires = ["setuptools"]
-build-backend = "setuptools.build_meta"
-
-[tool.setuptools.packages.find]
+[project]
+name = "mov-cli-files"
+description = " A mov-cli v4 plugin for watching files on your device."
+authors = [
+    {name = "Ananas", email = "ananas@r3tr0ananas.lol"}
+]
+readme = {file = "README.md", content-type = "text/markdown"}
+requires-python = ">=3.8"
+license = { file = "LICENSE" }
+keywords = [
+    "amazing mov-cli plugin"
+]
+classifiers = [
+	'Operating System :: Microsoft :: Windows :: Windows 11',
+    'Operating System :: Microsoft :: Windows :: Windows 10',
+    'Operating System :: POSIX :: Linux',
+    'License :: OSI Approved :: MIT License',
+    'Programming Language :: Python :: 3.8',
+    'Programming Language :: Python :: 3.9',
+    'Programming Language :: Python :: 3.10',
+	'Programming Language :: Python :: 3.11',
+    "Programming Language :: Python :: 3.12"
+]
+dependencies = [
+    "requests",
+    "importlib-metadata; python_version<'3.8'",
+
+    "mov-cli>=4.3.0",
+    "thefuzz"
+]
+
+dynamic = ["version"]
+
+[project.optional-dependencies]
+dev = [
+    "ruff",
+    "build"
+]
+
+[project.urls]
+GitHub = "https://github.com/mov-cli/mov-cli-files"
+BugTracker = "https://github.com/mov-cli/mov-cli-files/issues"
+
+[tool.setuptools.dynamic]
+version = { attr = "mov_cli_files.__version__" }
+
+[build-system]
+requires = ["setuptools"]
+build-backend = "setuptools.build_meta"
+
+[tool.setuptools.packages.find]
 include = ["mov_cli_files*"]
```

