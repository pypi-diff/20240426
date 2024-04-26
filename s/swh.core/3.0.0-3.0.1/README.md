# Comparing `tmp/swh.core-3.0.0.tar.gz` & `tmp/swh_core-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swh.core-3.0.0.tar", last modified: Fri Feb  2 09:13:05 2024, max compression
+gzip compressed data, was "swh_core-3.0.1.tar", last modified: Fri Apr 26 09:58:29 2024, max compression
```

## Comparing `swh.core-3.0.0.tar` & `swh_core-3.0.1.tar`

### file list

```diff
@@ -1,168 +1,168 @@
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 09:13:05.570176 swh.core-3.0.0/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      342 2024-02-02 09:12:58.000000 swh.core-3.0.0/.copier-answers.yml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      158 2024-02-02 09:12:58.000000 swh.core-3.0.0/.git-blame-ignore-revs
--rw-r--r--   0 jenkins    (115) jenkins    (120)      356 2024-02-02 09:12:58.000000 swh.core-3.0.0/.gitignore
--rw-r--r--   0 jenkins    (115) jenkins    (120)      968 2024-02-02 09:12:58.000000 swh.core-3.0.0/.pre-commit-config.yaml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      112 2024-02-02 09:12:58.000000 swh.core-3.0.0/AUTHORS
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3397 2024-02-02 09:12:58.000000 swh.core-3.0.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 jenkins    (115) jenkins    (120)       31 2024-02-02 09:12:58.000000 swh.core-3.0.0/CONTRIBUTORS
--rw-r--r--   0 jenkins    (115) jenkins    (120)    35147 2024-02-02 09:12:58.000000 swh.core-3.0.0/LICENSE
--rw-r--r--   0 jenkins    (115) jenkins    (120)      163 2024-02-02 09:12:58.000000 swh.core-3.0.0/Makefile
--rw-r--r--   0 jenkins    (115) jenkins    (120)       95 2024-02-02 09:12:58.000000 swh.core-3.0.0/Makefile.local
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3528 2024-02-02 09:13:05.570176 swh.core-3.0.0/PKG-INFO
--rw-r--r--   0 jenkins    (115) jenkins    (120)      293 2024-02-02 09:12:58.000000 swh.core-3.0.0/README.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)      712 2024-02-02 09:12:58.000000 swh.core-3.0.0/conftest.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 09:13:05.526177 swh.core-3.0.0/docs/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-02-02 09:12:58.000000 swh.core-3.0.0/docs/.gitignore
--rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-02-02 09:12:58.000000 swh.core-3.0.0/docs/Makefile
--rw-r--r--   0 jenkins    (115) jenkins    (120)      293 2024-02-02 09:12:58.000000 swh.core-3.0.0/docs/README.rst
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 09:13:05.526177 swh.core-3.0.0/docs/_static/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-02-02 09:12:58.000000 swh.core-3.0.0/docs/_static/.placeholder
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 09:13:05.526177 swh.core-3.0.0/docs/_templates/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-02-02 09:12:58.000000 swh.core-3.0.0/docs/_templates/.placeholder
--rw-r--r--   0 jenkins    (115) jenkins    (120)      383 2024-02-02 09:12:58.000000 swh.core-3.0.0/docs/cli.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)       43 2024-02-02 09:12:58.000000 swh.core-3.0.0/docs/conf.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6486 2024-02-02 09:12:58.000000 swh.core-3.0.0/docs/db.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)      273 2024-02-02 09:12:58.000000 swh.core-3.0.0/docs/index.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)      982 2024-02-02 09:12:58.000000 swh.core-3.0.0/mypy.ini
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2117 2024-02-02 09:12:58.000000 swh.core-3.0.0/pyproject.toml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      157 2024-02-02 09:12:58.000000 swh.core-3.0.0/pytest.ini
--rw-r--r--   0 jenkins    (115) jenkins    (120)       58 2024-02-02 09:12:58.000000 swh.core-3.0.0/requirements-db.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      147 2024-02-02 09:12:58.000000 swh.core-3.0.0/requirements-http.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)       15 2024-02-02 09:12:58.000000 swh.core-3.0.0/requirements-logging.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-02-02 09:12:58.000000 swh.core-3.0.0/requirements-swh.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      152 2024-02-02 09:12:58.000000 swh.core-3.0.0/requirements-test.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)       66 2024-02-02 09:12:58.000000 swh.core-3.0.0/requirements.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      120 2024-02-02 09:13:05.570176 swh.core-3.0.0/setup.cfg
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 09:13:05.526177 swh.core-3.0.0/swh/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      143 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/__main__.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 09:13:05.534176 swh.core-3.0.0/swh/core/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/__init__.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 09:13:05.534176 swh.core-3.0.0/swh/core/api/
--rw-r--r--   0 jenkins    (115) jenkins    (120)    20373 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/api/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6379 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/api/asynchronous.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2073 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/api/classes.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1192 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/api/gunicorn_config.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5812 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/api/negotiation.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    10114 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/api/serializers.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 09:13:05.538176 swh.core-3.0.0/swh/core/api/tests/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/api/tests/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/api/tests/conftest.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4292 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/api/tests/server_testing.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     7863 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/api/tests/test_async.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2755 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/api/tests/test_classes.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4879 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/api/tests/test_gunicorn.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      862 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/api/tests/test_init.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6129 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/api/tests/test_rpc_client.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5170 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/api/tests/test_rpc_client_server.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     7968 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/api/tests/test_rpc_server.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4871 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/api/tests/test_rpc_server_asynchronous.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8925 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/api/tests/test_serializers.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)       63 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/api_async.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 09:13:05.538176 swh.core-3.0.0/swh/core/cli/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5496 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/cli/__init__.py
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)    14013 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/cli/db.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2044 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/collections.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     9207 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/config.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 09:13:05.538176 swh.core-3.0.0/swh/core/db/
--rw-r--r--   0 jenkins    (115) jenkins    (120)    10619 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/db/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4888 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/db/common.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    24051 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/db/db_utils.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 09:13:05.538176 swh.core-3.0.0/swh/core/db/sql/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      664 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/db/sql/35-dbversion.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      683 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/db/sql/36-dbmodule.sql
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 09:13:05.542176 swh.core-3.0.0/swh/core/db/tests/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/db/tests/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2554 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/db/tests/conftest.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 09:13:05.514177 swh.core-3.0.0/swh/core/db/tests/data/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 09:13:05.514177 swh.core-3.0.0/swh/core/db/tests/data/cli/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 09:13:05.542176 swh.core-3.0.0/swh/core/db/tests/data/cli/sql/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       41 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/db/tests/data/cli/sql/0-superuser-init.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      790 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/db/tests/data/cli/sql/15-flavor.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      137 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/db/tests/data/cli/sql/30-schema.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      156 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/db/tests/data/cli/sql/40-funcs.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      126 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/db/tests/data/cli/sql/50-data.sql
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 09:13:05.546176 swh.core-3.0.0/swh/core/db/tests/data/cli/sql/upgrades/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      199 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/db/tests/data/cli/sql/upgrades/001.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)       82 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/db/tests/data/cli/sql/upgrades/002.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)       82 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/db/tests/data/cli/sql/upgrades/003.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)       82 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/db/tests/data/cli/sql/upgrades/004.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      306 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/db/tests/data/cli/sql/upgrades/005-bis.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)       82 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/db/tests/data/cli/sql/upgrades/005.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      196 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/db/tests/data/cli/sql/upgrades/006.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)    15397 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/db/tests/test_cli.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    13826 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/db/tests/test_db.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     9400 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/db/tests/test_db_utils.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 09:13:05.546176 swh.core-3.0.0/swh/core/github/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/github/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6612 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/github/pytest_plugin.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 09:13:05.546176 swh.core-3.0.0/swh/core/github/tests/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/github/tests/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    14265 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/github/tests/test_github_utils.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1440 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/github/tests/test_pytest_plugin.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    11211 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/github/utils.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4331 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/logger.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2583 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/logging.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)       27 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/py.typed
--rw-r--r--   0 jenkins    (115) jenkins    (120)    12543 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/pytest_plugin.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3271 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/retry.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3355 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/sentry.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    16759 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/statsd.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8364 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/tarball.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 09:13:05.550176 swh.core-3.0.0/swh/core/tests/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       98 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 09:13:05.550176 swh.core-3.0.0/swh/core/tests/data/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 09:13:05.558176 swh.core-3.0.0/swh/core/tests/data/archives/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2028 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/tests/data/archives/ca-certificates-20210603-1-any.pkg.tar.zst
--rw-r--r--   0 jenkins    (115) jenkins    (120)  1087901 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/tests/data/archives/groff-1.02.tar.Z
--rw-r--r--   0 jenkins    (115) jenkins    (120)      550 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/tests/data/archives/hello.jar
--rw-r--r--   0 jenkins    (115) jenkins    (120)    10240 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/tests/data/archives/hello.tar
--rw-r--r--   0 jenkins    (115) jenkins    (120)      199 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/tests/data/archives/hello.tar.bz2
--rw-r--r--   0 jenkins    (115) jenkins    (120)      181 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/tests/data/archives/hello.tar.gz
--rw-r--r--   0 jenkins    (115) jenkins    (120)      190 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/tests/data/archives/hello.tar.lz
--rw-r--r--   0 jenkins    (115) jenkins    (120)    10240 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/tests/data/archives/hello.tar.x
--rw-r--r--   0 jenkins    (115) jenkins    (120)      199 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/tests/data/archives/hello.tbz
--rw-r--r--   0 jenkins    (115) jenkins    (120)      199 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/tests/data/archives/hello.tbz2
--rw-r--r--   0 jenkins    (115) jenkins    (120)      551 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/tests/data/archives/hello.war
--rw-r--r--   0 jenkins    (115) jenkins    (120)      162 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/tests/data/archives/hello.zip
--rw-r--r--   0 jenkins    (115) jenkins    (120)   845917 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/tests/data/archives/msk316src.zip
--rw-r--r--   0 jenkins    (115) jenkins    (120)    45185 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/tests/data/archives/tokei-12.1.2.crate
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 09:13:05.558176 swh.core-3.0.0/swh/core/tests/data/http_example.com/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       12 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/tests/data/http_example.com/something.json
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 09:13:05.558176 swh.core-3.0.0/swh/core/tests/data/https_example.com/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       23 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/tests/data/https_example.com/file.json
--rw-r--r--   0 jenkins    (115) jenkins    (120)       28 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/tests/data/https_example.com/file.json,name=doe,firstname=jane
--rw-r--r--   0 jenkins    (115) jenkins    (120)       25 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/tests/data/https_example.com/file.json_visit1
--rw-r--r--   0 jenkins    (115) jenkins    (120)        9 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/tests/data/https_example.com/other.json
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 09:13:05.558176 swh.core-3.0.0/swh/core/tests/data/https_forge.s.o/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       12 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/tests/data/https_forge.s.o/api_diffusion,attachments[uris]=1
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 09:13:05.558176 swh.core-3.0.0/swh/core/tests/data/https_www.reference.com/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       17 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/tests/data/https_www.reference.com/web,q=What+Is+an+Example+of+a+URL?,qo=contentPageRelatedSearch,o=600605,l=dir,sga=1
--rw-r--r--   0 jenkins    (115) jenkins    (120)      642 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/tests/data/logging-config.yaml
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 09:13:05.562176 swh.core-3.0.0/swh/core/tests/fixture/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/tests/fixture/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      401 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/tests/fixture/conftest.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 09:13:05.514177 swh.core-3.0.0/swh/core/tests/fixture/data/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 09:13:05.562176 swh.core-3.0.0/swh/core/tests/fixture/data/https_example.com/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       25 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/tests/fixture/data/https_example.com/file.json
--rw-r--r--   0 jenkins    (115) jenkins    (120)      797 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/tests/fixture/test_pytest_plugin.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    11839 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/tests/test_cli.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2439 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/tests/test_collections.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    10147 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/tests/test_config.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3738 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/tests/test_logger.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2826 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/tests/test_logging.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4018 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/tests/test_pytest_plugin.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2580 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/tests/test_retry.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4483 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/tests/test_sentry.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    18746 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/tests/test_statsd.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     9873 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/tests/test_tarball.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5422 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/tests/test_utils.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5788 2024-02-02 09:12:58.000000 swh.core-3.0.0/swh/core/utils.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 09:13:05.562176 swh.core-3.0.0/swh.core.egg-info/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3528 2024-02-02 09:13:05.000000 swh.core-3.0.0/swh.core.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4363 2024-02-02 09:13:05.000000 swh.core-3.0.0/swh.core.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)        1 2024-02-02 09:13:05.000000 swh.core-3.0.0/swh.core.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      148 2024-02-02 09:13:05.000000 swh.core-3.0.0/swh.core.egg-info/entry_points.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      648 2024-02-02 09:13:05.000000 swh.core-3.0.0/swh.core.egg-info/requires.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)        4 2024-02-02 09:13:05.000000 swh.core-3.0.0/swh.core.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1866 2024-02-02 09:12:58.000000 swh.core-3.0.0/tox.ini
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:29.350315 swh_core-3.0.1/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      342 2024-04-26 09:58:23.000000 swh_core-3.0.1/.copier-answers.yml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      158 2024-04-26 09:58:23.000000 swh_core-3.0.1/.git-blame-ignore-revs
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      356 2024-04-26 09:58:23.000000 swh_core-3.0.1/.gitignore
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1410 2024-04-26 09:58:23.000000 swh_core-3.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      112 2024-04-26 09:58:23.000000 swh_core-3.0.1/AUTHORS
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3397 2024-04-26 09:58:23.000000 swh_core-3.0.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       31 2024-04-26 09:58:23.000000 swh_core-3.0.1/CONTRIBUTORS
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    35147 2024-04-26 09:58:23.000000 swh_core-3.0.1/LICENSE
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      163 2024-04-26 09:58:23.000000 swh_core-3.0.1/Makefile
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       95 2024-04-26 09:58:23.000000 swh_core-3.0.1/Makefile.local
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3541 2024-04-26 09:58:29.350315 swh_core-3.0.1/PKG-INFO
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      293 2024-04-26 09:58:23.000000 swh_core-3.0.1/README.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      712 2024-04-26 09:58:23.000000 swh_core-3.0.1/conftest.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:29.306316 swh_core-3.0.1/docs/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-04-26 09:58:23.000000 swh_core-3.0.1/docs/.gitignore
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-04-26 09:58:23.000000 swh_core-3.0.1/docs/Makefile
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      293 2024-04-26 09:58:23.000000 swh_core-3.0.1/docs/README.rst
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:29.306316 swh_core-3.0.1/docs/_static/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:23.000000 swh_core-3.0.1/docs/_static/.placeholder
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:29.306316 swh_core-3.0.1/docs/_templates/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:23.000000 swh_core-3.0.1/docs/_templates/.placeholder
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      383 2024-04-26 09:58:23.000000 swh_core-3.0.1/docs/cli.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       43 2024-04-26 09:58:23.000000 swh_core-3.0.1/docs/conf.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6486 2024-04-26 09:58:23.000000 swh_core-3.0.1/docs/db.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      273 2024-04-26 09:58:23.000000 swh_core-3.0.1/docs/index.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      982 2024-04-26 09:58:23.000000 swh_core-3.0.1/mypy.ini
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2117 2024-04-26 09:58:23.000000 swh_core-3.0.1/pyproject.toml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      156 2024-04-26 09:58:23.000000 swh_core-3.0.1/pytest.ini
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       58 2024-04-26 09:58:23.000000 swh_core-3.0.1/requirements-db.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      147 2024-04-26 09:58:23.000000 swh_core-3.0.1/requirements-http.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       15 2024-04-26 09:58:23.000000 swh_core-3.0.1/requirements-logging.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:23.000000 swh_core-3.0.1/requirements-swh.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      159 2024-04-26 09:58:23.000000 swh_core-3.0.1/requirements-test.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       71 2024-04-26 09:58:23.000000 swh_core-3.0.1/requirements.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      120 2024-04-26 09:58:29.350315 swh_core-3.0.1/setup.cfg
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:29.306316 swh_core-3.0.1/swh/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      143 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/__main__.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:29.310316 swh_core-3.0.1/swh/core/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/__init__.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:29.314316 swh_core-3.0.1/swh/core/api/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    20373 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/api/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6379 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/api/asynchronous.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2073 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/api/classes.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1192 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/api/gunicorn_config.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5812 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/api/negotiation.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    10114 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/api/serializers.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:29.318316 swh_core-3.0.1/swh/core/api/tests/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/api/tests/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/api/tests/conftest.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4292 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/api/tests/server_testing.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     7863 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/api/tests/test_async.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2755 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/api/tests/test_classes.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5404 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/api/tests/test_gunicorn.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      862 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/api/tests/test_init.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6129 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/api/tests/test_rpc_client.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5170 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/api/tests/test_rpc_client_server.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     7968 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/api/tests/test_rpc_server.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4871 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/api/tests/test_rpc_server_asynchronous.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8925 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/api/tests/test_serializers.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       63 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/api_async.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:29.318316 swh_core-3.0.1/swh/core/cli/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5496 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/cli/__init__.py
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)    14013 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/cli/db.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2044 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/collections.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     9207 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/config.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:29.318316 swh_core-3.0.1/swh/core/db/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    10619 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/db/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4888 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/db/common.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    24051 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/db/db_utils.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:29.318316 swh_core-3.0.1/swh/core/db/sql/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      664 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/db/sql/35-dbversion.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      683 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/db/sql/36-dbmodule.sql
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:29.322316 swh_core-3.0.1/swh/core/db/tests/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/db/tests/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2554 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/db/tests/conftest.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:29.294316 swh_core-3.0.1/swh/core/db/tests/data/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:29.294316 swh_core-3.0.1/swh/core/db/tests/data/cli/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:29.322316 swh_core-3.0.1/swh/core/db/tests/data/cli/sql/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       41 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/db/tests/data/cli/sql/0-superuser-init.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      790 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/db/tests/data/cli/sql/15-flavor.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      137 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/db/tests/data/cli/sql/30-schema.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      156 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/db/tests/data/cli/sql/40-funcs.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      126 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/db/tests/data/cli/sql/50-data.sql
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:29.326315 swh_core-3.0.1/swh/core/db/tests/data/cli/sql/upgrades/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      199 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/db/tests/data/cli/sql/upgrades/001.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       82 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/db/tests/data/cli/sql/upgrades/002.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       82 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/db/tests/data/cli/sql/upgrades/003.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       82 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/db/tests/data/cli/sql/upgrades/004.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      306 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/db/tests/data/cli/sql/upgrades/005-bis.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       82 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/db/tests/data/cli/sql/upgrades/005.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      196 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/db/tests/data/cli/sql/upgrades/006.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    15397 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/db/tests/test_cli.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    13826 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/db/tests/test_db.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     9400 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/db/tests/test_db_utils.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:29.326315 swh_core-3.0.1/swh/core/github/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/github/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6612 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/github/pytest_plugin.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:29.326315 swh_core-3.0.1/swh/core/github/tests/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/github/tests/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    14265 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/github/tests/test_github_utils.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1440 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/github/tests/test_pytest_plugin.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    11211 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/github/utils.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4331 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/logger.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2583 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/logging.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       27 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/py.typed
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    12994 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/pytest_plugin.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3271 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/retry.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3603 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/sentry.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    16759 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/statsd.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8364 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tarball.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:29.330315 swh_core-3.0.1/swh/core/tests/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       98 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:29.330315 swh_core-3.0.1/swh/core/tests/data/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:29.338315 swh_core-3.0.1/swh/core/tests/data/archives/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2028 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/data/archives/ca-certificates-20210603-1-any.pkg.tar.zst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)  1087901 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/data/archives/groff-1.02.tar.Z
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      550 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/data/archives/hello.jar
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    10240 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/data/archives/hello.tar
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      199 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/data/archives/hello.tar.bz2
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      181 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/data/archives/hello.tar.gz
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      190 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/data/archives/hello.tar.lz
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    10240 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/data/archives/hello.tar.x
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      199 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/data/archives/hello.tbz
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      199 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/data/archives/hello.tbz2
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      551 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/data/archives/hello.war
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      162 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/data/archives/hello.zip
+-rw-r--r--   0 jenkins    (115) jenkins    (120)   845917 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/data/archives/msk316src.zip
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    45185 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/data/archives/tokei-12.1.2.crate
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:29.338315 swh_core-3.0.1/swh/core/tests/data/http_example.com/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       12 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/data/http_example.com/something.json
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:29.338315 swh_core-3.0.1/swh/core/tests/data/https_example.com/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       23 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/data/https_example.com/file.json
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       28 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/data/https_example.com/file.json,name=doe,firstname=jane
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       25 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/data/https_example.com/file.json_visit1
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        9 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/data/https_example.com/other.json
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:29.338315 swh_core-3.0.1/swh/core/tests/data/https_forge.s.o/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       12 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/data/https_forge.s.o/api_diffusion,attachments[uris]=1
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:29.338315 swh_core-3.0.1/swh/core/tests/data/https_www.reference.com/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       17 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/data/https_www.reference.com/web,q=What+Is+an+Example+of+a+URL?,qo=contentPageRelatedSearch,o=600605,l=dir,sga=1
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      642 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/data/logging-config.yaml
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:29.342315 swh_core-3.0.1/swh/core/tests/fixture/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/fixture/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      401 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/fixture/conftest.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:29.294316 swh_core-3.0.1/swh/core/tests/fixture/data/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:29.342315 swh_core-3.0.1/swh/core/tests/fixture/data/https_example.com/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       25 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/fixture/data/https_example.com/file.json
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      797 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/fixture/test_pytest_plugin.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    11911 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/test_cli.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2439 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/test_collections.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    10147 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/test_config.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3738 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/test_logger.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2826 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/test_logging.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4018 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/test_pytest_plugin.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2580 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/test_retry.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4879 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/test_sentry.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    18746 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/test_statsd.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     9873 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/test_tarball.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5422 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/test_utils.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5788 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/utils.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:29.342315 swh_core-3.0.1/swh.core.egg-info/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3541 2024-04-26 09:58:29.000000 swh_core-3.0.1/swh.core.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4363 2024-04-26 09:58:29.000000 swh_core-3.0.1/swh.core.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        1 2024-04-26 09:58:29.000000 swh_core-3.0.1/swh.core.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      148 2024-04-26 09:58:29.000000 swh_core-3.0.1/swh.core.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      661 2024-04-26 09:58:29.000000 swh_core-3.0.1/swh.core.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        4 2024-04-26 09:58:29.000000 swh_core-3.0.1/swh.core.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1550 2024-04-26 09:58:23.000000 swh_core-3.0.1/tox.ini
```

### Comparing `swh.core-3.0.0/CODE_OF_CONDUCT.md` & `swh_core-3.0.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `swh.core-3.0.0/LICENSE` & `swh_core-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `swh.core-3.0.0/PKG-INFO` & `swh_core-3.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.core
-Version: 3.0.0
+Version: 3.0.1
 Summary: Software Heritage core utilities
 Author-email: Software Heritage developers <swh-devel@inria.fr>
 Project-URL: Homepage, https://gitlab.softwareheritage.org/swh/devel/swh-core
 Project-URL: Bug Reports, https://gitlab.softwareheritage.org/swh/devel/swh-core/-/issues
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Documentation, https://docs.softwareheritage.org/devel/swh-core/
 Project-URL: Source, https://gitlab.softwareheritage.org/swh/devel/swh-core.git
@@ -18,19 +18,19 @@
 License-File: LICENSE
 License-File: AUTHORS
 Requires-Dist: click
 Requires-Dist: deprecated
 Requires-Dist: python-magic
 Requires-Dist: pyyaml
 Requires-Dist: requests
-Requires-Dist: sentry-sdk
+Requires-Dist: sentry-sdk>=2
 Requires-Dist: tenacity
 Provides-Extra: testing-core
 Requires-Dist: hypothesis>=3.11.0; extra == "testing-core"
-Requires-Dist: pytest; extra == "testing-core"
+Requires-Dist: pytest>=8.1; extra == "testing-core"
 Requires-Dist: pytest-mock; extra == "testing-core"
 Requires-Dist: pytest-postgresql>5; extra == "testing-core"
 Requires-Dist: pytz; extra == "testing-core"
 Requires-Dist: requests-mock; extra == "testing-core"
 Requires-Dist: types-deprecated; extra == "testing-core"
 Requires-Dist: types-psycopg2; extra == "testing-core"
 Requires-Dist: types-pytz; extra == "testing-core"
@@ -47,15 +47,15 @@
 Requires-Dist: blinker; extra == "http"
 Requires-Dist: flask; extra == "http"
 Requires-Dist: iso8601; extra == "http"
 Requires-Dist: msgpack>=1.0.0; extra == "http"
 Requires-Dist: requests; extra == "http"
 Provides-Extra: testing
 Requires-Dist: hypothesis>=3.11.0; extra == "testing"
-Requires-Dist: pytest; extra == "testing"
+Requires-Dist: pytest>=8.1; extra == "testing"
 Requires-Dist: pytest-mock; extra == "testing"
 Requires-Dist: pytest-postgresql>5; extra == "testing"
 Requires-Dist: pytz; extra == "testing"
 Requires-Dist: requests-mock; extra == "testing"
 Requires-Dist: types-deprecated; extra == "testing"
 Requires-Dist: types-psycopg2; extra == "testing"
 Requires-Dist: types-pytz; extra == "testing"
```

### Comparing `swh.core-3.0.0/conftest.py` & `swh_core-3.0.1/conftest.py`

 * *Files identical despite different names*

### Comparing `swh.core-3.0.0/docs/db.rst` & `swh_core-3.0.1/docs/db.rst`

 * *Files identical despite different names*

### Comparing `swh.core-3.0.0/mypy.ini` & `swh_core-3.0.1/mypy.ini`

 * *Files identical despite different names*

### Comparing `swh.core-3.0.0/pyproject.toml` & `swh_core-3.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `swh.core-3.0.0/swh/core/api/__init__.py` & `swh_core-3.0.1/swh/core/api/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.core-3.0.0/swh/core/api/asynchronous.py` & `swh_core-3.0.1/swh/core/api/asynchronous.py`

 * *Files identical despite different names*

### Comparing `swh.core-3.0.0/swh/core/api/classes.py` & `swh_core-3.0.1/swh/core/api/classes.py`

 * *Files identical despite different names*

### Comparing `swh.core-3.0.0/swh/core/api/gunicorn_config.py` & `swh_core-3.0.1/swh/core/api/gunicorn_config.py`

 * *Files identical despite different names*

### Comparing `swh.core-3.0.0/swh/core/api/negotiation.py` & `swh_core-3.0.1/swh/core/api/negotiation.py`

 * *Files identical despite different names*

### Comparing `swh.core-3.0.0/swh/core/api/serializers.py` & `swh_core-3.0.1/swh/core/api/serializers.py`

 * *Files identical despite different names*

### Comparing `swh.core-3.0.0/swh/core/api/tests/server_testing.py` & `swh_core-3.0.1/swh/core/api/tests/server_testing.py`

 * *Files identical despite different names*

### Comparing `swh.core-3.0.0/swh/core/api/tests/test_async.py` & `swh_core-3.0.1/swh/core/api/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `swh.core-3.0.0/swh/core/api/tests/test_classes.py` & `swh_core-3.0.1/swh/core/api/tests/test_classes.py`

 * *Files identical despite different names*

### Comparing `swh.core-3.0.0/swh/core/api/tests/test_gunicorn.py` & `swh_core-3.0.1/swh/core/api/tests/test_gunicorn.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,156 +1,180 @@
-# Copyright (C) 2019  The Software Heritage developers
+# Copyright (C) 2019-2024  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 import os
-from unittest.mock import patch
 
 import pkg_resources
 
 import swh.core.api.gunicorn_config as gunicorn_config
 
 
-def test_post_fork_default():
-    with patch("sentry_sdk.init") as sentry_sdk_init:
-        gunicorn_config.post_fork(None, None)
+def test_post_fork_default(mocker):
+    flask_integration = object()  # unique object to check for equality
+    logging_integration = object()  # unique object to check for equality
+    mocker.patch(
+        "sentry_sdk.integrations.flask.FlaskIntegration", new=lambda: flask_integration
+    )
+    mocker.patch(
+        "sentry_sdk.integrations.logging.LoggingIntegration",
+        new=lambda event_level: logging_integration,
+    )
+    sentry_sdk_init = mocker.patch("sentry_sdk.init")
 
-    sentry_sdk_init.assert_not_called()
+    gunicorn_config.post_fork(None, None)
 
+    sentry_sdk_init.assert_called_once_with(
+        dsn=None,
+        integrations=[flask_integration, logging_integration],
+        debug=False,
+        release=None,
+        environment=None,
+    )
 
-def test_post_fork_with_dsn_env():
+
+def test_post_fork_with_dsn_env(mocker):
     flask_integration = object()  # unique object to check for equality
     logging_integration = object()  # unique object to check for equality
-    with patch(
+    mocker.patch(
         "sentry_sdk.integrations.flask.FlaskIntegration", new=lambda: flask_integration
-    ), patch(
+    )
+    mocker.patch(
         "sentry_sdk.integrations.logging.LoggingIntegration",
         new=lambda event_level: logging_integration,
-    ), patch(
-        "sentry_sdk.init"
-    ) as sentry_sdk_init, patch.dict(
-        os.environ, {"SWH_SENTRY_DSN": "test_dsn"}
-    ):
-        gunicorn_config.post_fork(None, None)
+    )
+    sentry_sdk_init = mocker.patch("sentry_sdk.init")
+    mocker.patch.dict(os.environ, {"SWH_SENTRY_DSN": "test_dsn"})
+
+    gunicorn_config.post_fork(None, None)
 
     sentry_sdk_init.assert_called_once_with(
         dsn="test_dsn",
         integrations=[flask_integration, logging_integration],
         debug=False,
         release=None,
         environment=None,
     )
 
 
-def test_post_fork_with_package_env():
+def test_post_fork_with_package_env(mocker):
     flask_integration = object()
     logging_integration = object()
 
-    with patch(
+    mocker.patch(
         "sentry_sdk.integrations.flask.FlaskIntegration", new=lambda: flask_integration
-    ), patch(
+    )
+    mocker.patch(
         "sentry_sdk.integrations.logging.LoggingIntegration",
         new=lambda event_level: logging_integration,
-    ), patch(
-        "sentry_sdk.init"
-    ) as sentry_sdk_init, patch.dict(
+    )
+    sentry_sdk_init = mocker.patch("sentry_sdk.init")
+    mocker.patch.dict(
         os.environ,
         {
             "SWH_SENTRY_DSN": "test_dsn",
             "SWH_SENTRY_ENVIRONMENT": "tests",
             "SWH_MAIN_PACKAGE": "swh.core",
         },
-    ):
-        gunicorn_config.post_fork(None, None)
+    )
+
+    gunicorn_config.post_fork(None, None)
 
     version = pkg_resources.get_distribution("swh.core").version
 
     sentry_sdk_init.assert_called_once_with(
         dsn="test_dsn",
         integrations=[flask_integration, logging_integration],
         debug=False,
         release="swh.core@" + version,
         environment="tests",
     )
 
 
-def test_post_fork_debug():
+def test_post_fork_debug(mocker):
     flask_integration = object()
     logging_integration = object()
 
-    with patch(
+    mocker.patch(
         "sentry_sdk.integrations.flask.FlaskIntegration", new=lambda: flask_integration
-    ), patch(
+    )
+    mocker.patch(
         "sentry_sdk.integrations.logging.LoggingIntegration",
         new=lambda event_level: logging_integration,
-    ), patch(
-        "sentry_sdk.init"
-    ) as sentry_sdk_init, patch.dict(
+    )
+    sentry_sdk_init = mocker.patch("sentry_sdk.init")
+    mocker.patch.dict(
         os.environ, {"SWH_SENTRY_DSN": "test_dsn", "SWH_SENTRY_DEBUG": "1"}
-    ):
-        gunicorn_config.post_fork(None, None)
+    )
+
+    gunicorn_config.post_fork(None, None)
 
     sentry_sdk_init.assert_called_once_with(
         dsn="test_dsn",
         integrations=[flask_integration, logging_integration],
         debug=True,
         release=None,
         environment=None,
     )
 
 
-def test_post_fork_no_flask():
+def test_post_fork_no_flask(mocker):
     logging_integration = object()
-
-    with patch("sentry_sdk.init") as sentry_sdk_init, patch(
+    sentry_sdk_init = mocker.patch("sentry_sdk.init")
+    mocker.patch(
         "sentry_sdk.integrations.logging.LoggingIntegration",
         new=lambda event_level: logging_integration,
-    ), patch.dict(os.environ, {"SWH_SENTRY_DSN": "test_dsn"}):
-        gunicorn_config.post_fork(None, None, flask=False)
+    )
+    mocker.patch.dict(os.environ, {"SWH_SENTRY_DSN": "test_dsn"})
+
+    gunicorn_config.post_fork(None, None, flask=False)
 
     sentry_sdk_init.assert_called_once_with(
         dsn="test_dsn",
         integrations=[logging_integration],
         debug=False,
         release=None,
         environment=None,
     )
 
 
-def test_post_fork_override_logging_events_envvar():
-    with patch("sentry_sdk.init") as sentry_sdk_init, patch.dict(
+def test_post_fork_override_logging_events_envvar(mocker):
+    sentry_sdk_init = mocker.patch("sentry_sdk.init")
+    mocker.patch.dict(
         os.environ,
         {"SWH_SENTRY_DSN": "test_dsn", "SWH_SENTRY_DISABLE_LOGGING_EVENTS": "false"},
-    ):
-        gunicorn_config.post_fork(None, None, flask=False)
+    )
+
+    gunicorn_config.post_fork(None, None, flask=False)
 
     sentry_sdk_init.assert_called_once_with(
         dsn="test_dsn",
         integrations=[],
         debug=False,
         release=None,
         environment=None,
     )
 
 
-def test_post_fork_extras():
+def test_post_fork_extras(mocker):
     flask_integration = object()  # unique object to check for equality
-    with patch(
+    mocker.patch(
         "sentry_sdk.integrations.flask.FlaskIntegration", new=lambda: flask_integration
-    ):
-        with patch("sentry_sdk.init") as sentry_sdk_init:
-            with patch.dict(os.environ, {"SWH_SENTRY_DSN": "test_dsn"}):
-                gunicorn_config.post_fork(
-                    None,
-                    None,
-                    sentry_integrations=["foo"],
-                    extra_sentry_kwargs={"bar": "baz"},
-                    disable_logging_events=False,
-                )
+    )
+    sentry_sdk_init = mocker.patch("sentry_sdk.init")
+    mocker.patch.dict(os.environ, {"SWH_SENTRY_DSN": "test_dsn"})
+
+    gunicorn_config.post_fork(
+        None,
+        None,
+        sentry_integrations=["foo"],
+        extra_sentry_kwargs={"bar": "baz"},
+        disable_logging_events=False,
+    )
 
     sentry_sdk_init.assert_called_once_with(
         dsn="test_dsn",
         integrations=["foo", flask_integration],
         debug=False,
         bar="baz",
         release=None,
```

### Comparing `swh.core-3.0.0/swh/core/api/tests/test_init.py` & `swh_core-3.0.1/swh/core/api/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `swh.core-3.0.0/swh/core/api/tests/test_rpc_client.py` & `swh_core-3.0.1/swh/core/api/tests/test_rpc_client.py`

 * *Files identical despite different names*

### Comparing `swh.core-3.0.0/swh/core/api/tests/test_rpc_client_server.py` & `swh_core-3.0.1/swh/core/api/tests/test_rpc_client_server.py`

 * *Files identical despite different names*

### Comparing `swh.core-3.0.0/swh/core/api/tests/test_rpc_server.py` & `swh_core-3.0.1/swh/core/api/tests/test_rpc_server.py`

 * *Files identical despite different names*

### Comparing `swh.core-3.0.0/swh/core/api/tests/test_rpc_server_asynchronous.py` & `swh_core-3.0.1/swh/core/api/tests/test_rpc_server_asynchronous.py`

 * *Files identical despite different names*

### Comparing `swh.core-3.0.0/swh/core/api/tests/test_serializers.py` & `swh_core-3.0.1/swh/core/api/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `swh.core-3.0.0/swh/core/cli/__init__.py` & `swh_core-3.0.1/swh/core/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.core-3.0.0/swh/core/cli/db.py` & `swh_core-3.0.1/swh/core/cli/db.py`

 * *Files identical despite different names*

### Comparing `swh.core-3.0.0/swh/core/collections.py` & `swh_core-3.0.1/swh/core/collections.py`

 * *Files identical despite different names*

### Comparing `swh.core-3.0.0/swh/core/config.py` & `swh_core-3.0.1/swh/core/config.py`

 * *Files identical despite different names*

### Comparing `swh.core-3.0.0/swh/core/db/__init__.py` & `swh_core-3.0.1/swh/core/db/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.core-3.0.0/swh/core/db/common.py` & `swh_core-3.0.1/swh/core/db/common.py`

 * *Files identical despite different names*

### Comparing `swh.core-3.0.0/swh/core/db/db_utils.py` & `swh_core-3.0.1/swh/core/db/db_utils.py`

 * *Files identical despite different names*

### Comparing `swh.core-3.0.0/swh/core/db/sql/35-dbversion.sql` & `swh_core-3.0.1/swh/core/db/sql/35-dbversion.sql`

 * *Files identical despite different names*

### Comparing `swh.core-3.0.0/swh/core/db/sql/36-dbmodule.sql` & `swh_core-3.0.1/swh/core/db/sql/36-dbmodule.sql`

 * *Files identical despite different names*

### Comparing `swh.core-3.0.0/swh/core/db/tests/conftest.py` & `swh_core-3.0.1/swh/core/db/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `swh.core-3.0.0/swh/core/db/tests/data/cli/sql/15-flavor.sql` & `swh_core-3.0.1/swh/core/db/tests/data/cli/sql/15-flavor.sql`

 * *Files identical despite different names*

### Comparing `swh.core-3.0.0/swh/core/db/tests/test_cli.py` & `swh_core-3.0.1/swh/core/db/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `swh.core-3.0.0/swh/core/db/tests/test_db.py` & `swh_core-3.0.1/swh/core/db/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `swh.core-3.0.0/swh/core/db/tests/test_db_utils.py` & `swh_core-3.0.1/swh/core/db/tests/test_db_utils.py`

 * *Files identical despite different names*

### Comparing `swh.core-3.0.0/swh/core/github/pytest_plugin.py` & `swh_core-3.0.1/swh/core/github/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `swh.core-3.0.0/swh/core/github/tests/test_github_utils.py` & `swh_core-3.0.1/swh/core/github/tests/test_github_utils.py`

 * *Files identical despite different names*

### Comparing `swh.core-3.0.0/swh/core/github/tests/test_pytest_plugin.py` & `swh_core-3.0.1/swh/core/github/tests/test_pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `swh.core-3.0.0/swh/core/github/utils.py` & `swh_core-3.0.1/swh/core/github/utils.py`

 * *Files identical despite different names*

### Comparing `swh.core-3.0.0/swh/core/logger.py` & `swh_core-3.0.1/swh/core/logger.py`

 * *Files identical despite different names*

### Comparing `swh.core-3.0.0/swh/core/logging.py` & `swh_core-3.0.1/swh/core/logging.py`

 * *Files identical despite different names*

### Comparing `swh.core-3.0.0/swh/core/pytest_plugin.py` & `swh_core-3.0.1/swh/core/pytest_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2019-2021  The Software Heritage developers
+# Copyright (C) 2019-2024  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 from collections import deque
 from functools import partial
 import logging
@@ -369,39 +369,52 @@
     statsd._socket = FakeSocket()
     yield statsd
 
 
 @pytest.fixture
 def monkeypatch_sentry_transport():
     # Inspired by
-    # https://github.com/getsentry/sentry-python/blob/1.5.9/tests/conftest.py#L168-L184
+    # https://github.com/getsentry/sentry-python/blob/2.0.0/tests/conftest.py#L175-L219
 
     initialized = False
 
     def setup_sentry_transport_monkeypatch(*a, **kw):
         nonlocal initialized
         assert not initialized, "already initialized"
         initialized = True
         hub = sentry_sdk.Hub.current
         client = sentry_sdk.Client(*a, **kw)
         hub.bind_client(client)
         client.transport = TestTransport()
 
-    class TestTransport:
+    from sentry_sdk.transport import Transport
+
+    class TestTransport(Transport):
         def __init__(self):
+            super().__init__()
             self.events = []
             self.envelopes = []
 
-        def capture_event(self, event):
-            self.events.append(event)
-
         def capture_envelope(self, envelope):
+            for item in envelope:
+                if item.headers.get("type") in ("event", "transaction"):
+                    self.events.append(item.payload.json)
             self.envelopes.append(envelope)
 
     with sentry_sdk.Hub(None):
         yield setup_sentry_transport_monkeypatch
 
 
 @pytest.fixture
 def sentry_events(monkeypatch_sentry_transport):
     monkeypatch_sentry_transport()
     return sentry_sdk.Hub.current.client.transport.events
+
+
+@pytest.fixture(autouse=True)
+def clean_scopes():
+    # https://github.com/getsentry/sentry-python/blob/2.0.0/tests/conftest.py#L61-L68
+    from sentry_sdk import scope
+
+    scope._global_scope = None
+    scope._isolation_scope.set(None)
+    scope._current_scope.set(None)
```

### Comparing `swh.core-3.0.0/swh/core/retry.py` & `swh_core-3.0.1/swh/core/retry.py`

 * *Files identical despite different names*

### Comparing `swh.core-3.0.0/swh/core/sentry.py` & `swh_core-3.0.1/swh/core/sentry.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2019-2020  The Software Heritage developers
+# Copyright (C) 2019-2024  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 import logging
 import os
 from typing import Dict, List, Optional
@@ -45,14 +45,15 @@
     *,
     main_package: Optional[str] = None,
     environment: Optional[str] = None,
     debug: bool = False,
     disable_logging_events: bool = False,
     integrations: Optional[List] = None,
     extra_kwargs: Optional[Dict] = None,
+    deferred_init: bool = False,
 ):
     """Configure the sentry integration
 
     Args:
       sentry_dsn: Sentry DSN; where sentry report will be sent. Overridden by
         :envvar:`SWH_SENTRY_DSN`
       main_package: Full name of main Python package associated to Sentry DSN.
@@ -60,14 +61,16 @@
       environment: Sentry environment. Overridden by :envvar:`SWH_SENTRY_ENVIRONMENT`
       debug: turn on Sentry SDK debug mode. Overridden by :envvar:`SWH_SENTRY_DEBUG`
       disable_logging_events: if set, disable the automatic reporting of error/exception
         log entries as Sentry events. Overridden by
         :envvar:`SWH_SENTRY_DISABLE_LOGGING_EVENTS`
       integrations: list of dedicated Sentry integrations to include
       extra_kwargs: dict of additional parameters passed to :func:`sentry_sdk.init`
+      deferred_init: indicates that sentry will be properly initialized in subsequent
+        calls and that no warnings about missing DSN should be logged
 
     """
     if integrations is None:
         integrations = []
     if extra_kwargs is None:
         extra_kwargs = {}
 
@@ -75,23 +78,25 @@
     environment = os.environ.get("SWH_SENTRY_ENVIRONMENT", environment)
 
     debug = override_with_bool_envvar("SWH_SENTRY_DEBUG", debug)
     disable_logging_events = override_with_bool_envvar(
         "SWH_SENTRY_DISABLE_LOGGING_EVENTS", disable_logging_events
     )
 
-    if sentry_dsn:
-        import sentry_sdk
+    if sentry_dsn is None and not deferred_init:
+        logger.warning("Sentry DSN not provided, events will not be sent.")
 
-        if disable_logging_events:
-            from sentry_sdk.integrations.logging import LoggingIntegration
+    import sentry_sdk
 
-            integrations.append(LoggingIntegration(event_level=None))
+    if disable_logging_events:
+        from sentry_sdk.integrations.logging import LoggingIntegration
 
-        sentry_sdk.init(
-            release=get_sentry_release(main_package),
-            environment=environment,
-            dsn=sentry_dsn,
-            integrations=integrations,
-            debug=debug,
-            **extra_kwargs,
-        )
+        integrations.append(LoggingIntegration(event_level=None))
+
+    sentry_sdk.init(
+        release=get_sentry_release(main_package),
+        environment=environment,
+        dsn=sentry_dsn,
+        integrations=integrations,
+        debug=debug,
+        **extra_kwargs,
+    )
```

### Comparing `swh.core-3.0.0/swh/core/statsd.py` & `swh_core-3.0.1/swh/core/statsd.py`

 * *Files identical despite different names*

### Comparing `swh.core-3.0.0/swh/core/tarball.py` & `swh_core-3.0.1/swh/core/tarball.py`

 * *Files identical despite different names*

### Comparing `swh.core-3.0.0/swh/core/tests/data/archives/ca-certificates-20210603-1-any.pkg.tar.zst` & `swh_core-3.0.1/swh/core/tests/data/archives/ca-certificates-20210603-1-any.pkg.tar.zst`

 * *Files identical despite different names*

### Comparing `swh.core-3.0.0/swh/core/tests/data/archives/groff-1.02.tar.Z` & `swh_core-3.0.1/swh/core/tests/data/archives/groff-1.02.tar.Z`

 * *Files identical despite different names*

### Comparing `swh.core-3.0.0/swh/core/tests/data/archives/hello.jar` & `swh_core-3.0.1/swh/core/tests/data/archives/hello.jar`

 * *Files identical despite different names*

### Comparing `swh.core-3.0.0/swh/core/tests/data/archives/hello.tar` & `swh_core-3.0.1/swh/core/tests/data/archives/hello.tar`

 * *Files identical despite different names*

### Comparing `swh.core-3.0.0/swh/core/tests/data/archives/hello.tar.x` & `swh_core-3.0.1/swh/core/tests/data/archives/hello.tar.x`

 * *Files identical despite different names*

### Comparing `swh.core-3.0.0/swh/core/tests/data/archives/hello.war` & `swh_core-3.0.1/swh/core/tests/data/archives/hello.war`

 * *Files identical despite different names*

### Comparing `swh.core-3.0.0/swh/core/tests/data/archives/msk316src.zip` & `swh_core-3.0.1/swh/core/tests/data/archives/msk316src.zip`

 * *Files identical despite different names*

### Comparing `swh.core-3.0.0/swh/core/tests/data/archives/tokei-12.1.2.crate` & `swh_core-3.0.1/swh/core/tests/data/archives/tokei-12.1.2.crate`

 * *Files identical despite different names*

### Comparing `swh.core-3.0.0/swh/core/tests/data/logging-config.yaml` & `swh_core-3.0.1/swh/core/tests/data/logging-config.yaml`

 * *Files identical despite different names*

### Comparing `swh.core-3.0.0/swh/core/tests/fixture/test_pytest_plugin.py` & `swh_core-3.0.1/swh/core/tests/fixture/test_pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `swh.core-3.0.0/swh/core/tests/test_cli.py` & `swh_core-3.0.1/swh/core/tests/test_cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-# Copyright (C) 2019  The Software Heritage developers
+# Copyright (C) 2019-2024  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 import logging
 import textwrap
 from typing import List
-from unittest.mock import patch
 
 import click
 from click.testing import CliRunner
 import pkg_resources
 import pytest
 import yaml
 
@@ -94,24 +93,30 @@
     result = runner.invoke(swhmain, ["--help"])
     assert result.exit_code == 0
     for section, snippets in help_msg_snippets:
         for snippet in snippets:
             assert_section_contains(result.output, section, snippet)
 
 
-def test_command(swhmain):
+def test_command(swhmain, mocker):
     @swhmain.command(name="test")
     @click.pass_context
     def swhtest(ctx):
         click.echo("Hello SWH!")
 
     runner = CliRunner()
-    with patch("sentry_sdk.init") as sentry_sdk_init:
-        result = runner.invoke(swhmain, ["test"])
-    sentry_sdk_init.assert_not_called()
+    sentry_sdk_init = mocker.patch("sentry_sdk.init")
+    result = runner.invoke(swhmain, ["test"])
+    sentry_sdk_init.assert_called_once_with(
+        dsn=None,
+        debug=False,
+        integrations=[],
+        release=None,
+        environment=None,
+    )
     assert result.exit_code == 0
     assert result.output.strip() == "Hello SWH!"
 
 
 def test_loglevel_default(caplog, swhmain):
     @swhmain.command(name="test")
     @click.pass_context
@@ -147,94 +152,94 @@
 
     runner = CliRunner()
     result = runner.invoke(swhmain, ["-l", "DEBUG", "test"])
     assert result.exit_code == 0
     assert result.output.strip() == """Hello SWH!"""
 
 
-def test_sentry(swhmain):
+def test_sentry(swhmain, mocker):
     @swhmain.command(name="test")
     @click.pass_context
     def swhtest(ctx):
         click.echo("Hello SWH!")
 
     runner = CliRunner()
-    with patch("sentry_sdk.init") as sentry_sdk_init:
-        result = runner.invoke(swhmain, ["--sentry-dsn", "test_dsn", "test"])
+    sentry_sdk_init = mocker.patch("sentry_sdk.init")
+    result = runner.invoke(swhmain, ["--sentry-dsn", "test_dsn", "test"])
     assert result.exit_code == 0
     assert result.output.strip() == """Hello SWH!"""
     sentry_sdk_init.assert_called_once_with(
         dsn="test_dsn",
         debug=False,
         integrations=[],
         release=None,
         environment=None,
     )
 
 
-def test_sentry_debug(swhmain):
+def test_sentry_debug(swhmain, mocker):
     @swhmain.command(name="test")
     @click.pass_context
     def swhtest(ctx):
         click.echo("Hello SWH!")
 
     runner = CliRunner()
-    with patch("sentry_sdk.init") as sentry_sdk_init:
-        result = runner.invoke(
-            swhmain, ["--sentry-dsn", "test_dsn", "--sentry-debug", "test"]
-        )
+    sentry_sdk_init = mocker.patch("sentry_sdk.init")
+    result = runner.invoke(
+        swhmain, ["--sentry-dsn", "test_dsn", "--sentry-debug", "test"]
+    )
     assert result.exit_code == 0
     assert result.output.strip() == """Hello SWH!"""
     sentry_sdk_init.assert_called_once_with(
         dsn="test_dsn",
         debug=True,
         integrations=[],
         release=None,
         environment=None,
     )
 
 
-def test_sentry_env(swhmain):
+def test_sentry_env(swhmain, mocker):
     @swhmain.command(name="test")
     @click.pass_context
     def swhtest(ctx):
         click.echo("Hello SWH!")
 
     runner = CliRunner()
-    with patch("sentry_sdk.init") as sentry_sdk_init:
-        env = {
-            "SWH_SENTRY_DSN": "test_dsn",
-            "SWH_SENTRY_DEBUG": "1",
-        }
-        result = runner.invoke(swhmain, ["test"], env=env, auto_envvar_prefix="SWH")
+    sentry_sdk_init = mocker.patch("sentry_sdk.init")
+    env = {
+        "SWH_SENTRY_DSN": "test_dsn",
+        "SWH_SENTRY_DEBUG": "1",
+    }
+    result = runner.invoke(swhmain, ["test"], env=env, auto_envvar_prefix="SWH")
     assert result.exit_code == 0
     assert result.output.strip() == """Hello SWH!"""
     sentry_sdk_init.assert_called_once_with(
         dsn="test_dsn",
         debug=True,
         integrations=[],
         release=None,
         environment=None,
     )
 
 
-def test_sentry_env_main_package(swhmain):
+def test_sentry_env_main_package(swhmain, mocker):
     @swhmain.command(name="test")
     @click.pass_context
     def swhtest(ctx):
         click.echo("Hello SWH!")
 
     runner = CliRunner()
-    with patch("sentry_sdk.init") as sentry_sdk_init:
-        env = {
-            "SWH_SENTRY_DSN": "test_dsn",
-            "SWH_MAIN_PACKAGE": "swh.core",
-            "SWH_SENTRY_ENVIRONMENT": "tests",
-        }
-        result = runner.invoke(swhmain, ["test"], env=env, auto_envvar_prefix="SWH")
+    sentry_sdk_init = mocker.patch("sentry_sdk.init")
+    env = {
+        "SWH_SENTRY_DSN": "test_dsn",
+        "SWH_MAIN_PACKAGE": "swh.core",
+        "SWH_SENTRY_ENVIRONMENT": "tests",
+    }
+    result = runner.invoke(swhmain, ["test"], env=env, auto_envvar_prefix="SWH")
     assert result.exit_code == 0
 
     version = pkg_resources.get_distribution("swh.core").version
 
     assert result.output.strip() == """Hello SWH!"""
     sentry_sdk_init.assert_called_once_with(
         dsn="test_dsn",
```

### Comparing `swh.core-3.0.0/swh/core/tests/test_collections.py` & `swh_core-3.0.1/swh/core/tests/test_collections.py`

 * *Files identical despite different names*

### Comparing `swh.core-3.0.0/swh/core/tests/test_config.py` & `swh_core-3.0.1/swh/core/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `swh.core-3.0.0/swh/core/tests/test_logger.py` & `swh_core-3.0.1/swh/core/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `swh.core-3.0.0/swh/core/tests/test_logging.py` & `swh_core-3.0.1/swh/core/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `swh.core-3.0.0/swh/core/tests/test_pytest_plugin.py` & `swh_core-3.0.1/swh/core/tests/test_pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `swh.core-3.0.0/swh/core/tests/test_retry.py` & `swh_core-3.0.1/swh/core/tests/test_retry.py`

 * *Files identical despite different names*

### Comparing `swh.core-3.0.0/swh/core/tests/test_sentry.py` & `swh_core-3.0.1/swh/core/tests/test_sentry.py`

 * *Files 3% similar despite different names*

```diff
@@ -143,7 +143,20 @@
     init_sentry(
         SENTRY_DSN,
     )
     assert sentry_sdk_init.call_args_list[-1][1]["release"] is None
 
     init_sentry(SENTRY_DSN, main_package="swh.core")
     assert sentry_sdk_init.call_args_list[-1][1]["release"].startswith("swh.core@")
+
+
+@pytest.mark.parametrize("deferred_init", [False, True])
+def test_sentry_deferred_init(caplog, deferred_init):
+    init_sentry(None, deferred_init=deferred_init)
+    if not deferred_init:
+        assert caplog.records
+        assert (
+            caplog.records[0].message
+            == "Sentry DSN not provided, events will not be sent."
+        )
+    else:
+        assert not caplog.records
```

### Comparing `swh.core-3.0.0/swh/core/tests/test_statsd.py` & `swh_core-3.0.1/swh/core/tests/test_statsd.py`

 * *Files identical despite different names*

### Comparing `swh.core-3.0.0/swh/core/tests/test_tarball.py` & `swh_core-3.0.1/swh/core/tests/test_tarball.py`

 * *Files identical despite different names*

### Comparing `swh.core-3.0.0/swh/core/tests/test_utils.py` & `swh_core-3.0.1/swh/core/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `swh.core-3.0.0/swh/core/utils.py` & `swh_core-3.0.1/swh/core/utils.py`

 * *Files identical despite different names*

### Comparing `swh.core-3.0.0/swh.core.egg-info/PKG-INFO` & `swh_core-3.0.1/swh.core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.core
-Version: 3.0.0
+Version: 3.0.1
 Summary: Software Heritage core utilities
 Author-email: Software Heritage developers <swh-devel@inria.fr>
 Project-URL: Homepage, https://gitlab.softwareheritage.org/swh/devel/swh-core
 Project-URL: Bug Reports, https://gitlab.softwareheritage.org/swh/devel/swh-core/-/issues
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Documentation, https://docs.softwareheritage.org/devel/swh-core/
 Project-URL: Source, https://gitlab.softwareheritage.org/swh/devel/swh-core.git
@@ -18,19 +18,19 @@
 License-File: LICENSE
 License-File: AUTHORS
 Requires-Dist: click
 Requires-Dist: deprecated
 Requires-Dist: python-magic
 Requires-Dist: pyyaml
 Requires-Dist: requests
-Requires-Dist: sentry-sdk
+Requires-Dist: sentry-sdk>=2
 Requires-Dist: tenacity
 Provides-Extra: testing-core
 Requires-Dist: hypothesis>=3.11.0; extra == "testing-core"
-Requires-Dist: pytest; extra == "testing-core"
+Requires-Dist: pytest>=8.1; extra == "testing-core"
 Requires-Dist: pytest-mock; extra == "testing-core"
 Requires-Dist: pytest-postgresql>5; extra == "testing-core"
 Requires-Dist: pytz; extra == "testing-core"
 Requires-Dist: requests-mock; extra == "testing-core"
 Requires-Dist: types-deprecated; extra == "testing-core"
 Requires-Dist: types-psycopg2; extra == "testing-core"
 Requires-Dist: types-pytz; extra == "testing-core"
@@ -47,15 +47,15 @@
 Requires-Dist: blinker; extra == "http"
 Requires-Dist: flask; extra == "http"
 Requires-Dist: iso8601; extra == "http"
 Requires-Dist: msgpack>=1.0.0; extra == "http"
 Requires-Dist: requests; extra == "http"
 Provides-Extra: testing
 Requires-Dist: hypothesis>=3.11.0; extra == "testing"
-Requires-Dist: pytest; extra == "testing"
+Requires-Dist: pytest>=8.1; extra == "testing"
 Requires-Dist: pytest-mock; extra == "testing"
 Requires-Dist: pytest-postgresql>5; extra == "testing"
 Requires-Dist: pytz; extra == "testing"
 Requires-Dist: requests-mock; extra == "testing"
 Requires-Dist: types-deprecated; extra == "testing"
 Requires-Dist: types-psycopg2; extra == "testing"
 Requires-Dist: types-pytz; extra == "testing"
```

### Comparing `swh.core-3.0.0/swh.core.egg-info/SOURCES.txt` & `swh_core-3.0.1/swh.core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swh.core-3.0.0/swh.core.egg-info/requires.txt` & `swh_core-3.0.1/swh.core.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 click
 deprecated
 python-magic
 pyyaml
 requests
-sentry-sdk
+sentry-sdk>=2
 tenacity
 
 [db]
 psycopg2
 typing-extensions
 
 [http]
@@ -20,15 +20,15 @@
 requests
 
 [logging]
 systemd-python
 
 [testing]
 hypothesis>=3.11.0
-pytest
+pytest>=8.1
 pytest-mock
 pytest-postgresql>5
 pytz
 requests-mock
 types-deprecated
 types-psycopg2
 types-pytz
@@ -43,15 +43,15 @@
 msgpack>=1.0.0
 requests
 psycopg2
 typing-extensions
 
 [testing_core]
 hypothesis>=3.11.0
-pytest
+pytest>=8.1
 pytest-mock
 pytest-postgresql>5
 pytz
 requests-mock
 types-deprecated
 types-psycopg2
 types-pytz
```

### Comparing `swh.core-3.0.0/tox.ini` & `swh_core-3.0.1/tox.ini`

 * *Files 26% similar despite different names*

```diff
@@ -3,35 +3,32 @@
 envlist =
   black
   flake8
   mypy
   py3-{core,db,server,github}
 
 [testenv]
+usedevelop = true
 passenv = PYTHONASYNCIODEBUG
 extras =
   testing-core
   core: logging
   db: db
   server: http
 deps =
   cover: pytest-cov
 commands =
   pytest --doctest-modules \
-  --rootdir {envsitepackagesdir} \
-  slow: --hypothesis-profile=slow \
-  cover: --cov={envsitepackagesdir}/swh/core --cov-branch \
-  core: {envsitepackagesdir}/swh/core/tests \
-  db: {envsitepackagesdir}/swh/core/db/tests \
-  server: {envsitepackagesdir}/swh/core/api/tests \
-  github: {envsitepackagesdir}/swh/core/github/tests \
-    {posargs}
-# --rootdir (with --import-mode from pytest.ini) are required to make tests
-# that depends on the test file to be a proper submodule of the swh namespace
-# after migration to PEP420 (implicit namespace).
+  slow:  --hypothesis-profile=slow \
+  cover: --cov=swh/core --cov-branch \
+  core:  swh/core/tests \
+  db:    swh/core/db/tests \
+  server: swh/core/api/tests \
+  github: swh/core/github/tests \
+         {posargs}
 
 [testenv:py3{,7,8,9,10,11,12,13},pypy3{,7,8,9,10,11,12,13}]
 skip_install = true
 allowlist_externals = tox
 commands = tox run -e {env_name}-core-db-server-github-slow-cover -- {posargs}
 
 [testenv:black]
@@ -54,15 +51,15 @@
 extras =
   testing-core
   logging
   db
   http
   github
 deps =
-  mypy==1.0.1
+  mypy==1.8.0
 commands =
   mypy swh
 
 # build documentation outside swh-environment using the current
 # git HEAD of swh-docs, is executed on CI for each diff to prevent
 # breaking doc build
 [testenv:sphinx]
```

