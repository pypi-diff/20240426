# Comparing `tmp/sqlalchemy-hana-2.0.0.tar.gz` & `tmp/sqlalchemy_hana-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy-hana-2.0.0.tar", last modified: Sat Mar 16 08:04:59 2024, max compression
+gzip compressed data, was "sqlalchemy_hana-2.1.0.tar", last modified: Fri Apr 26 05:41:59 2024, max compression
```

## Comparing `sqlalchemy-hana-2.0.0.tar` & `sqlalchemy_hana-2.1.0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:04:59.091574 sqlalchemy-hana-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11325 2024-03-16 08:04:50.000000 sqlalchemy-hana-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    17426 2024-03-16 08:04:59.091574 sqlalchemy-hana-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15271 2024-03-16 08:04:50.000000 sqlalchemy-hana-2.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-03-16 08:04:50.000000 sqlalchemy-hana-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-16 08:04:59.091574 sqlalchemy-hana-2.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:04:59.087574 sqlalchemy-hana-2.0.0/sqlalchemy_hana/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 08:04:50.000000 sqlalchemy-hana-2.0.0/sqlalchemy_hana/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-03-16 08:04:50.000000 sqlalchemy-hana-2.0.0/sqlalchemy_hana/alembic.py
--rw-r--r--   0 runner    (1001) docker     (127)    41111 2024-03-16 08:04:50.000000 sqlalchemy-hana-2.0.0/sqlalchemy_hana/dialect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-03-16 08:04:50.000000 sqlalchemy-hana-2.0.0/sqlalchemy_hana/elements.py
--rw-r--r--   0 runner    (1001) docker     (127)     6420 2024-03-16 08:04:50.000000 sqlalchemy-hana-2.0.0/sqlalchemy_hana/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 08:04:50.000000 sqlalchemy-hana-2.0.0/sqlalchemy_hana/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-03-16 08:04:50.000000 sqlalchemy-hana-2.0.0/sqlalchemy_hana/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:04:59.087574 sqlalchemy-hana-2.0.0/sqlalchemy_hana.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17426 2024-03-16 08:04:59.000000 sqlalchemy-hana-2.0.0/sqlalchemy_hana.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-03-16 08:04:59.000000 sqlalchemy-hana-2.0.0/sqlalchemy_hana.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-16 08:04:59.000000 sqlalchemy-hana-2.0.0/sqlalchemy_hana.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-16 08:04:59.000000 sqlalchemy-hana-2.0.0/sqlalchemy_hana.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-03-16 08:04:59.000000 sqlalchemy-hana-2.0.0/sqlalchemy_hana.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-16 08:04:59.000000 sqlalchemy-hana-2.0.0/sqlalchemy_hana.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:04:59.087574 sqlalchemy-hana-2.0.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     4345 2024-03-16 08:04:50.000000 sqlalchemy-hana-2.0.0/test/test_alembic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-03-16 08:04:50.000000 sqlalchemy-hana-2.0.0/test/test_alembic_dialect_suite.py
--rw-r--r--   0 runner    (1001) docker     (127)     7111 2024-03-16 08:04:50.000000 sqlalchemy-hana-2.0.0/test/test_dialect.py
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-03-16 08:04:50.000000 sqlalchemy-hana-2.0.0/test/test_elements.py
--rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-03-16 08:04:50.000000 sqlalchemy-hana-2.0.0/test/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-03-16 08:04:50.000000 sqlalchemy-hana-2.0.0/test/test_select.py
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-03-16 08:04:50.000000 sqlalchemy-hana-2.0.0/test/test_sql_compile.py
--rw-r--r--   0 runner    (1001) docker     (127)     5520 2024-03-16 08:04:50.000000 sqlalchemy-hana-2.0.0/test/test_sqlalchemy_dialect_suite.py
--rw-r--r--   0 runner    (1001) docker     (127)     6226 2024-03-16 08:04:50.000000 sqlalchemy-hana-2.0.0/test/test_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 05:41:59.242327 sqlalchemy_hana-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11325 2024-04-26 05:41:49.000000 sqlalchemy_hana-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    17549 2024-04-26 05:41:59.242327 sqlalchemy_hana-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15394 2024-04-26 05:41:49.000000 sqlalchemy_hana-2.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-04-26 05:41:49.000000 sqlalchemy_hana-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 05:41:59.242327 sqlalchemy_hana-2.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 05:41:59.238326 sqlalchemy_hana-2.1.0/sqlalchemy_hana/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 05:41:49.000000 sqlalchemy_hana-2.1.0/sqlalchemy_hana/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-04-26 05:41:49.000000 sqlalchemy_hana-2.1.0/sqlalchemy_hana/alembic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41274 2024-04-26 05:41:49.000000 sqlalchemy_hana-2.1.0/sqlalchemy_hana/dialect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-04-26 05:41:49.000000 sqlalchemy_hana-2.1.0/sqlalchemy_hana/elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6480 2024-04-26 05:41:49.000000 sqlalchemy_hana-2.1.0/sqlalchemy_hana/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 05:41:49.000000 sqlalchemy_hana-2.1.0/sqlalchemy_hana/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-04-26 05:41:49.000000 sqlalchemy_hana-2.1.0/sqlalchemy_hana/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 05:41:59.242327 sqlalchemy_hana-2.1.0/sqlalchemy_hana.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17549 2024-04-26 05:41:59.000000 sqlalchemy_hana-2.1.0/sqlalchemy_hana.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-26 05:41:59.000000 sqlalchemy_hana-2.1.0/sqlalchemy_hana.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 05:41:59.000000 sqlalchemy_hana-2.1.0/sqlalchemy_hana.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-26 05:41:59.000000 sqlalchemy_hana-2.1.0/sqlalchemy_hana.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-26 05:41:59.000000 sqlalchemy_hana-2.1.0/sqlalchemy_hana.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-26 05:41:59.000000 sqlalchemy_hana-2.1.0/sqlalchemy_hana.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 05:41:59.242327 sqlalchemy_hana-2.1.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     4345 2024-04-26 05:41:49.000000 sqlalchemy_hana-2.1.0/test/test_alembic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-26 05:41:49.000000 sqlalchemy_hana-2.1.0/test/test_alembic_dialect_suite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7111 2024-04-26 05:41:49.000000 sqlalchemy_hana-2.1.0/test/test_dialect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-26 05:41:49.000000 sqlalchemy_hana-2.1.0/test/test_elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-04-26 05:41:49.000000 sqlalchemy_hana-2.1.0/test/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-26 05:41:49.000000 sqlalchemy_hana-2.1.0/test/test_inspector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-26 05:41:49.000000 sqlalchemy_hana-2.1.0/test/test_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-26 05:41:49.000000 sqlalchemy_hana-2.1.0/test/test_sql_compile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5520 2024-04-26 05:41:49.000000 sqlalchemy_hana-2.1.0/test/test_sqlalchemy_dialect_suite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6226 2024-04-26 05:41:49.000000 sqlalchemy_hana-2.1.0/test/test_types.py
```

### Comparing `sqlalchemy-hana-2.0.0/LICENSE` & `sqlalchemy_hana-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy-hana-2.0.0/PKG-INFO` & `sqlalchemy_hana-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-hana
-Version: 2.0.0
+Version: 2.1.0
 Summary: SQLAlchemy dialect for SAP HANA
 Author-email: Christoph Heer <christoph.heer@sap.com>
 Maintainer-email: Christoph Heer <christoph.heer@sap.com>, Kai Mueller <kai.mueller01@sap.com>
 License: Apache-2.0
 Project-URL: Repository, https://github.com/SAP/sqlalchemy-hana
 Project-URL: Issue Tracker, https://github.com/SAP/sqlalchemy-hana/issues
 Project-URL: Changelog, https://github.com/SAP/sqlalchemy-hana/blob/main/CHANGES.rst
@@ -28,26 +28,26 @@
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: sqlalchemy<3,>=1.4.0
 Requires-Dist: hdbcli~=2.10
 Provides-Extra: dev
 Requires-Dist: isort==5.13.2; extra == "dev"
-Requires-Dist: black==24.2.0; extra == "dev"
-Requires-Dist: pre-commit==3.6.2; extra == "dev"
+Requires-Dist: black==24.4.0; extra == "dev"
+Requires-Dist: pre-commit==3.7.0; extra == "dev"
 Requires-Dist: flake8==7.0.0; extra == "dev"
 Requires-Dist: pylint==3.1.0; extra == "dev"
 Requires-Dist: mypy==1.9.0; extra == "dev"
-Requires-Dist: types-hdbcli==2.19.0.20240310; extra == "dev"
-Requires-Dist: typing-extensions==4.10.0; extra == "dev"
+Requires-Dist: types-hdbcli==2.20.0.20240418; extra == "dev"
+Requires-Dist: typing-extensions==4.11.0; extra == "dev"
 Provides-Extra: test
 Requires-Dist: pytest==8.1.1; extra == "test"
-Requires-Dist: pytest-cov==4.1.0; extra == "test"
-Requires-Dist: coverage[toml]==7.4.3; extra == "test"
-Requires-Dist: diff-cover[toml]==8.0.3; extra == "test"
+Requires-Dist: pytest-cov==5.0.0; extra == "test"
+Requires-Dist: coverage[toml]==7.4.4; extra == "test"
+Requires-Dist: diff-cover[toml]==9.0.0; extra == "test"
 Provides-Extra: alembic
 Requires-Dist: alembic~=1.12; extra == "alembic"
 
 SQLAlchemy dialect for SAP HANA
 ===============================
 
 .. image:: https://api.reuse.software/badge/github.com/SAP/sqlalchemy-hana
@@ -80,14 +80,20 @@
 only be added in major releases.
 Please note, that only the following modules are considered to be part of the public API
 
 - ``sqlalchemy_hana.types``
 
 For these, only exported members (part of ``__all__`` ) are guaranteed to be stable.
 
+Supported HANA Versions/Editions
+--------------------------------
+* SAP HANA Cloud
+* SAP HANA
+* SAP HANA, express edition
+
 Getting started
 ---------------
 If you do not have access to a SAP HANA server, you can also use the
 `SAP HANA Express edition <https://www.sap.com/cmp/td/sap-hana-express-edition.html>`_.
 
 After installation of sqlalchemy-hana, you can create a engine which connects to a SAP HANA
 instance. This engine works like all other engines of SQLAlchemy.
```

### Comparing `sqlalchemy-hana-2.0.0/README.rst` & `sqlalchemy_hana-2.1.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,20 @@
 only be added in major releases.
 Please note, that only the following modules are considered to be part of the public API
 
 - ``sqlalchemy_hana.types``
 
 For these, only exported members (part of ``__all__`` ) are guaranteed to be stable.
 
+Supported HANA Versions/Editions
+--------------------------------
+* SAP HANA Cloud
+* SAP HANA
+* SAP HANA, express edition
+
 Getting started
 ---------------
 If you do not have access to a SAP HANA server, you can also use the
 `SAP HANA Express edition <https://www.sap.com/cmp/td/sap-hana-express-edition.html>`_.
 
 After installation of sqlalchemy-hana, you can create a engine which connects to a SAP HANA
 instance. This engine works like all other engines of SQLAlchemy.
```

### Comparing `sqlalchemy-hana-2.0.0/pyproject.toml` & `sqlalchemy_hana-2.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sqlalchemy-hana"
-version = "2.0.0"
+version = "2.1.0"
 description = "SQLAlchemy dialect for SAP HANA"
 keywords = ["sqlalchemy", "sap", "hana"]
 requires-python = "~=3.8"
 readme = "README.rst"
 authors = [{ name = "Christoph Heer", email = "christoph.heer@sap.com" }]
 maintainers = [
     { name = "Christoph Heer", email = "christoph.heer@sap.com" },
@@ -33,27 +33,27 @@
     "Typing :: Typed",
 ]
 dependencies = ["sqlalchemy>=1.4.0,<3", "hdbcli~=2.10"]
 
 [project.optional-dependencies]
 dev = [
     "isort==5.13.2",
-    "black==24.2.0",
-    "pre-commit==3.6.2",
+    "black==24.4.0",
+    "pre-commit==3.7.0",
     "flake8==7.0.0",
     "pylint==3.1.0",
     "mypy==1.9.0",
-    "types-hdbcli==2.19.0.20240310",
-    "typing-extensions==4.10.0",
+    "types-hdbcli==2.20.0.20240418",
+    "typing-extensions==4.11.0",
 ]
 test = [
     "pytest==8.1.1",
-    "pytest-cov==4.1.0",
-    "coverage[toml]==7.4.3",
-    "diff-cover[toml]==8.0.3",
+    "pytest-cov==5.0.0",
+    "coverage[toml]==7.4.4",
+    "diff-cover[toml]==9.0.0",
 ]
 alembic = ["alembic~=1.12"]
 
 [project.entry-points."sqlalchemy.dialects"]
 hana = "sqlalchemy_hana.dialect:HANAHDBCLIDialect"
 "hana.hdbcli" = "sqlalchemy_hana.dialect:HANAHDBCLIDialect"
 
@@ -122,14 +122,15 @@
     "too-many-ancestors",
     "too-few-public-methods",
     "too-many-public-methods",
     "too-many-function-args",
     "too-many-lines",
     "too-many-branches",
     "too-many-return-statements",
+    "duplicate-code",
 ]
 
 [tool.pylint.basic]
 good-names = ["visit_TINYINT", "visit_SMALLDECIMAL", "visit_SECONDDATE", "visit_ALPHANUM"]
 
 [tool.mypy]
 # formatting
```

### Comparing `sqlalchemy-hana-2.0.0/sqlalchemy_hana/alembic.py` & `sqlalchemy_hana-2.1.0/sqlalchemy_hana/alembic.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-hana-2.0.0/sqlalchemy_hana/dialect.py` & `sqlalchemy_hana-2.1.0/sqlalchemy_hana/dialect.py`

 * *Files 2% similar despite different names*

```diff
@@ -458,20 +458,21 @@
         return res[0]
 
 
 class HANAInspector(reflection.Inspector):
     dialect: HANAHDBCLIDialect
 
     def get_table_oid(self, table_name: str, schema: str | None = None) -> int:
-        return self.dialect.get_table_oid(
-            self.bind,  # type:ignore[arg-type]
-            table_name,
-            schema,
-            info_cache=self.info_cache,
-        )
+        with self._operation_context() as conn:
+            return self.dialect.get_table_oid(
+                conn,
+                table_name,
+                schema,
+                info_cache=self.info_cache,
+            )
 
 
 class HANAHDBCLIDialect(default.DefaultDialect):
     name = "hana"
     driver = "hdbcli"
     default_paramstyle = "qmark"
     max_identifier_length = 127
@@ -770,14 +771,15 @@
                 schema=self.denormalize_name(schema_name),
             )
         )
 
         tables = list(self.normalize_name(row[0]) for row in result.fetchall())
         return tables
 
+    @cache
     def get_temp_table_names(
         self, connection: Connection, schema: str | None = None, **kw: Any
     ) -> list[str]:
         schema_name = schema or self.default_schema_name
 
         result = connection.execute(
             sql.text(
@@ -789,14 +791,15 @@
         )
 
         temp_table_names = list(
             self.normalize_name(row[0]) for row in result.fetchall()
         )
         return temp_table_names
 
+    @cache
     def get_view_names(
         self, connection: Connection, schema: str | None = None, **kw: Any
     ) -> list[str]:
         schema_name = schema or self.default_schema_name
 
         result = connection.execute(
             sql.text(
@@ -805,14 +808,15 @@
                 schema=self.denormalize_name(schema_name),
             )
         )
 
         views = list(self.normalize_name(row[0]) for row in result.fetchall())
         return views
 
+    @cache
     def get_view_definition(
         self,
         connection: Connection,
         view_name: str,
         schema: str | None = None,
         **kw: Any,
     ) -> str:
@@ -827,14 +831,15 @@
             )
         ).scalar()
 
         if result is None:
             raise exc.NoSuchTableError()
         return result
 
+    @cache
     def get_columns(
         self,
         connection: Connection,
         table_name: str,
         schema: str | None = None,
         **kw: Any,
     ) -> list[ReflectedColumn]:
@@ -907,14 +912,15 @@
             sql.text(
                 "SELECT SEQUENCE_NAME FROM SYS.SEQUENCES "
                 "WHERE SCHEMA_NAME=:schema ORDER BY SEQUENCE_NAME"
             ).bindparams(schema=self.denormalize_name(schema_name))
         )
         return [self.normalize_name(row[0]) for row in result]
 
+    @cache
     def get_foreign_keys(
         self,
         connection: Connection,
         table_name: str,
         schema: str | None = None,
         **kw: Any,
     ) -> list[ReflectedForeignKeyConstraint]:
@@ -964,14 +970,15 @@
             foreign_keys_list,
             key=lambda foreign_key: (
                 foreign_key["name"] is not None,
                 foreign_key["name"],
             ),
         )
 
+    @cache
     def get_indexes(
         self,
         connection: Connection,
         table_name: str,
         schema: str | None = None,
         **kw: Any,
     ) -> list[ReflectedIndex]:
@@ -1014,14 +1021,15 @@
                 indexes[name]["column_names"].append(column)
 
         return sorted(
             list(indexes.values()),
             key=lambda index: (index["name"] is not None, index["name"]),
         )
 
+    @cache
     def get_pk_constraint(
         self,
         connection: Connection,
         table_name: str,
         schema: str | None = None,
         **kw: Any,
     ) -> ReflectedPrimaryKeyConstraint:
@@ -1048,14 +1056,15 @@
             constrained_columns.append(self.normalize_name(row[1]))
 
         return {
             "name": self.normalize_name(cast(str, constraint_name)),
             "constrained_columns": constrained_columns,
         }
 
+    @cache
     def get_unique_constraints(
         self,
         connection: Connection,
         table_name: str,
         schema: str | None = None,
         **kw: Any,
     ) -> list[ReflectedUniqueConstraint]:
@@ -1097,14 +1106,15 @@
             constraint["column_names"].append(self.normalize_name(column_name))
 
         return sorted(
             constraints,
             key=lambda constraint: (constraint["name"] is not None, constraint["name"]),
         )
 
+    @cache
     def get_check_constraints(
         self,
         connection: Connection,
         table_name: str,
         schema: str | None = None,
         **kw: Any,
     ) -> list[ReflectedCheckConstraint]:
@@ -1137,14 +1147,15 @@
             # technical constraints comes first
             key=lambda constraint: (
                 not constraint["name"].startswith("_SYS_"),  # type:ignore[union-attr]
                 constraint["name"],
             ),
         )
 
+    @cache
     def get_table_oid(
         self,
         connection: Connection,
         table_name: str,
         schema: str | None = None,
         **kw: Any,
     ) -> int:
@@ -1157,14 +1168,15 @@
             ).bindparams(
                 schema=self.denormalize_name(schema_name),
                 table=self.denormalize_name(table_name),
             )
         )
         return cast(int, result.scalar())
 
+    @cache
     def get_table_comment(
         self,
         connection: Connection,
         table_name: str,
         schema: str | None = None,
         **kw: Any,
     ) -> ReflectedTableComment:
```

### Comparing `sqlalchemy-hana-2.0.0/sqlalchemy_hana/elements.py` & `sqlalchemy_hana-2.1.0/sqlalchemy_hana/elements.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-hana-2.0.0/sqlalchemy_hana/errors.py` & `sqlalchemy_hana-2.1.0/sqlalchemy_hana/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,20 +138,19 @@
     ):
         return DatabaseOutOfMemoryError.from_dbapi_error(dbapi_error)
     if (
         error.errorcode == 129
         and "max number of SqlExecutor threads are exceeded" in error.errortext
     ):
         return DatabaseOverloadedError.from_dbapi_error(dbapi_error)
-    if (
-        # ERR_SQL_CONNECT_NOT_ALLOWED: user not allowed to connect from client
+    if (  # ERR_SQL_CONNECT_NOT_ALLOWED: user not allowed to connect from client
         error.errorcode == 663
         # GBA503: geo blocking service responded with a 503
         and "Error GBA503: Service is unavailable" in error.errortext
-    ):
+    ) or error.errortext == "HANA Cloud region is in maintenance window":
         return DatabaseConnectNotPossibleError.from_dbapi_error(dbapi_error)
     if (
         # 129 -> ERR_TX_ROLLBACK: transaction rolled back by an internal error
         error.errorcode in [129, 145]
         or "An error occurred while opening the channel" in error.errortext
         or "Exception in executor plan" in error.errortext
         or "DTX commit(first phase commit) failed" in error.errortext
```

### Comparing `sqlalchemy-hana-2.0.0/sqlalchemy_hana/types.py` & `sqlalchemy_hana-2.1.0/sqlalchemy_hana/types.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-hana-2.0.0/sqlalchemy_hana.egg-info/PKG-INFO` & `sqlalchemy_hana-2.1.0/sqlalchemy_hana.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-hana
-Version: 2.0.0
+Version: 2.1.0
 Summary: SQLAlchemy dialect for SAP HANA
 Author-email: Christoph Heer <christoph.heer@sap.com>
 Maintainer-email: Christoph Heer <christoph.heer@sap.com>, Kai Mueller <kai.mueller01@sap.com>
 License: Apache-2.0
 Project-URL: Repository, https://github.com/SAP/sqlalchemy-hana
 Project-URL: Issue Tracker, https://github.com/SAP/sqlalchemy-hana/issues
 Project-URL: Changelog, https://github.com/SAP/sqlalchemy-hana/blob/main/CHANGES.rst
@@ -28,26 +28,26 @@
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: sqlalchemy<3,>=1.4.0
 Requires-Dist: hdbcli~=2.10
 Provides-Extra: dev
 Requires-Dist: isort==5.13.2; extra == "dev"
-Requires-Dist: black==24.2.0; extra == "dev"
-Requires-Dist: pre-commit==3.6.2; extra == "dev"
+Requires-Dist: black==24.4.0; extra == "dev"
+Requires-Dist: pre-commit==3.7.0; extra == "dev"
 Requires-Dist: flake8==7.0.0; extra == "dev"
 Requires-Dist: pylint==3.1.0; extra == "dev"
 Requires-Dist: mypy==1.9.0; extra == "dev"
-Requires-Dist: types-hdbcli==2.19.0.20240310; extra == "dev"
-Requires-Dist: typing-extensions==4.10.0; extra == "dev"
+Requires-Dist: types-hdbcli==2.20.0.20240418; extra == "dev"
+Requires-Dist: typing-extensions==4.11.0; extra == "dev"
 Provides-Extra: test
 Requires-Dist: pytest==8.1.1; extra == "test"
-Requires-Dist: pytest-cov==4.1.0; extra == "test"
-Requires-Dist: coverage[toml]==7.4.3; extra == "test"
-Requires-Dist: diff-cover[toml]==8.0.3; extra == "test"
+Requires-Dist: pytest-cov==5.0.0; extra == "test"
+Requires-Dist: coverage[toml]==7.4.4; extra == "test"
+Requires-Dist: diff-cover[toml]==9.0.0; extra == "test"
 Provides-Extra: alembic
 Requires-Dist: alembic~=1.12; extra == "alembic"
 
 SQLAlchemy dialect for SAP HANA
 ===============================
 
 .. image:: https://api.reuse.software/badge/github.com/SAP/sqlalchemy-hana
@@ -80,14 +80,20 @@
 only be added in major releases.
 Please note, that only the following modules are considered to be part of the public API
 
 - ``sqlalchemy_hana.types``
 
 For these, only exported members (part of ``__all__`` ) are guaranteed to be stable.
 
+Supported HANA Versions/Editions
+--------------------------------
+* SAP HANA Cloud
+* SAP HANA
+* SAP HANA, express edition
+
 Getting started
 ---------------
 If you do not have access to a SAP HANA server, you can also use the
 `SAP HANA Express edition <https://www.sap.com/cmp/td/sap-hana-express-edition.html>`_.
 
 After installation of sqlalchemy-hana, you can create a engine which connects to a SAP HANA
 instance. This engine works like all other engines of SQLAlchemy.
```

### Comparing `sqlalchemy-hana-2.0.0/sqlalchemy_hana.egg-info/SOURCES.txt` & `sqlalchemy_hana-2.1.0/sqlalchemy_hana.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -15,11 +15,12 @@
 sqlalchemy_hana.egg-info/requires.txt
 sqlalchemy_hana.egg-info/top_level.txt
 test/test_alembic.py
 test/test_alembic_dialect_suite.py
 test/test_dialect.py
 test/test_elements.py
 test/test_errors.py
+test/test_inspector.py
 test/test_select.py
 test/test_sql_compile.py
 test/test_sqlalchemy_dialect_suite.py
 test/test_types.py
```

### Comparing `sqlalchemy-hana-2.0.0/test/test_alembic.py` & `sqlalchemy_hana-2.1.0/test/test_alembic.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-hana-2.0.0/test/test_alembic_dialect_suite.py` & `sqlalchemy_hana-2.1.0/test/test_alembic_dialect_suite.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-hana-2.0.0/test/test_dialect.py` & `sqlalchemy_hana-2.1.0/test/test_dialect.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-hana-2.0.0/test/test_elements.py` & `sqlalchemy_hana-2.1.0/test/test_elements.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-hana-2.0.0/test/test_errors.py` & `sqlalchemy_hana-2.1.0/test/test_errors.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,14 +56,19 @@
             ),
             (
                 663,
                 "Error GBA503: Service is unavailable",
                 DatabaseConnectNotPossibleError,
             ),
             (
+                1897,
+                "HANA Cloud region is in maintenance window",
+                DatabaseConnectNotPossibleError,
+            ),
+            (
                 129,
                 "An error occurred while opening the channel",
                 StatementExecutionError,
             ),
             (
                 2048,
                 "An error occurred while opening the channel",
```

### Comparing `sqlalchemy-hana-2.0.0/test/test_select.py` & `sqlalchemy_hana-2.1.0/test/test_select.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-hana-2.0.0/test/test_sql_compile.py` & `sqlalchemy_hana-2.1.0/test/test_sql_compile.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-hana-2.0.0/test/test_sqlalchemy_dialect_suite.py` & `sqlalchemy_hana-2.1.0/test/test_sqlalchemy_dialect_suite.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-hana-2.0.0/test/test_types.py` & `sqlalchemy_hana-2.1.0/test/test_types.py`

 * *Files identical despite different names*

