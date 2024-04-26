# Comparing `tmp/pysql-repo-0.6.0.tar.gz` & `tmp/pysql-repo-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysql-repo-0.6.0.tar", last modified: Thu Apr 25 15:17:45 2024, max compression
+gzip compressed data, was "pysql-repo-0.6.1.tar", last modified: Fri Apr 26 10:00:34 2024, max compression
```

## Comparing `pysql-repo-0.6.0.tar` & `pysql-repo-0.6.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:17:45.073656 pysql-repo-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)    41337 2024-04-25 15:17:45.073656 pysql-repo-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    40736 2024-04-25 15:17:35.000000 pysql-repo-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:17:45.073656 pysql-repo-0.6.0/pysql_repo/
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-25 15:17:35.000000 pysql-repo-0.6.0/pysql_repo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:17:45.073656 pysql-repo-0.6.0/pysql_repo/_constants/
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-25 15:17:35.000000 pysql-repo-0.6.0/pysql_repo/_constants/enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     5969 2024-04-25 15:17:35.000000 pysql-repo-0.6.0/pysql_repo/_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     6287 2024-04-25 15:17:35.000000 pysql-repo-0.6.0/pysql_repo/_database_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-04-25 15:17:35.000000 pysql-repo-0.6.0/pysql_repo/_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    18597 2024-04-25 15:17:35.000000 pysql-repo-0.6.0/pysql_repo/_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-25 15:17:35.000000 pysql-repo-0.6.0/pysql_repo/_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    22775 2024-04-25 15:17:35.000000 pysql-repo-0.6.0/pysql_repo/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:17:45.073656 pysql-repo-0.6.0/pysql_repo/asyncio/
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-25 15:17:35.000000 pysql-repo-0.6.0/pysql_repo/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6239 2024-04-25 15:17:35.000000 pysql-repo-0.6.0/pysql_repo/asyncio/async_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-04-25 15:17:35.000000 pysql-repo-0.6.0/pysql_repo/asyncio/async_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)    19391 2024-04-25 15:17:35.000000 pysql-repo-0.6.0/pysql_repo/asyncio/async_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-25 15:17:35.000000 pysql-repo-0.6.0/pysql_repo/asyncio/async_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:17:45.073656 pysql-repo-0.6.0/pysql_repo/libs/
--rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-04-25 15:17:35.000000 pysql-repo-0.6.0/pysql_repo/libs/file_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:17:45.073656 pysql-repo-0.6.0/pysql_repo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    41337 2024-04-25 15:17:45.000000 pysql-repo-0.6.0/pysql_repo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-25 15:17:45.000000 pysql-repo-0.6.0/pysql_repo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 15:17:45.000000 pysql-repo-0.6.0/pysql_repo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-25 15:17:45.000000 pysql-repo-0.6.0/pysql_repo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-25 15:17:45.000000 pysql-repo-0.6.0/pysql_repo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 15:17:45.073656 pysql-repo-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-25 15:17:42.000000 pysql-repo-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:00:34.950392 pysql-repo-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    41337 2024-04-26 10:00:34.950392 pysql-repo-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    40736 2024-04-26 10:00:32.000000 pysql-repo-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:00:34.946392 pysql-repo-0.6.1/pysql_repo/
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-26 10:00:32.000000 pysql-repo-0.6.1/pysql_repo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:00:34.950392 pysql-repo-0.6.1/pysql_repo/_constants/
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-26 10:00:32.000000 pysql-repo-0.6.1/pysql_repo/_constants/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5986 2024-04-26 10:00:32.000000 pysql-repo-0.6.1/pysql_repo/_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6287 2024-04-26 10:00:32.000000 pysql-repo-0.6.1/pysql_repo/_database_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-04-26 10:00:32.000000 pysql-repo-0.6.1/pysql_repo/_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18597 2024-04-26 10:00:32.000000 pysql-repo-0.6.1/pysql_repo/_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-26 10:00:32.000000 pysql-repo-0.6.1/pysql_repo/_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22775 2024-04-26 10:00:32.000000 pysql-repo-0.6.1/pysql_repo/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:00:34.950392 pysql-repo-0.6.1/pysql_repo/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-26 10:00:32.000000 pysql-repo-0.6.1/pysql_repo/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6266 2024-04-26 10:00:32.000000 pysql-repo-0.6.1/pysql_repo/asyncio/async_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-04-26 10:00:32.000000 pysql-repo-0.6.1/pysql_repo/asyncio/async_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19391 2024-04-26 10:00:32.000000 pysql-repo-0.6.1/pysql_repo/asyncio/async_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-26 10:00:32.000000 pysql-repo-0.6.1/pysql_repo/asyncio/async_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:00:34.950392 pysql-repo-0.6.1/pysql_repo/libs/
+-rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-04-26 10:00:32.000000 pysql-repo-0.6.1/pysql_repo/libs/file_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:00:34.946392 pysql-repo-0.6.1/pysql_repo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    41337 2024-04-26 10:00:34.000000 pysql-repo-0.6.1/pysql_repo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-26 10:00:34.000000 pysql-repo-0.6.1/pysql_repo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 10:00:34.000000 pysql-repo-0.6.1/pysql_repo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-26 10:00:34.000000 pysql-repo-0.6.1/pysql_repo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-26 10:00:34.000000 pysql-repo-0.6.1/pysql_repo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 10:00:34.950392 pysql-repo-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-26 10:00:34.000000 pysql-repo-0.6.1/setup.py
```

### Comparing `pysql-repo-0.6.0/PKG-INFO` & `pysql-repo-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pysql-repo
-Version: 0.6.0
+Version: 0.6.1
 Summary: A project to have a base repository class to perform select/insert/update/delete with dynamic syntax
 Home-page: https://github.com/Impro02/pysql-repo
-Download-URL: https://github.com/Impro02/pysql-repo/archive/refs/tags/0.6.0.tar.gz
+Download-URL: https://github.com/Impro02/pysql-repo/archive/refs/tags/0.6.1.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pysql-repo-0.6.0/README.md` & `pysql-repo-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `pysql-repo-0.6.0/pysql_repo/__init__.py` & `pysql-repo-0.6.1/pysql_repo/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,25 @@
+# MODULES
 import logging
 import time
 
+# SQLALCHEMY
 from sqlalchemy import Engine, event
+
+# PYSQL_REPO
 from pysql_repo._database import DataBase
 from pysql_repo._decorators import with_session
 from pysql_repo._repository import Repository
 from pysql_repo._service import Service
 from pysql_repo._utils import RelationshipOption
 from pysql_repo._constants.enum import Operators, LoadingTechnique
 
 
 logging.basicConfig()
-_logger = logging.getLogger("pysql_repo")
+_logger = logging.getLogger("pysql_repo.cursor")
 _logger.setLevel(logging.INFO)
 
 
 @event.listens_for(Engine, "before_cursor_execute")
 def before_cursor_execute(conn, cursor, statement, parameters, context, executemany):
     conn.info.setdefault("query_start_time", []).append(time.perf_counter())
     _logger.debug("Start Query: %s, {%s}", statement, parameters)
```

### Comparing `pysql-repo-0.6.0/pysql_repo/_constants/enum.py` & `pysql-repo-0.6.1/pysql_repo/_constants/enum.py`

 * *Files identical despite different names*

### Comparing `pysql-repo-0.6.0/pysql_repo/_database.py` & `pysql-repo-0.6.1/pysql_repo/_database.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # MODULES
+import logging
 from typing import Any, Generator, List, Optional
 from pathlib import Path
-from logging import Logger
 
 # SQLALCHEMY
 from sqlalchemy import text, MetaData, create_engine, Table
 from sqlalchemy.orm import DeclarativeMeta, Session, sessionmaker
 from sqlalchemy.inspection import inspect
 
 # CONTEXTLIB
@@ -13,14 +13,16 @@
 
 # UTILS
 from pysql_repo._database_base import (
     DataBase as _DataBase,
     DataBaseConfigTypedDict as _DataBaseConfigTypedDict,
 )
 
+_logger = logging.getLogger("pysql_repo.database")
+
 
 class DataBase(_DataBase):
     """
     Represents a database connection and provides methods for database operations.
 
     Args:
         _database_config (DataBaseConfigTypedDict): The configuration for the databases.
@@ -42,15 +44,14 @@
         session_factory: Context manager for creating a session.
         init_tables_from_json_files: Initializes tables from JSON files.
     """
 
     def __init__(
         self,
         databases_config: _DataBaseConfigTypedDict,
-        logger: Logger,
         base: DeclarativeMeta,
         metadata_views: Optional[List[MetaData]] = None,
         autoflush: bool = False,
         expire_on_commit: bool = False,
         echo: bool = False,
     ) -> None:
         """
@@ -58,15 +59,15 @@
 
         Args:
             databases_config (_DataBaseConfigTypedDict): A dictionary containing the configuration for the databases.
             logger (Logger): The logger object to be used for logging.
             base (DeclarativeMeta): The base class for the declarative models.
             metadata_views (List[MetaData] | None, optional): A list of metadata views. Defaults to None.
         """
-        super().__init__(databases_config, logger, base, metadata_views)
+        super().__init__(databases_config, _logger, base, metadata_views)
 
         self._engine = create_engine(
             self._database_config.get("connection_string"),
             echo=echo,
             connect_args=self._database_config.get("connect_args") or {},
         )
```

### Comparing `pysql-repo-0.6.0/pysql_repo/_database_base.py` & `pysql-repo-0.6.1/pysql_repo/_database_base.py`

 * *Files identical despite different names*

### Comparing `pysql-repo-0.6.0/pysql_repo/_decorators.py` & `pysql-repo-0.6.1/pysql_repo/_decorators.py`

 * *Files identical despite different names*

### Comparing `pysql-repo-0.6.0/pysql_repo/_repository.py` & `pysql-repo-0.6.1/pysql_repo/_repository.py`

 * *Files identical despite different names*

### Comparing `pysql-repo-0.6.0/pysql_repo/_service.py` & `pysql-repo-0.6.1/pysql_repo/_service.py`

 * *Files identical despite different names*

### Comparing `pysql-repo-0.6.0/pysql_repo/_utils.py` & `pysql-repo-0.6.1/pysql_repo/_utils.py`

 * *Files identical despite different names*

### Comparing `pysql-repo-0.6.0/pysql_repo/asyncio/async_database.py` & `pysql-repo-0.6.1/pysql_repo/asyncio/async_database.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # MODULES
-from typing import Any, Generator, List, Optional
+import logging
+from typing import Any, AsyncGenerator, List, Optional
 from pathlib import Path
-from logging import Logger
 
 # SQLALCHEMY
 from sqlalchemy import text, MetaData, Connection, Table
 from sqlalchemy.orm import DeclarativeMeta
 from sqlalchemy.inspection import inspect
 from sqlalchemy.ext.asyncio import (
     create_async_engine,
@@ -18,14 +18,16 @@
 
 # UTILS
 from pysql_repo._database_base import (
     DataBase as _DataBase,
     DataBaseConfigTypedDict as _DataBaseConfigTypedDict,
 )
 
+_logger = logging.getLogger("pysql_repo.async_database")
+
 
 class AsyncDataBase(_DataBase):
     """
     Represents an asynchronous database.
 
     Attributes:
         _database_config (DataBaseConfigTypedDict): The configuration for the databases.
@@ -47,15 +49,14 @@
         session_factory: Context manager for creating an async session.
         init_tables_from_json_files: Initializes tables from JSON files.
     """
 
     def __init__(
         self,
         databases_config: _DataBaseConfigTypedDict,
-        logger: Logger,
         base: DeclarativeMeta,
         metadata_views: Optional[List[MetaData]] = None,
         autoflush: bool = False,
         expire_on_commit: bool = False,
         echo: bool = False,
     ) -> None:
         """
@@ -66,15 +67,15 @@
             logger: The logger object to be used for logging.
             base: The base class for declarative models.
             metadata_views: Optional list of metadata views.
 
         Returns:
             None
         """
-        super().__init__(databases_config, logger, base, metadata_views)
+        super().__init__(databases_config, _logger, base, metadata_views)
 
         self._engine = create_async_engine(
             self._database_config.get("connection_string"),
             echo=echo,
             connect_args=self._database_config.get("connect_args") or {},
         )
 
@@ -108,15 +109,15 @@
                 if view.key.lower() in current_view_names:
                     await session.execute(text(f"DROP VIEW {view}"))
 
         async with self._engine.begin() as conn:
             await conn.run_sync(self._base.metadata.create_all)
 
     @asynccontextmanager
-    async def session_factory(self) -> Generator[AsyncSession, Any, None]:
+    async def session_factory(self) -> AsyncGenerator[AsyncSession, Any]:
         """
         Context manager for creating an async session.
 
         Yields:
             AsyncSession: The async session object.
 
         Raises:
```

### Comparing `pysql-repo-0.6.0/pysql_repo/asyncio/async_decorator.py` & `pysql-repo-0.6.1/pysql_repo/asyncio/async_decorator.py`

 * *Files identical despite different names*

### Comparing `pysql-repo-0.6.0/pysql_repo/asyncio/async_repository.py` & `pysql-repo-0.6.1/pysql_repo/asyncio/async_repository.py`

 * *Files identical despite different names*

### Comparing `pysql-repo-0.6.0/pysql_repo/asyncio/async_service.py` & `pysql-repo-0.6.1/pysql_repo/asyncio/async_service.py`

 * *Files identical despite different names*

### Comparing `pysql-repo-0.6.0/pysql_repo/libs/file_lib.py` & `pysql-repo-0.6.1/pysql_repo/libs/file_lib.py`

 * *Files identical despite different names*

### Comparing `pysql-repo-0.6.0/pysql_repo.egg-info/PKG-INFO` & `pysql-repo-0.6.1/pysql_repo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pysql-repo
-Version: 0.6.0
+Version: 0.6.1
 Summary: A project to have a base repository class to perform select/insert/update/delete with dynamic syntax
 Home-page: https://github.com/Impro02/pysql-repo
-Download-URL: https://github.com/Impro02/pysql-repo/archive/refs/tags/0.6.0.tar.gz
+Download-URL: https://github.com/Impro02/pysql-repo/archive/refs/tags/0.6.1.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pysql-repo-0.6.0/pysql_repo.egg-info/SOURCES.txt` & `pysql-repo-0.6.1/pysql_repo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pysql-repo-0.6.0/setup.py` & `pysql-repo-0.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = "0.6.0"
+version = "0.6.1"
 
 with open("requirements.txt") as f:
     required_packages = f.read().splitlines()
 
 setup(
     name="pysql-repo",
     version=version,
```

