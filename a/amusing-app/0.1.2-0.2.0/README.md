# Comparing `tmp/amusing_app-0.1.2.tar.gz` & `tmp/amusing_app-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amusing_app-0.1.2.tar", max compression
+gzip compressed data, was "amusing_app-0.2.0.tar", max compression
```

## Comparing `amusing_app-0.1.2.tar` & `amusing_app-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,18 @@
--rw-r--r--   0        0        0    13168 2024-01-01 17:51:06.345184 amusing_app-0.1.2/README.md
--rw-r--r--   0        0        0       41 2024-01-01 17:51:06.345184 amusing_app-0.1.2/amusing/appconfig.example.yaml
--rw-r--r--   0        0        0     3607 2024-01-01 17:51:06.345184 amusing_app-0.1.2/amusing/cli.py
--rw-r--r--   0        0        0     4891 2024-01-01 17:51:06.345184 amusing_app-0.1.2/amusing/cli_operations.py
--rw-r--r--   0        0        0        0 2024-01-01 17:51:06.345184 amusing_app-0.1.2/amusing/core/__init__.py
--rw-r--r--   0        0        0      957 2024-01-01 17:51:06.345184 amusing_app-0.1.2/amusing/core/download.py
--rw-r--r--   0        0        0     5400 2024-01-01 17:51:06.345184 amusing_app-0.1.2/amusing/core/parse_csv.py
--rw-r--r--   0        0        0     2707 2024-01-01 17:51:06.345184 amusing_app-0.1.2/amusing/core/parse_xml.py
--rw-r--r--   0        0        0     1525 2024-01-01 17:51:06.345184 amusing_app-0.1.2/amusing/core/save_to_db.py
--rw-r--r--   0        0        0     1193 2024-01-01 17:51:06.345184 amusing_app-0.1.2/amusing/core/search.py
--rw-r--r--   0        0        0        0 2024-01-01 17:51:06.345184 amusing_app-0.1.2/amusing/db/__init__.py
--rw-r--r--   0        0        0      410 2024-01-01 17:51:06.345184 amusing_app-0.1.2/amusing/db/engine.py
--rw-r--r--   0        0        0      937 2024-01-01 17:51:06.345184 amusing_app-0.1.2/amusing/db/models.py
--rw-r--r--   0        0        0       85 2024-01-01 17:51:06.345184 amusing_app-0.1.2/amusing/scripts/README.md
--rw-r--r--   0        0        0     5347 2024-01-01 17:51:06.345184 amusing_app-0.1.2/amusing/scripts/am_download_all.py
--rw-r--r--   0        0        0     1920 2024-01-01 17:51:06.345184 amusing_app-0.1.2/amusing/scripts/am_parse.py
--rw-r--r--   0        0        0        0 2024-01-01 17:51:06.345184 amusing_app-0.1.2/amusing/utils/__init__.py
--rw-r--r--   0        0        0      975 2024-01-01 17:51:06.345184 amusing_app-0.1.2/amusing/utils/config.py
--rw-r--r--   0        0        0      359 2024-01-01 17:51:06.345184 amusing_app-0.1.2/amusing/utils/funcs.py
--rw-r--r--   0        0        0     1117 2024-01-01 17:51:06.349184 amusing_app-0.1.2/pyproject.toml
--rw-r--r--   0        0        0    14597 1970-01-01 00:00:00.000000 amusing_app-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    13996 2024-04-26 14:43:20.511980 amusing_app-0.2.0/README.md
+-rw-r--r--   0        0        0       41 2024-04-26 14:43:20.511980 amusing_app-0.2.0/amusing/appconfig.example.yaml
+-rw-r--r--   0        0        0     4129 2024-04-26 14:43:20.511980 amusing_app-0.2.0/amusing/cli.py
+-rw-r--r--   0        0        0     5799 2024-04-26 14:43:20.511980 amusing_app-0.2.0/amusing/cli_operations.py
+-rw-r--r--   0        0        0        0 2024-04-26 14:43:20.511980 amusing_app-0.2.0/amusing/core/__init__.py
+-rw-r--r--   0        0        0     5181 2024-04-26 14:43:20.511980 amusing_app-0.2.0/amusing/core/download.py
+-rw-r--r--   0        0        0     3715 2024-04-26 14:43:20.511980 amusing_app-0.2.0/amusing/core/parse_csv.py
+-rw-r--r--   0        0        0     2899 2024-04-26 14:43:20.511980 amusing_app-0.2.0/amusing/core/parse_xml.py
+-rw-r--r--   0        0        0     1529 2024-04-26 14:43:20.511980 amusing_app-0.2.0/amusing/core/save_to_db.py
+-rw-r--r--   0        0        0      929 2024-04-26 14:43:20.511980 amusing_app-0.2.0/amusing/core/search.py
+-rw-r--r--   0        0        0        0 2024-04-26 14:43:20.511980 amusing_app-0.2.0/amusing/db/__init__.py
+-rw-r--r--   0        0        0      410 2024-04-26 14:43:20.511980 amusing_app-0.2.0/amusing/db/engine.py
+-rw-r--r--   0        0        0     2275 2024-04-26 14:43:20.511980 amusing_app-0.2.0/amusing/db/models.py
+-rw-r--r--   0        0        0        0 2024-04-26 14:43:20.511980 amusing_app-0.2.0/amusing/utils/__init__.py
+-rw-r--r--   0        0        0     1453 2024-04-26 14:43:20.511980 amusing_app-0.2.0/amusing/utils/config.py
+-rw-r--r--   0        0        0      363 2024-04-26 14:43:20.511980 amusing_app-0.2.0/amusing/utils/funcs.py
+-rw-r--r--   0        0        0     1104 2024-04-26 14:43:20.515980 amusing_app-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    15411 1970-01-01 00:00:00.000000 amusing_app-0.2.0/PKG-INFO
```

### Comparing `amusing_app-0.1.2/README.md` & `amusing_app-0.2.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,118 +1,176 @@
-<h1> 🎧 Amusing 🎸 </h1>
+# 🎧 Amusing 🎸
 
-A CLI to help download music independently or from your exported apple music library.
+A CLI to download music independently and from your exported Apple Music library.
 
-## Why should you use <strong>Amusing</strong>?
+## Why should you use **Amusing**?
 
 - To download your entire Apple Music Library and store it locally in one go
 - To search and download individual songs from YouTube
 - To keep track of your ever growing music collection
 
-## 🛠️ Install it!
+## 📦 Install it!
 
-```console
-$ pip install amusing-app
+Install it as a [PyPI](https://pypi.org/) package:
+
+```
+pip install amusing-app
 ```
 
+You will also need [FFmpeg](https://ffmpeg.org/) installed, which is required to embed song metadata (title, artist, album, cover art, ...) in the audio file.
+
 ## ✨ Getting set up
 
 There are three things to know before moving on to the next section:
 
 - The CLI takes in a `appconfig.yaml` file similar to what's indicated in `appconfig.example.yaml`. You can simply rename it.
+
   The file looks like this:
 
   ```yaml
   root_download_path: "..."
   db_name: "..."
   ```
 
+  The file can be placed in two locations:
+  1. `~/Downloads/Amusing/appconfig.yaml`: default one. If the file is not found anywhere it will be created here.
+  2. `~/.config/amusing/appconfig.yaml`: only if the default one does not exist.
+
 - A dedicated sqlite database called `db_name` will be created in `root_download_path/db_name.db` to store two tables `Song` and `Album` as defined in `amusing/db/models.py`. All songs downloaded locally will be getting a row in the `Song` table and a row for their corresponding album in the `Album` table.
 - The songs are downloaded in `root_download_path/songs` directory.
 - That's it. You're done. Let's look at the commands available next.
 
 ## 💬 Available commands
 
-There are currently 6 commands available, excluding the `amusing --version`.
+There are currently 7 commands available, excluding the `amusing --version`.
 
-The first time you run a command (eg. --help), an `Amusing` directory will be created in your `pathlib.Path.home()/Downloads` folder. For eg., on MacOS, it's in `/Users/Username/Downloads`.
+The first time you run a command (eg. `--help`), an `Amusing` directory will be created in the `~/Downloads` folder.
+For eg., on MacOS, it's in `/Users/Username/Downloads`.
 
 ```console
 $ amusing --help
 
- Created a new config file: /Users/username/Downloads/Amusing/appconfig.yaml
-
  Usage: amusing [OPTIONS] COMMAND [ARGS]...
 
- Amusing CLI to help download music independently or from your exported apple music library.
+ CLI to download music independently and from your exported Apple Music library.
+
+╭─ Options ─────────────────────────────────────────────────────────────────────╮
+│ --version  -v                                                                 │
+│ --help               Show this message and exit.                              │
+╰───────────────────────────────────────────────────────────────────────────────╯
+╭─ Commands ────────────────────────────────────────────────────────────────────╮
+│ download           Download the entire DB library.                            │
+│ parse              Parse the entire Apple Music library and make/update the   │
+│                    DB as needed.                                              │
+│ showsimilar        Look up the db and show if similar/exact song(s) are       │
+│                    found.                                                     │
+│ showsimilaralbum   Look up the db and show albums similar to the album        │
+│                    searched.                                                  │
+│ showsimilarartist  Look up the db and show songs for similar/exact artist     │
+│                    searched.                                                  │
+│ song               Search and download the song and add it to the db. Creates │
+│                    a new album if not already present.                        │
+╰───────────────────────────────────────────────────────────────────────────────╯
+```
+
+<details>
 
-╭─ Options ──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
-│ --version  -v                                                                                                                                  │
-│ --help               Show this message and exit.                                                                                               │
-╰────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
-╭─ Commands ─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
-│ download           Parse the entire AM library and download songs and make/update the db as needed.                                            │
-│ showsimilar        Look up the db and show if similar/exact song(s) are found.                                                                 │
-│ showsimilaralbum   Look up the db and show albums similar to the album searched.                                                               │
-│ showsimilarartist  Look up the db and show songs for similar/exact artist searched.                                                            │
-│ song               Search and download the song and add it to the db. Use --force to overwrite the existing song in the db. Creates a new      │
-│                    album if not already present.                                                                                               │
-╰────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+<summary><h3>Parse an exported `Library.xml` file from your Apple Music account</h3></summary>
 
+You can also use a previously parsed `Library.csv`, that already contains mappings with YouTube video IDs and possible URLs to download custom album artworks.
 
+```console
+$ amusing parse --help
+
+ Usage: amusing parse [OPTIONS] LIBRARY_PATH
+
+ Parse the entire Apple Music library and make/update the DB as needed.
+
+╭─ Arguments ───────────────────────────────────────────────────────────────────╮
+│ *    library_path      TEXT  The path to the 'Library.xml' or 'Library.csv'   │
+│                              exported from Apple Music.                       │
+│                              [default: None]                                  │
+│                              [required]                                       │
+╰───────────────────────────────────────────────────────────────────────────────╯
+╭─ Options ─────────────────────────────────────────────────────────────────────╮
+│ --help          Show this message and exit.                                   │
+╰───────────────────────────────────────────────────────────────────────────────╯
+
+# Example
+$ amusing parse 'your/path/to/Library.xml'
 ```
 
-### To parse an exported `Library.xml` file from your Apple Music account, use:
+</details>
+
+
+<details>
+
+<summary><h3>Download the entire exported Apple Music library</h3></summary>
+
+You can also pass a `Library.xml` or `Library.csv` file to parse before downloading the songs.
 
 ```console
 $ amusing download --help
 
- Usage: amusing download [OPTIONS] [PATH]
+ Usage: amusing download [OPTIONS] [LIBRARY_PATH]
 
- Parse the entire AM library and download songs and make/update the db as needed.
+ Download the entire DB library.
+ If passed, parse the library and update the DB before download.
 
-╭─ Arguments ────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
-│   path      [PATH]  The path to the Library.xml exported from Apple Music. [default: ./Library.xml]                                            │
-╰────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
-╭─ Options ──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
-│ --help          Show this message and exit.                                                                                                    │
-╰────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Arguments ───────────────────────────────────────────────────────────────────╮
+│   library_path      [LIBRARY_PATH]  The path to the 'Library.xml' or          │
+│                                     'Library.csv' exported from Apple Music.  │
+╰───────────────────────────────────────────────────────────────────────────────╯
+╭─ Options ─────────────────────────────────────────────────────────────────────╮
+│ --help          Show this message and exit.                                   │
+╰───────────────────────────────────────────────────────────────────────────────╯
 
 # Example
-$ amusing download "your/path/to/Library.xml"
+$ amusing download 'your/path/to/Library.xml'
 
+# Is equivalent to run
+$ amusing parse 'your/path/to/Library.xml'
+$ amusing download
 ```
 
-### To download a song individually, use:
+</details>
+
+
+<details>
+
+<summary><h3>Download an individual song</h3></summary>
 
 ```console
 $ amusing song --help
 
  Usage: amusing song [OPTIONS] NAME ARTIST ALBUM
 
- Search and download the song and add it to the db. Use --force to overwrite the existing song in the db. Creates a new album if not already
- present.
-
-╭─ Arguments ────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
-│ *    name        TEXT  Name of the song. [default: None] [required]                                                                            │
-│ *    artist      TEXT  Aritst of the song. [default: None] [required]                                                                          │
-│ *    album       TEXT  Album the song belongs to. [default: None] [required]                                                                   │
-╰────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
-╭─ Options ──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
-│ --force    --no-force      Overwrite the song if present. [default: no-force]                                                                  │
-│ --help                     Show this message and exit.                                                                                         │
-╰────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+ Search and download the song and add it to the db. Creates a new album if not
+ already present.
 
+╭─ Arguments ───────────────────────────────────────────────────────────────────╮
+│ *    name        TEXT  Name of the song. [default: None] [required]           │
+│ *    artist      TEXT  Aritst of the song. [default: None] [required]         │
+│ *    album       TEXT  Album the song belongs to. [default: None] [required]  │
+╰───────────────────────────────────────────────────────────────────────────────╯
+╭─ Options ─────────────────────────────────────────────────────────────────────╮
+│ --force    --no-force      Overwrite the song if present. [default: no-force] │
+│ --help                     Show this message and exit.                        │
+╰───────────────────────────────────────────────────────────────────────────────╯
 
 # Example, the search keywords need not be exact of course:
 $ amusing song "Run" "One Republic" "Human"
-
 ```
 
-### Search for a similar song, album or artist in your db/downloads:
+</details>
+
+
+<details>
+
+<summary><h3>Search for a similar song, album or artist in your DB/downloads</h3></summary>
 
 ```console
 $ amusing showsimilar "Someday"
 
 Song to look up:  someday
 ┏━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┓
 ┃ Song                 ┃ Artist        ┃ Album                                ┃
@@ -133,22 +191,48 @@
 │ No Vacancy      │ OneRepublic │ No Vacancy - Single                               │
 │ RUNAWAY         │ OneRepublic │ RUNAWAY - Single                                  │
 │ Sunshine        │ OneRepublic │ Sunshine - Single                                 │
 │ I Ain't Worried │ OneRepublic │ Top Gun: Maverick (Music from the Motion Picture) │
 │ West Coast      │ OneRepublic │ West Coast - Single                               │
 └─────────────────┴─────────────┴───────────────────────────────────────────────────┘
 
+
 $ amusing showsimilaralbum "Human"
 
 Album to look up:  Human
 ┏━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━┓
 ┃ Album          ┃ Number of songs ┃
 ┡━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━┩
 │ Human (Deluxe) │ 2               │
 └────────────────┴─────────────────┘
-
 ```
 
-## TODO 📝
+</details>
+
+
+## 🛠️ Library customization
+
+The resulting `Library.csv` file will be automatically updated by Amusing at every DB change.
+
+You can manually modify it to change which YouTube video to download for a specific song.
+You can also add a custom URL to download a specific album artwork.
+
+Here are some great tools you can use to find album artworks:
+- [Ben Dodson's iTunes Artwork Finder](https://bendodson.com/projects/itunes-artwork-finder/)
+- [Ben Dodson's Apple Music Artwork Finder](https://bendodson.com/projects/apple-music-artwork-finder)
+
+Copy the image link into your CSV file and Amusing will download it and embed it into your song the next time you run `amusing download '/path/to/Library.csv'`!
+
+
+## 📝 TODO
 
 1. Provide an option to choose which searched result is downloaded.
 2. Provide a command to show all songs in an album
+3. Provide a command to download a song from youtube link
+4. Better metadata availability (Musicbrainz, Discog etc)
+5. Coverarts (Musicbrainz, somewhere else?)
+6. Lyrics!
+7. Export playlists from Apple Music
+8. Look at which music player to integrate with, make changes to architecture of the library accordingly. The Music player needs to have:
+   - Aesthetic UI, intuitive UX similar to Apple Music or Spotify
+   - Play count, gapless playback, fade-in-out playback
+   - Docker compose support
```

### Comparing `amusing_app-0.1.2/amusing/cli.py` & `amusing_app-0.2.0/amusing/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,22 +4,23 @@
 import typer
 from rich.console import Console
 from rich.table import Table
 
 from amusing.cli_operations import (
     download_song_operation,
     parse_library_operation,
+    download_library_operation,
     show_similar_albums_in_db_operation,
     show_similar_songs_for_artist_in_db_operation,
     show_similar_songs_in_db_operation,
 )
 from amusing.utils.config import APP_CONFIG
 
 app = typer.Typer(
-    help="Amusing CLI to help download music independently or from your exported apple music library.",
+    help="CLI to download music independently and from your exported Apple Music library.",
     add_completion=False,
 )
 __version__ = metadata.version("amusing-app")
 
 
 def version_callback(value: bool) -> None:
     if value:
@@ -37,34 +38,54 @@
 @app.command("song")
 def download_song(
     name: Annotated[str, typer.Argument(help="Name of the song.")],
     artist: Annotated[str, typer.Argument(help="Aritst of the song.")],
     album: Annotated[str, typer.Argument(help="Album the song belongs to.")],
     force: Annotated[bool, typer.Option(help="Overwrite the song if present.")] = False,
 ):
-    """Search and download the song and add it to the db. Use --force to overwrite the existing song in the db.
+    """Search and download the song and add it to the db.
     Creates a new album if not already present.
     """
     print(f"Given: {name} from {album} by {artist} and force is {force}")
     output = download_song_operation(
         album, name, artist, APP_CONFIG["root_download_path"], False
     )
     print(output)
 
 
-@app.command("download")
+@app.command("parse")
 def parse_library(
-    path: Annotated[
+    library_path: Annotated[
         str,
-        typer.Argument(help="The path to the Library.xml exported from Apple Music."),
-    ] = "./Library.xml"
+        typer.Argument(help="The path to the 'Library.xml' or 'Library.csv' exported from Apple Music."),
+    ]
 ):
-    """Parse the entire AM library and download songs and make/update the db as needed."""
-    print(f"Gotten path: {path}")
-    parse_library_operation(APP_CONFIG["root_download_path"], path)
+    """Parse the entire Apple Music library and make/update the DB as needed."""
+    output = parse_library_operation(APP_CONFIG['root_download_path'], library_path)
+    if output:
+        print(output)
+
+
+@app.command('download')
+def download_library(
+    library_path: Annotated[
+        str,
+        typer.Argument(help="The path to the 'Library.xml' or 'Library.csv' exported from Apple Music."),
+    ] = ""
+):
+    """Download the entire DB library.
+
+    If passed, parse the library and update the DB before download.
+    """
+    if library_path:
+        parse_library_operation(APP_CONFIG['root_download_path'], library_path)
+
+    output = download_library_operation(APP_CONFIG['root_download_path'])
+    if output:
+        print(output)
 
 
 @app.command("showsimilar")
 def show_similar_songs_in_db(
     name: Annotated[str, typer.Argument(help="Name of the song to search.")]
 ):
     """Look up the db and show if similar/exact song(s) are found."""
```

### Comparing `amusing_app-0.1.2/amusing/cli_operations.py` & `amusing_app-0.2.0/amusing/cli_operations.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,101 +1,134 @@
 import os
 
-from amusing.core.download import download_song_from_id
 from amusing.core.parse_csv import process_csv
 from amusing.core.parse_xml import parse_library_xml
-from amusing.core.save_to_db import create_new_album, create_new_song
-from amusing.core.search import search_a_song
+from amusing.core.download import download
+import amusing.core.save_to_db
+import amusing.core.search
 from amusing.db.engine import get_new_db_session
 from amusing.db.models import Album, Song
-from amusing.utils.funcs import construct_db_path, construct_download_path
-
+from amusing.utils.funcs import construct_db_path
 
 def download_song_operation(
     album_name: str,
     song_name: str,
     artist_name: str,
     root_download_path: str,
     overwrite: bool = False,
-):
+) -> str:
     """Download a particular song and add it to the db.
 
     Parameters:
     album_name (str): name of the album
     song_name (str): name of the song
     artist_name (str): name of the artist
     root_download_path (str): the path to download songs and put db into.
     overwrite (bool): whether to overwrite the song if present in db and downloads.
 
     """
+    song = Song(
+        title=song_name,
+        artist=artist_name,
+        album=Album(title=album_name),
+    )
     # fetch song from YT Music
-    song_fetched = search_a_song(song_name, artist_name, album_name)
+    song_fetched = search(song)
     if not song_fetched:
         return "Couldn't find song through YouTube Music Search."
-    album_name = song_fetched["album"]
-    song_name = song_fetched["song_name"]
-    artist_name = song_fetched["artist_name"]
-
-    # download song into album
-    album_dir = os.path.join(
-        construct_download_path(root_download_path), song_fetched["album"]
-    )
-    error = download_song_from_id(song_fetched["videoId"], album_dir)
-    if error:
-        return "Something went wrong in downloading song. Please try again."
+    album_name = song_fetched.album.title
+    song_name = song_fetched.title
+    artist_name = song_fetched.artist
+
+    try:
+        download(song_fetched, root_download_path)
+    except RuntimeError as e:
+        print(f"[!] Error: {e}")
+        return "Something went wrong while downloading a song. Please try again."
+    except FileNotFoundError as e:
+        print(f"[!] Error: {e}")
+        return "Is FFmpeg installed? It is required to generate the songs."
 
     # insert into db
     session = get_new_db_session(construct_db_path(root_download_path))
     if not album_name:
         album_name = song_name
     album_in_db, error = create_new_album(album_name, album_dir, session)
     if error:
         return "Something went wrong in creating album. Please try again."
 
     error = create_new_song(
-        song_name, artist_name, song_fetched["videoId"], album_in_db, session, overwrite
+        song_name, artist_name, song_fetched.video_id, album_in_db, session, overwrite
     )
     if error:
         return "Something went wrong in creating song. Please try again."
+
     return "Added song!"
 
 
-def parse_library_operation(root_download_path: str, lib_path: str):
-    """Parse the Library XML file and download all songs.
+def parse_library_operation(root_download_path: str, lib_path: str) -> str:
+    """Parse the Library XML or CSV file.
 
     Parameters:
-    root_download_path (str): the path to download songs and put db into.
-    lib_path (str): the full path to the Library.xml file exported from Apple Music.
+    lib_path (str): the full path to the Library.xml file exported from Apple Music or a Library.csv file
 
     """
-    error = parse_library_xml(root_download_path, lib_path)
-    if error:
-        return "Something went wrong in creating a parsed CSV file from XML. Please try again."
+    if lib_path.lower().endswith('.xml'):
+        error = parse_library_xml(root_download_path, lib_path)
+        if error:
+            return "Something went wrong in creating a parsed CSV file from XML. Please try again."
+        parsed_library = os.path.join(root_download_path, "Library.csv")
+    elif lib_path.lower().endswith('.csv'):
+        parsed_library = lib_path
+    else:
+        return "A 'Library.xml' or 'Library.csv' file was expected."
 
-    download_path = construct_download_path(root_download_path)
     session = get_new_db_session(construct_db_path(root_download_path))
-    process_csv(
-        os.path.join(root_download_path, "Library_parsed.csv"), download_path, session
-    )
+    process_csv(parsed_library, session)
+
+    return ""
+
+
+def download_library_operation(root_download_path: str) -> str:
+    """Download all songs in DB.
+
+    Parameters:
+    root_download_path (str): songs download path.
+
+    """
+    session = get_new_db_session(construct_db_path(root_download_path))
+    albums = session.query(Album).order_by(Album.title)
+    for album in albums:
+        for song in album.songs:
+            try:
+                download(song, root_download_path)
+            except RuntimeError as e:
+                print(f"[!] Error: {e}")
+                print('[!] Something went wrong while downloading. Skipping song.')
+            except FileNotFoundError as e:
+                print(f"[!] Error: {e}")
+                return 'Is FFmpeg installed? It is required to generate the songs.'
+
+    return ""
 
 
 def show_similar_songs_in_db_operation(song_name: str, root_download_path: str):
     """Look up the db for song_name.
 
     Parameters:
     song_name (str): the name of the song to look up
     root_download_path (str): the path to the root downloads folder where the db is situated.
 
     """
     session = get_new_db_session(construct_db_path(root_download_path))
-    song_query = session.query(Song).filter(Song.name.ilike(f"%{song_name}%")).all()
+    song_query = session.query(Song).filter(Song.title.ilike(f"%{song_name}%")).all()
     song_list_found = []
     for song in song_query:
         song_list_found.append(
-            {"name": song.name, "artist": song.artist, "album": song.album.name}
+            {"name": song.title, "artist": song.artist, "album": song.album.title}
         )
     return song_list_found
 
 
 def show_similar_songs_for_artist_in_db_operation(
     artist_name: str, root_download_path: str
 ):
@@ -107,28 +140,28 @@
 
     """
     session = get_new_db_session(construct_db_path(root_download_path))
     song_query = session.query(Song).filter(Song.artist.ilike(f"%{artist_name}%")).all()
     song_list_found = []
     for song in song_query:
         song_list_found.append(
-            {"name": song.name, "artist": song.artist, "album": song.album.name}
+            {"name": song.title, "artist": song.artist, "album": song.album.title}
         )
     return song_list_found
 
 
 def show_similar_albums_in_db_operation(album_name: str, root_download_path: str):
     """Look up the db for album_name.
 
     Parameters:
     album_name (str): the name of the album to look up
     root_download_path (str): the path to the root downloads folder where the db is situated.
 
     """
     session = get_new_db_session(construct_db_path(root_download_path))
-    album_query = session.query(Album).filter(Album.name.ilike(f"%{album_name}%")).all()
+    album_query = session.query(Album).filter(Album.title.ilike(f"%{album_name}%")).all()
     album_list_found = []
     for album in album_query:
         album_list_found.append(
-            {"name": album.name, "number_of_songs": len(album.songs)}
+            {"name": album.title, "number_of_songs": len(album.songs)}
         )
     return album_list_found
```

### Comparing `amusing_app-0.1.2/amusing/core/parse_xml.py` & `amusing_app-0.2.0/amusing/core/parse_xml.py`

 * *Files 19% similar despite different names*

```diff
@@ -56,16 +56,23 @@
                 list_values = [i for i in dict1.values()]
                 list_keys = [j for j in dict1.keys()]
                 df_temp = pd.DataFrame([list_values], columns=list_keys)
                 df = pd.concat([df, df_temp], axis=0, ignore_index=True, sort=True)
             return df
 
         df_apple_music = df_creation(apple_music, list(apple_music_cols))
-        # df_podcast = df_creation(podcast,podcast_cols)
-        # df_purchased = df_creation(purchased,purchased_cols)
+
+        # Move title column at the beginning
+        title_column = df_apple_music.pop('Name')
+        df_apple_music.insert(0, 'Title', title_column)
+        # Add album artwork column
+        df_apple_music.insert(2, 'Artwork URL', '')
+        # Add video_id column
+        df_apple_music.insert(2, 'Video ID', '')
+
         print("Dataframe created of length: ", len(df_apple_music))
         df_apple_music.to_csv(
-            os.path.join(root_download_path, "Library_parsed.csv"), index=False
+            os.path.join(root_download_path, "Library.csv"), index=False
         )
     except Exception as e:
         print("Something went wrong in parsing your Library XML file: ", e)
         return 1
```

### Comparing `amusing_app-0.1.2/amusing/core/save_to_db.py` & `amusing_app-0.2.0/amusing/core/save_to_db.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,17 +10,17 @@
     try:
         dir_already_present = False
         if os.path.exists(album_dir) and os.path.isdir(album_dir):
             dir_already_present = True
         else:
             os.makedirs(album_dir, exist_ok=True)
 
-        album = session.query(Album).filter_by(name=album_name).first()
+        album = session.query(Album).filter_by(title=album_name).first()
         if not album:
-            album = Album(name=album_name)
+            album = Album(title=album_name)
             session.add(album)
             session.commit()
         return album, 0
     except Exception as e:
         print(f"Exception {e} when creating album.")
         return None, 1
 
@@ -33,20 +33,20 @@
     session: Session,
     overwrite: bool = False,
 ):
     """To add a new song into the db."""
     try:
         song_query = (
             session.query(Song)
-            .filter_by(name=song_name, artist=artist_name, album=album)
+            .filter_by(title=song_name, artist=artist_name, album=album)
             .first()
         )
         if song_query and overwrite:
             session.delete(song_query)
         elif song_query and not overwrite:
             return
-        song = Song(name=song_name, artist=artist_name, video_id=videoId, album=album)
+        song = Song(title=song_name, artist=artist_name, video_id=videoId, album=album)
         session.add(song)
         session.commit()
     except Exception as e:
         print(f"Exception {e} when creating the song.")
         return 1
```

### Comparing `amusing_app-0.1.2/amusing/utils/config.py` & `amusing_app-0.2.0/amusing/utils/config.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,30 +4,37 @@
 import yaml
 
 APP_CONFIG = {}
 
 
 def find_or_create_config_file():
     # Define the file path
-    os.makedirs(os.path.join(Path.home(), "Downloads", "Amusing"), exist_ok=True)
-    file_path = os.path.join(Path.home(), "Downloads", "Amusing", "appconfig.yaml")
+    default_root_download_path = os.path.join(Path.home(), 'Downloads', 'Amusing')
+    default_config_path = os.path.join(default_root_download_path, 'appconfig.yaml')
+    alternative_config_path = os.path.join(os.path.join(Path.home(), '.config', 'amusing'), 'appconfig.yaml')
+
+    file_path = default_config_path
+    if not os.path.exists(file_path) and os.path.exists(alternative_config_path):
+        file_path = alternative_config_path
 
     # Check if the file exists
     if os.path.exists(file_path):
         return file_path
     else:
+        os.makedirs(os.path.join(default_root_download_path), exist_ok=True)
         # Create the file
         with open(file_path, "w") as file:
             # Write default configuration (you can customize this)
             config_data = {
-                "root_download_path": str(
-                    os.path.join(Path.home(), "Downloads", "Amusing", "data")
-                ),
+                "root_download_path": str(default_root_download_path),
                 "db_name": "library.db",
             }
             yaml.dump(config_data, file)
             print(f"Created a new config file: {file_path}")
         return file_path
 
 
 with open(find_or_create_config_file(), "r") as file:
     APP_CONFIG = yaml.safe_load(file)
+    # Expand possible ~ in paths
+    APP_CONFIG['db_name'] = os.path.expanduser(APP_CONFIG['db_name'])
+    APP_CONFIG['root_download_path'] = os.path.expanduser(APP_CONFIG['root_download_path'])
```

### Comparing `amusing_app-0.1.2/pyproject.toml` & `amusing_app-0.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "amusing-app"
-version = "0.1.2"
-description = "Amusing CLI to help download music independently or from your exported apple music library."
+version = "0.2.0"
+description = "CLI to download music independently and from your exported Apple Music library."
 authors = ["Yash Prakash <yashprakash13@gmail.com>"]
 readme = "README.md"
 packages = [{include = "amusing"}]
 
 [tool.poetry.scripts]
 amusing = "amusing.cli:app"
 
@@ -32,22 +32,22 @@
 six = "1.16.0"
 sqlalchemy = "2.0.24"
 typer = "0.9.0"
 typing-extensions = "4.9.0"
 tzdata = "2023.3"
 urllib3 = "2.1.0"
 websockets = "12.0"
-yt-dlp = "2023.11.16"
+yt-dlp = "2024.4.9"
 ytmusicapi = "1.3.2"
 
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.6.0"
 black = "^23.12.1"
 isort = "^5.13.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
-profile = "black"
+profile = "black"
```

