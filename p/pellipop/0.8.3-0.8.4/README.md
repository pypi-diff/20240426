# Comparing `tmp/pellipop-0.8.3.tar.gz` & `tmp/pellipop-0.8.4.tar.gz`

## Comparing `pellipop-0.8.3.tar` & `pellipop-0.8.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     7123 2020-02-02 00:00:00.000000 pellipop-0.8.3/pellipop/Video.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 pellipop-0.8.3/pellipop/__about__.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 pellipop-0.8.3/pellipop/__init__.py
--rw-r--r--   0        0        0     3782 2020-02-02 00:00:00.000000 pellipop-0.8.3/pellipop/cli.py
--rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 pellipop-0.8.3/pellipop/file_finder.py
--rw-r--r--   0        0        0    16483 2020-02-02 00:00:00.000000 pellipop-0.8.3/pellipop/gui.py
--rw-r--r--   0        0        0    16528 2020-02-02 00:00:00.000000 pellipop-0.8.3/pellipop/main.py
--rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 pellipop-0.8.3/pellipop/path_fixer.py
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 pellipop-0.8.3/pellipop/whisper_from_url.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pellipop-0.8.3/pellipop/speech_to_text/__init__.py
--rw-r--r--   0        0        0     5479 2020-02-02 00:00:00.000000 pellipop-0.8.3/pellipop/speech_to_text/whisperMode.py
--rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 pellipop-0.8.3/.gitignore
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pellipop-0.8.3/.hgignore
--rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 pellipop-0.8.3/LICENSE.txt
--rw-r--r--   0        0        0     3957 2020-02-02 00:00:00.000000 pellipop-0.8.3/pyproject.toml
--rw-r--r--   0        0        0     4421 2020-02-02 00:00:00.000000 pellipop-0.8.3/readme.md
--rw-r--r--   0        0        0     6303 2020-02-02 00:00:00.000000 pellipop-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0     7123 2020-02-02 00:00:00.000000 pellipop-0.8.4/pellipop/Video.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 pellipop-0.8.4/pellipop/__about__.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 pellipop-0.8.4/pellipop/__init__.py
+-rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 pellipop-0.8.4/pellipop/cli.py
+-rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 pellipop-0.8.4/pellipop/file_finder.py
+-rw-r--r--   0        0        0    16545 2020-02-02 00:00:00.000000 pellipop-0.8.4/pellipop/gui.py
+-rw-r--r--   0        0        0    17144 2020-02-02 00:00:00.000000 pellipop-0.8.4/pellipop/main.py
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 pellipop-0.8.4/pellipop/path_fixer.py
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 pellipop-0.8.4/pellipop/whisper_from_url.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pellipop-0.8.4/pellipop/speech_to_text/__init__.py
+-rw-r--r--   0        0        0     5479 2020-02-02 00:00:00.000000 pellipop-0.8.4/pellipop/speech_to_text/whisperMode.py
+-rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 pellipop-0.8.4/.gitignore
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pellipop-0.8.4/.hgignore
+-rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 pellipop-0.8.4/LICENSE.txt
+-rw-r--r--   0        0        0     3957 2020-02-02 00:00:00.000000 pellipop-0.8.4/pyproject.toml
+-rw-r--r--   0        0        0     4421 2020-02-02 00:00:00.000000 pellipop-0.8.4/readme.md
+-rw-r--r--   0        0        0     6303 2020-02-02 00:00:00.000000 pellipop-0.8.4/PKG-INFO
```

### Comparing `pellipop-0.8.3/pellipop/Video.py` & `pellipop-0.8.4/pellipop/Video.py`

 * *Files identical despite different names*

### Comparing `pellipop-0.8.3/pellipop/cli.py` & `pellipop-0.8.4/pellipop/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from argparse import ArgumentParser, Namespace
+from argparse import ArgumentParser
 from sys import argv
 
 from pellipop.__about__ import __version__
 from pellipop.path_fixer import Path
 
 # Possibilité de paramétrage dans le terminal/l'invite de commandes
 parser = ArgumentParser()
@@ -53,14 +53,15 @@
     "-g", "--gui", type=bool, default=False, nargs='?', const=True,
     help="Permet d'utiliser l'interface graphique"
 )
 parser.add_argument(
     "-v", "--version", action="version", version=f"%(prog)s {__version__}"
 )
 
+
 def main() -> dict[str, Path | None]:
     args = parser.parse_args()
 
     if args.gui or len(argv) < 2:
         from pellipop.gui import main as gui
         return gui()
```

### Comparing `pellipop-0.8.3/pellipop/file_finder.py` & `pellipop-0.8.4/pellipop/file_finder.py`

 * *Files identical despite different names*

### Comparing `pellipop-0.8.3/pellipop/gui.py` & `pellipop-0.8.4/pellipop/gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -280,14 +280,15 @@
         "reduce": int(reduce_length.get()),
         "offset": int(offset_length.get()),
         "parents_in_name": int(parents_length.get()),
         "with_text": True,  # TODO : With text or only text ? Should we let the user choose ?
     }
 
     try:
+        print(f" Launching pellipop with config :\n{config}")
         pelli = Pellipop(**config)
         csv_outp = pelli.launch()
 
     except Exception as e:
         print(e)
         lancer_button.config(state="normal")
         lancer_button.bell()
```

### Comparing `pellipop-0.8.3/pellipop/main.py` & `pellipop-0.8.4/pellipop/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import json
 import re
 import subprocess
 from math import ceil, floor
+from time import sleep
 from typing import Optional
 
 from tqdm.auto import tqdm
 
 from pellipop.Video import Video
 from pellipop.file_finder import file_finder, how_many_files
 from pellipop.path_fixer import Path
@@ -46,14 +47,15 @@
     # To parse frame numbers: 000000.jpg
     ending_digits = re.compile(r"\d+$")
     # To parse back times: 00h_00m_00s.jpg or 00h_00m_00s or 00h_00m_00s_to_
     ending_time = re.compile(r"(\d{2}h_\d{2}m_\d{2}s)(?:.jpg|_to_|$)")
 
     def __init__(
             self,
+            /,
             *args,
             intervale: float,
             input_folder: str | Path,
             output_folder: str | Path = Path.home() / "Documents" / "Pellipop",
             i_frame_mode: bool = True,
             decouper: bool = True,
             retranscrire: bool = False,
@@ -64,14 +66,16 @@
             offset: int = 0,
             parents_in_name: int = 0,
 
             on_progress: callable = None,  # TODO: Add a progress bar
 
             whisper_config: dict = None,
             keep_audio: bool = False,
+
+            **kwargs,
     ):
         if args:
             raise
 
         self.intervale = intervale if intervale else 1
         self.input_folder = input_folder
         self.output_folder = output_folder
@@ -200,29 +204,32 @@
                 self.from_frame_to_time(video)
 
             self._from_time_to_timespan_folder(video)
 
         return self.outputs["image"], self.outputs["audio"]
 
     def from_frame_to_time(self, video: Video, fps: int = 0):
-        lst_img = sorted(video.image_folder.glob("*.jpg"))
+        lst_img = sorted(video.image_folder.glob("*.jpg"), key=lambda x: int(self.ending_digits.findall(x.stem)[0]))
 
         if self.i_frame_mode:
             rename_func = self._ftt_no_duplicates
         else:
             rename_func = self._ftt_duplicates
 
         for img in lst_img:
             new_img = rename_func(img, fps)
             if new_img.exists():
                 print(f"Collision détectée: {img.name} -> {new_img.name}")
-                continue
+                # img.unlink()
+                # continue
             img.rename(new_img)
             pass
 
+        sleep(0.1)
+
         video.images = sorted(video.image_folder.glob("*.jpg"))
 
     def _ftt_no_duplicates(self, img: Path, fps: int) -> Path:
         frame_number = int(self.ending_digits.findall(img.stem)[0])
         time = self.format_time(frame_number // fps)
         new_name = time.join(img.name.rsplit(str(frame_number), 1))
         return img.with_name(new_name)
@@ -403,30 +410,45 @@
 
 
 if __name__ == "__main__":
     # testdir = "/home/marceau/PycharmProjects/tksel/videos-collecte1"
     testdir = "/home/marceau/Téléchargements/pelli/"
     print(how_many_files(testdir))
 
-    p = Pellipop(
-        intervale=4,
-        input_folder=testdir,
-        output_folder=default_output_path,
-        i_frame_mode=True,
-        decouper=True,
-        retranscrire=True,
-        csv=True,
-        with_text=True,
-        only_text=False,
-        keep_audio=True,
-
-        reduce=10,
-        offset=5,
-        parents_in_name=2,
-    )
+    config = {
+        'intervale': None,
+        'input_folder': '/home/marceau/Téléchargements/pelli',
+        'output_folder': '/home/marceau/Documents/Pellipop',
+        'i_frame_mode': True,
+        'decouper': True,
+        'retranscrire': False,
+        'csv': True,
+        'reduce': -1,
+        'offset': 0,
+        'parents_in_name': 0,
+        'with_text': True
+    }
+    p = Pellipop(**config)
+
+    # p = Pellipop(
+    #     intervale=4,
+    #     input_folder=testdir,
+    #     output_folder=default_output_path,
+    #     i_frame_mode=True,
+    #     decouper=True,
+    #     retranscrire=True,
+    #     csv=True,
+    #     with_text=True,
+    #     only_text=False,
+    #     keep_audio=True,
+    #
+    #     reduce=10,
+    #     offset=5,
+    #     parents_in_name=2,
+    # )
     p.launch()
 
     ## Csv only test
     # p.output_folder = Path("/home/marceau/Documents/Pellipop")
     # videos = list(file_finder(testdir, file_type="video"))
     # videos_stems = {v.stem for v in videos}
     # p.fichiers_stems = videos_stems
```

### Comparing `pellipop-0.8.3/pellipop/path_fixer.py` & `pellipop-0.8.4/pellipop/path_fixer.py`

 * *Files identical despite different names*

### Comparing `pellipop-0.8.3/pellipop/whisper_from_url.py` & `pellipop-0.8.4/pellipop/whisper_from_url.py`

 * *Files identical despite different names*

### Comparing `pellipop-0.8.3/pellipop/speech_to_text/whisperMode.py` & `pellipop-0.8.4/pellipop/speech_to_text/whisperMode.py`

 * *Files identical despite different names*

### Comparing `pellipop-0.8.3/.gitignore` & `pellipop-0.8.4/.gitignore`

 * *Files identical despite different names*

### Comparing `pellipop-0.8.3/LICENSE.txt` & `pellipop-0.8.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pellipop-0.8.3/pyproject.toml` & `pellipop-0.8.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pellipop-0.8.3/readme.md` & `pellipop-0.8.4/readme.md`

 * *Files identical despite different names*

### Comparing `pellipop-0.8.3/PKG-INFO` & `pellipop-0.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pellipop
-Version: 0.8.3
+Version: 0.8.4
 Summary: A graphical and command-line tool to extract key frames from videos along with their retranscription. It uses the Whisper API to transcribe the audio. It also generates a CSV file with the extracted key frames and their corresponding text.
 Project-URL: Homepage, https://github.com/CERES-Sorbonne/Pellipop
 Project-URL: Documentation, https://github.com/CERES-Sorbonne/Pellipop#readme
 Project-URL: Issues, https://github.com/CERES-Sorbonne/Pellipop/issues
 Project-URL: Source, https://github.com/CERES-Sorbonne/Pellipop
 Author: EdouardBoute
 Author-email: Marceau-h <pypi@marceau-h.fr>, Orion Alié <someonefefe@gmail.com>
```

