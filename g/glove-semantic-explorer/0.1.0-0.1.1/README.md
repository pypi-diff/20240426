# Comparing `tmp/glove_semantic_explorer-0.1.0.tar.gz` & `tmp/glove_semantic_explorer-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glove_semantic_explorer-0.1.0.tar", max compression
+gzip compressed data, was "glove_semantic_explorer-0.1.1.tar", max compression
```

## Comparing `glove_semantic_explorer-0.1.0.tar` & `glove_semantic_explorer-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1095 2023-11-16 10:09:25.974966 glove_semantic_explorer-0.1.0/LICENSE
--rw-r--r--   0        0        0       57 2023-11-16 10:09:25.974966 glove_semantic_explorer-0.1.0/README.md
--rw-r--r--   0        0        0       86 2024-04-10 11:43:51.453406 glove_semantic_explorer-0.1.0/glove_semantic_explorer/__main__.py
--rw-r--r--   0        0        0     3269 2024-04-10 12:01:25.789659 glove_semantic_explorer-0.1.0/glove_semantic_explorer/cli.py
--rw-r--r--   0        0        0     1341 2024-04-10 11:56:41.221117 glove_semantic_explorer-0.1.0/glove_semantic_explorer/templates.py
--rw-r--r--   0        0        0      542 2024-04-10 12:10:18.738268 glove_semantic_explorer-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      848 1970-01-01 00:00:00.000000 glove_semantic_explorer-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1095 2023-11-16 10:09:25.974966 glove_semantic_explorer-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1694 2024-04-26 08:17:44.214808 glove_semantic_explorer-0.1.1/README.md
+-rw-r--r--   0        0        0       86 2024-04-10 11:43:51.453406 glove_semantic_explorer-0.1.1/glove_semantic_explorer/__main__.py
+-rw-r--r--   0        0        0     3598 2024-04-26 08:16:51.712241 glove_semantic_explorer-0.1.1/glove_semantic_explorer/cli.py
+-rw-r--r--   0        0        0     1338 2024-04-26 08:11:24.862432 glove_semantic_explorer-0.1.1/glove_semantic_explorer/templates.py
+-rw-r--r--   0        0        0      542 2024-04-26 08:18:54.238456 glove_semantic_explorer-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2485 1970-01-01 00:00:00.000000 glove_semantic_explorer-0.1.1/PKG-INFO
```

### Comparing `glove_semantic_explorer-0.1.0/LICENSE` & `glove_semantic_explorer-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `glove_semantic_explorer-0.1.0/glove_semantic_explorer/cli.py` & `glove_semantic_explorer-0.1.1/glove_semantic_explorer/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 from pathlib import Path
-from typing import Iterable
+from typing import Iterable, Optional, Union
 
 from embedding_explorer.app import get_dash_app
 from embedding_explorer.blueprints.explorer import create_explorer
 from gensim.models import KeyedVectors
 from gensim.utils import tokenize
 from glovpy import GloVe
 from radicli import Arg, Radicli
 
-from glove_semantic_explorer.templates import (
-    COMPOSE_TEMPLATE,
-    DOCKERFILE_TEMPLATE,
-    MAIN_FILE_TEMPLATE,
-)
+from glove_semantic_explorer.templates import (COMPOSE_TEMPLATE,
+                                               DOCKERFILE_TEMPLATE,
+                                               MAIN_FILE_TEMPLATE)
 
 cli = Radicli()
 
 
-def stream_sentences(files: list[str]) -> Iterable[list[str]]:
+def stream_sentences(files: Iterable[Union[str, Path]]) -> Iterable[list[str]]:
     for file in files:
         with open(file) as in_file:
             for line in in_file:
                 yield list(tokenize(line, lower=True, deacc=True))
 
 
 @cli.command(
@@ -33,25 +31,25 @@
         "--out_file",
         "-o",
         help="Path to the output file in keyed vector format.",
     ),
 )
 def train_model(data_folder: str, out_path: str = "model/glove.kv") -> None:
     print("Collecting training data.")
-    data_folder = Path(data_folder)
-    files = data_folder.glob("*.txt")
+    data_path = Path(data_folder)
+    files = data_path.glob("*.txt")
     sentences = list(stream_sentences(files))
     print("Training Word embeddings.")
     model = GloVe(vector_size=50)
     model.train(sentences)
     print("Saving embeddings.")
-    out_path = Path(out_path)
-    out_dir = out_path.parent
+    out_file = Path(out_path)
+    out_dir = out_file.parent
     out_dir.mkdir(exist_ok=True)
-    model.wv.save(str(out_path))
+    model.wv.save(str(out_file))
     print("DONE")
 
 
 @cli.command(
     "run_explorer",
     model_path=Arg(
         "--model_file",
@@ -65,46 +63,49 @@
     blueprint = create_explorer(corpus=kv.index_to_key, embeddings=kv.vectors)
     app = get_dash_app(blueprint=blueprint, name=__name__, use_pages=False)
     app.run_server(debug=False, port=port, host="0.0.0.0")
 
 
 @cli.command(
     "generate_docker",
+    project_name=Arg(help="Name of the project in the compose file."),
     model_path=Arg(
         "--model_file",
         "-m",
         help="Path to the model file in keyed vector format.",
     ),
     port=Arg("--port", "-p", help="Port to run the app on."),
     url_base_pathname=Arg(
         "--url_base_pathname",
         "-u",
-        help="Base path name of the app at the port.",
+        help="Base path name of the app at the port. If not specified it is set to project_name.",
     ),
     out_dir=Arg(
         "--out_dir",
         "-o",
         help="Folder to output the container information to.",
     ),
 )
 def generate_docker(
+    project_name: str,
     model_path: str = "model/glove.kv",
     port: int = 8080,
-    url_base_pathname: str = "/",
+    url_base_pathname: Optional[str] = None,
     out_dir: str = "deployment/",
 ):
-    out_dir = Path(out_dir)
-    out_dir.mkdir(exist_ok=True)
+    out_path = Path(out_dir)
+    out_path.mkdir(exist_ok=True)
     print("Generating files for deployment.")
-    with out_dir.joinpath("main.py").open("w") as main_file:
+    with out_path.joinpath("main.py").open("w") as main_file:
         main_file.write(MAIN_FILE_TEMPLATE)
-    with out_dir.joinpath("Dockerfile").open("w") as dockerfile:
+    with out_path.joinpath("Dockerfile").open("w") as dockerfile:
         dockerfile.write(DOCKERFILE_TEMPLATE)
-    with out_dir.joinpath("compose.yaml").open("w") as dockerfile:
+    with out_path.joinpath("compose.yaml").open("w") as dockerfile:
         dockerfile.write(
             COMPOSE_TEMPLATE.format(
                 port=port,
                 model_path=Path(model_path).absolute(),
-                url_base_pathname=url_base_pathname,
+                url_base_pathname=url_base_pathname or f"/{project_name}/",
+                project_name=project_name,
             )
         )
     print("DONE")
```

### Comparing `glove_semantic_explorer-0.1.0/glove_semantic_explorer/templates.py` & `glove_semantic_explorer-0.1.1/glove_semantic_explorer/templates.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 EXPOSE 8080
 CMD gunicorn --timeout 0 -b 0.0.0.0:8080 --worker-tmp-dir /dev/shm --workers=2 --threads=4 --worker-class=gthread main:server
 """
 
 COMPOSE_TEMPLATE = """
 services:
   server:
-    image: sermon_embeddings/server
+    image: {project_name}/server
     build: .
     ports: 
       - "{port}:8080"
     deploy:
       restart_policy:
         condition: on-failure
         delay: 5s
```

### Comparing `glove_semantic_explorer-0.1.0/pyproject.toml` & `glove_semantic_explorer-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 line-length=79
 
 [tool.black]
 line-length=79
 
 [tool.poetry]
 name = "glove-semantic-explorer"
-version = "0.1.0"
+version = "0.1.1"
 description = "Easy to use CLI to set up embedding-explorer for deployment on a corpus with GloVe word embeddings"
 authors = ["Márton Kardos <power.up1163@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

