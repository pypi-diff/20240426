# Comparing `tmp/swh_objstorage-2.9.3.tar.gz` & `tmp/swh_objstorage-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swh_objstorage-2.9.3.tar", last modified: Thu Apr 18 13:06:38 2024, max compression
+gzip compressed data, was "swh_objstorage-3.0.0.tar", last modified: Fri Apr 26 11:21:20 2024, max compression
```

## Comparing `swh_objstorage-2.9.3.tar` & `swh_objstorage-3.0.0.tar`

### file list

```diff
@@ -1,141 +1,145 @@
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 13:06:38.182711 swh_objstorage-2.9.3/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      360 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/.copier-answers.yml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      140 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/.git-blame-ignore-revs
--rw-r--r--   0 jenkins    (115) jenkins    (120)      388 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/.gitignore
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1538 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/.pre-commit-config.yaml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      112 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/AUTHORS
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3397 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 jenkins    (115) jenkins    (120)       15 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/CONTRIBUTORS
--rw-r--r--   0 jenkins    (115) jenkins    (120)    35147 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/LICENSE
--rw-r--r--   0 jenkins    (115) jenkins    (120)      163 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/Makefile
--rw-r--r--   0 jenkins    (115) jenkins    (120)       37 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/Makefile.local
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4453 2024-04-18 13:06:38.182711 swh_objstorage-2.9.3/PKG-INFO
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2275 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/README.rst
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 13:06:38.150711 swh_objstorage-2.9.3/bin/
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)     3435 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/bin/swh-objstorage-azure
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3948 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/conftest.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 13:06:38.154711 swh_objstorage-2.9.3/docs/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/docs/.gitignore
--rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/docs/Makefile
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 13:06:38.154711 swh_objstorage-2.9.3/docs/_static/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/docs/_static/.placeholder
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 13:06:38.154711 swh_objstorage-2.9.3/docs/_templates/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/docs/_templates/.placeholder
--rw-r--r--   0 jenkins    (115) jenkins    (120)      163 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/docs/cli.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)       43 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/docs/conf.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      284 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/docs/index.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5513 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/docs/winery.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)      629 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/mypy.ini
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2004 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/pyproject.toml
--rw-r--r--   0 jenkins    (115) jenkins    (120)       96 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/pytest.ini
--rw-r--r--   0 jenkins    (115) jenkins    (120)      125 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/requirements-azure.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)       16 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/requirements-libcloud.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)       69 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/requirements-swh.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      172 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/requirements-test.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)       31 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/requirements-winery.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      297 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/requirements.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      210 2024-04-18 13:06:38.182711 swh_objstorage-2.9.3/setup.cfg
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 13:06:38.142711 swh_objstorage-2.9.3/swh/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 13:06:38.158711 swh_objstorage-2.9.3/swh/objstorage/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 13:06:38.158711 swh_objstorage-2.9.3/swh/objstorage/api/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1974 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/api/client.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5013 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/api/server.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 13:06:38.158711 swh_objstorage-2.9.3/swh/objstorage/backends/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/backends/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    17381 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/backends/azure.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5150 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/backends/generator.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3170 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/backends/http.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1780 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/backends/in_memory.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8283 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/backends/libcloud.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1115 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/backends/noop.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    11190 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/backends/pathslicing.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 13:06:38.162711 swh_objstorage-2.9.3/swh/objstorage/backends/seaweedfs/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       61 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/backends/seaweedfs/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4060 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/backends/seaweedfs/http.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4925 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/backends/seaweedfs/objstorage.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 13:06:38.162711 swh_objstorage-2.9.3/swh/objstorage/backends/winery/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       55 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/backends/winery/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8317 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/backends/winery/database.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    14679 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/backends/winery/objstorage.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    14565 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/backends/winery/roshard.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3283 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/backends/winery/rwshard.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    18323 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/backends/winery/sharedbase.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      944 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/backends/winery/sleep.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2810 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/backends/winery/stats.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     7079 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/backends/winery/throttler.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    12577 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/cli.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      547 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/constants.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1466 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/exc.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2970 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/factory.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8544 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/interface.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 13:06:38.162711 swh_objstorage-2.9.3/swh/objstorage/multiplexer/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      121 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/multiplexer/__init__.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 13:06:38.166711 swh_objstorage-2.9.3/swh/objstorage/multiplexer/filter/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2617 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/multiplexer/filter/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2721 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/multiplexer/filter/filter.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      785 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/multiplexer/filter/read_write_filter.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    11782 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/multiplexer/multiplexer_objstorage.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     7416 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/objstorage.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)       27 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/py.typed
--rw-r--r--   0 jenkins    (115) jenkins    (120)      956 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/pytest_plugin.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 13:06:38.170711 swh_objstorage-2.9.3/swh/objstorage/tests/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/tests/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    13564 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/tests/objstorage_testing.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1519 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/tests/test_interface.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1372 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/tests/test_objstorage_api.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    12670 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/tests/test_objstorage_azure.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     7083 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/tests/test_objstorage_cloud.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4694 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/tests/test_objstorage_http.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      466 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/tests/test_objstorage_in_memory.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      794 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/tests/test_objstorage_instantiation.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3747 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/tests/test_objstorage_multiplexer.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      512 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/tests/test_objstorage_noop.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5672 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/tests/test_objstorage_pathslicing.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1630 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/tests/test_objstorage_random_generator.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    10093 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/tests/test_objstorage_seaweedfs.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    38512 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/tests/test_objstorage_winery.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2761 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/tests/test_pathslicer.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2952 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/tests/test_readonly_filter.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4017 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/tests/test_server.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    20137 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/tests/winery_benchmark.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6707 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/tests/winery_testing_helpers.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      903 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/utils.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 13:06:38.178711 swh_objstorage-2.9.3/swh.objstorage.egg-info/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4453 2024-04-18 13:06:38.000000 swh_objstorage-2.9.3/swh.objstorage.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4097 2024-04-18 13:06:38.000000 swh_objstorage-2.9.3/swh.objstorage.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)        1 2024-04-18 13:06:38.000000 swh_objstorage-2.9.3/swh.objstorage.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)       58 2024-04-18 13:06:38.000000 swh_objstorage-2.9.3/swh.objstorage.egg-info/entry_points.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      476 2024-04-18 13:06:38.000000 swh_objstorage-2.9.3/swh.objstorage.egg-info/requires.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)        4 2024-04-18 13:06:38.000000 swh_objstorage-2.9.3/swh.objstorage.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1253 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/tox.ini
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 13:06:38.174711 swh_objstorage-2.9.3/winery-test-environment/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2649 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/winery-test-environment/README.md
--rw-r--r--   0 jenkins    (115) jenkins    (120)      209 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/winery-test-environment/ansible.cfg
--rw-r--r--   0 jenkins    (115) jenkins    (120)      955 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/winery-test-environment/bootstrap.yml
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)     4204 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/winery-test-environment/build-vms.sh
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2038 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/winery-test-environment/ceph.yml
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3932 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/winery-test-environment/fed4fire.rspec
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)      844 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/winery-test-environment/fed4fire.sh
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1836 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/winery-test-environment/grid5000.yml
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 13:06:38.174711 swh_objstorage-2.9.3/winery-test-environment/inventory/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 13:06:38.142711 swh_objstorage-2.9.3/winery-test-environment/inventory/group_vars/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 13:06:38.174711 swh_objstorage-2.9.3/winery-test-environment/inventory/group_vars/all/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      108 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/winery-test-environment/inventory/group_vars/all/rw.yml
--rw-r--r--   0 jenkins    (115) jenkins    (120)       91 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/winery-test-environment/inventory/groups.yml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      822 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/winery-test-environment/inventory/hosts.yml
--rw-r--r--   0 jenkins    (115) jenkins    (120)       84 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/winery-test-environment/inventory/osd.yml
--rw-r--r--   0 jenkins    (115) jenkins    (120)       75 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/winery-test-environment/libvirt.yml
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 13:06:38.178711 swh_objstorage-2.9.3/winery-test-environment/mitogen-strategy/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       80 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/winery-test-environment/mitogen-strategy/README.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/winery-test-environment/mitogen-strategy/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2757 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/winery-test-environment/mitogen-strategy/mitogen.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2763 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/winery-test-environment/mitogen-strategy/mitogen_free.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2895 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/winery-test-environment/mitogen-strategy/mitogen_host_pinned.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2765 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/winery-test-environment/mitogen-strategy/mitogen_linear.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      824 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/winery-test-environment/osd.yml
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)     1333 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/winery-test-environment/remote-tox.sh
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1733 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/winery-test-environment/render-stats.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)       40 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/winery-test-environment/requirements.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      198 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/winery-test-environment/rng.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2727 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/winery-test-environment/rw.yml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      632 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/winery-test-environment/tests.yml
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 11:21:20.737814 swh_objstorage-3.0.0/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      360 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/.copier-answers.yml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      140 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/.git-blame-ignore-revs
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      388 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/.gitignore
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1538 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      112 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/AUTHORS
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3397 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       15 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/CONTRIBUTORS
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    35147 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/LICENSE
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      163 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/Makefile
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       37 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/Makefile.local
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4453 2024-04-26 11:21:20.737814 swh_objstorage-3.0.0/PKG-INFO
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2275 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/README.rst
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 11:21:20.709815 swh_objstorage-3.0.0/bin/
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)     3435 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/bin/swh-objstorage-azure
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3948 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/conftest.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 11:21:20.709815 swh_objstorage-3.0.0/docs/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/docs/.gitignore
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/docs/Makefile
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 11:21:20.709815 swh_objstorage-3.0.0/docs/_static/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/docs/_static/.placeholder
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 11:21:20.709815 swh_objstorage-3.0.0/docs/_templates/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/docs/_templates/.placeholder
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      163 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/docs/cli.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       43 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/docs/conf.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      284 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/docs/index.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5513 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/docs/winery.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      629 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/mypy.ini
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2004 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/pyproject.toml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       96 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/pytest.ini
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      125 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/requirements-azure.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       16 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/requirements-libcloud.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       69 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/requirements-swh.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      172 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/requirements-test.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       31 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/requirements-winery.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      297 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/requirements.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      210 2024-04-26 11:21:20.737814 swh_objstorage-3.0.0/setup.cfg
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 11:21:20.701815 swh_objstorage-3.0.0/swh/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 11:21:20.713815 swh_objstorage-3.0.0/swh/objstorage/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 11:21:20.713815 swh_objstorage-3.0.0/swh/objstorage/api/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1974 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/swh/objstorage/api/client.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5013 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/swh/objstorage/api/server.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 11:21:20.717815 swh_objstorage-3.0.0/swh/objstorage/backends/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/swh/objstorage/backends/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    17381 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/swh/objstorage/backends/azure.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5150 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/swh/objstorage/backends/generator.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3170 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/swh/objstorage/backends/http.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1780 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/swh/objstorage/backends/in_memory.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8283 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/swh/objstorage/backends/libcloud.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1115 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/swh/objstorage/backends/noop.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    11964 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/swh/objstorage/backends/pathslicing.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 11:21:20.717815 swh_objstorage-3.0.0/swh/objstorage/backends/seaweedfs/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       61 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/swh/objstorage/backends/seaweedfs/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4060 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/swh/objstorage/backends/seaweedfs/http.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4925 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/swh/objstorage/backends/seaweedfs/objstorage.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 11:21:20.721814 swh_objstorage-3.0.0/swh/objstorage/backends/winery/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      191 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/swh/objstorage/backends/winery/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2076 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/swh/objstorage/backends/winery/database.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      639 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/swh/objstorage/backends/winery/gunicorn.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    15419 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/swh/objstorage/backends/winery/objstorage.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    16100 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/swh/objstorage/backends/winery/roshard.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6803 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/swh/objstorage/backends/winery/rwshard.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    17191 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/swh/objstorage/backends/winery/sharedbase.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      944 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/swh/objstorage/backends/winery/sleep.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 11:21:20.721814 swh_objstorage-3.0.0/swh/objstorage/backends/winery/sql/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1170 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/swh/objstorage/backends/winery/sql/30-schema.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/swh/objstorage/backends/winery/sql/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2810 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/swh/objstorage/backends/winery/stats.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6455 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/swh/objstorage/backends/winery/throttler.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    12642 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/swh/objstorage/cli.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1115 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/swh/objstorage/constants.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1466 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/swh/objstorage/exc.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2970 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/swh/objstorage/factory.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8544 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/swh/objstorage/interface.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 11:21:20.721814 swh_objstorage-3.0.0/swh/objstorage/multiplexer/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      121 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/swh/objstorage/multiplexer/__init__.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 11:21:20.721814 swh_objstorage-3.0.0/swh/objstorage/multiplexer/filter/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2617 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/swh/objstorage/multiplexer/filter/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2721 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/swh/objstorage/multiplexer/filter/filter.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      785 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/swh/objstorage/multiplexer/filter/read_write_filter.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    11782 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/swh/objstorage/multiplexer/multiplexer_objstorage.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     7416 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/swh/objstorage/objstorage.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       27 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/swh/objstorage/py.typed
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      956 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/swh/objstorage/pytest_plugin.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 11:21:20.725814 swh_objstorage-3.0.0/swh/objstorage/tests/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/swh/objstorage/tests/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    13564 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/swh/objstorage/tests/objstorage_testing.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1519 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/swh/objstorage/tests/test_interface.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1372 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/swh/objstorage/tests/test_objstorage_api.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    12670 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/swh/objstorage/tests/test_objstorage_azure.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     7083 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/swh/objstorage/tests/test_objstorage_cloud.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4694 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/swh/objstorage/tests/test_objstorage_http.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      466 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/swh/objstorage/tests/test_objstorage_in_memory.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      794 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/swh/objstorage/tests/test_objstorage_instantiation.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3747 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/swh/objstorage/tests/test_objstorage_multiplexer.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      512 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/swh/objstorage/tests/test_objstorage_noop.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     7192 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/swh/objstorage/tests/test_objstorage_pathslicing.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1630 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/swh/objstorage/tests/test_objstorage_random_generator.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    10093 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/swh/objstorage/tests/test_objstorage_seaweedfs.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    45626 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/swh/objstorage/tests/test_objstorage_winery.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2761 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/swh/objstorage/tests/test_pathslicer.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2952 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/swh/objstorage/tests/test_readonly_filter.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4017 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/swh/objstorage/tests/test_server.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    19921 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/swh/objstorage/tests/winery_benchmark.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6882 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/swh/objstorage/tests/winery_testing_helpers.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      903 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/swh/objstorage/utils.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 11:21:20.733814 swh_objstorage-3.0.0/swh.objstorage.egg-info/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4453 2024-04-26 11:21:20.000000 swh_objstorage-3.0.0/swh.objstorage.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4236 2024-04-26 11:21:20.000000 swh_objstorage-3.0.0/swh.objstorage.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        1 2024-04-26 11:21:20.000000 swh_objstorage-3.0.0/swh.objstorage.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       58 2024-04-26 11:21:20.000000 swh_objstorage-3.0.0/swh.objstorage.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      476 2024-04-26 11:21:20.000000 swh_objstorage-3.0.0/swh.objstorage.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        4 2024-04-26 11:21:20.000000 swh_objstorage-3.0.0/swh.objstorage.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1253 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/tox.ini
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 11:21:20.729814 swh_objstorage-3.0.0/winery-test-environment/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2649 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/winery-test-environment/README.md
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      209 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/winery-test-environment/ansible.cfg
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      955 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/winery-test-environment/bootstrap.yml
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)     4204 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/winery-test-environment/build-vms.sh
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2038 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/winery-test-environment/ceph.yml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3932 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/winery-test-environment/fed4fire.rspec
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)      844 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/winery-test-environment/fed4fire.sh
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1836 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/winery-test-environment/grid5000.yml
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 11:21:20.733814 swh_objstorage-3.0.0/winery-test-environment/inventory/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 11:21:20.701815 swh_objstorage-3.0.0/winery-test-environment/inventory/group_vars/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 11:21:20.733814 swh_objstorage-3.0.0/winery-test-environment/inventory/group_vars/all/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      108 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/winery-test-environment/inventory/group_vars/all/rw.yml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       91 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/winery-test-environment/inventory/groups.yml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      822 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/winery-test-environment/inventory/hosts.yml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       84 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/winery-test-environment/inventory/osd.yml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       75 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/winery-test-environment/libvirt.yml
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 11:21:20.733814 swh_objstorage-3.0.0/winery-test-environment/mitogen-strategy/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       80 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/winery-test-environment/mitogen-strategy/README.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/winery-test-environment/mitogen-strategy/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2757 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/winery-test-environment/mitogen-strategy/mitogen.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2763 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/winery-test-environment/mitogen-strategy/mitogen_free.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2895 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/winery-test-environment/mitogen-strategy/mitogen_host_pinned.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2765 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/winery-test-environment/mitogen-strategy/mitogen_linear.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      824 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/winery-test-environment/osd.yml
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)     1333 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/winery-test-environment/remote-tox.sh
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1733 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/winery-test-environment/render-stats.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       40 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/winery-test-environment/requirements.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      198 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/winery-test-environment/rng.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2727 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/winery-test-environment/rw.yml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      632 2024-04-26 11:21:15.000000 swh_objstorage-3.0.0/winery-test-environment/tests.yml
```

### Comparing `swh_objstorage-2.9.3/.pre-commit-config.yaml` & `swh_objstorage-3.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `swh_objstorage-2.9.3/CODE_OF_CONDUCT.md` & `swh_objstorage-3.0.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `swh_objstorage-2.9.3/LICENSE` & `swh_objstorage-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `swh_objstorage-2.9.3/PKG-INFO` & `swh_objstorage-3.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.objstorage
-Version: 2.9.3
+Version: 3.0.0
 Summary: Software Heritage object storage
 Author-email: Software Heritage developers <swh-devel@inria.fr>
 Project-URL: Homepage, https://gitlab.softwareheritage.org/swh/devel/swh-objstorage
 Project-URL: Bug Reports, https://gitlab.softwareheritage.org/swh/devel/swh-objstorage/-/issues
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Documentation, https://docs.softwareheritage.org/devel/swh-objstorage/
 Project-URL: Source, https://gitlab.softwareheritage.org/swh/devel/swh-objstorage.git
```

### Comparing `swh_objstorage-2.9.3/README.rst` & `swh_objstorage-3.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `swh_objstorage-2.9.3/bin/swh-objstorage-azure` & `swh_objstorage-3.0.0/bin/swh-objstorage-azure`

 * *Files identical despite different names*

### Comparing `swh_objstorage-2.9.3/conftest.py` & `swh_objstorage-3.0.0/conftest.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-2.9.3/docs/winery.rst` & `swh_objstorage-3.0.0/docs/winery.rst`

 * *Files identical despite different names*

### Comparing `swh_objstorage-2.9.3/mypy.ini` & `swh_objstorage-3.0.0/mypy.ini`

 * *Files identical despite different names*

### Comparing `swh_objstorage-2.9.3/pyproject.toml` & `swh_objstorage-3.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `swh_objstorage-2.9.3/swh/objstorage/api/client.py` & `swh_objstorage-3.0.0/swh/objstorage/api/client.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-2.9.3/swh/objstorage/api/server.py` & `swh_objstorage-3.0.0/swh/objstorage/api/server.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-2.9.3/swh/objstorage/backends/azure.py` & `swh_objstorage-3.0.0/swh/objstorage/backends/azure.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-2.9.3/swh/objstorage/backends/generator.py` & `swh_objstorage-3.0.0/swh/objstorage/backends/generator.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-2.9.3/swh/objstorage/backends/http.py` & `swh_objstorage-3.0.0/swh/objstorage/backends/http.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-2.9.3/swh/objstorage/backends/in_memory.py` & `swh_objstorage-3.0.0/swh/objstorage/backends/in_memory.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-2.9.3/swh/objstorage/backends/libcloud.py` & `swh_objstorage-3.0.0/swh/objstorage/backends/libcloud.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-2.9.3/swh/objstorage/backends/noop.py` & `swh_objstorage-3.0.0/swh/objstorage/backends/noop.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-2.9.3/swh/objstorage/backends/pathslicing.py` & `swh_objstorage-3.0.0/swh/objstorage/backends/pathslicing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 # Copyright (C) 2015-2024  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 from contextlib import contextmanager
 from itertools import islice
+import logging
 import os
 import tempfile
-from typing import Iterator, List, Optional
+from typing import Iterator, List, Literal, Optional
 
-from swh.objstorage.constants import DEFAULT_LIMIT, ID_HASH_ALGO, ID_HEXDIGEST_LENGTH
+from swh.objstorage.constants import (
+    DEFAULT_LIMIT,
+    ID_HASH_ALGO,
+    ID_HEXDIGEST_LENGTH,
+    is_valid_hexdigest,
+)
 from swh.objstorage.exc import ObjNotFoundError
 from swh.objstorage.interface import CompositeObjId, ObjId
 from swh.objstorage.objstorage import (
     CompressionFormat,
     ObjStorage,
     compressors,
     objid_to_default_hex,
@@ -21,14 +27,23 @@
 
 BUFSIZ = 1048576
 
 DIR_MODE = 0o755
 FILE_MODE = 0o644
 
 
+logger = logging.getLogger(__name__)
+
+
+def is_valid_filename(filename: str, algo: Literal["sha1", "sha256"] = ID_HASH_ALGO):
+    """Checks that the file points to a valid hexdigest for the given algo."""
+
+    return is_valid_hexdigest(os.path.basename(filename), algo)
+
+
 class PathSlicer:
     """Helper class to compute a path based on a hash.
 
     Used to compute a directory path based on the object hash according to a
     given slicing. Each slicing correspond to a directory that is named
     according to the hash of its content.
 
@@ -147,15 +162,15 @@
             the disk.
         slicing (str): string that indicates the slicing to perform
             on the hash of the content to know the path where it should
             be stored (see the documentation of the PathSlicer class).
 
     """
 
-    PRIMARY_HASH = "sha1"
+    PRIMARY_HASH: Literal["sha1"] = "sha1"
 
     def __init__(
         self, root, slicing, compression: CompressionFormat = "gzip", **kwargs
     ):
         super().__init__(**kwargs)
         self.root = root
         self.slicer = PathSlicer(root, slicing)
@@ -209,14 +224,17 @@
         """
 
         # XXX hackish: it does not verify that the depth of found files
         # matches the slicing depth of the storage
         for root, _dirs, files in os.walk(self.root):
             _dirs.sort()
             for f in sorted(files):
+                if not is_valid_filename(f, algo=self.PRIMARY_HASH):
+                    logger.warning("__iter__ skipping over invalid file %s/%s", root, f)
+                    continue
                 yield {self.PRIMARY_HASH: bytes.fromhex(f)}
 
     def __len__(self) -> int:
         """Compute the number of objects available in the storage.
 
         Warning: this currently uses `__iter__`, its warning about bad
         performances applies
@@ -285,14 +303,19 @@
             dirs.sort()
             if dirs and root == os.path.join(self.root, *slices[:level]):
                 cslice = slices[level]
                 for d in dirs[:]:
                     if d < cslice:
                         dirs.remove(d)
             for f in sorted(files):
+                if not is_valid_filename(f, algo=self.PRIMARY_HASH):
+                    logger.warning(
+                        "iter_from skipping over invalid file %s/%s", root, f
+                    )
+                    continue
                 if f > hex_obj_id:
                     yield {self.PRIMARY_HASH: bytes.fromhex(f)}
         if n_leaf:
             yield i
 
     @contextmanager
     def _write_obj_file(self, hex_obj_id):
```

### Comparing `swh_objstorage-2.9.3/swh/objstorage/backends/seaweedfs/http.py` & `swh_objstorage-3.0.0/swh/objstorage/backends/seaweedfs/http.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-2.9.3/swh/objstorage/backends/seaweedfs/objstorage.py` & `swh_objstorage-3.0.0/swh/objstorage/backends/seaweedfs/objstorage.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-2.9.3/swh/objstorage/backends/winery/objstorage.py` & `swh_objstorage-3.0.0/swh/objstorage/backends/winery/objstorage.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # Copyright (C) 2022-2024  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
+from functools import partial
 import logging
 from multiprocessing import Process
-from typing import Callable, Optional, Tuple
+from typing import Callable, List, Optional, Tuple
 
 from swh.objstorage.exc import ObjNotFoundError
 from swh.objstorage.interface import ObjId
 from swh.objstorage.objstorage import ObjStorage
 
 from .roshard import (
     DEFAULT_IMAGE_FEATURES_UNSUPPORTED,
@@ -32,17 +33,14 @@
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         if kwargs.get("readonly"):
             self.winery = WineryReader(**kwargs)
         else:
             self.winery = WineryWriter(**kwargs)
 
-    def uninit(self):
-        self.winery.uninit()
-
     def get(self, obj_id: ObjId) -> bytes:
         return self.winery.get(self._hash(obj_id))
 
     def check_config(self, *, check_write: bool) -> bool:
         return True
 
     def __contains__(self, obj_id: ObjId) -> bool:
@@ -58,29 +56,29 @@
 
     def _hash(self, obj_id: ObjId) -> bytes:
         if isinstance(obj_id, dict):
             return obj_id[self.PRIMARY_HASH]
         else:
             return obj_id
 
+    def on_shutdown(self):
+        self.winery.on_shutdown()
+
 
 class WineryBase:
     def __init__(self, **kwargs):
         self.args = kwargs
-        self.init()
-
-    def init(self):
         self.base = SharedBase(**self.args)
 
-    def uninit(self):
-        self.base.uninit()
-
     def __contains__(self, obj_id):
         return self.base.contains(obj_id)
 
+    def on_shutdown(self):
+        return
+
 
 class WineryReader(WineryBase):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.ro_shards = {}
         self.rw_shards = {}
 
@@ -88,25 +86,24 @@
         if name not in self.ro_shards:
             try:
                 shard = ROShard(name, **self.args)
             except ShardNotMapped:
                 return None
             self.ro_shards[name] = shard
             if name in self.rw_shards:
-                self.rw_shards[name].uninit()
                 del self.rw_shards[name]
         return self.ro_shards[name]
 
     def rwshard(self, name) -> RWShard:
         if name not in self.rw_shards:
             shard = RWShard(name, **self.args)
             self.rw_shards[name] = shard
         return self.rw_shards[name]
 
-    def get(self, obj_id: ObjId) -> bytes:
+    def get(self, obj_id: bytes) -> bytes:
         shard_info = self.base.get(obj_id)
         if shard_info is None:
             raise ObjNotFoundError(obj_id)
         name, state = shard_info
         content: Optional[bytes] = None
         if state.image_available:
             roshard = self.roshard(name)
@@ -115,25 +112,16 @@
         if content is None:
             rwshard = self.rwshard(name)
             content = rwshard.get(obj_id)
         if content is None:
             raise ObjNotFoundError(obj_id)
         return content
 
-    def uninit(self):
-        for shard in self.rw_shards.values():
-            shard.uninit()
-        self.rw_shards = {}
-        for shard in self.ro_shards.values():
-            shard.close()
-        self.ro_shards = {}
-        super().uninit()
-
 
-def pack(shard, shared_base=None, clean_immediately=False, **kwargs):
+def pack(shard, shared_base=None, clean_immediately=False, **kwargs) -> bool:
     stats = Stats(kwargs.get("output_dir"))
     rw = RWShard(shard, **kwargs)
 
     count = rw.count()
     logger.info("Creating RO shard %s for %s objects", shard, count)
     with ROShardCreator(shard, count, **kwargs) as ro:
         logger.info("Created RO shard %s", shard)
@@ -143,87 +131,110 @@
                 stats.stats_read(obj_id, content)
                 stats.stats_write(obj_id, content)
             if i % 100 == 99:
                 logger.debug("RO shard %s: added %s/%s objects", shard, i + 1, count)
 
         logger.debug("RO shard %s: added %s objects, saving", shard, count)
 
-    logger.debug("RO shard %s: saved", shard)
+    logger.info("RO shard %s: saved", shard)
 
-    uninit_base = False
     if not shared_base:
         shared_base = SharedBase(**kwargs)
-        uninit_base = True
     shared_base.shard_packing_ends(shard)
-    rw.uninit()
     if clean_immediately:
         cleanup_rw_shard(shard, shared_base=shared_base, **kwargs)
-    if uninit_base:
-        shared_base.uninit()
     return True
 
 
-def cleanup_rw_shard(shard, shared_base=None, **kwargs):
+def cleanup_rw_shard(shard, shared_base=None, **kwargs) -> bool:
     rw = RWShard(shard, **{"shard_max_size": 0, **kwargs})
 
-    uninit_base = False
-    try:
-        if not shared_base:
-            shared_base = SharedBase(**kwargs)
-            uninit_base = True
-
-        rw.drop()
-        shared_base.set_shard_state(name=shard, new_state=ShardState.READONLY)
-    finally:
-        if shared_base and uninit_base:
-            shared_base.uninit()
+    rw.drop()
+
+    if not shared_base:
+        shared_base = SharedBase(**kwargs)
+    shared_base.set_shard_state(name=shard, new_state=ShardState.READONLY)
 
     return True
 
 
 class WineryWriter(WineryReader):
-    def __init__(self, **kwargs):
-        self.pack_immediately = kwargs.get("pack_immediately", True)
-        self.clean_immediately = kwargs.get("clean_immediately", True)
+    def __init__(
+        self,
+        pack_immediately: bool = True,
+        clean_immediately: bool = True,
+        rwshard_idle_timeout: float = 300,
+        **kwargs,
+    ):
+        self.pack_immediately = pack_immediately
+        self.clean_immediately = clean_immediately
         super().__init__(**kwargs)
-        self.shards_filled = []
-        self.packers = []
+        self.shards_filled: List[str] = []
+        self.packers: List[Process] = []
+        self._shard: Optional[RWShard] = None
+        self.idle_timeout = rwshard_idle_timeout
+
+    def release_shard(
+        self,
+        shard: Optional[RWShard] = None,
+        from_idle_handler: bool = False,
+        new_state: ShardState = ShardState.STANDBY,
+    ):
+        """Release the currently locked shard"""
+        if not shard:
+            shard = self._shard
 
-    def init(self):
-        super().init()
-        self.shard = RWShard(self.base.locked_shard, **self.args)
-        logger.debug("WineryBase: RWShard %s instantiated", self.base.locked_shard)
-
-    def uninit(self):
-        self.shard.uninit()
-        super().uninit()
+        if not shard:
+            return
 
-    def add(self, content: bytes, obj_id: ObjId, check_presence: bool = True) -> None:
+        logger.debug("WineryWriter releasing shard %s", shard.name)
+
+        self.base.set_shard_state(new_state=new_state, name=shard.name)
+        if not from_idle_handler:
+            logger.debug("Shard released, disabling idle handler")
+            shard.disable_idle_handler()
+        self._shard = None
+
+    @property
+    def shard(self):
+        """Lock a shard to be able to use it. Release it after :attr:`idle_timeout`."""
+        if not self._shard:
+            self._shard = RWShard(
+                self.base.locked_shard,
+                idle_timeout_cb=partial(self.release_shard, from_idle_handler=True),
+                idle_timeout=self.idle_timeout,
+                **self.args,
+            )
+            logger.debug(
+                "WineryBase: locked RWShard %s, releasing it in %s",
+                self._shard.name,
+                self.idle_timeout,
+            )
+        return self._shard
+
+    def add(self, content: bytes, obj_id: bytes, check_presence: bool = True) -> None:
         if check_presence and obj_id in self:
             return
 
-        shard = self.base.add_phase_1(obj_id)
-        if shard != self.base.locked_shard_id:
-            #  this object is the responsibility of another shard
-            return
+        with self.base.pool.connection() as db, db.transaction():
+            shard = self.base.record_new_obj_id(db, obj_id)
+            if shard != self.base.locked_shard_id:
+                #  this object is the responsibility of another shard
+                return
 
-        self.shard.add(obj_id, content)
-        self.base.add_phase_2(obj_id)
+            self.shard.add(db, obj_id, content)
 
         if self.shard.is_full():
-            self.base.set_shard_state(new_state=ShardState.FULL)
-            self.shards_filled.append(self.shard.name)
+            filled_name = self.shard.name
+            self.release_shard(new_state=ShardState.FULL)
+            self.shards_filled.append(filled_name)
             if self.pack_immediately:
-                self.pack()
-            else:
-                # Switch shards
-                self.uninit()
-                self.init()
+                self.pack(filled_name)
 
-    def delete(self, obj_id: ObjId):
+    def delete(self, obj_id: bytes):
         shard_info = self.base.get(obj_id)
         if shard_info is None:
             raise ObjNotFoundError(obj_id)
         name, state = shard_info
         # We only care about RWShard for now. ROShards will be
         # taken care in a batch job.
         if not state.image_available:
@@ -241,31 +252,35 @@
         self.base.delete(obj_id)
 
     def check(self, obj_id: ObjId) -> None:
         # load all shards packing == True and not locked (i.e. packer
         # was interrupted for whatever reason) run pack for each of them
         pass
 
-    def pack(self):
-        self.base.shard_packing_starts(self.shard.name)
+    def pack(self, shard_name: str):
+        self.base.shard_packing_starts(shard_name)
         p = Process(
             target=pack,
             kwargs={
-                "shard": self.shard.name,
+                "shard": shard_name,
                 "clean_immediately": self.clean_immediately,
                 **self.args,
             },
         )
-        self.uninit()
         p.start()
         self.packers.append(p)
-        self.init()
+
+    def on_shutdown(self):
+        self.release_shard()
 
     def __del__(self):
-        for p in self.packers:
+        for p in getattr(self, "packers", []):
+            if not p.is_alive():
+                continue
+            logger.warning("Killing packer %s", p)
             p.kill()
             p.join()
 
 
 def never_stop(_: int) -> bool:
     return False
 
@@ -275,25 +290,25 @@
         return shards_packed >= max_shards_packed
 
     return stop
 
 
 def shard_packer(
     base_dsn: str,
-    shard_dsn: str,
     shard_max_size: int,
     throttle_read: int,
     throttle_write: int,
     application_name: Optional[str] = None,
     rbd_pool_name: str = "shards",
     rbd_data_pool_name: Optional[str] = None,
     rbd_image_features_unsupported: Tuple[
         str, ...
     ] = DEFAULT_IMAGE_FEATURES_UNSUPPORTED,
     rbd_use_sudo: bool = True,
+    rbd_map_options: str = "",
     rbd_create_images: bool = True,
     rbd_wait_for_image: Callable[[int], None] = sleep_exponential(
         min_duration=5,
         factor=2,
         max_duration=60,
         message="Waiting for RBD image mapping",
     ),
@@ -308,15 +323,14 @@
 ) -> int:
     """Pack shards until the `stop_packing` function returns True.
 
     When no shards are available for packing, call the `wait_for_shard` function.
 
     Arguments:
       base_dsn: PostgreSQL dsn for the shared database
-      shard_dsn: PostgreSQL dsn for the individual shard databases
       shard_max_size: Max size of a shard (used to size new shards)
       throttle_read: reads per second
       throttle_write: writes per second
       application_name: the application name sent to PostgreSQL
       rbd_create_images: create images directly (or wait for RBD mapper)
       rbd_wait_for_image: sleep function called to wait for an image (when
        `rbd_create_images`=`False`)
@@ -328,54 +342,53 @@
     application_name = application_name or "Winery Shard Packer"
 
     base = SharedBase(base_dsn=base_dsn, application_name=application_name)
 
     shards_packed = 0
     waited_for_shards = 0
     while not stop_packing(shards_packed):
-        shard_to_pack = base.lock_one_shard(
+        locked = base.maybe_lock_one_shard(
             current_state=ShardState.FULL, new_state=ShardState.PACKING
         )
 
-        if not shard_to_pack:
+        if not locked:
             wait_for_shard(waited_for_shards)
             waited_for_shards += 1
             continue
 
         waited_for_shards = 0
 
-        name, _ = shard_to_pack
-        logger.info("shard_packer: Locked shard %s to pack", name)
-        ret = pack(
-            name,
-            base_dsn=base_dsn,
-            shard_dsn=shard_dsn,
-            shard_max_size=shard_max_size,
-            output_dir=output_dir,
-            shared_base=base,
-            throttle_read=throttle_read,
-            throttle_write=throttle_write,
-            application_name=application_name,
-            rbd_use_sudo=rbd_use_sudo,
-            rbd_create_images=rbd_create_images,
-            rbd_wait_for_image=rbd_wait_for_image,
-            rbd_pool_name=rbd_pool_name,
-            rbd_data_pool_name=rbd_data_pool_name,
-            rbd_image_features_unsupported=rbd_image_features_unsupported,
-        )
-        if not ret:
-            raise ValueError("Packing shard %s failed" % name)
-        shards_packed += 1
+        with locked:
+            logger.info("shard_packer: Locked shard %s to pack", locked.name)
+            ret = pack(
+                locked.name,
+                base_dsn=base_dsn,
+                shard_max_size=shard_max_size,
+                output_dir=output_dir,
+                shared_base=base,
+                throttle_read=throttle_read,
+                throttle_write=throttle_write,
+                application_name=application_name,
+                rbd_use_sudo=rbd_use_sudo,
+                rbd_map_options=rbd_map_options,
+                rbd_create_images=rbd_create_images,
+                rbd_wait_for_image=rbd_wait_for_image,
+                rbd_pool_name=rbd_pool_name,
+                rbd_data_pool_name=rbd_data_pool_name,
+                rbd_image_features_unsupported=rbd_image_features_unsupported,
+            )
+            if not ret:
+                raise ValueError("Packing shard %s failed" % locked.name)
+            shards_packed += 1
 
     return shards_packed
 
 
 def rw_shard_cleaner(
     base_dsn: str,
-    shard_dsn: str,
     min_mapped_hosts: int,
     application_name: Optional[str] = None,
     stop_cleaning: Callable[[int], bool] = never_stop,
     wait_for_shard: Callable[[int], None] = sleep_exponential(
         min_duration=5,
         factor=2,
         max_duration=60,
@@ -384,53 +397,52 @@
 ) -> int:
     """Clean up RW shards until the `stop_cleaning` function returns True.
 
     When no shards are available for packing, call the `wait_for_shard` function.
 
     Arguments:
       base_dsn: PostgreSQL dsn for the shared database
-      shard_dsn: PostgreSQL dsn for the individual shard databases
       min_mapped_hosts: how many hosts should have mapped the image read-only before
         cleaning it
       application_name: the application name sent to PostgreSQL
       stop_cleaning: callback to determine whether the cleaner should exit
       wait_for_shard: sleep function called when no shards are available to be cleaned
     """
     application_name = application_name or "Winery RW shard cleaner"
     base = SharedBase(base_dsn=base_dsn, application_name=application_name)
 
     shards_cleaned = 0
     waited_for_shards = 0
     while not stop_cleaning(shards_cleaned):
-        shard_to_clean = base.lock_one_shard(
+        locked = base.maybe_lock_one_shard(
             current_state=ShardState.PACKED,
             new_state=ShardState.CLEANING,
             min_mapped_hosts=min_mapped_hosts,
         )
 
-        if not shard_to_clean:
+        if not locked:
             wait_for_shard(waited_for_shards)
             waited_for_shards += 1
             continue
 
         waited_for_shards = 0
 
-        name, _ = shard_to_clean
-        logger.info("rw_shard_cleaner: Locked shard %s to clean", name)
+        with locked:
+            logger.info("rw_shard_cleaner: Locked shard %s to clean", locked.name)
 
-        ret = cleanup_rw_shard(
-            name,
-            base_dsn=base_dsn,
-            shard_dsn=shard_dsn,
-            shared_base=base,
-            application_name=application_name,
-        )
-        if not ret:
-            raise ValueError("Cleaning shard %s failed" % name)
-        shards_cleaned += 1
+            ret = cleanup_rw_shard(
+                locked.name,
+                base_dsn=base_dsn,
+                shared_base=base,
+                application_name=application_name,
+            )
+            if not ret:
+                raise ValueError("Cleaning shard %s failed" % locked.name)
+
+            shards_cleaned += 1
 
     return shards_cleaned
 
 
 def deleted_objects_cleaner(
     base: SharedBase,
     pool: Pool,
```

### Comparing `swh_objstorage-2.9.3/swh/objstorage/backends/winery/roshard.py` & `swh_objstorage-3.0.0/swh/objstorage/backends/winery/roshard.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 from collections import Counter
 import logging
 import math
 import os
+import shlex
 import socket
+import stat
 import subprocess
 import time
 from types import TracebackType
 from typing import Callable, Dict, Iterable, Optional, Tuple, Type
 
 from systemd.daemon import notify
 from typing_extensions import Literal
@@ -39,38 +41,44 @@
     Arguments:
       shard_max_size: max size of shard contents
       rbd_use_sudo: whether to use sudo for rbd commands
       rbd_pool_name: name of the pool used for RBD images (metadata)
       rbd_data_pool_name: name of the pool used for RBD images (data)
       rbd_image_features_unsupported: features not supported by the kernel
         mounting the rbd images
+      rbd_map_options: options to pass to ``rbd device map``, e.g.
+        ``ms_mode=prefer-secure`` to connect to a ceph cluster with encryption
+        enabled
     """
 
     def __init__(
         self,
         shard_max_size: int,
         rbd_use_sudo: bool = True,
         rbd_pool_name: str = "shards",
         rbd_data_pool_name: Optional[str] = None,
         rbd_image_features_unsupported: Tuple[
             str, ...
         ] = DEFAULT_IMAGE_FEATURES_UNSUPPORTED,
+        rbd_map_options: str = "",
     ) -> None:
         self.use_sudo = rbd_use_sudo
         self.pool_name = rbd_pool_name
         self.data_pool_name = rbd_data_pool_name or f"{self.pool_name}-data"
         self.features_unsupported = rbd_image_features_unsupported
+        self.map_options = rbd_map_options
         self.image_size = math.ceil((shard_max_size * 2) / (1024 * 1024))
 
     POOL_CONFIG: Tuple[str, ...] = (
         "shard_max_size",
         "rbd_use_sudo",
         "rbd_pool_name",
         "rbd_data_pool_name",
         "rbd_image_features_unsupported",
+        "rbd_map_options",
     )
 
     @classmethod
     def from_kwargs(cls, **kwargs) -> "Pool":
         """Create a Pool from a set of arbitrary keyword arguments"""
         return cls(**{k: kwargs[k] for k in cls.POOL_CONFIG if k in kwargs})
 
@@ -137,15 +145,21 @@
                 "disable",
                 f"{self.pool_name}/{image}",
                 *self.features_unsupported,
             )
         self.image_map(image, "rw")
 
     def image_map(self, image: str, options: str):
-        self.rbd("device", "map", "-o", options, image)
+        self.rbd(
+            "device",
+            "map",
+            "-o",
+            f"{options},{self.map_options}" if self.map_options else options,
+            image,
+        )
 
     def image_remap_ro(self, image: str):
         self.image_unmap(image)
         self.image_map(image, "ro")
 
     def image_unmap(self, image: str):
         if os.path.exists(self.image_path(image)):
@@ -320,16 +334,14 @@
     def close(self):
         if self.shard:
             self.shard.close()
         self.shard = None
 
     def __del__(self):
         self.close()
-        self.throttler.uninit()
-        super().__del__()
 
     @staticmethod
     def delete(pool, shard_name, obj_id):
         image_status = pool.image_mapped(shard_name)
         if image_status == "ro":
             raise PermissionError(
                 f"Cannot delete object from {shard_name}, mapped read-only"
@@ -379,26 +391,57 @@
             self.pool.image_create(self.name)
         else:
             attempt = 0
             while not os.path.exists(self.path):
                 self.rbd_wait_for_image(attempt)
                 attempt += 1
 
+        self.zero_image_if_needed()
+
         self.shard = ShardCreator(self.path, self.count)
         logger.debug("ROShard %s: created", self.name)
         self.shard.__enter__()
         return self
 
     def __exit__(
         self,
         exc_type: Optional[Type[BaseException]],
         exc_val: Optional[BaseException],
         exc_tb: Optional[TracebackType],
     ) -> None:
         self.shard.__exit__(exc_type, exc_val, exc_tb)
         if self.rbd_create_images and not exc_type:
             self.pool.image_remap_ro(self.name)
-        if not exc_type:
-            self.throttler.uninit()
+
+    def zero_image_if_needed(self):
+        """Check whether the image is empty, and zero it out if it's not.
+
+        We really check only the first 1kB, as we assume that the SWHShard
+        marker will have been written at the beginning of the image under all
+        circumstances if the RO Shard creation has been interrupted.
+        """
+        with open(self.path, "rb") as f:
+            start = f.read(1024)
+            if set(start) == {0}:
+                return
+
+        logger.warning("RO Shard %s isn't empty, cleaning it up", self.path)
+        st = os.stat(self.path)
+        if stat.S_ISBLK(st.st_mode):
+            # Block device, use DISCARD
+            command = ["/usr/sbin/blkdiscard", self.path]
+        else:
+            # Regular file, use fallocate --punch-hole
+            command = [
+                "/usr/bin/fallocate",
+                "--punch-hole",
+                "-l",
+                str(st.st_size),
+                self.path,
+            ]
+        try:
+            subprocess.run(command, check=True, capture_output=True)
+        except subprocess.CalledProcessError:
+            logger.warning("%s failed:", shlex.join(command), self.path, exc_info=True)
 
     def add(self, content, obj_id):
         return self.throttler.throttle_add(self.shard.write, obj_id, content)
```

### Comparing `swh_objstorage-2.9.3/swh/objstorage/backends/winery/sharedbase.py` & `swh_objstorage-3.0.0/swh/objstorage/backends/winery/sharedbase.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,21 +2,22 @@
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 from contextlib import ExitStack
 from enum import Enum
 import logging
-from typing import Iterator, Optional, Set, Tuple
+from types import TracebackType
+from typing import Iterator, Optional, Set, Tuple, Type
 import uuid
 
 import psycopg
 import psycopg.errors
 
-from .database import Database, DatabaseAdmin
+from .database import Database
 
 WRITER_UUID = uuid.uuid4()
 
 logger = logging.getLogger(__name__)
 
 
 class ShardState(Enum):
@@ -43,116 +44,82 @@
 
 class SignatureState(Enum):
     INFLIGHT = "inflight"
     PRESENT = "present"
     DELETED = "deleted"
 
 
-class SharedBase(Database):
-    def __init__(self, **kwargs) -> None:
-        DatabaseAdmin(
-            dsn=kwargs["base_dsn"],
-            dbname="sharedbase",
-            application_name=kwargs.get("application_name"),
-        ).create_database()
-        super().__init__(
-            dsn=kwargs["base_dsn"],
-            dbname="sharedbase",
-            application_name=kwargs.get("application_name"),
+class TemporaryShardLocker:
+    """Opportunistically lock a shard, and provide a context manager to unlock
+    the shard if an operation fails.
+
+    Use this through the :meth:`SharedBase.maybe_lock_one_shard` method.
+    """
+
+    def __init__(
+        self,
+        base: "SharedBase",
+        current_state: ShardState,
+        new_state: ShardState,
+        min_mapped_hosts: int = 0,
+    ) -> None:
+        self.base = base
+        self.previous_state = current_state
+        self.name: Optional[str] = None
+        self.id: Optional[int] = None
+        locked = self.base.lock_one_shard(
+            current_state=current_state,
+            new_state=new_state,
+            min_mapped_hosts=min_mapped_hosts,
         )
-        self.create_tables()
-        self._locked_shard: Optional[Tuple[str, int]] = None
+        if locked:
+            self.name, self.id = locked
 
-        logger.debug("SharedBase %s: instantiated", WRITER_UUID)
+    def __bool__(self) -> bool:
+        return self.name is not None
 
-    def uninit(self):
-        if self._locked_shard is not None:
-            self.set_shard_state(new_state=ShardState.STANDBY)
-        self._locked_shard = None
-        super().uninit()
+    def __enter__(self) -> "TemporaryShardLocker":
+        if not self:
+            raise ValueError("No shard was locked")
+        return self
 
-    @property
-    def lock(self):
-        return 314116  # an arbitrary unique number
+    def __exit__(
+        self,
+        exc_type: Optional[Type[Exception]],
+        exc_value: Optional[Exception],
+        traceback: Optional[TracebackType],
+    ) -> None:
+        """If an exception has been raised, restore the shard to its previous state"""
+        if not self:
+            return
 
-    @property
-    def database_tables(self):
-        return [
-            f"""\
-        DO $$ BEGIN
-          CREATE TYPE shard_state AS ENUM (
-            {", ".join("'%s'" % value.value for value in ShardState)}
-          );
-        EXCEPTION
-          WHEN duplicate_object THEN null;
-        END $$;
-            """,
-            "ALTER TYPE shard_state ADD VALUE IF NOT EXISTS 'cleaning' AFTER 'packed';",
-            """
-        CREATE TABLE IF NOT EXISTS shards(
-            id BIGSERIAL PRIMARY KEY,
-            state shard_state NOT NULL DEFAULT 'standby',
-            locker_ts TIMESTAMPTZ,
-            locker UUID,
-            name CHAR(32) NOT NULL UNIQUE,
-            mapped_on_hosts_when_packed TEXT[] NOT NULL DEFAULT '{}'
-        )
-        """,
-            """\
-        ALTER TABLE shards
-            ADD COLUMN
-              IF NOT EXISTS
-              mapped_on_hosts_when_packed TEXT[]
-              NOT NULL
-              DEFAULT '{}'
-        """,
-            f"""\
-        DO $$ BEGIN
-          CREATE TYPE signature_state AS ENUM (
-            {", ".join("'%s'" % value.value for value in SignatureState)}
-          );
-        EXCEPTION
-          WHEN duplicate_object THEN null;
-        END $$;
-        """,
-            """
-        CREATE TABLE IF NOT EXISTS signature2shard(
-            signature BYTEA PRIMARY KEY,
-            state signature_state NOT NULL DEFAULT 'inflight',
-            shard BIGINT NOT NULL REFERENCES shards(id)
+        if not exc_type:
+            return
+
+        try:
+            self.base.set_shard_state(
+                name=self.name, new_state=self.previous_state, check_locker=True
+            )
+        except Exception:
+            logger.warning("Could not unlock shard %s:", self.name, exc_info=True)
+
+
+class SharedBase(Database):
+    current_version: int = 1
+
+    def __init__(
+        self, base_dsn: str, application_name: str = "SWH Winery SharedBase", **kwargs
+    ) -> None:
+        super().__init__(
+            dsn=base_dsn,
+            application_name=application_name,
         )
-        """,
-            """\
-        DO $$ BEGIN
-            ALTER TABLE signature2shard
-                ALTER COLUMN inflight TYPE signature_state USING (
-                    CASE
-                      WHEN inflight THEN 'inflight'::signature_state
-                      ELSE 'present'::signature_state
-                    END),
-                ALTER COLUMN inflight SET DEFAULT 'inflight';
-            ALTER TABLE signature2shard
-                RENAME COLUMN inflight TO state;
-        EXCEPTION
-          WHEN undefined_column THEN NULL;
-        END $$;
-        """,
-            """\
-        ALTER TYPE signature_state ADD VALUE IF NOT EXISTS 'deleted' AFTER 'present';
-        """,
-            """\
-        CREATE INDEX IF NOT EXISTS signature2shard_deleted
-            ON signature2shard(signature, shard)
-         WHERE state = 'deleted'
-        """,
-            """\
-        CREATE INDEX IF NOT EXISTS signature2shard_shard_state
-            ON signature2shard(shard, state)
-        """,
-        ]
+        self._locked_shard: Optional[Tuple[str, int]] = None
+
+        logger.debug("SharedBase %s: instantiated", WRITER_UUID)
 
     @property
     def locked_shard(self) -> str:
         self.set_locked_shard()
 
         assert self._locked_shard, "failed to lock a shard"
         return self._locked_shard[0]
@@ -248,28 +215,60 @@
                     return None
                 else:
                     logger.debug(
                         "SharedBase %s: shard %s locked", WRITER_UUID, shard_name
                     )
                     return c.fetchone()
 
+    def maybe_lock_one_shard(
+        self,
+        current_state: ShardState,
+        new_state: ShardState,
+        min_mapped_hosts: int = 0,
+    ) -> TemporaryShardLocker:
+        """Opportunistically lock a shard, and, if a shard was locked, provide a
+        context manager to rollback the locking on failure.
+
+        Example::
+
+           locked = base.maybe_lock_one_shard(
+               current_state=ShardState.FULL,
+               new_state=ShardState.PACKING,
+           )
+           if not locked:
+               wait_a_minute()
+               return
+
+           with locked:
+               do_something_with_locked_shard(locked.name)
+
+        If ``do_something_with_locked_shard`` fails, the shard will be moved
+        back to the ``current_state`` on exit.
+        """
+        return TemporaryShardLocker(
+            base=self,
+            current_state=current_state,
+            new_state=new_state,
+            min_mapped_hosts=min_mapped_hosts,
+        )
+
     def set_shard_state(
         self,
         new_state: ShardState,
         set_locker: bool = False,
         check_locker: bool = False,
         name: Optional[str] = None,
         db: Optional[psycopg.Connection] = None,
     ):
-        reset_locked_shard = False
         if not name:
             if not self._locked_shard:
                 raise ValueError("Can't set shard state, no shard specified or locked")
             name = self._locked_shard[0]
-            reset_locked_shard = True
+
+        reset_locked_shard = self._locked_shard and self._locked_shard[0] == name
 
         with ExitStack() as stack:
             if not db:
                 db = stack.enter_context(self.pool.connection())
 
             assert isinstance(db, psycopg.Connection)
 
@@ -290,15 +289,16 @@
                     check_locker,
                     WRITER_UUID,
                 ),
             )
             affected = c.rowcount
             if affected != 1:
                 raise ValueError(
-                    "set_pack_state(%s) affected %s rows, expected 1" % (name, affected)
+                    "set_shard_state(%s) affected %s rows, expected 1"
+                    % (name, affected)
                 )
 
             logger.debug(
                 "SharedBase %s: shard %s moved into state %s",
                 WRITER_UUID,
                 name,
                 new_state,
@@ -428,20 +428,15 @@
                 (name,),
             )
             row = c.fetchone()
             if not row:
                 return 0
             return row[1]
 
-    def record_shard_mapped(self, host: str, name: Optional[str] = None) -> Set[str]:
-        if not name:
-            if not self._locked_shard:
-                raise ValueError("Can't set shard state, no shard specified or locked")
-            name = self._locked_shard[0]
-
+    def record_shard_mapped(self, host: str, name: str) -> Set[str]:
         with self.pool.connection() as db, db.transaction():
             with db.cursor() as c:
                 c.execute(
                     """SELECT mapped_on_hosts_when_packed
                        FROM shards
                        WHERE name = %s
                        FOR UPDATE SKIP LOCKED""",
@@ -475,42 +470,24 @@
 
     def get(self, obj_id) -> Optional[Tuple[str, ShardState]]:
         id = self.contains(obj_id)
         if id is None:
             return None
         return self.get_shard_info(id)
 
-    def add_phase_1(self, obj_id) -> Optional[int]:
-        try:
-            with self.pool.connection() as db:
-                db.execute(
-                    "INSERT INTO signature2shard (signature, shard, state) "
-                    "VALUES (%s, %s, 'inflight')",
-                    (obj_id, self.locked_shard_id),
-                )
-            return self.locked_shard_id
-        except psycopg.errors.UniqueViolation:
-            with self.pool.connection() as db:
-                c = db.execute(
-                    "SELECT shard FROM signature2shard WHERE "
-                    "signature = %s AND state = 'inflight'",
-                    (obj_id,),
-                )
-                row = c.fetchone()
-                if not row:
-                    return None
-                return row[0]
-
-    def add_phase_2(self, obj_id):
-        with self.pool.connection() as db:
-            db.execute(
-                "UPDATE signature2shard SET state = 'present' "
-                "WHERE signature = %s AND shard = %s",
-                (obj_id, self.locked_shard_id),
-            )
+    def record_new_obj_id(self, db, obj_id) -> Optional[int]:
+        db.execute(
+            "INSERT INTO signature2shard (signature, shard, state) "
+            "VALUES (%s, %s, 'present') ON CONFLICT (signature) DO NOTHING",
+            (obj_id, self.locked_shard_id),
+        )
+        cur = db.execute(
+            "SELECT shard FROM signature2shard WHERE signature = %s", (obj_id,)
+        )
+        return cur.fetchone()[0]
 
     def delete(self, obj_id):
         with self.pool.connection() as db:
             db.execute(
                 "UPDATE signature2shard SET state = 'deleted' WHERE signature = %s",
                 (obj_id,),
             )
```

### Comparing `swh_objstorage-2.9.3/swh/objstorage/backends/winery/sleep.py` & `swh_objstorage-3.0.0/swh/objstorage/backends/winery/sleep.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-2.9.3/swh/objstorage/backends/winery/stats.py` & `swh_objstorage-3.0.0/swh/objstorage/backends/winery/stats.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-2.9.3/swh/objstorage/backends/winery/throttler.py` & `swh_objstorage-3.0.0/swh/objstorage/backends/winery/throttler.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # See top-level LICENSE file for more information
 
 import collections
 import datetime
 import logging
 import time
 
-from .database import Database, DatabaseAdmin
+from .database import Database
 
 logger = logging.getLogger(__name__)
 
 
 class LeakyBucket:
     """
     Leaky bucket that can contain at most `total` and leaks it within a second.
@@ -96,26 +96,24 @@
     only allow max_speed/(number of instances) so that the total
     bandwidth is shared equally between instances.
     """
 
     def __init__(self, name, **kwargs):
         super().__init__(
             dsn=kwargs["base_dsn"],
-            dbname="throttler",
             application_name=kwargs.get("application_name", "SWH Winery Throttler"),
         )
         self.name = name
         self.init_db()
         self.last_sync = 0
         self.max_speed = kwargs["throttle_" + name]
         self.bucket = LeakyBucket(self.max_speed)
         self.bandwidth = BandwidthCalculator()
 
     def init_db(self):
-        self.create_tables()
         with self.pool.connection() as db, db.transaction(), db.cursor() as cur:
             cur.execute(
                 f"INSERT INTO t_{self.name} (updated, bytes) VALUES (%s, %s) RETURNING id",
                 (datetime.datetime.now(), 0),
             )
             self.rowid = cur.fetchone()[0]
             cur.execute(
@@ -124,31 +122,14 @@
             cur.execute(
                 f"DELETE FROM t_{self.name} WHERE id IN ("
                 f"SELECT id FROM t_{self.name} WHERE updated < NOW() - INTERVAL '30 days' "
                 " FOR UPDATE SKIP LOCKED)"
             )
         self.sync_interval = 60
 
-    @property
-    def lock(self):
-        return 9485433  # an arbitrary unique number
-
-    @property
-    def database_tables(self):
-        return [
-            f"""
-        CREATE TABLE IF NOT EXISTS t_{name} (
-            id SERIAL PRIMARY KEY,
-            updated TIMESTAMP NOT NULL,
-            bytes INTEGER NOT NULL
-        )
-       """
-            for name in ("read", "write")
-        ]
-
     def download_info(self):
         with self.pool.connection() as db:
             cur = db.execute(
                 f"SELECT COUNT(*), SUM(bytes) FROM t_{self.name} "
                 "WHERE bytes > 0 AND updated > NOW() - INTERVAL '5 minutes'"
             )
             return cur.fetchone()
@@ -190,23 +171,18 @@
 class Throttler:
     """Throttle reads and writes to not exceed limits imposed by the
     `thottle_read` and `throttle_write` arguments, as measured by the
     cumulated bandwidth reported by each Throttler instance.
     """
 
     def __init__(self, **kwargs):
-        DatabaseAdmin(kwargs["base_dsn"], "throttler").create_database()
         self.read = IOThrottler("read", **kwargs)
         self.write = IOThrottler("write", **kwargs)
 
     def throttle_get(self, fun, key):
         content = fun(key)
         self.read.add(len(content))
         return content
 
     def throttle_add(self, fun, obj_id, content):
         self.write.add(len(obj_id) + len(content))
         return fun(obj_id, content)
-
-    def uninit(self):
-        self.read.uninit()
-        self.write.uninit()
```

### Comparing `swh_objstorage-2.9.3/swh/objstorage/cli.py` & `swh_objstorage-3.0.0/swh/objstorage/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -127,40 +127,40 @@
 
     def set_signal_received(signum: int, _stack_frame: Optional[FrameType]) -> None:
         nonlocal signal_received
         logger.warning("Received signal %s, exiting", signal.strsignal(signum))
         signal_received = True
 
     base_dsn = config["base_dsn"]
-    shard_dsn = config["shard_dsn"]
     shard_max_size = config["shard_max_size"]
     throttle_read = config.get("throttle_read", 200 * 1024 * 1024)
     throttle_write = config.get("throttle_write", 200 * 1024 * 1024)
     output_dir = config.get("output_dir")
     rbd_pool_name = config.get("rbd_pool_name", "shards")
     rbd_data_pool_name = config.get("rbd_data_pool_name")
     rbd_use_sudo = config.get("rbd_use_sudo", True)
     rbd_image_features_unsupported = tuple(
         config.get("rbd_image_features_unsupported", DEFAULT_IMAGE_FEATURES_UNSUPPORTED)
     )
     rbd_create_images = config.get("rbd_create_images", True)
+    rbd_map_options = config.get("rbd_map_options", "")
 
     signal.signal(signal.SIGINT, set_signal_received)
     signal.signal(signal.SIGTERM, set_signal_received)
 
     ret = shard_packer(
         base_dsn=base_dsn,
-        shard_dsn=shard_dsn,
         shard_max_size=shard_max_size,
         throttle_read=throttle_read,
         throttle_write=throttle_write,
         rbd_pool_name=rbd_pool_name,
         rbd_data_pool_name=rbd_data_pool_name,
         rbd_image_features_unsupported=rbd_image_features_unsupported,
         rbd_use_sudo=rbd_use_sudo,
+        rbd_map_options=rbd_map_options,
         rbd_create_images=rbd_create_images,
         output_dir=output_dir,
         stop_packing=stop_packing,
     )
 
     logger.info("Packed %s shards", ret)
 
@@ -209,24 +209,26 @@
     rbd_pool_name = config.get("rbd_pool_name", "shards")
     rbd_data_pool_name = config.get("rbd_data_pool_name")
     rbd_use_sudo = config.get("rbd_use_sudo", True)
     rbd_image_features_unsupported = tuple(
         config.get("rbd_image_features_unsupported", DEFAULT_IMAGE_FEATURES_UNSUPPORTED)
     )
     rbd_manage_rw_images = config.get("rbd_manage_rw_images", True)
+    rbd_map_options = config.get("rbd_map_options", "")
 
     signal.signal(signal.SIGINT, set_signal_received)
     signal.signal(signal.SIGTERM, set_signal_received)
 
     pool = Pool(
         shard_max_size=shard_max_size,
         rbd_pool_name=rbd_pool_name,
         rbd_data_pool_name=rbd_data_pool_name,
         rbd_use_sudo=rbd_use_sudo,
         rbd_image_features_unsupported=rbd_image_features_unsupported,
+        rbd_map_options=rbd_map_options,
     )
 
     pool.manage_images(
         base_dsn=base_dsn,
         manage_rw_images=rbd_manage_rw_images,
         wait_for_image=wait_for_image,
         stop_running=stop_running,
@@ -282,22 +284,20 @@
 
     def set_signal_received(signum: int, _stack_frame: Optional[FrameType]) -> None:
         nonlocal stop_on_next_iteration
         logger.warning("Received signal %s, exiting", signal.strsignal(signum))
         stop_on_next_iteration = True
 
     base_dsn = config["base_dsn"]
-    shard_dsn = config["base_dsn"]
 
     signal.signal(signal.SIGINT, set_signal_received)
     signal.signal(signal.SIGTERM, set_signal_received)
 
     ret = rw_shard_cleaner(
         base_dsn=base_dsn,
-        shard_dsn=shard_dsn,
         min_mapped_hosts=min_mapped_hosts,
         stop_cleaning=stop_cleaning,
         wait_for_shard=wait_for_shard,
     )
 
     logger.info("RW shard cleaner exiting, %d shards cleaned", ret)
```

### Comparing `swh_objstorage-2.9.3/swh/objstorage/exc.py` & `swh_objstorage-3.0.0/swh/objstorage/exc.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-2.9.3/swh/objstorage/factory.py` & `swh_objstorage-3.0.0/swh/objstorage/factory.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-2.9.3/swh/objstorage/interface.py` & `swh_objstorage-3.0.0/swh/objstorage/interface.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-2.9.3/swh/objstorage/multiplexer/filter/__init__.py` & `swh_objstorage-3.0.0/swh/objstorage/multiplexer/filter/__init__.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-2.9.3/swh/objstorage/multiplexer/filter/filter.py` & `swh_objstorage-3.0.0/swh/objstorage/multiplexer/filter/filter.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-2.9.3/swh/objstorage/multiplexer/filter/read_write_filter.py` & `swh_objstorage-3.0.0/swh/objstorage/multiplexer/filter/read_write_filter.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-2.9.3/swh/objstorage/multiplexer/multiplexer_objstorage.py` & `swh_objstorage-3.0.0/swh/objstorage/multiplexer/multiplexer_objstorage.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-2.9.3/swh/objstorage/objstorage.py` & `swh_objstorage-3.0.0/swh/objstorage/objstorage.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-2.9.3/swh/objstorage/pytest_plugin.py` & `swh_objstorage-3.0.0/swh/objstorage/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-2.9.3/swh/objstorage/tests/objstorage_testing.py` & `swh_objstorage-3.0.0/swh/objstorage/tests/objstorage_testing.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-2.9.3/swh/objstorage/tests/test_interface.py` & `swh_objstorage-3.0.0/swh/objstorage/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-2.9.3/swh/objstorage/tests/test_objstorage_api.py` & `swh_objstorage-3.0.0/swh/objstorage/tests/test_objstorage_api.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-2.9.3/swh/objstorage/tests/test_objstorage_azure.py` & `swh_objstorage-3.0.0/swh/objstorage/tests/test_objstorage_azure.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-2.9.3/swh/objstorage/tests/test_objstorage_cloud.py` & `swh_objstorage-3.0.0/swh/objstorage/tests/test_objstorage_cloud.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-2.9.3/swh/objstorage/tests/test_objstorage_http.py` & `swh_objstorage-3.0.0/swh/objstorage/tests/test_objstorage_http.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-2.9.3/swh/objstorage/tests/test_objstorage_instantiation.py` & `swh_objstorage-3.0.0/swh/objstorage/tests/test_objstorage_instantiation.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-2.9.3/swh/objstorage/tests/test_objstorage_multiplexer.py` & `swh_objstorage-3.0.0/swh/objstorage/tests/test_objstorage_multiplexer.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-2.9.3/swh/objstorage/tests/test_objstorage_noop.py` & `swh_objstorage-3.0.0/swh/objstorage/tests/test_objstorage_noop.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-2.9.3/swh/objstorage/tests/test_objstorage_pathslicing.py` & `swh_objstorage-3.0.0/swh/objstorage/tests/test_objstorage_pathslicing.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # Copyright (C) 2015-2024  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
+import logging
+import os
 
 import pytest
 
 from swh.model import hashutil
 from swh.objstorage.constants import ID_DIGEST_LENGTH
 from swh.objstorage.exc import ObjCorruptedError
 
@@ -128,14 +130,52 @@
         with open(self.content_path(obj_id), "wb") as f:  # Replace by garbage.
             f.write(b"garbage")
         with pytest.raises(ObjCorruptedError, match="Object corrupted") as error:
             self.storage.check(obj_id)
         if self.compression != "none":
             assert "not a proper compressed file" in error.value.args[0]
 
+    def test__iter__skip_tmpfile(self, caplog):
+        content, obj_id = self.hash_content(b"skip_tmpfile")
+        self.storage.add(content, obj_id=obj_id)
+        path = self.storage.slicer.get_path(obj_id.hex())
+
+        dir = os.path.dirname(path)
+        bogus_path = os.path.join(dir, "bogus_file")
+        with open(bogus_path, "w") as f:
+            f.write("bogus")
+
+        with caplog.at_level(logging.WARNING, "swh.objstorage.backends.pathslicing"):
+            for _ in self.storage:
+                pass
+
+        assert len(caplog.records) == 1, [log.getMessage() for log in caplog.records]
+        message = caplog.records[0].getMessage()
+        assert "__iter__" in message
+        assert bogus_path in message
+
+    def test_iter_from_skip_tmpfile(self, caplog):
+        content, obj_id = self.hash_content(b"skip_tmpfile")
+        self.storage.add(content, obj_id=obj_id)
+        path = self.storage.slicer.get_path(obj_id.hex())
+
+        dir = os.path.dirname(path)
+        bogus_path = os.path.join(dir, "bogus_file")
+        with open(bogus_path, "w") as f:
+            f.write("bogus")
+
+        with caplog.at_level(logging.WARNING, "swh.objstorage.backends.pathslicing"):
+            for _ in self.storage.iter_from(obj_id=b"\x00" * 20):
+                pass
+
+        assert len(caplog.records) == 1, [log.getMessage() for log in caplog.records]
+        message = caplog.records[0].getMessage()
+        assert "iter_from" in message
+        assert bogus_path in message
+
 
 class TestPathSlicingObjStorageGzip(TestPathSlicingObjStorage):
     compression = "gzip"
 
 
 @pytest.mark.all_compression_methods
 class TestPathSlicingObjStorageZlib(TestPathSlicingObjStorage):
```

### Comparing `swh_objstorage-2.9.3/swh/objstorage/tests/test_objstorage_random_generator.py` & `swh_objstorage-3.0.0/swh/objstorage/tests/test_objstorage_random_generator.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-2.9.3/swh/objstorage/tests/test_objstorage_seaweedfs.py` & `swh_objstorage-3.0.0/swh/objstorage/tests/test_objstorage_seaweedfs.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-2.9.3/swh/objstorage/tests/test_objstorage_winery.py` & `swh_objstorage-3.0.0/swh/objstorage/tests/test_objstorage_winery.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,34 +2,39 @@
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 from collections import Counter
 from dataclasses import asdict, dataclass
 import datetime
+from functools import partial
 import logging
 import os
 import shutil
+import threading
 import time
 from typing import Any, Dict
 
 from click.testing import CliRunner
 import pytest
+from pytest_postgresql import factories
 import yaml
 
-from swh.objstorage.backends.winery.database import DatabaseAdmin
+from swh.core.db.db_utils import initialize_database_for_module
+import swh.objstorage.backends.winery.objstorage
 from swh.objstorage.backends.winery.objstorage import (
+    WineryObjStorage,
     cleanup_rw_shard,
     deleted_objects_cleaner,
     pack,
     rw_shard_cleaner,
     shard_packer,
     stop_after_shards,
 )
-from swh.objstorage.backends.winery.sharedbase import ShardState
+from swh.objstorage.backends.winery.sharedbase import ShardState, SharedBase
 from swh.objstorage.backends.winery.sleep import sleep_exponential
 from swh.objstorage.backends.winery.stats import Stats
 from swh.objstorage.backends.winery.throttler import (
     BandwidthCalculator,
     IOThrottler,
     LeakyBucket,
     Throttler,
@@ -74,42 +79,57 @@
                 return super().invoke(*args, **kwargs)
 
     return CapsysDisabledCliRunner()
 
 
 @pytest.fixture
 def remove_pool(request, pytestconfig):
+    if os.environ.get("CEPH_HARDCODE_POOL"):
+        return False
     marker = request.node.get_closest_marker("use_benchmark_flags")
     if marker is None:
         return True
 
     return pytestconfig.getoption("--winery-bench-remove-pool")
 
 
 @pytest.fixture
 def remove_images(request, pytestconfig):
+    if os.environ.get("CEPH_HARDCODE_POOL"):
+        return False
     marker = request.node.get_closest_marker("use_benchmark_flags")
     if marker is None:
         return True
 
     return pytestconfig.getoption("--winery-bench-remove-images")
 
 
 @pytest.fixture
 def rbd_pool_name(request, pytestconfig):
+    if os.environ.get("CEPH_HARDCODE_POOL"):
+        return os.environ["CEPH_HARDCODE_POOL"]
     marker = request.node.get_closest_marker("use_benchmark_flags")
     if marker is None:
         return "winery-test-shards"
 
     return pytestconfig.getoption("--winery-bench-rbd-pool")
 
 
 @pytest.fixture
-def ceph_pool(remove_pool, remove_images, rbd_pool_name, needs_ceph):
-    pool = PoolHelper(shard_max_size=10 * 1024 * 1024, rbd_pool_name=rbd_pool_name)
+def rbd_map_options():
+    return os.environ.get("RBD_MAP_OPTIONS", "")
+
+
+@pytest.fixture
+def ceph_pool(remove_pool, remove_images, rbd_pool_name, rbd_map_options, needs_ceph):
+    pool = PoolHelper(
+        shard_max_size=10 * 1024 * 1024,
+        rbd_pool_name=rbd_pool_name,
+        rbd_map_options=rbd_map_options,
+    )
     if remove_pool:
         pool.remove()
         pool.pool_create()
     else:
         logger.info("Not removing pool")
 
     yield pool
@@ -149,22 +169,30 @@
 
 
 @pytest.fixture
 def image_pool(request):
     return request.getfixturevalue(request.param)
 
 
+winery_postgresql_proc = factories.postgresql_proc(
+    load=[
+        partial(
+            initialize_database_for_module,
+            modname="objstorage.backends.winery",
+            version=SharedBase.current_version,
+        ),
+    ],
+)
+
+winery_postgresql = factories.postgresql("winery_postgresql_proc")
+
+
 @pytest.fixture
-def postgresql_dsn(postgresql_proc):
-    dsn = f"user={postgresql_proc.user} host={postgresql_proc.host} port={postgresql_proc.port}"
-    yield dsn
-    d = DatabaseAdmin(dsn)
-    for database in d.list_databases():
-        if database not in (postgresql_proc.dbname, f"{postgresql_proc.dbname}_tmpl"):
-            DatabaseAdmin(dsn, database).drop_database()
+def postgresql_dsn(winery_postgresql):
+    return winery_postgresql.info.dsn
 
 
 @pytest.fixture
 def shard_max_size(request) -> int:
     marker = request.node.get_closest_marker("shard_max_size")
     if marker is None:
         return 1024
@@ -188,50 +216,62 @@
         return True
     else:
         return marker.args[0]
 
 
 @pytest.fixture
 def storage(
-    shard_max_size, pack_immediately, clean_immediately, rbd_pool_name, postgresql_dsn
+    shard_max_size,
+    pack_immediately,
+    clean_immediately,
+    rbd_pool_name,
+    rbd_map_options,
+    postgresql_dsn,
 ):
     storage = get_objstorage(
         cls="winery",
         base_dsn=postgresql_dsn,
-        shard_dsn=postgresql_dsn,
         shard_max_size=shard_max_size,
         throttle_write=200 * 1024 * 1024,
         throttle_read=100 * 1024 * 1024,
         pack_immediately=pack_immediately,
         clean_immediately=clean_immediately,
         rbd_pool_name=rbd_pool_name,
+        rbd_map_options=rbd_map_options,
     )
+    assert isinstance(storage, WineryObjStorage)
     logger.debug("Instantiated storage %s on rbd pool %s", storage, rbd_pool_name)
     yield storage
-    storage.winery.uninit()
+    storage.on_shutdown()
+    names = [
+        thread.name
+        for thread in threading.enumerate()
+        if thread.name.startswith("IdleHandler")
+    ]
+    assert not names, f"Some IdleHandlers are still alive: {','.join(names)}"
 
 
 @pytest.fixture
 def winery(storage):
     return storage.winery
 
 
 def test_winery_sharedbase(winery):
     base = winery.base
-    shard1 = base.locked_shard
+    shard1 = winery.shard.name
     assert shard1 is not None
     assert shard1 == base.locked_shard
 
     id1 = base.locked_shard_id
     assert id1 is not None
     assert id1 == base.locked_shard_id
 
     assert base.get_shard_state(shard1) == ShardState.WRITING
 
-    winery.base.uninit()
+    winery.release_shard()
 
     assert winery.base._locked_shard is None
     assert base.get_shard_state(shard1) == ShardState.STANDBY
 
     shard2 = winery.base.locked_shard
 
     assert shard1 == shard2, "Locked a different shard?"
@@ -252,14 +292,61 @@
     assert winery.base.locked_shard == shard
     assert winery.get(obj_id) == content
     with pytest.raises(ObjNotFoundError):
         winery.get(b"unknown")
     winery.shard.drop()
 
 
+def test_winery_add_concurrent(winery, mocker):
+    num_threads = 4
+
+    class ManualReleaseSharedBase(SharedBase):
+        def __init__(self, *args, **kwargs):
+            super().__init__(*args, **kwargs)
+            self.release_obj_id = threading.Event()
+
+        def record_new_obj_id(self, *args, **kwargs):
+            ret = super().record_new_obj_id(*args, **kwargs)
+            self.release_obj_id.wait()
+            return ret
+
+    mocker.patch(
+        "swh.objstorage.backends.winery.objstorage.SharedBase", ManualReleaseSharedBase
+    )
+
+    content = b"test_concurrency"
+    obj_id = compute_hash(content, "sha256")
+
+    def add_object(my_storage):
+        my_storage.add(content=content, obj_id=obj_id)
+
+        assert my_storage.get(obj_id) == content
+
+    storages = [get_objstorage(cls="winery", **winery.args) for _ in range(num_threads)]
+
+    threads = [
+        threading.Thread(target=add_object, args=[storage]) for storage in storages
+    ]
+    for thread in threads:
+        thread.start()
+
+    for storage in reversed(storages):
+        storage.winery.base.release_obj_id.set()
+
+    for thread in threads:
+        thread.join()
+
+    assert winery.get(obj_id) == content
+    assert sum(1 for _ in winery.base.list_shards()) >= num_threads
+
+    for storage in storages:
+        assert isinstance(storage, WineryObjStorage)
+        storage.on_shutdown()
+
+
 @pytest.mark.shard_max_size(1)
 def test_winery_add_and_pack(winery, mocker):
     mocker.patch("swh.objstorage.backends.winery.objstorage.pack", return_value=True)
     shard = winery.base.locked_shard
     content = b"SOMETHING"
     winery.add(content=content, obj_id=compute_hash(content, "sha256"))
     assert winery.base.locked_shard != shard
@@ -382,17 +469,22 @@
 
 def test_winery_get_shard_info(winery):
     assert winery.base.get_shard_info(1234) is None
     assert winery.base.get_shard_state("nothing") is None
 
 
 def test_winery_base_record_shard_mapped(winery):
-    assert {"test"} == winery.base.record_shard_mapped("test")
-    assert {"test"} == winery.base.record_shard_mapped("test")
-    assert {"test", "test2"} == winery.base.record_shard_mapped("test2")
+    # Lock a shard
+    shard_name, shard_id = winery.base.create_shard(new_state=ShardState.PACKED)
+
+    assert {"test"} == winery.base.record_shard_mapped(host="test", name=shard_name)
+    assert {"test"} == winery.base.record_shard_mapped(host="test", name=shard_name)
+    assert {"test", "test2"} == winery.base.record_shard_mapped(
+        host="test2", name=shard_name
+    )
 
 
 @pytest.mark.shard_max_size(10 * 1024 * 1024)
 @pytest.mark.clean_immediately(False)
 def test_winery_pack(winery, image_pool):
     shard = winery.base.locked_shard
     content = b"SOMETHING"
@@ -490,89 +582,135 @@
 
     filled = storage.winery.shards_filled
     assert len(filled) == 4
 
     shard_info = dict(storage.winery.base.list_shards())
     for shard in filled:
         assert shard_info[shard] == ShardState.FULL
-    assert shard_info[storage.winery.base.locked_shard] == ShardState.WRITING
 
     # Pack a single shard
     assert (
         shard_packer(
             base_dsn=postgresql_dsn,
-            shard_dsn=postgresql_dsn,
             shard_max_size=shard_max_size,
             throttle_read=200 * 1024 * 1024,
             throttle_write=200 * 1024 * 1024,
             stop_packing=stop_after_shards(1),
             rbd_pool_name=image_pool.pool_name,
+            rbd_map_options=image_pool.map_options,
         )
         == 1
     )
 
     shard_counts = Counter(state for _, state in storage.winery.base.list_shards())
     assert shard_counts == {
         ShardState.FULL: 3,
         ShardState.PACKED: 1,
-        ShardState.WRITING: 1,
     }
 
     # Clean up the RW shard for the packed one
     assert (
         rw_shard_cleaner(
             base_dsn=postgresql_dsn,
-            shard_dsn=postgresql_dsn,
             min_mapped_hosts=0,
             stop_cleaning=stop_after_shards(1),
         )
         == 1
     )
 
     shard_counts = Counter(state for _, state in storage.winery.base.list_shards())
     assert shard_counts == {
         ShardState.FULL: 3,
         ShardState.READONLY: 1,
-        ShardState.WRITING: 1,
     }
 
     # Pack all remaining shards
     assert (
         shard_packer(
             base_dsn=postgresql_dsn,
-            shard_dsn=postgresql_dsn,
             shard_max_size=shard_max_size,
             throttle_read=200 * 1024 * 1024,
             throttle_write=200 * 1024 * 1024,
             stop_packing=stop_after_shards(3),
             rbd_pool_name=image_pool.pool_name,
+            rbd_map_options=image_pool.map_options,
         )
         == 3
     )
 
     shard_counts = Counter(state for _, state in storage.winery.base.list_shards())
     assert shard_counts == {
         ShardState.PACKED: 3,
         ShardState.READONLY: 1,
-        ShardState.WRITING: 1,
     }
 
     # Clean up the RW shard for the packed one
     assert (
         rw_shard_cleaner(
             base_dsn=postgresql_dsn,
-            shard_dsn=postgresql_dsn,
             min_mapped_hosts=0,
             stop_cleaning=stop_after_shards(3),
         )
         == 3
     )
 
     shard_counts = Counter(state for _, state in storage.winery.base.list_shards())
-    assert shard_counts == {ShardState.READONLY: 4, ShardState.WRITING: 1}
+    assert shard_counts == {ShardState.READONLY: 4}
+
+
+@pytest.mark.shard_max_size(1024)
+@pytest.mark.pack_immediately(False)
+def test_winery_packer_clean_up_interrupted_shard(
+    shard_max_size, image_pool, postgresql_dsn, storage, caplog
+):
+    caplog.set_level(logging.CRITICAL)
+
+    # create 1 full shard
+    for i in range(4):
+        content = i.to_bytes(256, "little")
+        obj_id = compute_hash(content, "sha256")
+        storage.add(content=content, obj_id=obj_id)
+
+    filled = storage.winery.shards_filled
+    assert len(filled) == 1
+
+    shard = filled[0]
+
+    if not image_pool.image_mapped(shard):
+        image_pool.image_create(shard)
+
+    with open(image_pool.image_path(shard), "wb") as f:
+        f.write(b"SWHShard interrupted bla")
+
+    with caplog.at_level(logging.WARNING, "swh.objstorage.backends.winery.roshard"):
+        # Pack a single shard
+        ret = shard_packer(
+            base_dsn=postgresql_dsn,
+            shard_max_size=shard_max_size,
+            throttle_read=200 * 1024 * 1024,
+            throttle_write=200 * 1024 * 1024,
+            stop_packing=stop_after_shards(1),
+            rbd_pool_name=image_pool.pool_name,
+            rbd_create_images=False,
+        )
+
+    assert ret == 1
+    found_cleanup_message = False
+    found_subprocess_error = False
+    for record in caplog.records:
+        msg = record.getMessage()
+        if image_pool.image_path(shard) in msg:
+            if "cleaning it up" in msg:
+                found_cleanup_message = True
+            elif "failed:" in msg:
+                found_subprocess_error = True
+    else:
+        assert found_cleanup_message and not found_subprocess_error, [
+            r.getMessage() for r in caplog.records
+        ]
 
 
 @pytest.mark.shard_max_size(1024)
 @pytest.mark.pack_immediately(False)
 @pytest.mark.clean_immediately(False)
 def test_winery_cli_packer(image_pool, storage, tmp_path, cli_runner):
     # create 4 shards
@@ -583,15 +721,14 @@
 
     filled = storage.winery.shards_filled
     assert len(filled) == 4
 
     shard_info = dict(storage.winery.base.list_shards())
     for shard in filled:
         assert shard_info[shard] == ShardState.FULL
-    assert shard_info[storage.winery.base.locked_shard] == ShardState.WRITING
 
     with open(tmp_path / "config.yml", "w") as f:
         yaml.safe_dump(
             {"objstorage": {"cls": "winery", **storage.winery.args}}, stream=f
         )
 
     result = cli_runner.invoke(
@@ -605,28 +742,73 @@
     shard_info = dict(storage.winery.base.list_shards())
     for shard in filled:
         assert shard_info[shard] == ShardState.PACKED
 
 
 @pytest.mark.shard_max_size(1024)
 @pytest.mark.pack_immediately(False)
+@pytest.mark.clean_immediately(False)
+def test_winery_cli_packer_rollback_on_error(image_pool, storage, tmp_path, cli_runner):
+    # create 4 shards
+    for i in range(16):
+        content = i.to_bytes(256, "little")
+        obj_id = compute_hash(content, "sha256")
+        storage.add(content=content, obj_id=obj_id)
+
+    filled = storage.winery.shards_filled
+    assert len(filled) == 4
+
+    shard_info = dict(storage.winery.base.list_shards())
+    for shard in filled:
+        assert shard_info[shard] == ShardState.FULL
+
+    with open(tmp_path / "config.yml", "w") as f:
+        yaml.safe_dump(
+            {"objstorage": {"cls": "winery", **storage.winery.args}}, stream=f
+        )
+
+    # pytest-mock doesn't seem to interact very well with the cli_runner
+    def failing_pack(*args, **kwargs):
+        raise ValueError("Packing failed")
+
+    orig_pack = swh.objstorage.backends.winery.objstorage.pack
+    try:
+        swh.objstorage.backends.winery.objstorage.pack = failing_pack
+        result = cli_runner.invoke(
+            swh_cli_group,
+            ("objstorage", "winery", "packer", "--stop-after-shards=4"),
+            env={"SWH_CONFIG_FILENAME": str(tmp_path / "config.yml")},
+        )
+    finally:
+        swh.objstorage.backends.winery.objstorage.pack = orig_pack
+
+    assert result.exit_code == 1
+
+    shard_info = dict(storage.winery.base.list_shards())
+    for shard in filled:
+        assert (
+            shard_info[shard] == ShardState.FULL
+        ), f"{shard} in state {shard_info[shard]}"
+
+
+@pytest.mark.shard_max_size(1024)
+@pytest.mark.pack_immediately(False)
 def test_winery_cli_rbd(image_pool, storage, tmp_path, cli_runner):
     # create 4 shards
     for i in range(16):
         content = i.to_bytes(256, "little")
         obj_id = compute_hash(content, "sha256")
         storage.add(content=content, obj_id=obj_id)
 
     filled = storage.winery.shards_filled
     assert len(filled) == 4
 
     shard_info = dict(storage.winery.base.list_shards())
     for shard in filled:
         assert shard_info[shard] == ShardState.FULL
-    assert shard_info[storage.winery.base.locked_shard] == ShardState.WRITING
 
     with open(tmp_path / "config.yml", "w") as f:
         yaml.safe_dump(
             {"objstorage": {"cls": "winery", **storage.winery.args}}, stream=f
         )
 
     result = cli_runner.invoke(
@@ -673,39 +855,36 @@
     for packer in storage.winery.packers:
         packer.join()
         assert packer.exitcode == 0
 
     shard_info = dict(storage.winery.base.list_shards())
     for shard in filled:
         assert shard_info[shard] == ShardState.PACKED
-    assert shard_info[storage.winery.base.locked_shard] == ShardState.WRITING
 
     with open(tmp_path / "config.yml", "w") as f:
         yaml.safe_dump(
             {"objstorage": {"cls": "winery", **storage.winery.args}}, stream=f
         )
 
-    db_admin = DatabaseAdmin(postgresql_dsn)
-
-    databases = set(db_admin.list_databases())
+    shard_tables = set(storage.winery.base.list_shard_tables())
     for shard in filled:
-        assert shard in databases
+        assert shard in shard_tables
 
     result = cli_runner.invoke(
         swh_cli_group,
         ("objstorage", "winery", "rw-shard-cleaner", "--stop-instead-of-waiting"),
         env={"SWH_CONFIG_FILENAME": str(tmp_path / "config.yml")},
     )
 
     assert result.exit_code == 0
 
     # No hosts have mapped the shard as remapped, so the cleaner has done nothing
-    databases = set(db_admin.list_databases())
+    shard_tables = set(storage.winery.base.list_shard_tables())
     for shard in filled:
-        assert shard in databases
+        assert shard in shard_tables
 
     result = cli_runner.invoke(
         swh_cli_group,
         (
             "objstorage",
             "winery",
             "rw-shard-cleaner",
@@ -714,17 +893,80 @@
         ),
         env={"SWH_CONFIG_FILENAME": str(tmp_path / "config.yml")},
     )
 
     assert result.exit_code == 0
 
     # Now we've forced action
-    databases = set(db_admin.list_databases())
+    shard_tables = set(storage.winery.base.list_shard_tables())
+    for shard in filled:
+        assert shard not in shard_tables
+
+
+@pytest.mark.shard_max_size(1024)
+@pytest.mark.pack_immediately(True)
+@pytest.mark.clean_immediately(False)
+def test_winery_cli_rw_shard_cleaner_rollback_on_error(
+    image_pool, postgresql_dsn, storage, tmp_path, cli_runner
+):
+    # create 4 shards
+    for i in range(16):
+        content = i.to_bytes(256, "little")
+        obj_id = compute_hash(content, "sha256")
+        storage.add(content=content, obj_id=obj_id)
+
+    filled = storage.winery.shards_filled
+    assert len(filled) == 4
+
+    for packer in storage.winery.packers:
+        packer.join()
+        assert packer.exitcode == 0
+
+    shard_info = dict(storage.winery.base.list_shards())
+    for shard in filled:
+        assert shard_info[shard] == ShardState.PACKED
+
+    with open(tmp_path / "config.yml", "w") as f:
+        yaml.safe_dump(
+            {"objstorage": {"cls": "winery", **storage.winery.args}}, stream=f
+        )
+
+    shard_tables = set(storage.winery.base.list_shard_tables())
     for shard in filled:
-        assert shard not in databases
+        assert shard in shard_tables
+
+    # pytest-mock doesn't seem to interact very well with the cli_runner
+    def failing_cleanup(*args, **kwargs):
+        raise ValueError("Cleanup failed")
+
+    orig_cleanup = swh.objstorage.backends.winery.objstorage.cleanup_rw_shard
+    try:
+        swh.objstorage.backends.winery.objstorage.cleanup_rw_shard = failing_cleanup
+
+        result = cli_runner.invoke(
+            swh_cli_group,
+            (
+                "objstorage",
+                "winery",
+                "rw-shard-cleaner",
+                "--stop-instead-of-waiting",
+                "--min-mapped-hosts=0",
+            ),
+            env={"SWH_CONFIG_FILENAME": str(tmp_path / "config.yml")},
+        )
+    finally:
+        swh.objstorage.backends.winery.objstorage.cleanup_rw_shard = orig_cleanup
+
+    assert result.exit_code == 1
+
+    shard_tables = set(storage.winery.base.list_shard_tables())
+    shard_info = dict(storage.winery.base.list_shards())
+    for shard in filled:
+        assert shard in shard_tables
+        assert shard_info[shard] == ShardState.PACKED
 
 
 @pytest.mark.shard_max_size(1024)
 @pytest.mark.pack_immediately(False)
 def test_winery_standalone_packer_never_stop_packing(
     image_pool, postgresql_dsn, shard_max_size, storage
 ):
@@ -736,74 +978,75 @@
 
     filled = storage.winery.shards_filled
     assert len(filled) == 4
 
     shard_info = dict(storage.winery.base.list_shards())
     for shard in filled:
         assert shard_info[shard] == ShardState.FULL
-    assert shard_info[storage.winery.base.locked_shard] == ShardState.WRITING
 
     class NoShardLeft(Exception):
         pass
 
     called = []
 
     def wait_five_times(attempt) -> None:
         called.append(attempt)
         if attempt >= 4:
             raise NoShardLeft(attempt)
 
     with pytest.raises(NoShardLeft):
         shard_packer(
             base_dsn=postgresql_dsn,
-            shard_dsn=postgresql_dsn,
             shard_max_size=shard_max_size,
             throttle_read=200 * 1024 * 1024,
             throttle_write=200 * 1024 * 1024,
             wait_for_shard=wait_five_times,
             rbd_pool_name=image_pool.pool_name,
+            rbd_map_options=image_pool.map_options,
         )
 
     assert called == list(range(5))
 
     shard_counts = Counter(state for _, state in storage.winery.base.list_shards())
-    assert shard_counts == {ShardState.PACKED: 4, ShardState.WRITING: 1}
+    assert shard_counts == {ShardState.PACKED: 4}
 
     called = []
 
     with pytest.raises(NoShardLeft):
         rw_shard_cleaner(
             base_dsn=postgresql_dsn,
-            shard_dsn=postgresql_dsn,
             min_mapped_hosts=0,
             wait_for_shard=wait_five_times,
         )
 
     assert called == list(range(5))
 
     shard_counts = Counter(state for _, state in storage.winery.base.list_shards())
-    assert shard_counts == {ShardState.READONLY: 4, ShardState.WRITING: 1}
+    assert shard_counts == {ShardState.READONLY: 4}
 
 
 @pytest.mark.shard_max_size(10 * 1024 * 1024)
 def test_winery_get_object(winery, image_pool):
     shard = winery.base.locked_shard
     content = b"SOMETHING"
     obj_id = compute_hash(content, "sha256")
     winery.add(content=content, obj_id=obj_id)
     winery.base.set_shard_state(ShardState.FULL)
     winery.base.shard_packing_starts(shard)
     assert pack(shard, **winery.args) is True
     assert winery.get(obj_id) == content
 
 
-def test_winery_ceph_pool(needs_ceph):
+@pytest.mark.skipif("CEPH_HARDCODE_POOL" in os.environ, reason="Ceph pool hardcoded")
+def test_winery_ceph_pool(needs_ceph, rbd_map_options):
     name = "IMAGE"
     pool = PoolHelper(
-        shard_max_size=10 * 1024 * 1024, rbd_pool_name="test-winery-ceph-pool"
+        shard_max_size=10 * 1024 * 1024,
+        rbd_pool_name="test-winery-ceph-pool",
+        rbd_map_options=rbd_map_options,
     )
     pool.remove()
     pool.pool_create()
     assert pool.image_mapped(name) is None
     pool.image_create(name)
     assert pool.image_mapped(name) == "rw"
     p = pool.image_path(name)
@@ -835,15 +1078,14 @@
     shards_info = list(storage.winery.base.list_shards())
     assert shards_info == [(locked_shard, ShardState.WRITING)]
     assert (
         work("rw", storage=storage, time_remaining=datetime.timedelta(seconds=300))
         == "rw"
     )
     shards_info = dict(storage.winery.base.list_shards())
-    assert len(shards_info) == 2
     assert shards_info[locked_shard].image_available
     #
     # ro worker reads a shard
     #
     args = {**storage.winery.args, "readonly": True}
     assert (
         work(
@@ -856,15 +1098,14 @@
     )
 
 
 @pytest.mark.shard_max_size(10 * 1024 * 1024)
 def test_winery_bench_work_pack(storage, image_pool):
     pack_args = {
         "base_dsn": storage.winery.args["base_dsn"],
-        "shard_dsn": storage.winery.args["shard_dsn"],
         "shard_max_size": storage.winery.args["shard_max_size"],
         "throttle_read": storage.winery.args["throttle_read"],
         "throttle_write": storage.winery.args["throttle_write"],
         "rbd_pool_name": image_pool.pool_name,
     }
     assert (
         work(
@@ -880,37 +1121,37 @@
 @pytest.mark.shard_max_size(10 * 1024 * 1024)
 def test_winery_bench_work_rbd(storage, image_pool):
     rbd_args = {
         "base_dsn": storage.winery.args["base_dsn"],
         "shard_max_size": storage.winery.args["shard_max_size"],
         "duration": 1,
         "rbd_pool_name": image_pool.pool_name,
+        "rbd_map_options": image_pool.map_options,
     }
     assert (
         work(
             "rbd",
             storage=storage,
             worker_args={"rbd": rbd_args},
             time_remaining=datetime.timedelta(seconds=300),
         )
         == "rbd"
     )
 
 
 @pytest.mark.shard_max_size(10 * 1024 * 1024)
 def test_winery_bench_work_rw_shard_cleaner(storage):
-    rbd_args = {
+    rw_shard_cleaner_args = {
         "base_dsn": storage.winery.args["base_dsn"],
-        "shard_dsn": storage.winery.args["shard_dsn"],
     }
     assert (
         work(
             "rw_shard_cleaner",
             storage=storage,
-            worker_args={"rw_shard_cleaner": rbd_args},
+            worker_args={"rw_shard_cleaner": rw_shard_cleaner_args},
             time_remaining=datetime.timedelta(seconds=300),
         )
         == "rw_shard_cleaner"
     )
 
 
 @pytest.mark.shard_max_size(10 * 1024 * 1024)
@@ -968,26 +1209,25 @@
     storage_config: Dict[str, Any]
     workers_per_kind: Dict[WorkerKind, int]
     worker_args: Dict[WorkerKind, Dict]
     duration: float
 
 
 @pytest.fixture
-def bench_options(pytestconfig, postgresql_dsn) -> WineryBenchOptions:
+def bench_options(pytestconfig, postgresql_dsn, rbd_map_options) -> WineryBenchOptions:
     output_dir = pytestconfig.getoption("--winery-bench-output-directory")
     shard_max_size = pytestconfig.getoption("--winery-bench-shard-max-size")
     pack_immediately = pytestconfig.getoption("--winery-bench-pack-immediately")
     duration = pytestconfig.getoption("--winery-bench-duration")
 
     storage_config = {
         "output_dir": output_dir,
         "shard_max_size": shard_max_size,
         "pack_immediately": pack_immediately,
         "base_dsn": postgresql_dsn,
-        "shard_dsn": postgresql_dsn,
         "throttle_read": pytestconfig.getoption("--winery-bench-throttle-read"),
         "throttle_write": pytestconfig.getoption("--winery-bench-throttle-write"),
         "rbd_pool_name": pytestconfig.getoption("--winery-bench-rbd-pool"),
     }
     workers_per_kind: Dict[WorkerKind, int] = {
         "ro": pytestconfig.getoption("--winery-bench-ro-workers"),
         "rw": pytestconfig.getoption("--winery-bench-rw-workers"),
@@ -999,36 +1239,34 @@
         "ro": {
             "max_request": pytestconfig.getoption(
                 "--winery-bench-ro-worker-max-request"
             )
         },
         "pack": {
             "base_dsn": postgresql_dsn,
-            "shard_dsn": postgresql_dsn,
             "output_dir": output_dir,
             "shard_max_size": shard_max_size,
             "rbd_create_images": False,
             "rbd_pool_name": pytestconfig.getoption("--winery-bench-rbd-pool"),
             "throttle_read": pytestconfig.getoption("--winery-bench-throttle-read"),
             "throttle_write": pytestconfig.getoption("--winery-bench-throttle-write"),
         },
         "stats": {
             "base_dsn": postgresql_dsn,
-            "shard_dsn": postgresql_dsn,
             "shard_max_size": shard_max_size,
             "interval": pytestconfig.getoption("--winery-bench-stats-interval"),
         },
         "rw_shard_cleaner": {
             "base_dsn": postgresql_dsn,
-            "shard_dsn": postgresql_dsn,
         },
         "rbd": {
             "base_dsn": postgresql_dsn,
             "shard_max_size": shard_max_size,
             "rbd_pool_name": pytestconfig.getoption("--winery-bench-rbd-pool"),
+            "rbd_map_options": rbd_map_options,
             "duration": duration,
         },
     }
 
     if not pack_immediately:
         worker_args["rw"] = {"block_until_packed": False}
         workers_per_kind["pack"] = pytestconfig.getoption("--winery-bench-pack-workers")
@@ -1198,15 +1436,14 @@
         going_down.append(b.get())
     going_down.reverse()
     assert going_up[:-1] == going_down
     assert len(b.history) == b.duration - 1
 
 
 def test_winery_io_throttler(postgresql_dsn, mocker):
-    DatabaseAdmin(postgresql_dsn, "throttler").create_database()
     sleep = mocker.spy(time, "sleep")
     speed = 100
     i = IOThrottler("read", base_dsn=postgresql_dsn, throttle_read=100)
     count = speed
     i.add(count)
     sleep.assert_not_called()
     i.add(count)
```

### Comparing `swh_objstorage-2.9.3/swh/objstorage/tests/test_pathslicer.py` & `swh_objstorage-3.0.0/swh/objstorage/tests/test_pathslicer.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-2.9.3/swh/objstorage/tests/test_readonly_filter.py` & `swh_objstorage-3.0.0/swh/objstorage/tests/test_readonly_filter.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-2.9.3/swh/objstorage/tests/test_server.py` & `swh_objstorage-3.0.0/swh/objstorage/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-2.9.3/swh/objstorage/tests/winery_benchmark.py` & `swh_objstorage-3.0.0/swh/objstorage/tests/winery_benchmark.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,25 +69,25 @@
                         **storage,
                         "readonly": True,
                     },
                 )
             return ROWorker(storage, **kind_args).run(time_remaining=time_remaining)
         finally:
             if isinstance(storage, WineryObjStorage):
-                storage.winery.uninit()
+                storage.on_shutdown()
     elif kind == "rw":
         try:
             if isinstance(storage, dict):
                 storage = get_objstorage(
                     cls="winery", application_name=application_name, **storage
                 )
             return RWWorker(storage, **kind_args).run(time_remaining=time_remaining)
         finally:
             if isinstance(storage, WineryObjStorage):
-                storage.winery.uninit()
+                storage.on_shutdown()
     elif kind == "pack":
         return PackWorker(application_name=application_name, **kind_args).run()
     elif kind == "rbd":
         return RBDWorker(application_name=application_name, **kind_args).run()
     elif kind == "rw_shard_cleaner":
         return RWShardCleanerWorker(
             application_name=application_name, **kind_args
@@ -112,25 +112,23 @@
         raise NotImplementedError
 
 
 class PackWorker:
     def __init__(
         self,
         base_dsn: str,
-        shard_dsn: str,
         shard_max_size: int,
         throttle_read: int,
         throttle_write: int,
         application_name: Optional[str] = None,
         rbd_create_images: bool = True,
         rbd_pool_name: str = "shards",
         output_dir: Optional[str] = None,
     ):
         self.base_dsn = base_dsn
-        self.shard_dsn = shard_dsn
         self.shard_max_size = shard_max_size
         self.output_dir = output_dir
         self.throttle_read = throttle_read
         self.throttle_write = throttle_write
         self.rbd_create_images = rbd_create_images
         self.rbd_pool_name = rbd_pool_name
         self.application_name = application_name
@@ -144,15 +142,14 @@
             raise ValueError("Shard waited for too long")
         time.sleep(0.1)
         self.waited += 1
 
     def run(self) -> Literal["pack"]:
         shard_packer(
             base_dsn=self.base_dsn,
-            shard_dsn=self.shard_dsn,
             shard_max_size=self.shard_max_size,
             throttle_read=self.throttle_read,
             throttle_write=self.throttle_write,
             rbd_pool_name=self.rbd_pool_name,
             rbd_create_images=self.rbd_create_images,
             rbd_wait_for_image=self.wait_for_shard,
             output_dir=self.output_dir,
@@ -164,22 +161,24 @@
 
 
 class RBDWorker:
     def __init__(
         self,
         base_dsn: str,
         rbd_pool_name: str,
+        rbd_map_options: str,
         shard_max_size: int,
         application_name: Optional[str] = None,
         duration: int = 10,
     ):
         self.base_dsn = base_dsn
         self.pool = Pool(
             shard_max_size=shard_max_size,
             rbd_pool_name=rbd_pool_name,
+            rbd_map_options=rbd_map_options,
         )
         self.duration = duration
         self.started = time.monotonic()
         self.application_name = application_name
         self.waited = 0
 
     def wait_for_shard(self, attempt: int) -> None:
@@ -200,21 +199,19 @@
         return "rbd"
 
 
 class RWShardCleanerWorker:
     def __init__(
         self,
         base_dsn: str,
-        shard_dsn: str,
         min_mapped_hosts: int = 1,
         application_name: Optional[str] = None,
         duration: int = 10,
     ):
         self.base_dsn = base_dsn
-        self.shard_dsn = shard_dsn
         self.min_mapped_hosts = min_mapped_hosts
         self.application_name = application_name
         self.duration = duration
         self.started = time.monotonic()
         self.waited = 0
 
     def stop_cleaning(self, num_cleaned: int) -> bool:
@@ -223,43 +220,39 @@
     def wait_for_shard(self, attempt: int) -> None:
         time.sleep(1)
         self.waited += 1
 
     def run(self) -> Literal["rw_shard_cleaner"]:
         rw_shard_cleaner(
             base_dsn=self.base_dsn,
-            shard_dsn=self.shard_dsn,
             min_mapped_hosts=self.min_mapped_hosts,
             stop_cleaning=self.stop_cleaning,
             wait_for_shard=self.wait_for_shard,
             application_name=self.application_name,
         )
         return "rw_shard_cleaner"
 
 
 class StatsPrinter:
     def __init__(
         self,
         base_dsn: str,
-        shard_dsn: str,
         shard_max_size: int,
         application_name: Optional[str] = None,
         interval: int = 5 * 60,
     ):
         self.base_dsn = base_dsn
-        self.shard_dsn = shard_dsn
         self.shard_max_size = shard_max_size
         self.interval = datetime.timedelta(seconds=interval)
         self.application_name = application_name or "Winery Benchmark Stats Printer"
         self.objects_per_shard: Dict[str, int] = {}
 
     def get_winery_reader(self) -> WineryReader:
         return WineryReader(
             base_dsn=self.base_dsn,
-            shard_dsn=self.shard_dsn,
             shard_max_size=self.shard_max_size,
             application_name=self.application_name,
         )
 
     def run(self, time_remaining: datetime.timedelta) -> Literal["stats"]:
         try:
             return self._run(time_remaining)
@@ -402,15 +395,15 @@
                     if self.stats.stats_active:
                         self.stats.stats_read(obj_id, content)
 
         elapsed = time.monotonic() - start
         logger.info("Worker(ro, %s): finished (%.2fs)", os.getpid(), elapsed)
 
     def finalize(self):
-        self.storage.winery.uninit()
+        self.storage.on_shutdown()
 
 
 class RWWorker(Worker):
     """A read-write benchmark worker
 
     Args:
       storage: the read-write storage used
@@ -478,15 +471,15 @@
             return False
         if self.single_shard and self.winery.shards_filled:
             return False
 
         return True
 
     def finalize(self):
-        self.winery.uninit()
+        self.storage.on_shutdown()
 
         if not self.block_until_packed:
             return
         logger.info(
             "Worker(rw, %s): waiting for %s objects to be packed",
             os.getpid(),
             self.count,
```

### Comparing `swh_objstorage-2.9.3/swh/objstorage/tests/winery_testing_helpers.py` & `swh_objstorage-3.0.0/swh/objstorage/tests/winery_testing_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,23 +37,25 @@
         shard_max_size: int,
         rbd_use_sudo: bool = True,
         rbd_pool_name: str = "test-shards",
         rbd_data_pool_name: Optional[str] = None,
         rbd_image_features_unsupported: Tuple[
             str, ...
         ] = DEFAULT_IMAGE_FEATURES_UNSUPPORTED,
+        rbd_map_options: str = "",
         rbd_erasure_code_profile=None,
         rbd_data_pool_settings=None,
     ):
         super().__init__(
             shard_max_size=shard_max_size,
             rbd_use_sudo=rbd_use_sudo,
             rbd_pool_name=rbd_pool_name,
             rbd_data_pool_name=rbd_data_pool_name,
             rbd_image_features_unsupported=rbd_image_features_unsupported,
+            rbd_map_options=rbd_map_options,
         )
         self.erasure_code_profile_settings = (
             rbd_erasure_code_profile or DEFAULT_ERASURE_CODE_PROFILE.copy()
         )
         self.erasure_code_profile = self.erasure_code_profile_settings.pop(
             "name", DEFAULT_ERASURE_CODE_PROFILE["name"]
         )
@@ -192,14 +194,16 @@
         return [entry.name for entry in self.pool_dir.iterdir() if entry.is_file()]
 
     def image_path(self, image: str) -> str:
         return str(self.pool_dir / image)
 
     def image_create(self, image: str) -> None:
         path = self.image_path(image)
+        if os.path.exists(path):
+            raise ValueError(f"Image {image} already exists")
         open(path, "w").close()
         os.truncate(path, self.image_size * 1024 * 1024)
         self.image_map(image, "rw")
 
     def image_map(self, image: str, options: str) -> None:
         if "ro" in options:
             os.chmod(self.image_path(image), 0o400)
```

### Comparing `swh_objstorage-2.9.3/swh/objstorage/utils.py` & `swh_objstorage-3.0.0/swh/objstorage/utils.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-2.9.3/swh.objstorage.egg-info/PKG-INFO` & `swh_objstorage-3.0.0/swh.objstorage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.objstorage
-Version: 2.9.3
+Version: 3.0.0
 Summary: Software Heritage object storage
 Author-email: Software Heritage developers <swh-devel@inria.fr>
 Project-URL: Homepage, https://gitlab.softwareheritage.org/swh/devel/swh-objstorage
 Project-URL: Bug Reports, https://gitlab.softwareheritage.org/swh/devel/swh-objstorage/-/issues
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Documentation, https://docs.softwareheritage.org/devel/swh-objstorage/
 Project-URL: Source, https://gitlab.softwareheritage.org/swh/devel/swh-objstorage.git
```

### Comparing `swh_objstorage-2.9.3/swh.objstorage.egg-info/SOURCES.txt` & `swh_objstorage-3.0.0/swh.objstorage.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -56,21 +56,24 @@
 swh/objstorage/backends/noop.py
 swh/objstorage/backends/pathslicing.py
 swh/objstorage/backends/seaweedfs/__init__.py
 swh/objstorage/backends/seaweedfs/http.py
 swh/objstorage/backends/seaweedfs/objstorage.py
 swh/objstorage/backends/winery/__init__.py
 swh/objstorage/backends/winery/database.py
+swh/objstorage/backends/winery/gunicorn.py
 swh/objstorage/backends/winery/objstorage.py
 swh/objstorage/backends/winery/roshard.py
 swh/objstorage/backends/winery/rwshard.py
 swh/objstorage/backends/winery/sharedbase.py
 swh/objstorage/backends/winery/sleep.py
 swh/objstorage/backends/winery/stats.py
 swh/objstorage/backends/winery/throttler.py
+swh/objstorage/backends/winery/sql/30-schema.sql
+swh/objstorage/backends/winery/sql/__init__.py
 swh/objstorage/multiplexer/__init__.py
 swh/objstorage/multiplexer/multiplexer_objstorage.py
 swh/objstorage/multiplexer/filter/__init__.py
 swh/objstorage/multiplexer/filter/filter.py
 swh/objstorage/multiplexer/filter/read_write_filter.py
 swh/objstorage/tests/__init__.py
 swh/objstorage/tests/objstorage_testing.py
```

### Comparing `swh_objstorage-2.9.3/tox.ini` & `swh_objstorage-3.0.0/tox.ini`

 * *Files identical despite different names*

### Comparing `swh_objstorage-2.9.3/winery-test-environment/README.md` & `swh_objstorage-3.0.0/winery-test-environment/README.md`

 * *Files identical despite different names*

### Comparing `swh_objstorage-2.9.3/winery-test-environment/bootstrap.yml` & `swh_objstorage-3.0.0/winery-test-environment/bootstrap.yml`

 * *Files identical despite different names*

### Comparing `swh_objstorage-2.9.3/winery-test-environment/build-vms.sh` & `swh_objstorage-3.0.0/winery-test-environment/build-vms.sh`

 * *Files identical despite different names*

### Comparing `swh_objstorage-2.9.3/winery-test-environment/ceph.yml` & `swh_objstorage-3.0.0/winery-test-environment/ceph.yml`

 * *Files identical despite different names*

### Comparing `swh_objstorage-2.9.3/winery-test-environment/fed4fire.rspec` & `swh_objstorage-3.0.0/winery-test-environment/fed4fire.rspec`

 * *Files identical despite different names*

### Comparing `swh_objstorage-2.9.3/winery-test-environment/fed4fire.sh` & `swh_objstorage-3.0.0/winery-test-environment/fed4fire.sh`

 * *Files identical despite different names*

### Comparing `swh_objstorage-2.9.3/winery-test-environment/grid5000.yml` & `swh_objstorage-3.0.0/winery-test-environment/grid5000.yml`

 * *Files identical despite different names*

### Comparing `swh_objstorage-2.9.3/winery-test-environment/inventory/hosts.yml` & `swh_objstorage-3.0.0/winery-test-environment/inventory/hosts.yml`

 * *Files identical despite different names*

### Comparing `swh_objstorage-2.9.3/winery-test-environment/mitogen-strategy/mitogen.py` & `swh_objstorage-3.0.0/winery-test-environment/mitogen-strategy/mitogen.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-2.9.3/winery-test-environment/mitogen-strategy/mitogen_free.py` & `swh_objstorage-3.0.0/winery-test-environment/mitogen-strategy/mitogen_free.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-2.9.3/winery-test-environment/mitogen-strategy/mitogen_host_pinned.py` & `swh_objstorage-3.0.0/winery-test-environment/mitogen-strategy/mitogen_host_pinned.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-2.9.3/winery-test-environment/mitogen-strategy/mitogen_linear.py` & `swh_objstorage-3.0.0/winery-test-environment/mitogen-strategy/mitogen_linear.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-2.9.3/winery-test-environment/osd.yml` & `swh_objstorage-3.0.0/winery-test-environment/osd.yml`

 * *Files identical despite different names*

### Comparing `swh_objstorage-2.9.3/winery-test-environment/remote-tox.sh` & `swh_objstorage-3.0.0/winery-test-environment/remote-tox.sh`

 * *Files identical despite different names*

### Comparing `swh_objstorage-2.9.3/winery-test-environment/render-stats.py` & `swh_objstorage-3.0.0/winery-test-environment/render-stats.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-2.9.3/winery-test-environment/rw.yml` & `swh_objstorage-3.0.0/winery-test-environment/rw.yml`

 * *Files identical despite different names*

### Comparing `swh_objstorage-2.9.3/winery-test-environment/tests.yml` & `swh_objstorage-3.0.0/winery-test-environment/tests.yml`

 * *Files identical despite different names*

