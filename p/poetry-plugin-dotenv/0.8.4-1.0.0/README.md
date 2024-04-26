# Comparing `tmp/poetry_plugin_dotenv-0.8.4.tar.gz` & `tmp/poetry_plugin_dotenv-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_plugin_dotenv-0.8.4.tar", max compression
+gzip compressed data, was "poetry_plugin_dotenv-1.0.0.tar", max compression
```

## Comparing `poetry_plugin_dotenv-0.8.4.tar` & `poetry_plugin_dotenv-1.0.0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     1077 2024-04-11 19:29:23.553611 poetry_plugin_dotenv-0.8.4/LICENSE
--rw-r--r--   0        0        0     7560 2024-04-11 19:29:23.553611 poetry_plugin_dotenv-0.8.4/README.md
--rw-r--r--   0        0        0     6944 2024-04-11 19:29:50.837627 poetry_plugin_dotenv-0.8.4/pyproject.toml
--rw-r--r--   0        0        0      695 2024-04-11 19:29:50.837627 poetry_plugin_dotenv-0.8.4/src/poetry_plugin_dotenv/__init__.py
--rw-r--r--   0        0        0      335 2024-04-11 19:29:23.561611 poetry_plugin_dotenv-0.8.4/src/poetry_plugin_dotenv/dotenv/__init__.py
--rw-r--r--   0        0        0     5221 2024-04-11 19:29:23.561611 poetry_plugin_dotenv-0.8.4/src/poetry_plugin_dotenv/dotenv/core.py
--rw-r--r--   0        0        0     5969 2024-04-11 19:29:23.561611 poetry_plugin_dotenv-0.8.4/src/poetry_plugin_dotenv/dotenv/parsers.py
--rw-r--r--   0        0        0     1445 2024-04-11 19:29:23.561611 poetry_plugin_dotenv-0.8.4/src/poetry_plugin_dotenv/dotenv/variables.py
--rw-r--r--   0        0        0     3508 2024-04-11 19:29:23.561611 poetry_plugin_dotenv-0.8.4/src/poetry_plugin_dotenv/plugin.py
--rw-r--r--   0        0        0        0 2024-04-11 19:29:23.561611 poetry_plugin_dotenv-0.8.4/src/poetry_plugin_dotenv/py.typed
--rw-r--r--   0        0        0     9563 1970-01-01 00:00:00.000000 poetry_plugin_dotenv-0.8.4/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-04-26 13:27:43.809873 poetry_plugin_dotenv-1.0.0/LICENSE
+-rw-r--r--   0        0        0     9687 2024-04-26 13:27:43.809873 poetry_plugin_dotenv-1.0.0/README.md
+-rw-r--r--   0        0        0     7129 2024-04-26 13:28:13.862198 poetry_plugin_dotenv-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      778 2024-04-26 13:28:13.866198 poetry_plugin_dotenv-1.0.0/src/poetry_plugin_dotenv/__init__.py
+-rw-r--r--   0        0        0     3084 2024-04-26 13:27:43.817873 poetry_plugin_dotenv-1.0.0/src/poetry_plugin_dotenv/config.py
+-rw-r--r--   0        0        0      335 2024-04-26 13:27:43.817873 poetry_plugin_dotenv-1.0.0/src/poetry_plugin_dotenv/dotenv/__init__.py
+-rw-r--r--   0        0        0     5421 2024-04-26 13:27:43.817873 poetry_plugin_dotenv-1.0.0/src/poetry_plugin_dotenv/dotenv/core.py
+-rw-r--r--   0        0        0     6005 2024-04-26 13:27:43.817873 poetry_plugin_dotenv-1.0.0/src/poetry_plugin_dotenv/dotenv/parsers.py
+-rw-r--r--   0        0        0     1572 2024-04-26 13:27:43.817873 poetry_plugin_dotenv-1.0.0/src/poetry_plugin_dotenv/dotenv/variables.py
+-rw-r--r--   0        0        0     3287 2024-04-26 13:27:43.817873 poetry_plugin_dotenv-1.0.0/src/poetry_plugin_dotenv/plugin.py
+-rw-r--r--   0        0        0        0 2024-04-26 13:27:43.817873 poetry_plugin_dotenv-1.0.0/src/poetry_plugin_dotenv/py.typed
+-rw-r--r--   0        0        0    11690 1970-01-01 00:00:00.000000 poetry_plugin_dotenv-1.0.0/PKG-INFO
```

### Comparing `poetry_plugin_dotenv-0.8.4/LICENSE` & `poetry_plugin_dotenv-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_plugin_dotenv-0.8.4/pyproject.toml` & `poetry_plugin_dotenv-1.0.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-plugin-dotenv"
-version = "0.8.4"
+version = "1.0.0"
 description = "poetry-plugin-dotenv - is the plugin that automatically loads environment variables from a dotenv file into the environment before poetry commands are run."
 license = "MIT"
 authors = ["Volodymyr Pivoshenko <volodymyr.pivoshenko@gmail.com>"]
 maintainers = ["Volodymyr Pivoshenko <volodymyr.pivoshenko@gmail.com>"]
 keywords = [
   "python",
   "pypi",
@@ -55,14 +55,15 @@
 python = ">=3.8.1,<4.0"
 poetry = ">=1.5.1"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = ">=3.5.0"
 poethepoet = ">=0.24.2"
 ipdb = ">=0.13.13"
+ipython = "8.12.3"
 
 [tool.poetry.group.formatters.dependencies]
 isort = ">=5.13.2"
 black = ">=24.1.1"
 pyupgrade = ">=3.15.0"
 
 [tool.poetry.group.linters.dependencies]
@@ -171,27 +172,26 @@
 target-version = "py311"
 line-length = 100
 exclude = ["__init__.py"]
 
 [tool.ruff.lint]
 select = ["ALL"]
 ignore = [
-  "ARG002",
-  "ANN002",
-  "ANN003",
   "ANN101",
-  "ANN102",
   "D202",
   "I001",
-  "PTH",
-  "FBT",
+  "TD003",
+  "FIX002",
 ]
 
 [tool.ruff.lint.per-file-ignores]
-"tests/*.*" = ["INP001", "S101"]
+"tests/*.*" = ["INP001", "S101", "PTH"]
+"src/poetry_plugin_dotenv/plugin.py" = ["ANN002", "ANN003", "ARG002"]
+"src/poetry_plugin_dotenv/dotenv/core.py" = ["PTH"]
+"src/poetry_plugin_dotenv/dotenv/variables.py" = ["ANN002", "ANN003", "ARG002"]
 
 [tool.ruff.lint.isort]
 lines-after-imports = 2
 lines-between-types = 1
 order-by-type = false
 force-single-line = true
 force-sort-within-sections = true
```

### Comparing `poetry_plugin_dotenv-0.8.4/src/poetry_plugin_dotenv/__init__.py` & `poetry_plugin_dotenv-1.0.0/src/poetry_plugin_dotenv/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 """poetry-plugin-dotenv - is the plugin that automatically loads environment variables from a dotenv file into the environment before poetry commands are run."""
 
 __title__ = "poetry-plugin-dotenv"
 __summary__ = "poetry-plugin-dotenv - is the plugin that automatically loads environment variables from a dotenv file into the environment before poetry commands are run."
 __uri__ = "https://github.com/pivoshenko/poetry-plugin-dotenv"
 
-__version__ = "0.8.4"
+__version__ = "1.0.0"
 
 __author__ = "Volodymyr Pivoshenko"
 __email__ = "volodymyr.pivoshenko@gmail.com"
 
 __license__ = "MIT"
 __copyright__ = "Copyright 2023, Volodymyr Pivoshenko"
 
+from poetry_plugin_dotenv import config
 from poetry_plugin_dotenv import dotenv
 from poetry_plugin_dotenv import plugin
+
+
+__all__ = ["dotenv", "plugin", "config"]
```

### Comparing `poetry_plugin_dotenv-0.8.4/src/poetry_plugin_dotenv/dotenv/core.py` & `poetry_plugin_dotenv-1.0.0/src/poetry_plugin_dotenv/dotenv/core.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,61 +1,69 @@
 """Module that contains core dotenv functionality."""
 
 from __future__ import annotations
 
 import io
 import os
 import sys
-import typing
 import contextlib
 
 from collections import OrderedDict
+from typing import IO
+from typing import TYPE_CHECKING
 
 from poetry_plugin_dotenv.dotenv import parsers
 from poetry_plugin_dotenv.dotenv import variables
 
 
+if TYPE_CHECKING:  # pragma: no cover
+    from collections.abc import Generator
+    from collections.abc import Iterable
+    from collections.abc import Iterator
+
+
 class DotEnv:
     """Model of a dotenv file."""
 
     def __init__(
         self,
         filepath: str | None = None,
-        stream: typing.IO[str] | None = None,
+        stream: IO[str] | None = None,
+        *,
         interpolate: bool = True,
         override: bool = True,
     ) -> None:
         """Initialize."""
 
         self.stream = stream
         self.override = override
         self.filepath = filepath
         self.interpolate = interpolate
 
         self.encoding = "utf-8"
 
-        self._dict: typing.OrderedDict[str, str] | None = None
+        self._dict: OrderedDict[str, str] | None = None
 
-    def dict(self) -> typing.OrderedDict[str, str]:
+    def dict(self) -> OrderedDict[str, str]:
         """Return content of a dotenv file."""
 
         if self._dict:
             return self._dict
 
         raw_values = self.parse()
 
         if self.interpolate:
             self._dict = resolve(raw_values, override=self.override)
 
         else:
             self._dict = OrderedDict(raw_values)
 
-        return self._dict
+        return self._dict  # type: ignore[return-value]
 
-    def parse(self) -> typing.Generator:
+    def parse(self) -> Generator:
         """Parse a dotenv file."""
 
         with self._get_stream() as stream:
             for mapping in parsers.parse_stream(stream):
                 if mapping.key is not None:
                     yield mapping.key, mapping.value
 
@@ -71,60 +79,61 @@
                     os.environ[key] = value
 
             return True
 
         return False  # pragma: nocover
 
     @contextlib.contextmanager
-    def _get_stream(self) -> typing.Iterator[typing.IO[str]]:
+    def _get_stream(self) -> Iterator[IO[str]]:
         """Get a dotenv stream."""
 
         if self.filepath and os.path.isfile(self.filepath):
             with open(self.filepath, encoding=self.encoding) as stream:
                 yield stream
 
         elif self.stream:
             yield self.stream
 
         else:
             yield io.StringIO("")  # pragma: nocover
 
 
 def resolve(
-    values: typing.Iterable[tuple[str, str]],
+    values: Iterable[tuple[str, str]],
+    *,
     override: bool,
-) -> typing.OrderedDict[str, str]:
+) -> OrderedDict[str, str]:
     """Resolve dotenv variables."""
 
-    new_values: typing.OrderedDict[str, str] = OrderedDict()
+    new_values: OrderedDict[str, str] = OrderedDict()
 
     for name, value in values:
         if value is None:
             result = None  # pragma: nocover
 
         else:
             atoms = variables.parse(value)
-            env: typing.OrderedDict[str, str] = OrderedDict()
+            env: OrderedDict[str, str] = OrderedDict()
 
             if override:
                 env.update(os.environ)
                 env.update(new_values)
 
             else:
                 env.update(new_values)
                 env.update(os.environ)
 
             result = "".join(atom.resolve(env) for atom in atoms)
 
-        new_values[name] = result
+        new_values[name] = result  # type: ignore[assignment]
 
     return new_values
 
 
-def walk_to_root(path: str) -> typing.Iterator[str]:
+def walk_to_root(path: str) -> Iterator[str]:
     """Yield directories starting from the given directory up to the root."""
 
     if not os.path.exists(path):
         msg = "Starting path not found."
         raise OSError(msg)  # pragma: nocover
 
     if os.path.isfile(path):
@@ -135,15 +144,15 @@
 
     while last_dir != current_dir:
         yield current_dir
         parent_dir = os.path.abspath(os.path.join(current_dir, os.path.pardir))
         last_dir, current_dir = current_dir, parent_dir
 
 
-def find(filename: str = ".env", usecwd: bool = False) -> str:
+def find(filename: str = ".env", *, usecwd: bool = False) -> str:
     """Search in increasingly higher folders for the given file."""
 
     if usecwd or getattr(sys, "frozen", False):
         path = os.getcwd()
 
     else:  # pragma: no cover
         frame = sys._getframe()  # noqa: SLF001
@@ -164,15 +173,16 @@
             return check_path
 
     return ""
 
 
 def load(
     filepath: str | None = None,
-    stream: typing.IO[str] | None = None,
+    stream: IO[str] | None = None,
+    *,
     interpolate: bool = True,
     override: bool = True,
 ) -> bool:
     """Parse a dotenv file and then load all the variables found as environment variables."""
 
     dotenv = DotEnv(
         filepath=filepath,
@@ -181,13 +191,14 @@
         stream=stream,
     )
     return dotenv.set_as_environment_variables()
 
 
 def values(
     filepath: str | None = None,
-    stream: typing.IO[str] | None = None,
+    stream: IO[str] | None = None,
+    *,
     interpolate: bool = True,
-) -> typing.OrderedDict[str, str]:
+) -> OrderedDict[str, str]:
     """Parse a dotenv file and return its content as a dictionary."""
 
     return DotEnv(filepath=filepath, stream=stream, interpolate=interpolate).dict()
```

### Comparing `poetry_plugin_dotenv-0.8.4/src/poetry_plugin_dotenv/dotenv/parsers.py` & `poetry_plugin_dotenv-1.0.0/src/poetry_plugin_dotenv/dotenv/parsers.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import dataclasses
 
 from typing import IO
 from typing import NamedTuple
 from typing import TYPE_CHECKING
 
 
-if TYPE_CHECKING:
+if TYPE_CHECKING:  # pragma: no cover
     from collections.abc import Iterator
 
 
 class Original(NamedTuple):
     """Position of the original string in the file."""
 
     string: str
@@ -62,15 +62,15 @@
 class Position:
     """Model of a cursor position."""
 
     chars: int
     line: int
 
     @classmethod
-    def start(cls) -> Position:
+    def start(cls) -> Position:  # noqa: ANN102
         """Get a start position."""
 
         return cls(chars=0, line=1)
 
     def set(self, other: Position) -> None:
         """Set a position."""
```

### Comparing `poetry_plugin_dotenv-0.8.4/PKG-INFO` & `poetry_plugin_dotenv-1.0.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,7 @@
-Metadata-Version: 2.1
-Name: poetry-plugin-dotenv
-Version: 0.8.4
-Summary: poetry-plugin-dotenv - is the plugin that automatically loads environment variables from a dotenv file into the environment before poetry commands are run.
-Home-page: https://github.com/pivoshenko/poetry-plugin-dotenv
-License: MIT
-Keywords: python,pypi,poetry,plugin,plugins,poetry-plugin,poetry-plugins,env,dotenv,config,configuration,configuration-management,cross-platform,hacktoberfest
-Author: Volodymyr Pivoshenko
-Author-email: volodymyr.pivoshenko@gmail.com
-Maintainer: Volodymyr Pivoshenko
-Maintainer-email: volodymyr.pivoshenko@gmail.com
-Requires-Python: >=3.8.1,<4.0
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Other Environment
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Information Technology
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: poetry (>=1.5.1)
-Project-URL: Documentation, https://github.com/pivoshenko/poetry-plugin-dotenv
-Project-URL: Issues, https://github.com/pivoshenko/poetry-plugin-dotenv/issues
-Project-URL: Repository, https://github.com/pivoshenko/poetry-plugin-dotenv
-Project-URL: Releases, https://github.com/pivoshenko/poetry-plugin-dotenv/releases
-Project-URL: Say Thanks!, https://www.buymeacoffee.com/pivoshenko
-Description-Content-Type: text/markdown
-
 <div align="center">
     <img alt="logo" src="https://github.com/pivoshenko/poetry-plugin-dotenv/blob/main/docs/assets/logo.svg?raw=True" height=200>
 </div>
 
 <p align="center">
     <a href="https://opensource.org/licenses/MIT">
         <img alt="license" src="https://img.shields.io/pypi/l/poetry-plugin-dotenv?logo=opensourceinitiative">
@@ -129,92 +91,154 @@
         <img alt="standwithukraine" src="https://img.shields.io/badge/made_in-Ukraine-ffd700.svg?labelColor=0057b7">
     </a>
 </p>
 
 - [Overview](#overview)
   - [Features](#features)
 - [Installation](#installation)
-- [Usage](#usage)
+- [Usage and Configuration](#usage-and-configuration)
+  - [Configuration via file](#configuration-via-file)
+  - [Configuration via environment variables](#configuration-via-environment-variables)
+  - [Lookup hierarchy](#lookup-hierarchy)
+- [Examples](#examples)
 
 ## Overview
 
 `poetry-plugin-dotenv` - is the plugin that automatically loads environment variables from a dotenv file into the environment before `poetry` commands are run.
 
 ### Features
 
 - Doesn't require any dependencies
 - Supports templates, interpolating variables using POSIX variable expansions
 - Fully type safe
-- 100% tests coverage and "A" grade for maintainability
+- 100% test coverage and "A" grade for maintainability
 
 ## Installation
 
 ```bash
 poetry self add poetry-plugin-dotenv
 ```
 
-## Usage
+## Usage and Configuration
+
+By default, the plugin will load the `.env` file from the current working directory or "higher directories".
+
+To prevent `poetry` from loading the dotenv file, set the `ignore` option.
+
+If your dotenv file is located in a different path or has a different name you may set the `location`.
+
+`ignore` option can accept the next values:
+- As True: `y / yes / t / on / 1 / true`
+- As False: `n / no / f / off / 0 / false`
+
+### Configuration via file
+
+The plugin is able to read project-specific default values for its options from a `pyproject.toml` file.
+By default, `poetry-plugin-dotenv` looks for `pyproject.toml` containing a `[tool.poetry.plugins.dotenv]` section.
+
+Example `pyproject.toml`:
+
+```toml
+[tool.poetry.plugins.dotenv]
+ignore = "false"
+location = ".env.dev"
+```
+
+> [!IMPORTANT]
+> Due to the default `poetry` parser, options in the plugins sections should be always strings.
+
+### Configuration via environment variables
+
+`poetry-plugin-dotenv` supports the following configuration options via environment variables.
+
+- `POETRY_PLUGIN_DOTENV_LOCATION`
+- `POETRY_PLUGIN_DOTENV_IGNORE`
 
-By default, plugin will load the `.env` file from the current working directory or "higher directories".
+> [!IMPORTANT]
+> Due to the nature of environment variables, options should be always strings.
 
-To prevent ``poetry`` from loading the dotenv file, set the ``POETRY_DONT_LOAD_DOTENV`` environment variable.
+### Lookup hierarchy
 
-If your dotenv file is located in a different path or has a different name you may set the ``POETRY_DOTENV_LOCATION`` environment variable.
+A `pyproject.toml` can override default values. Options provided by the user via environment variables override both.
+
+## Examples
 
 <img alt="demo" src="https://github.com/pivoshenko/poetry-plugin-dotenv/blob/main/docs/assets/demo.gif?raw=True">
 
 ```dotenv
 # .env
 DB__HOST=localhost
-DB__DBNAME=prod
-DB__USER=admin
-DB__PASSWORD=admin
+DB__DBNAME=local_lakehouse
+DB__USER=volodymyr
+DB__PASSWORD=super_secret_password
 DB__ENGINE=postgresql://${DB__USER}:${DB__PASSWORD}@${DB__HOST}/${DB__DBNAME}
 ```
 
 ```dotenv
 # .env.dev
-DB__HOST=localhost
-DB__DBNAME=dev
-DB__USER=root
-DB__PASSWORD=root
+DB__HOST=dev.host
+DB__DBNAME=dev_lakehouse
+DB__USER=svc_team
+DB__PASSWORD=super_secret_password
 DB__ENGINE=postgresql://${DB__USER}:${DB__PASSWORD}@${DB__HOST}/${DB__DBNAME}
 ```
 
+```toml
+# pyroject.toml
+[tool.poetry.plugins.dotenv]
+location = ".env.dev"
+```
+
 ```python
 # main.py
+from __future__ import annotations
+
 import os
 
 
 if __name__ == "__main__":
     try:
-        print(f"Host: {os.environ['DB__HOST']!r}")
-        print(f"Name: {os.environ['DB__DBNAME']!r}")
-        print(f"Username: {os.environ['DB__USER']!r}")
-        print(f"Password: {os.environ['DB__PASSWORD']!r}")
-        print(f"Engine: {os.environ['DB__ENGINE']!r}")
+        print(f"Host: {os.environ['DB__HOST']!r}")  # noqa: T201
+        print(f"Name: {os.environ['DB__DBNAME']!r}")  # noqa: T201
+        print(f"Username: {os.environ['DB__USER']!r}")  # noqa: T201
+        print(f"Password: {os.environ['DB__PASSWORD']!r}")  # noqa: T201
+        print(f"Engine: {os.environ['DB__ENGINE']!r}")  # noqa: T201
 
     except KeyError:
-        print("Environment variables not set!")
+        print("Environment variables not set!")  # noqa: T201
 ```
 
-```bash
+```shell
 poetry run -vvv python main.py
 # Loading environment variables from '.env'.
 # Host: 'localhost'
-# Name: 'prod'
-# Username: 'admin'
-# Password: 'admin'
-# Engine 'postgresql://admin:admin@localhost/prod'
+# Name: 'local_lakehouse'
+# Username: 'volodymyr'
+# Password: 'super_secret_password'
+# Engine: 'postgresql://volodymyr:super_secret_password@localhost/local_lakehouse'
+
+# set location section in pyproject.toml
+poetry run -vvv python main.py
+# Loading environment variables from '.env.dev'.
+# Host: 'dev.host'
+# Name: 'dev_lakehouse'
+# Username: 'svc_team'
+# Password: 'super_secret_password'
+# Engine: 'postgresql://svc_team:super_secret_password@dev.host/dev_lakehouse'
 
-export POETRY_DOTENV_LOCATION=.env.dev && poetry run -vvv python main.py
+# set ignore = "true" in pyproject.toml
+poetry run -vvv python main.py
+# Not loading environment variables.
+# Environment variables not set!
+
+export POETRY_PLUGIN_DOTENV_LOCATION=.env.dev && poetry run -vvv python main.py
 # Loading environment variables from '.env.dev'.
-# Host: 'localhost'
-# Name: 'dev'
-# Username: 'root'
-# Password: 'root'
-# Engine 'postgresql://root:root@localhost/dev'
+# Host: 'dev.host'
+# Name: 'dev_lakehouse'
+# Username: 'svc_team'
+# Password: 'super_secret_password'
+# Engine: 'postgresql://svc_team:super_secret_password@dev.host/dev_lakehouse'
 
-export POETRY_DONT_LOAD_DOTENV=1 && poetry run -vvv python main.py
+export POETRY_PLUGIN_DOTENV_IGNORE=true && poetry run -vvv python main.py
 # Not loading environment variables.
+# Environment variables not set!
 ```
-
```

#### html2text {}

```diff
@@ -1,62 +1,64 @@
-Metadata-Version: 2.1 Name: poetry-plugin-dotenv Version: 0.8.4 Summary:
-poetry-plugin-dotenv - is the plugin that automatically loads environment
-variables from a dotenv file into the environment before poetry commands are
-run. Home-page: https://github.com/pivoshenko/poetry-plugin-dotenv License: MIT
-Keywords: python,pypi,poetry,plugin,plugins,poetry-plugin,poetry-
-plugins,env,dotenv,config,configuration,configuration-management,cross-
-platform,hacktoberfest Author: Volodymyr Pivoshenko Author-email:
-volodymyr.pivoshenko@gmail.com Maintainer: Volodymyr Pivoshenko Maintainer-
-email: volodymyr.pivoshenko@gmail.com Requires-Python: >=3.8.1,<4.0 Classifier:
-Development Status :: 5 - Production/Stable Classifier: Environment :: Other
-Environment Classifier: Intended Audience :: Developers Classifier: Intended
-Audience :: Information Technology Classifier: License :: OSI Approved :: MIT
-License Classifier: Natural Language :: English Classifier: Operating System ::
-OS Independent Classifier: Programming Language :: Python Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: 3.12 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Topic :: Scientific/Engineering Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Libraries Classifier: Topic ::
-Software Development :: Libraries :: Python Modules Requires-Dist: poetry
-(>=1.5.1) Project-URL: Documentation, https://github.com/pivoshenko/poetry-
-plugin-dotenv Project-URL: Issues, https://github.com/pivoshenko/poetry-plugin-
-dotenv/issues Project-URL: Repository, https://github.com/pivoshenko/poetry-
-plugin-dotenv Project-URL: Releases, https://github.com/pivoshenko/poetry-
-plugin-dotenv/releases Project-URL: Say Thanks!, https://www.buymeacoffee.com/
-pivoshenko Description-Content-Type: text/markdown
                                     [logo]
                        _[_l_i_c_e_n_s_e_]_[_p_y_t_h_o_n_]_[_p_y_p_i_]_[_r_e_l_e_a_s_e_]
         _[_b_l_a_c_k_]_[_i_s_o_r_t_]_[_r_u_f_f_]_[_m_y_p_y_]_[_s_e_m_a_n_t_i_c___r_e_l_e_a_s_e_]_[_p_o_e_t_r_y_]_[_n_u_m_p_y_d_o_c_]
              _[_d_e_p_e_n_d_a_b_o_t_]_[_C_I_]_[_C_D_]_[_D_e_p_e_n_d_e_n_c_y_ _R_e_v_i_e_w_]_[_h_o_o_k_s_]_[_w_h_e_e_l_]
               _[_c_o_d_e_c_o_v_]_[_c_o_d_e_c_l_i_m_a_t_e_]_[_d_o_w_n_l_o_a_d_s_]_[_s_t_a_r_s_]_[_w_a_k_a_t_i_m_e_]
               _[_b_u_y_m_e_a_c_o_f_f_e_e_]_[_s_t_a_n_d_w_i_t_h_u_k_r_a_i_n_e_]_[_s_t_a_n_d_w_i_t_h_u_k_r_a_i_n_e_]
 - [Overview](#overview) - [Features](#features) - [Installation](#installation)
-- [Usage](#usage) ## Overview `poetry-plugin-dotenv` - is the plugin that
-automatically loads environment variables from a dotenv file into the
-environment before `poetry` commands are run. ### Features - Doesn't require
-any dependencies - Supports templates, interpolating variables using POSIX
-variable expansions - Fully type safe - 100% tests coverage and "A" grade for
-maintainability ## Installation ```bash poetry self add poetry-plugin-dotenv
-``` ## Usage By default, plugin will load the `.env` file from the current
-working directory or "higher directories". To prevent ``poetry`` from loading
-the dotenv file, set the ``POETRY_DONT_LOAD_DOTENV`` environment variable. If
-your dotenv file is located in a different path or has a different name you may
-set the ``POETRY_DOTENV_LOCATION`` environment variable. [demo]```dotenv # .env
-DB__HOST=localhost DB__DBNAME=prod DB__USER=admin DB__PASSWORD=admin
-DB__ENGINE=postgresql://${DB__USER}:${DB__PASSWORD}@${DB__HOST}/${DB__DBNAME}
-``` ```dotenv # .env.dev DB__HOST=localhost DB__DBNAME=dev DB__USER=root
-DB__PASSWORD=root DB__ENGINE=postgresql://${DB__USER}:${DB__PASSWORD}@$
-{DB__HOST}/${DB__DBNAME} ``` ```python # main.py import os if __name__ ==
-"__main__": try: print(f"Host: {os.environ['DB__HOST']!r}") print(f"Name:
-{os.environ['DB__DBNAME']!r}") print(f"Username: {os.environ['DB__USER']!r}")
-print(f"Password: {os.environ['DB__PASSWORD']!r}") print(f"Engine: {os.environ
-['DB__ENGINE']!r}") except KeyError: print("Environment variables not set!")
-``` ```bash poetry run -vvv python main.py # Loading environment variables from
-'.env'. # Host: 'localhost' # Name: 'prod' # Username: 'admin' # Password:
-'admin' # Engine 'postgresql://admin:admin@localhost/prod' export
-POETRY_DOTENV_LOCATION=.env.dev && poetry run -vvv python main.py # Loading
-environment variables from '.env.dev'. # Host: 'localhost' # Name: 'dev' #
-Username: 'root' # Password: 'root' # Engine 'postgresql://root:root@localhost/
-dev' export POETRY_DONT_LOAD_DOTENV=1 && poetry run -vvv python main.py # Not
-loading environment variables. ```
+- [Usage and Configuration](#usage-and-configuration) - [Configuration via
+file](#configuration-via-file) - [Configuration via environment variables]
+(#configuration-via-environment-variables) - [Lookup hierarchy](#lookup-
+hierarchy) - [Examples](#examples) ## Overview `poetry-plugin-dotenv` - is the
+plugin that automatically loads environment variables from a dotenv file into
+the environment before `poetry` commands are run. ### Features - Doesn't
+require any dependencies - Supports templates, interpolating variables using
+POSIX variable expansions - Fully type safe - 100% test coverage and "A" grade
+for maintainability ## Installation ```bash poetry self add poetry-plugin-
+dotenv ``` ## Usage and Configuration By default, the plugin will load the
+`.env` file from the current working directory or "higher directories". To
+prevent `poetry` from loading the dotenv file, set the `ignore` option. If your
+dotenv file is located in a different path or has a different name you may set
+the `location`. `ignore` option can accept the next values: - As True: `y / yes
+/ t / on / 1 / true` - As False: `n / no / f / off / 0 / false` ###
+Configuration via file The plugin is able to read project-specific default
+values for its options from a `pyproject.toml` file. By default, `poetry-
+plugin-dotenv` looks for `pyproject.toml` containing a `
+[tool.poetry.plugins.dotenv]` section. Example `pyproject.toml`: ```toml
+[tool.poetry.plugins.dotenv] ignore = "false" location = ".env.dev" ``` >
+[!IMPORTANT] > Due to the default `poetry` parser, options in the plugins
+sections should be always strings. ### Configuration via environment variables
+`poetry-plugin-dotenv` supports the following configuration options via
+environment variables. - `POETRY_PLUGIN_DOTENV_LOCATION` -
+`POETRY_PLUGIN_DOTENV_IGNORE` > [!IMPORTANT] > Due to the nature of environment
+variables, options should be always strings. ### Lookup hierarchy A
+`pyproject.toml` can override default values. Options provided by the user via
+environment variables override both. ## Examples [demo]```dotenv # .env
+DB__HOST=localhost DB__DBNAME=local_lakehouse DB__USER=volodymyr
+DB__PASSWORD=super_secret_password DB__ENGINE=postgresql://${DB__USER}:$
+{DB__PASSWORD}@${DB__HOST}/${DB__DBNAME} ``` ```dotenv # .env.dev
+DB__HOST=dev.host DB__DBNAME=dev_lakehouse DB__USER=svc_team
+DB__PASSWORD=super_secret_password DB__ENGINE=postgresql://${DB__USER}:$
+{DB__PASSWORD}@${DB__HOST}/${DB__DBNAME} ``` ```toml # pyroject.toml
+[tool.poetry.plugins.dotenv] location = ".env.dev" ``` ```python # main.py from
+__future__ import annotations import os if __name__ == "__main__": try: print
+(f"Host: {os.environ['DB__HOST']!r}") # noqa: T201 print(f"Name: {os.environ
+['DB__DBNAME']!r}") # noqa: T201 print(f"Username: {os.environ['DB__USER']!r}")
+# noqa: T201 print(f"Password: {os.environ['DB__PASSWORD']!r}") # noqa: T201
+print(f"Engine: {os.environ['DB__ENGINE']!r}") # noqa: T201 except KeyError:
+print("Environment variables not set!") # noqa: T201 ``` ```shell poetry run -
+vvv python main.py # Loading environment variables from '.env'. # Host:
+'localhost' # Name: 'local_lakehouse' # Username: 'volodymyr' # Password:
+'super_secret_password' # Engine: 'postgresql://volodymyr:
+super_secret_password@localhost/local_lakehouse' # set location section in
+pyproject.toml poetry run -vvv python main.py # Loading environment variables
+from '.env.dev'. # Host: 'dev.host' # Name: 'dev_lakehouse' # Username:
+'svc_team' # Password: 'super_secret_password' # Engine: 'postgresql://
+svc_team:super_secret_password@dev.host/dev_lakehouse' # set ignore = "true" in
+pyproject.toml poetry run -vvv python main.py # Not loading environment
+variables. # Environment variables not set! export
+POETRY_PLUGIN_DOTENV_LOCATION=.env.dev && poetry run -vvv python main.py #
+Loading environment variables from '.env.dev'. # Host: 'dev.host' # Name:
+'dev_lakehouse' # Username: 'svc_team' # Password: 'super_secret_password' #
+Engine: 'postgresql://svc_team:super_secret_password@dev.host/dev_lakehouse'
+export POETRY_PLUGIN_DOTENV_IGNORE=true && poetry run -vvv python main.py # Not
+loading environment variables. # Environment variables not set! ```
```

