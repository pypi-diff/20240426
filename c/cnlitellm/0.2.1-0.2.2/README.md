# Comparing `tmp/cnlitellm-0.2.1.tar.gz` & `tmp/cnlitellm-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnlitellm-0.2.1.tar", last modified: Wed Apr 24 14:12:37 2024, max compression
+gzip compressed data, was "cnlitellm-0.2.2.tar", last modified: Fri Apr 26 09:53:30 2024, max compression
```

## Comparing `cnlitellm-0.2.1.tar` & `cnlitellm-0.2.2.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-04-24 14:12:37.161248 cnlitellm-0.2.1/
--rw-r--r--   0 everfly    (501) staff       (20)       44 2024-03-19 10:47:10.000000 cnlitellm-0.2.1/LICENSE
--rw-r--r--   0 everfly    (501) staff       (20)      448 2024-04-24 14:12:37.161077 cnlitellm-0.2.1/PKG-INFO
--rw-r--r--   0 everfly    (501) staff       (20)       82 2024-03-19 10:47:10.000000 cnlitellm-0.2.1/README.md
-drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-04-24 14:12:37.150160 cnlitellm-0.2.1/cnlitellm/
--rw-r--r--   0 everfly    (501) staff       (20)        0 2024-03-19 10:47:10.000000 cnlitellm-0.2.1/cnlitellm/__init__.py
-drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-04-24 14:12:37.151633 cnlitellm-0.2.1/cnlitellm/__pycache__/
--rw-r--r--   0 everfly    (501) staff       (20)      140 2024-03-21 11:21:03.000000 cnlitellm-0.2.1/cnlitellm/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0 everfly    (501) staff       (20)     1790 2024-03-21 11:21:03.000000 cnlitellm-0.2.1/cnlitellm/__pycache__/models.cpython-312.pyc
--rw-r--r--   0 everfly    (501) staff       (20)    14486 2024-03-29 11:12:45.000000 cnlitellm-0.2.1/cnlitellm/__pycache__/utils.cpython-312.pyc
--rw-r--r--   0 everfly    (501) staff       (20)     1967 2024-04-20 11:21:30.000000 cnlitellm-0.2.1/cnlitellm/api.py
--rw-r--r--   0 everfly    (501) staff       (20)      306 2024-03-19 10:47:10.000000 cnlitellm-0.2.1/cnlitellm/exceptions.py
--rw-r--r--   0 everfly    (501) staff       (20)     1195 2024-03-19 10:47:10.000000 cnlitellm-0.2.1/cnlitellm/models.py
-drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-04-24 14:12:37.155229 cnlitellm-0.2.1/cnlitellm/providers/
--rw-r--r--   0 everfly    (501) staff       (20)        0 2024-03-19 10:47:10.000000 cnlitellm-0.2.1/cnlitellm/providers/__init__.py
-drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-04-24 14:12:37.157216 cnlitellm-0.2.1/cnlitellm/providers/__pycache__/
--rw-r--r--   0 everfly    (501) staff       (20)      150 2024-03-21 11:21:03.000000 cnlitellm-0.2.1/cnlitellm/providers/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0 everfly    (501) staff       (20)     4455 2024-03-29 11:12:45.000000 cnlitellm-0.2.1/cnlitellm/providers/__pycache__/baichuan.cpython-312.pyc
--rw-r--r--   0 everfly    (501) staff       (20)     2682 2024-03-21 11:21:03.000000 cnlitellm-0.2.1/cnlitellm/providers/__pycache__/base_provider.cpython-312.pyc
--rw-r--r--   0 everfly    (501) staff       (20)     4252 2024-03-29 11:12:45.000000 cnlitellm-0.2.1/cnlitellm/providers/__pycache__/minimax.cpython-312.pyc
--rw-r--r--   0 everfly    (501) staff       (20)     4158 2024-03-29 11:12:45.000000 cnlitellm-0.2.1/cnlitellm/providers/__pycache__/moonshot.cpython-312.pyc
--rw-r--r--   0 everfly    (501) staff       (20)     4452 2024-03-29 11:12:45.000000 cnlitellm-0.2.1/cnlitellm/providers/__pycache__/qwen.cpython-312.pyc
--rw-r--r--   0 everfly    (501) staff       (20)     5144 2024-03-29 11:12:45.000000 cnlitellm-0.2.1/cnlitellm/providers/__pycache__/tiangong.cpython-312.pyc
--rw-r--r--   0 everfly    (501) staff       (20)     5051 2024-03-29 11:12:45.000000 cnlitellm-0.2.1/cnlitellm/providers/__pycache__/wenxin.cpython-312.pyc
--rw-r--r--   0 everfly    (501) staff       (20)     3935 2024-03-29 11:12:45.000000 cnlitellm-0.2.1/cnlitellm/providers/__pycache__/zhipu.cpython-312.pyc
--rw-r--r--   0 everfly    (501) staff       (20)      462 2024-03-29 11:12:45.000000 cnlitellm-0.2.1/cnlitellm/providers/a.json
--rw-r--r--   0 everfly    (501) staff       (20)     4622 2024-04-21 23:53:41.000000 cnlitellm-0.2.1/cnlitellm/providers/baichuan.py
--rw-r--r--   0 everfly    (501) staff       (20)     1613 2024-03-19 10:47:10.000000 cnlitellm-0.2.1/cnlitellm/providers/base_provider.py
--rw-r--r--   0 everfly    (501) staff       (20)     8848 2024-04-24 10:18:26.000000 cnlitellm-0.2.1/cnlitellm/providers/coze.py
--rw-r--r--   0 everfly    (501) staff       (20)     6826 2024-04-21 23:46:44.000000 cnlitellm-0.2.1/cnlitellm/providers/dify.py
--rw-r--r--   0 everfly    (501) staff       (20)     6402 2024-04-21 23:32:41.000000 cnlitellm-0.2.1/cnlitellm/providers/fastgpt.py
--rw-r--r--   0 everfly    (501) staff       (20)     4609 2024-04-22 00:05:51.000000 cnlitellm-0.2.1/cnlitellm/providers/minimax.py
--rw-r--r--   0 everfly    (501) staff       (20)     2642 2024-04-22 08:07:48.000000 cnlitellm-0.2.1/cnlitellm/providers/moonshot.py
--rw-r--r--   0 everfly    (501) staff       (20)     5968 2024-04-22 00:06:48.000000 cnlitellm-0.2.1/cnlitellm/providers/qwen.py
--rw-r--r--   0 everfly    (501) staff       (20)     5318 2024-04-22 07:20:13.000000 cnlitellm-0.2.1/cnlitellm/providers/tiangong.py
--rw-r--r--   0 everfly    (501) staff       (20)     5825 2024-04-22 07:25:41.000000 cnlitellm-0.2.1/cnlitellm/providers/wenxin.py
--rw-r--r--   0 everfly    (501) staff       (20)     9369 2024-04-22 07:59:20.000000 cnlitellm-0.2.1/cnlitellm/providers/xunfei.py
--rw-r--r--   0 everfly    (501) staff       (20)     2367 2024-04-17 10:38:01.000000 cnlitellm-0.2.1/cnlitellm/providers/zhipu.py
--rw-r--r--   0 everfly    (501) staff       (20)    11502 2024-04-22 00:20:28.000000 cnlitellm-0.2.1/cnlitellm/utils.py
-drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-04-24 14:12:37.151018 cnlitellm-0.2.1/cnlitellm.egg-info/
--rw-r--r--   0 everfly    (501) staff       (20)      448 2024-04-24 14:12:37.000000 cnlitellm-0.2.1/cnlitellm.egg-info/PKG-INFO
--rw-r--r--   0 everfly    (501) staff       (20)     1694 2024-04-24 14:12:37.000000 cnlitellm-0.2.1/cnlitellm.egg-info/SOURCES.txt
--rw-r--r--   0 everfly    (501) staff       (20)        1 2024-04-24 14:12:37.000000 cnlitellm-0.2.1/cnlitellm.egg-info/dependency_links.txt
--rw-r--r--   0 everfly    (501) staff       (20)       69 2024-04-24 14:12:37.000000 cnlitellm-0.2.1/cnlitellm.egg-info/requires.txt
--rw-r--r--   0 everfly    (501) staff       (20)       16 2024-04-24 14:12:37.000000 cnlitellm-0.2.1/cnlitellm.egg-info/top_level.txt
-drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-04-24 14:12:37.157453 cnlitellm-0.2.1/examples/
--rw-r--r--   0 everfly    (501) staff       (20)       48 2024-03-19 10:47:10.000000 cnlitellm-0.2.1/examples/example_usage.py
--rw-r--r--   0 everfly    (501) staff       (20)      406 2024-04-07 09:48:46.000000 cnlitellm-0.2.1/pyproject.toml
--rw-r--r--   0 everfly    (501) staff       (20)      140 2024-04-07 09:38:02.000000 cnlitellm-0.2.1/requirements.txt
--rw-r--r--   0 everfly    (501) staff       (20)       38 2024-04-24 14:12:37.161282 cnlitellm-0.2.1/setup.cfg
--rw-r--r--   0 everfly    (501) staff       (20)      528 2024-04-24 14:12:02.000000 cnlitellm-0.2.1/setup.py
-drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-04-24 14:12:37.160594 cnlitellm-0.2.1/tests/
--rw-r--r--   0 everfly    (501) staff       (20)        0 2024-03-19 10:47:10.000000 cnlitellm-0.2.1/tests/__init__.py
--rw-r--r--   0 everfly    (501) staff       (20)       65 2024-03-19 10:47:10.000000 cnlitellm-0.2.1/tests/test_api.py
--rw-r--r--   0 everfly    (501) staff       (20)     2000 2024-03-29 11:12:45.000000 cnlitellm-0.2.1/tests/test_baichuan.py
--rw-r--r--   0 everfly    (501) staff       (20)      980 2024-04-20 11:40:33.000000 cnlitellm-0.2.1/tests/test_coze.py
--rw-r--r--   0 everfly    (501) staff       (20)     1416 2024-04-20 10:17:01.000000 cnlitellm-0.2.1/tests/test_fastgpt.py
--rw-r--r--   0 everfly    (501) staff       (20)     2350 2024-03-29 11:12:45.000000 cnlitellm-0.2.1/tests/test_minimax.py
--rw-r--r--   0 everfly    (501) staff       (20)     2882 2024-03-29 11:13:20.000000 cnlitellm-0.2.1/tests/test_moonshot.py
--rw-r--r--   0 everfly    (501) staff       (20)     1693 2024-04-20 03:21:10.000000 cnlitellm-0.2.1/tests/test_moonshot2.py
--rw-r--r--   0 everfly    (501) staff       (20)     1866 2024-03-29 11:12:45.000000 cnlitellm-0.2.1/tests/test_qwen.py
--rw-r--r--   0 everfly    (501) staff       (20)     1947 2024-03-29 11:12:45.000000 cnlitellm-0.2.1/tests/test_tiangong.py
--rw-r--r--   0 everfly    (501) staff       (20)     1911 2024-03-29 11:12:45.000000 cnlitellm-0.2.1/tests/test_wenxin.py
--rw-r--r--   0 everfly    (501) staff       (20)     1555 2024-04-20 09:23:11.000000 cnlitellm-0.2.1/tests/test_zhipu.py
--rw-r--r--   0 everfly    (501) staff       (20)     1405 2024-04-20 09:25:47.000000 cnlitellm-0.2.1/tests/test_zhipu2.py
+drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-04-26 09:53:30.434846 cnlitellm-0.2.2/
+-rw-r--r--   0 everfly    (501) staff       (20)       44 2024-03-19 10:47:10.000000 cnlitellm-0.2.2/LICENSE
+-rw-r--r--   0 everfly    (501) staff       (20)      448 2024-04-26 09:53:30.434662 cnlitellm-0.2.2/PKG-INFO
+-rw-r--r--   0 everfly    (501) staff       (20)       82 2024-03-19 10:47:10.000000 cnlitellm-0.2.2/README.md
+drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-04-26 09:53:30.428219 cnlitellm-0.2.2/cnlitellm/
+-rw-r--r--   0 everfly    (501) staff       (20)        0 2024-03-19 10:47:10.000000 cnlitellm-0.2.2/cnlitellm/__init__.py
+drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-04-26 09:53:30.429457 cnlitellm-0.2.2/cnlitellm/__pycache__/
+-rw-r--r--   0 everfly    (501) staff       (20)      140 2024-03-21 11:21:03.000000 cnlitellm-0.2.2/cnlitellm/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0 everfly    (501) staff       (20)     1790 2024-03-21 11:21:03.000000 cnlitellm-0.2.2/cnlitellm/__pycache__/models.cpython-312.pyc
+-rw-r--r--   0 everfly    (501) staff       (20)    14486 2024-03-29 11:12:45.000000 cnlitellm-0.2.2/cnlitellm/__pycache__/utils.cpython-312.pyc
+-rw-r--r--   0 everfly    (501) staff       (20)     1967 2024-04-20 11:21:30.000000 cnlitellm-0.2.2/cnlitellm/api.py
+-rw-r--r--   0 everfly    (501) staff       (20)      306 2024-03-19 10:47:10.000000 cnlitellm-0.2.2/cnlitellm/exceptions.py
+-rw-r--r--   0 everfly    (501) staff       (20)     1195 2024-03-19 10:47:10.000000 cnlitellm-0.2.2/cnlitellm/models.py
+drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-04-26 09:53:30.431302 cnlitellm-0.2.2/cnlitellm/providers/
+-rw-r--r--   0 everfly    (501) staff       (20)        0 2024-03-19 10:47:10.000000 cnlitellm-0.2.2/cnlitellm/providers/__init__.py
+drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-04-26 09:53:30.433051 cnlitellm-0.2.2/cnlitellm/providers/__pycache__/
+-rw-r--r--   0 everfly    (501) staff       (20)      150 2024-03-21 11:21:03.000000 cnlitellm-0.2.2/cnlitellm/providers/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0 everfly    (501) staff       (20)     4455 2024-03-29 11:12:45.000000 cnlitellm-0.2.2/cnlitellm/providers/__pycache__/baichuan.cpython-312.pyc
+-rw-r--r--   0 everfly    (501) staff       (20)     2682 2024-03-21 11:21:03.000000 cnlitellm-0.2.2/cnlitellm/providers/__pycache__/base_provider.cpython-312.pyc
+-rw-r--r--   0 everfly    (501) staff       (20)     4252 2024-03-29 11:12:45.000000 cnlitellm-0.2.2/cnlitellm/providers/__pycache__/minimax.cpython-312.pyc
+-rw-r--r--   0 everfly    (501) staff       (20)     4158 2024-03-29 11:12:45.000000 cnlitellm-0.2.2/cnlitellm/providers/__pycache__/moonshot.cpython-312.pyc
+-rw-r--r--   0 everfly    (501) staff       (20)     4452 2024-03-29 11:12:45.000000 cnlitellm-0.2.2/cnlitellm/providers/__pycache__/qwen.cpython-312.pyc
+-rw-r--r--   0 everfly    (501) staff       (20)     5144 2024-03-29 11:12:45.000000 cnlitellm-0.2.2/cnlitellm/providers/__pycache__/tiangong.cpython-312.pyc
+-rw-r--r--   0 everfly    (501) staff       (20)     5051 2024-03-29 11:12:45.000000 cnlitellm-0.2.2/cnlitellm/providers/__pycache__/wenxin.cpython-312.pyc
+-rw-r--r--   0 everfly    (501) staff       (20)     3935 2024-03-29 11:12:45.000000 cnlitellm-0.2.2/cnlitellm/providers/__pycache__/zhipu.cpython-312.pyc
+-rw-r--r--   0 everfly    (501) staff       (20)      462 2024-03-29 11:12:45.000000 cnlitellm-0.2.2/cnlitellm/providers/a.json
+-rw-r--r--   0 everfly    (501) staff       (20)     5261 2024-04-26 05:00:16.000000 cnlitellm-0.2.2/cnlitellm/providers/baichuan.py
+-rw-r--r--   0 everfly    (501) staff       (20)     1537 2024-04-26 04:45:02.000000 cnlitellm-0.2.2/cnlitellm/providers/base_provider.py
+-rw-r--r--   0 everfly    (501) staff       (20)     9735 2024-04-26 09:17:08.000000 cnlitellm-0.2.2/cnlitellm/providers/coze.py
+-rw-r--r--   0 everfly    (501) staff       (20)     7578 2024-04-26 09:45:14.000000 cnlitellm-0.2.2/cnlitellm/providers/dify.py
+-rw-r--r--   0 everfly    (501) staff       (20)     7109 2024-04-26 09:50:55.000000 cnlitellm-0.2.2/cnlitellm/providers/fastgpt.py
+-rw-r--r--   0 everfly    (501) staff       (20)     4905 2024-04-26 06:06:18.000000 cnlitellm-0.2.2/cnlitellm/providers/minimax.py
+-rw-r--r--   0 everfly    (501) staff       (20)     2642 2024-04-26 07:38:29.000000 cnlitellm-0.2.2/cnlitellm/providers/moonshot.py
+-rw-r--r--   0 everfly    (501) staff       (20)     6739 2024-04-26 08:29:20.000000 cnlitellm-0.2.2/cnlitellm/providers/qwen.py
+-rw-r--r--   0 everfly    (501) staff       (20)     5965 2024-04-26 08:42:54.000000 cnlitellm-0.2.2/cnlitellm/providers/tiangong.py
+-rw-r--r--   0 everfly    (501) staff       (20)     6421 2024-04-26 08:49:29.000000 cnlitellm-0.2.2/cnlitellm/providers/wenxin.py
+-rw-r--r--   0 everfly    (501) staff       (20)     9369 2024-04-22 07:59:20.000000 cnlitellm-0.2.2/cnlitellm/providers/xunfei.py
+-rw-r--r--   0 everfly    (501) staff       (20)     2367 2024-04-17 10:38:01.000000 cnlitellm-0.2.2/cnlitellm/providers/zhipu.py
+-rw-r--r--   0 everfly    (501) staff       (20)    14435 2024-04-26 08:53:37.000000 cnlitellm-0.2.2/cnlitellm/utils.py
+drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-04-26 09:53:30.428805 cnlitellm-0.2.2/cnlitellm.egg-info/
+-rw-r--r--   0 everfly    (501) staff       (20)      448 2024-04-26 09:53:30.000000 cnlitellm-0.2.2/cnlitellm.egg-info/PKG-INFO
+-rw-r--r--   0 everfly    (501) staff       (20)     1694 2024-04-26 09:53:30.000000 cnlitellm-0.2.2/cnlitellm.egg-info/SOURCES.txt
+-rw-r--r--   0 everfly    (501) staff       (20)        1 2024-04-26 09:53:30.000000 cnlitellm-0.2.2/cnlitellm.egg-info/dependency_links.txt
+-rw-r--r--   0 everfly    (501) staff       (20)       69 2024-04-26 09:53:30.000000 cnlitellm-0.2.2/cnlitellm.egg-info/requires.txt
+-rw-r--r--   0 everfly    (501) staff       (20)       16 2024-04-26 09:53:30.000000 cnlitellm-0.2.2/cnlitellm.egg-info/top_level.txt
+drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-04-26 09:53:30.433261 cnlitellm-0.2.2/examples/
+-rw-r--r--   0 everfly    (501) staff       (20)       48 2024-03-19 10:47:10.000000 cnlitellm-0.2.2/examples/example_usage.py
+-rw-r--r--   0 everfly    (501) staff       (20)      406 2024-04-07 09:48:46.000000 cnlitellm-0.2.2/pyproject.toml
+-rw-r--r--   0 everfly    (501) staff       (20)      140 2024-04-07 09:38:02.000000 cnlitellm-0.2.2/requirements.txt
+-rw-r--r--   0 everfly    (501) staff       (20)       38 2024-04-26 09:53:30.434880 cnlitellm-0.2.2/setup.cfg
+-rw-r--r--   0 everfly    (501) staff       (20)      528 2024-04-26 09:52:38.000000 cnlitellm-0.2.2/setup.py
+drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-04-26 09:53:30.434441 cnlitellm-0.2.2/tests/
+-rw-r--r--   0 everfly    (501) staff       (20)        0 2024-03-19 10:47:10.000000 cnlitellm-0.2.2/tests/__init__.py
+-rw-r--r--   0 everfly    (501) staff       (20)       65 2024-03-19 10:47:10.000000 cnlitellm-0.2.2/tests/test_api.py
+-rw-r--r--   0 everfly    (501) staff       (20)     2000 2024-03-29 11:12:45.000000 cnlitellm-0.2.2/tests/test_baichuan.py
+-rw-r--r--   0 everfly    (501) staff       (20)      980 2024-04-20 11:40:33.000000 cnlitellm-0.2.2/tests/test_coze.py
+-rw-r--r--   0 everfly    (501) staff       (20)     1416 2024-04-20 10:17:01.000000 cnlitellm-0.2.2/tests/test_fastgpt.py
+-rw-r--r--   0 everfly    (501) staff       (20)     2350 2024-03-29 11:12:45.000000 cnlitellm-0.2.2/tests/test_minimax.py
+-rw-r--r--   0 everfly    (501) staff       (20)     2882 2024-03-29 11:13:20.000000 cnlitellm-0.2.2/tests/test_moonshot.py
+-rw-r--r--   0 everfly    (501) staff       (20)     1693 2024-04-20 03:21:10.000000 cnlitellm-0.2.2/tests/test_moonshot2.py
+-rw-r--r--   0 everfly    (501) staff       (20)     1866 2024-03-29 11:12:45.000000 cnlitellm-0.2.2/tests/test_qwen.py
+-rw-r--r--   0 everfly    (501) staff       (20)     1947 2024-03-29 11:12:45.000000 cnlitellm-0.2.2/tests/test_tiangong.py
+-rw-r--r--   0 everfly    (501) staff       (20)     1911 2024-03-29 11:12:45.000000 cnlitellm-0.2.2/tests/test_wenxin.py
+-rw-r--r--   0 everfly    (501) staff       (20)     1555 2024-04-20 09:23:11.000000 cnlitellm-0.2.2/tests/test_zhipu.py
+-rw-r--r--   0 everfly    (501) staff       (20)     1405 2024-04-20 09:25:47.000000 cnlitellm-0.2.2/tests/test_zhipu2.py
```

### Comparing `cnlitellm-0.2.1/cnlitellm/__pycache__/models.cpython-312.pyc` & `cnlitellm-0.2.2/cnlitellm/__pycache__/models.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.1/cnlitellm/__pycache__/utils.cpython-312.pyc` & `cnlitellm-0.2.2/cnlitellm/__pycache__/utils.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.1/cnlitellm/api.py` & `cnlitellm-0.2.2/cnlitellm/api.py`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.1/cnlitellm/models.py` & `cnlitellm-0.2.2/cnlitellm/models.py`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.1/cnlitellm/providers/__pycache__/baichuan.cpython-312.pyc` & `cnlitellm-0.2.2/cnlitellm/providers/__pycache__/baichuan.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.1/cnlitellm/providers/__pycache__/base_provider.cpython-312.pyc` & `cnlitellm-0.2.2/cnlitellm/providers/__pycache__/base_provider.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.1/cnlitellm/providers/__pycache__/minimax.cpython-312.pyc` & `cnlitellm-0.2.2/cnlitellm/providers/__pycache__/minimax.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.1/cnlitellm/providers/__pycache__/moonshot.cpython-312.pyc` & `cnlitellm-0.2.2/cnlitellm/providers/__pycache__/moonshot.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.1/cnlitellm/providers/__pycache__/qwen.cpython-312.pyc` & `cnlitellm-0.2.2/cnlitellm/providers/__pycache__/qwen.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.1/cnlitellm/providers/__pycache__/tiangong.cpython-312.pyc` & `cnlitellm-0.2.2/cnlitellm/providers/__pycache__/tiangong.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.1/cnlitellm/providers/__pycache__/wenxin.cpython-312.pyc` & `cnlitellm-0.2.2/cnlitellm/providers/__pycache__/wenxin.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.1/cnlitellm/providers/__pycache__/zhipu.cpython-312.pyc` & `cnlitellm-0.2.2/cnlitellm/providers/__pycache__/zhipu.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.1/cnlitellm/providers/baichuan.py` & `cnlitellm-0.2.2/cnlitellm/providers/minimax.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-import json
 from .base_provider import BaseProvider
-from cnlitellm.utils import ModelResponse, Message, Choices, Usage
+from cnlitellm.utils import ModelResponse, Message, Choices, Usage, Delta, StreamingChoices
 import requests
+import json
 import logging
 
-class BaiChuanOpenAIError(Exception):
+class MinimaxOpenAIError(Exception):
     def __init__(
         self,
         status_code,
         message,
     ):
         self.status_code = status_code
         self.message = message
         super().__init__(self.message)
 
-class BaiChuanAIProvider(BaseProvider):
+class MinimaxAIProvider(BaseProvider):
     def __init__(self, **model_kwargs):
         self.api_key = model_kwargs.get("api_key")
-        self.endpoint_url = "https://api.baichuan-ai.com/v1/chat/completions"
+        self.endpoint_url = "https://api.minimax.chat/v1/text/chatcompletion_v2"
 
     def pre_processing(self, **kwargs):
         supported_params = [
             "model", "messages", "max_tokens", "temperature", "top_p", "n",
             "logprobs", "stream", "stop", "presence_penalty", "frequency_penalty",
             "best_of", "logit_bias"
         ]
@@ -36,83 +36,87 @@
             "Authorization": f"Bearer {self.api_key}",
             "Content-Type": "application/json",
         }
         response = requests.post(self.endpoint_url, headers=headers, data=payload)
         for line in response.iter_lines():
             if line:
                 new_line = line.decode("utf-8").replace("data: ", "")
-                if new_line == "[DONE]":
-                    break
                 data = json.loads(new_line)
-                chunk_message = data["choices"][0]["delta"]
-                chunk_line = {
-                    "choices": [
-                        {
-                            "delta": {
-                                "role": chunk_message["role"],
-                                "content": chunk_message["content"],
-                            }
-                        }
-                    ]
-                }
-                if "usage" in data:
-                    usage_info = data["usage"]
-                    chunk_line["usage"] = {
-                        "total_tokens": usage_info["total_tokens"],
-                        "prompt_tokens": usage_info["prompt_tokens"],
-                        "completion_tokens": usage_info["completion_tokens"],
-                    }
-                yield json.dumps(chunk_line) + "\n\n"
+                choices = data.get("choices", [])
+                chunk_choices = []
+                if choices:
+                    for choice in choices:
+                        chunk_delta = Delta()
+                        delta = choice.get("delta")
+                        if delta:
+                            if "role" in choice['delta']:
+                                chunk_delta.role = choice['delta']["role"]
+                            if "content" in choice['delta']:
+                                chunk_delta.content = choice['delta']["content"]
+                            chunk_choices.append(StreamingChoices(index=choice['index'], delta=chunk_delta))
+                    if "usage" in data:
+                        chunk_usage = Usage()
+                        if "total_tokens" in data["usage"]:
+                            chunk_usage.total_tokens = data["usage"]["total_tokens"]
+
+                chunk_response = ModelResponse(
+                    id=data["id"],
+                    choices=chunk_choices,
+                    created=data["created"],
+                    model=model,
+                    usage=chunk_usage if "usage" in data else None,
+                    stream=True
+                )
+                yield chunk_response
 
     def create_model_response_wrapper(self, result, model):
         response_dict = result.json()
         choices = []
         for choice in response_dict["choices"]:
             message = Message(
-                content=choice["message"]["content"], role=choice["message"]["role"]
+                content=choice["message"]["content"],
+                role=choice["message"]["role"]
             )
             choices.append(
                 Choices(
                     message=message,
                     index=choice["index"],
                     finish_reason=choice["finish_reason"],
                 )
             )
         usage = Usage(
-            prompt_tokens=response_dict["usage"]["prompt_tokens"],
-            completion_tokens=response_dict["usage"]["completion_tokens"],
             total_tokens=response_dict["usage"]["total_tokens"],
         )
         response = ModelResponse(
             id=response_dict["id"],
             choices=choices,
             created=response_dict["created"],
             model=model,
             usage=usage,
         )
         return response
 
-
     def completion(self, model: str, messages: list, **kwargs):
         try:
             if model is None or messages is None:
-                raise BaiChuanOpenAIError(
+                raise MinimaxOpenAIError(
                     status_code=422, message=f"Missing model or messages"
                 )
             new_kwargs = self.pre_processing(**kwargs)
             stream = kwargs.get("stream", False)
 
             if stream:
-                return self.post_stream_processing_wrapper(model, messages, **new_kwargs)
+                return self.post_stream_processing_wrapper(model=model, messages=messages, **new_kwargs)
+            
             else:
                 payload = json.dumps({"model": model, "messages": messages, **new_kwargs})
                 headers = {
                     "Authorization": f"Bearer {self.api_key}",
                     "Content-Type": "application/json",
                 }
                 result = requests.post(self.endpoint_url, headers=headers, data=payload)
                 return self.create_model_response_wrapper(result, model=model)
         except Exception as e:
             if hasattr(e, "status_code"):
-                raise BaiChuanOpenAIError(status_code=e.status_code, message=str(e))
+                raise MinimaxOpenAIError(status_code=e.status_code, message=str(e))
             else:
-                raise BaiChuanOpenAIError(status_code=500, message=str(e))
+                raise MinimaxOpenAIError(status_code=500, message=str(e))
```

### Comparing `cnlitellm-0.2.1/cnlitellm/providers/base_provider.py` & `cnlitellm-0.2.2/cnlitellm/providers/base_provider.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,19 +30,15 @@
             choices.append(Choices(message=message, index=choice.index, finish_reason=choice.finish_reason))
 
         usage = Usage(
             prompt_tokens=openai_response.usage.prompt_tokens,
             completion_tokens=openai_response.usage.completion_tokens,
             total_tokens=openai_response.usage.total_tokens
         )
-
-        print("choices: ", choices)
-
         response =  ModelResponse(
             id=openai_response.id,
             choices=choices,
             created=openai_response.created,
             model=model,
             usage=usage
         )
-        print("response: ", response)
         pass
```

### Comparing `cnlitellm-0.2.1/cnlitellm/providers/coze.py` & `cnlitellm-0.2.2/cnlitellm/providers/coze.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from .base_provider import BaseProvider
 from cnlitellm.utils import ResponseModelInterface
-from cnlitellm.utils import ModelResponse, Message, Choices, Usage, Context, generate_unique_uid
+from cnlitellm.utils import ModelResponse, Message, Choices, Usage, Context, generate_unique_uid, Delta, StreamingChoices
 from openai import OpenAI
 import logging, json, time, requests
 
 
 class CozeAIError(Exception):
     def __init__(
         self,
@@ -64,51 +64,67 @@
             if line:
                 if line.startswith(b"data:"):
                     new_line = line.decode("utf-8").replace("data:", "")
                     if new_line == "[DONE]":
                         continue
 
                     data = json.loads(new_line)
+                    print("data is:",data)
                     chunk_line = {}
-                    context = []
+                    chunk_context = []
+                    chunk_choices = []
+                    index = 0
                     if "message" in data:
                         message = data["message"]
                         if message['role'] == 'assistant' and message['type'] == 'knowledge':
                             # 解析知识型内容
                             content = message['content']
                             conversation_id = data.get('conversation_id', 0)
                             # 假设knowledge类型内容是由"---\nrecall slice X:\n"分隔的
                             slices = content.split('---\n')
+                            index = 0
                             for slice in slices:
                                 if slice.strip().startswith('recall slice'):
                                     # 去掉前缀找到JSON部分
                                     json_part = slice.strip().split('\n', 1)[-1].strip()
+                                    # 如果不是以\"}结尾，则强制添加
+                                    if not json_part.endswith('\"}'):
+                                        json_part += '\"}'
                                     try:
                                         # 尝试解析JSON数据
                                         recall_data = json.loads(json_part)
-                                        context.append({
-                                            "id": conversation_id,
+                                        chunk_context.append({
+                                            "id": index,
                                             "content": str(recall_data)    
                                         })
+                                        index += 1
                                     except json.JSONDecodeError:
                                         raise CozeAIError(status_code=500, message=f"Error decoding JSON from slice: {json_part}")
-                            chunk_line["context"] = context
 
                         elif message['role'] == 'assistant' and message['type'] == 'answer':
-                            # 直接添加回复内容
-                            chunk_line["choices"] = [
-                                {
-                                    "delta": {
-                                        "role": message['role'],
-                                        "content": message["content"],
-                                    }
-                                }
-                            ]
-                    if chunk_line:
-                        yield json.dumps(chunk_line) + "\n\n"
+                            chunk_choices = []
+                            chunk_delta = Delta()
+                            if "role" in message:
+                                chunk_delta.role = message["role"]
+                            if "content" in message:
+                                chunk_delta.content = message["content"]
+                            chunk_choices.append(StreamingChoices(index=str(index), delta=chunk_delta))
+                        
+                        chunk_usage = Usage()
+                        chunk_response = ModelResponse(
+                            id=conversation_id,
+                            choices=chunk_choices,
+                            context=chunk_context,
+                            created=int(time.time()),
+                            model=model,
+                            usage=chunk_usage if chunk_usage else None,
+                            stream=True
+                        )
+                        index += 1
+                        yield chunk_response
 
     def create_model_response_wrapper(self, result, model):
         choices = []
         context = []
 
         result_dict = result.json()
         messages = result_dict.get('messages', [])
```

### Comparing `cnlitellm-0.2.1/cnlitellm/providers/dify.py` & `cnlitellm-0.2.2/cnlitellm/providers/dify.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 from .base_provider import BaseProvider
-from cnlitellm.utils import ModelResponse, Message, Choices, Usage, Context
+from cnlitellm.utils import ModelResponse, Message, Choices, Usage, Context, Delta, StreamingChoices
 import requests
 import logging, json, time
 
 class DifyOpenAIError(Exception):
     def __init__(
         self,
         status_code,
@@ -49,62 +49,73 @@
         payload = json.dumps({"query": query, "response_mode": mode, "user": "abc-123","conversation_id": "","inputs":{}})
 
         headers = {
             "Authorization": f"Bearer {self.api_key}",
             "Content-Type": "application/json",
         }
         response = requests.post(self.endpoint_url, headers=headers, data=payload)
-
+        chunk_choices = []
+        chunk_context = []
+        index = 0
         for line in response.iter_lines():
             if line:
                 # judge if the new_line begins with "data:"
                 if line.startswith(b"data:"):
                     new_line = line.decode("utf-8").replace("data: ", "")
                     if new_line == "[DONE]":
                         continue
 
                     data = json.loads(new_line)
-                    chunk_line = {}
+                    print("data is:",data)
                     if "answer" in data:
                         chunk_message = data["answer"]
+                        chunk_delta = Delta()
                         if chunk_message:
-                            chunk_line["choices"] = [
-                                {
-                                    "delta": {
-                                        "role": "assistant",
-                                        "content": chunk_message,
-                                    }
-                                }
-                            ]
+                            if "role" in chunk_message:
+                                chunk_delta.role = "assistant"
+                            if "content" in chunk_message:
+                                chunk_delta.content = chunk_message
+                            chunk_choices.append(StreamingChoices(index=str(index), delta=chunk_delta))
 
                     if "metadata" in data:
-                        context = []
                         metadata = data["metadata"]
                         if "usage" in metadata:
                             usage_info = metadata["usage"]
-                            chunk_line["usage"] = {
-                                "total_tokens": usage_info["total_tokens"],
-                                "prompt_tokens": usage_info["prompt_tokens"],
-                                "completion_tokens": usage_info["completion_tokens"],
-                            }
+                            chunk_usage = Usage()
+                            if "prompt_tokens" in usage_info:
+                                chunk_usage.prompt_tokens = usage_info["prompt_tokens"]
+                            if "completion_tokens" in usage_info:
+                                chunk_usage.completion_tokens = usage_info["completion_tokens"]
+                            if "total_tokens" in usage_info:
+                                chunk_usage.total_tokens = usage_info["total_tokens"]
 
                         if 'retriever_resources' in metadata:
-                            context = []
                             for resource in metadata['retriever_resources']:
-                                context.append({
+                                chunk_context.append({
                                     "id": resource["position"],
                                     "content": resource["content"],
                                     "score": resource["score"],    
                                 })
-                            chunk_line["context"] = context
 
-                    if chunk_line:
-                        yield json.dumps(chunk_line) + "\n\n"
+                    chunk_response = ModelResponse(
+                        id="hello",
+                        choices=chunk_choices,
+                        context=chunk_context,
+                        created=int(time.time()),
+                        model=model,
+                        usage=chunk_usage if chunk_usage else None,
+                        stream=True
+                    )
+                    index += 1
+                    yield chunk_response
 
     def create_model_response_wrapper(self, result, model):
+
+        print("result of dify:", result.json())
+
         response_dict = result.json()
         choices = []
         context = []
 
         message = Message(
             content=response_dict['answer'], role="assistant"
         )
@@ -118,24 +129,27 @@
 
         usage = Usage(
             prompt_tokens=response_dict['metadata']["usage"]["prompt_tokens"],
             completion_tokens=response_dict['metadata']["usage"]["completion_tokens"],
             total_tokens=response_dict['metadata']["usage"]["total_tokens"],
         )
 
-        retrieved_resources = response_dict['metadata']["retriever_resources"]
-        if retrieved_resources is not None:
-            for resource in retrieved_resources:
-                context.append(
-                    Context(
-                        id=resource["position"],
-                        content=resource["content"],
-                        score=resource["score"],
+        if 'retriever_resources' in response_dict['metadata']:
+            retrieved_resources = response_dict['metadata']["retriever_resources"]
+            if retrieved_resources is not None:
+                for resource in retrieved_resources:
+                    context.append(
+                        Context(
+                            id=resource["position"],
+                            content=resource["content"],
+                            score=resource["score"],
+                        )
                     )
-                )
+        else:
+            context = []
 
         response = ModelResponse(
             id=response_dict["id"],
             choices=choices,
             context=context,
             created=int(time.time()),            
             model=model,
```

### Comparing `cnlitellm-0.2.1/cnlitellm/providers/fastgpt.py` & `cnlitellm-0.2.2/cnlitellm/providers/fastgpt.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from .base_provider import BaseProvider
 from cnlitellm.utils import ResponseModelInterface
-from cnlitellm.utils import ModelResponse, Message, Choices, Usage, Context
+from cnlitellm.utils import ModelResponse, Message, Choices, Usage, Context, Delta, StreamingChoices
 from openai import OpenAI
 import logging, json, time, requests
 
 
 class FastGPTError(Exception):
     def __init__(
         self,
@@ -40,64 +40,75 @@
     def post_stream_processing_wrapper(self, model, messages, **new_kwargs):
         payload = json.dumps({"model": model, "messages": messages, **new_kwargs})
         headers = {
             "Authorization": f"Bearer {self.api_key}",
             "Content-Type": "application/json",
         }
         response = requests.post(self.endpoint_url, headers=headers, data=payload)
-
+        chunk_choices = []
+        chunk_context = []
+        index = 0
         # 解析stream返回信息并生成OpenAI兼容格式
         for line in response.iter_lines():
             if line:
                 if line.startswith(b"data:"):
                     new_line = line.decode("utf-8").replace("data: ", "")
                     if new_line == "[DONE]":
                         continue
                     data = json.loads(new_line)
-                    chunk_line = {}
+                    print("data is:",data)
+
                     if "choices" in data:
                         chunk_message = data["choices"][0]["delta"]
+                        chunk_delta = Delta()
                         if chunk_message:
-                            chunk_line["choices"] = [
-                                {
-                                    "delta": {
-                                        "role": chunk_message["role"],
-                                        "content": chunk_message["content"],
-                                    }
-                                }
-                            ]
+                            if "role" in chunk_message:
+                                chunk_delta.role = chunk_message['role']
+                            if "content" in chunk_message:
+                                chunk_delta.content = chunk_message['content']
+                            chunk_choices.append(StreamingChoices(index=str(index), delta=chunk_delta))
 
                     if "usage" in data:
                         usage_info = data["usage"]
-                        chunk_line["usage"] = {
-                            "total_tokens": usage_info["total_tokens"],
-                            "prompt_tokens": usage_info["prompt_tokens"],
-                            "completion_tokens": usage_info["completion_tokens"],
-                        }
+                        chunk_usage = Usage()
+                        if "prompt_tokens" in usage_info:
+                            chunk_usage.prompt_tokens = usage_info["prompt_tokens"]
+                        if "completion_tokens" in usage_info:
+                            chunk_usage.completion_tokens = usage_info["completion_tokens"]
+                        if "total_tokens" in usage_info:
+                            chunk_usage.total_tokens = usage_info["total_tokens"]
+                    else:
+                        chunk_usage = None
 
                     if isinstance(data, list):
                         for module in data:
                             if "quoteList" in module:
-                                context = []
                                 for quote in module["quoteList"]:
                                     content = f'question:[{quote["q"]}], answer:[{quote["a"]}]'
-                                    context.append(
+                                    chunk_context.append(
                                         {
                                             "id": quote["id"],
                                             "content": content,
                                         }    
                                     )
-
-                                chunk_line["context"] = context
-
-                    if chunk_line:
-                        yield json.dumps(chunk_line) + "\n\n"
+                    chunk_response = ModelResponse(
+                        id=data['id'] if 'id' in data else None,
+                        choices=chunk_choices,
+                        context=chunk_context,
+                        created=int(time.time()),
+                        model=model,
+                        usage=chunk_usage if chunk_usage else None,
+                        stream=True
+                    )
+                    index += 1
+                    yield chunk_response
 
     def create_model_response_wrapper(self, result):
         response_dict = result.json()
+        print(response_dict)
         choices = []
         context = []
         message = Message(
             content=response_dict['choices'][0]['message']['content'],
             role="assistant"
         )
         choices.append(
```

### Comparing `cnlitellm-0.2.1/cnlitellm/providers/minimax.py` & `cnlitellm-0.2.2/cnlitellm/providers/baichuan.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,27 @@
+import json
 from .base_provider import BaseProvider
-from cnlitellm.utils import ModelResponse, Message, Choices, Usage
+from cnlitellm.utils import ModelResponse, Message, Choices, Usage, Delta, StreamingChoices
 import requests
-import json
 import logging
 
-class MinimaxOpenAIError(Exception):
+class BaiChuanOpenAIError(Exception):
     def __init__(
         self,
         status_code,
         message,
     ):
         self.status_code = status_code
         self.message = message
         super().__init__(self.message)
 
-class MinimaxAIProvider(BaseProvider):
+class BaiChuanAIProvider(BaseProvider):
     def __init__(self, **model_kwargs):
         self.api_key = model_kwargs.get("api_key")
-        self.endpoint_url = "https://api.minimax.chat/v1/text/chatcompletion_v2"
+        self.endpoint_url = "https://api.baichuan-ai.com/v1/chat/completions"
 
     def pre_processing(self, **kwargs):
         supported_params = [
             "model", "messages", "max_tokens", "temperature", "top_p", "n",
             "logprobs", "stream", "stop", "presence_penalty", "frequency_penalty",
             "best_of", "logit_bias"
         ]
@@ -36,84 +36,93 @@
             "Authorization": f"Bearer {self.api_key}",
             "Content-Type": "application/json",
         }
         response = requests.post(self.endpoint_url, headers=headers, data=payload)
         for line in response.iter_lines():
             if line:
                 new_line = line.decode("utf-8").replace("data: ", "")
+                if new_line == "[DONE]":
+                    break
                 data = json.loads(new_line)
-                choices = data.get("choices", [])
-                if choices:
-                    choice = choices[0]
+                chunk_choices = []
+                for choice in data["choices"]:
+                    chunk_delta = Delta()
                     delta = choice.get("delta")
                     if delta:
-                        chunk_message = delta
-                        chunk_line = {
-                            "choices": [
-                                {
-                                    "delta": {
-                                        "role": chunk_message["role"],
-                                        "content": chunk_message["content"],
-                                    }
-                                }
-                            ]
-                        }
-                    else:
-                        chunk_line = {}
-                    if "usage" in data:
-                        chunk_line["usage"] = {
-                            "total_tokens": data["usage"]["total_tokens"],
-                        }
-                    yield json.dumps(chunk_line) + "\n\n"
+                        if "role" in choice['delta']:
+                            chunk_delta.role = choice['delta']["role"]
+                        if "content" in choice['delta']:
+                            chunk_delta.content = choice['delta']["content"]
+                        chunk_choices.append(StreamingChoices(index=choice['index'], delta=chunk_delta))
+
+                if "usage" in data:
+                    chunk_usage = Usage()
+                    if "prompt_tokens" in data["usage"]:
+                        chunk_usage.prompt_tokens = data["usage"]["prompt_tokens"]
+                    if "completion_tokens" in data["usage"]:
+                        chunk_usage.completion_tokens = data["usage"]["completion_tokens"]
+                    if "total_tokens" in data["usage"]:
+                        chunk_usage.total_tokens = data["usage"]["total_tokens"]
+                
+                chunk_response = ModelResponse(
+                    id=data["id"],
+                    choices=chunk_choices,
+                    created=data["created"],
+                    model=model,
+                    usage=chunk_usage if "usage" in data else None,
+                    stream=True
+                )
+                yield chunk_response
 
     def create_model_response_wrapper(self, result, model):
         response_dict = result.json()
         choices = []
         for choice in response_dict["choices"]:
             message = Message(
-                content=choice["message"]["content"],
-                role=choice["message"]["role"]
+                content=choice["message"]["content"], role=choice["message"]["role"]
             )
             choices.append(
                 Choices(
                     message=message,
                     index=choice["index"],
                     finish_reason=choice["finish_reason"],
                 )
             )
         usage = Usage(
+            prompt_tokens=response_dict["usage"]["prompt_tokens"],
+            completion_tokens=response_dict["usage"]["completion_tokens"],
             total_tokens=response_dict["usage"]["total_tokens"],
         )
         response = ModelResponse(
             id=response_dict["id"],
             choices=choices,
             created=response_dict["created"],
             model=model,
             usage=usage,
         )
         return response
 
+
     def completion(self, model: str, messages: list, **kwargs):
         try:
             if model is None or messages is None:
-                raise MinimaxOpenAIError(
+                raise BaiChuanOpenAIError(
                     status_code=422, message=f"Missing model or messages"
                 )
             new_kwargs = self.pre_processing(**kwargs)
             stream = kwargs.get("stream", False)
 
             if stream:
-                return self.post_stream_processing_wrapper(model=model, messages=messages, **new_kwargs)
-            
+                return self.post_stream_processing_wrapper(model, messages, **new_kwargs)
             else:
                 payload = json.dumps({"model": model, "messages": messages, **new_kwargs})
                 headers = {
                     "Authorization": f"Bearer {self.api_key}",
                     "Content-Type": "application/json",
                 }
                 result = requests.post(self.endpoint_url, headers=headers, data=payload)
                 return self.create_model_response_wrapper(result, model=model)
         except Exception as e:
             if hasattr(e, "status_code"):
-                raise MinimaxOpenAIError(status_code=e.status_code, message=str(e))
+                raise BaiChuanOpenAIError(status_code=e.status_code, message=str(e))
             else:
-                raise MinimaxOpenAIError(status_code=500, message=str(e))
+                raise BaiChuanOpenAIError(status_code=500, message=str(e))
```

### Comparing `cnlitellm-0.2.1/cnlitellm/providers/moonshot.py` & `cnlitellm-0.2.2/cnlitellm/providers/moonshot.py`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.1/cnlitellm/providers/qwen.py` & `cnlitellm-0.2.2/cnlitellm/providers/qwen.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json, time
 import dashscope
 from .base_provider import BaseProvider
 from http import HTTPStatus
 from dashscope import Generation
-from cnlitellm.utils import ModelResponse, Message, Choices, Usage
+from cnlitellm.utils import ModelResponse, Message, Choices, Usage, Delta, StreamingChoices
 
 class QwenOpenAIError(Exception):
     def __init__(
         self,
         status_code,
         message,
     ):
@@ -37,33 +37,47 @@
             messages=messages,
             result_format="message",
             incremental_output=True,
             **new_kwargs,
         )
         for response in responses:
             if response.status_code == HTTPStatus.OK:
-                chunk_message = response.output.choices[0].message
-                line = {
-                    "choices": [
-                        {
-                            "delta": {
-                                "role": chunk_message.role,
-                                "content": chunk_message.content,
-                            }
-                        }
-                    ]
-                }
+                # chunk_message = response.output.choices[0].message
+                chunk_choices = []
+                index = 0
+                for choice in response.output.choices:
+                    chunk_message = choice.message
+                    chunk_delta = Delta()
+                    if chunk_message:
+                        if "role" in chunk_message:
+                            chunk_delta.role = chunk_message["role"]
+                        if "content" in chunk_message:
+                            chunk_delta.content = chunk_message["content"]
+                        chunk_choices.append(StreamingChoices(index=str(index), delta=chunk_delta))
+
                 if hasattr(response, "usage") and response.usage is not None:
-                    chunk_usage = response.usage
-                    line["usage"] = {
-                        "prompt_tokens": chunk_usage["input_tokens"],
-                        "completion_tokens": chunk_usage["output_tokens"],
-                        "total_tokens": chunk_usage["total_tokens"],
-                    }
-                yield json.dumps(line) + "\n\n"
+                    chunk_usage = Usage()
+                    if "input_tokens" in response.usage:
+                        chunk_usage.prompt_tokens = response.usage["input_tokens"]
+                    if "output_tokens" in response.usage:
+                        chunk_usage.completion_tokens = response.usage["output_tokens"]
+                    if "total_tokens" in response.usage:
+                        chunk_usage.total_tokens = response.usage["total_tokens"]
+
+                chunk_response = ModelResponse(
+                    id=response.request_id,
+                    choices=chunk_choices,
+                    created=int(time.time()),
+                    model=model,
+                    usage=chunk_usage if chunk_usage else None,
+                    stream=True
+                )
+                index += 1
+                yield chunk_response
+
             else:
                 raise QwenOpenAIError(
                     status_code=response.status_code,
                     message=f"Request id: {response.request_id}, Status code: {response.status_code}, error code: {response.code}, error message: {response.message}",
                 )
 
     def create_model_response_wrapper(self, response, model):
```

### Comparing `cnlitellm-0.2.1/cnlitellm/providers/tiangong.py` & `cnlitellm-0.2.2/cnlitellm/providers/tiangong.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import time
 import requests
 import json
 import hashlib
 from .base_provider import BaseProvider
-from cnlitellm.utils import ModelResponse, Message, Choices, Usage
+from cnlitellm.utils import ModelResponse, Message, Choices, Usage, Delta, StreamingChoices
 
 class TianGongOpenAIError(Exception):
     def __init__(
         self,
         status_code,
         message,
     ):
@@ -48,35 +48,46 @@
             "app_key": self.app_key,
             "timestamp": timestamp,
             "sign": sign_result,
             "Content-Type": "application/json",
             "stream": "true",
         }
         result = requests.post(self.endpoint_url, headers=headers, json=payload, stream=True)
+        index = 0
         for line in result.iter_lines():
             if line:
                 new_line = json.loads(line.decode('utf-8'))
-                chunk_line = {
-                    "choices": [
-                        {
-                            "delta": {
-                                "role": "assistant",
-                                "content": new_line["resp_data"]["reply"],
-                            }
-                        }
-                    ]
-                }
-                if "usage" in new_line["resp_data"]:
-                    chunk_usage = new_line["resp_data"]["usage"]
-                    chunk_line["usage"] = {
-                        "prompt_tokens": chunk_usage["prompt_tokens"],
-                        "completion_tokens": chunk_usage["completion_tokens"],
-                        "total_tokens": chunk_usage["total_tokens"],
-                    }
-                yield json.dumps(chunk_line) + "\n\n"
+                chunk_choices = []
+                chunk_delta = Delta()
+                if 'reply' in new_line["resp_data"]:
+                    chunk_delta.role = "assistant"
+                    chunk_delta.content=new_line["resp_data"]["reply"]
+                    chunk_choices.append(StreamingChoices(index=index, delta=chunk_delta))
+
+                if 'usage' in new_line["resp_data"]:
+                    chunk_usage = Usage()
+                    if "input_tokens" in new_line["resp_data"]["usage"]:
+                        chunk_usage.prompt_tokens = new_line["resp_data"]["usage"]["prompt_tokens"],
+                    if "output_tokens" in new_line["resp_data"]["usage"]:
+                        chunk_usage.completion_tokens = new_line["resp_data"]["usage"]["output_tokens"]
+                    if "total_tokens" in new_line["resp_data"]["usage"]:
+                        chunk_usage.total_tokens = new_line["resp_data"]["usage"]["total_tokens"]
+                else:
+                    chunk_usage = None
+
+                chunk_response = ModelResponse(
+                    id=new_line['trace_id'],
+                    choices=chunk_choices,
+                    created=int(time.time()),
+                    model=model,
+                    usage=chunk_usage if chunk_usage else None,
+                    stream=True
+                )
+                index += 1
+                yield chunk_response
 
     def create_model_response_wrapper(self, result, model):
         response_dict = result.json()
         choices = []
         message = Message(content=response_dict["resp_data"]["reply"], role="assistant")
         choices.append(
             Choices(
@@ -95,14 +106,15 @@
             choices=choices,
             created=int(time.time()),
             model=model,
             usage=usage,
         )
         return response
 
+
     def completion(self, model: str, messages: list, **kwargs):
         try:
             if model is None or messages is None:
                 raise TianGongOpenAIError(
                     status_code=422, message=f"Missing model or messages"
                 )
             new_kwargs = self.pre_processing(**kwargs)
```

### Comparing `cnlitellm-0.2.1/cnlitellm/providers/wenxin.py` & `cnlitellm-0.2.2/cnlitellm/providers/wenxin.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import time
 import requests
 import json
 import logging
 import hashlib
 from .base_provider import BaseProvider
-from cnlitellm.utils import ModelResponse, Message, Choices, Usage
+from cnlitellm.utils import ModelResponse, Message, Choices, Usage, Delta, StreamingChoices
 
 class WenXinOpenAIError(Exception):
     def __init__(
         self,
         status_code,
         message,
     ):
@@ -48,38 +48,51 @@
         else:
             system = None
         return messages, system
 
     def post_stream_processing_wrapper(self, model, messages, **new_kwargs):
         payload = json.dumps({"model": model, "messages": messages, **new_kwargs})
         headers = {"Content-Type": "application/json"}
+        index = 0
         for line in requests.post(self.endpoint_url, headers=headers, data=payload, stream=True).iter_lines():
             if line:
                 try:
                     # Remove the "data: " prefix before decoding the JSON
                     line_without_prefix = line.decode('utf-8').removeprefix('data: ')
                     new_line = json.loads(line_without_prefix)
-                    chunk_line = {
-                        "choices": [
-                            {
-                                "delta": {
-                                    "role": "assistant",
-                                    "content": new_line.get("result", ""),
-                                }
-                            }
-                        ]
-                    }
-                    if "usage" in new_line:
-                        chunk_usage = new_line["usage"]
-                        chunk_line["usage"] = {
-                            "prompt_tokens": chunk_usage.get("prompt_tokens", 0),
-                            "completion_tokens": chunk_usage.get("completion_tokens", 0),
-                            "total_tokens": chunk_usage.get("total_tokens", 0),
-                        }
-                    yield json.dumps(chunk_line) + "\n\n"
+                    print(new_line)
+
+                    chunk_choices = []
+                    chunk_delta = Delta()
+                    if new_line.get("result"):
+                        chunk_delta.role = "assistant"
+                        chunk_delta.content=new_line.get("result", "")
+                        chunk_choices.append(StreamingChoices(index=index, delta=chunk_delta))
+                    if 'usage' in new_line:
+                        chunk_usage = Usage()
+                        if "input_tokens" in chunk_usage:
+                            chunk_usage.prompt_tokens = chunk_usage.get("prompt_tokens", 0),
+                        if "output_tokens" in chunk_usage:
+                            chunk_usage.completion_tokens = chunk_usage.get("completion_tokens", 0),
+                        if "total_tokens" in chunk_usage:
+                            chunk_usage.total_tokens = chunk_usage.get("total_tokens", 0)
+                    else:
+                        chunk_usage = None
+
+                    chunk_response = ModelResponse(
+                        id="hello",
+                        choices=chunk_choices,
+                        created=int(time.time()),
+                        model=model,
+                        usage=chunk_usage if chunk_usage else None,
+                        stream=True
+                    )
+                    index += 1
+                    yield chunk_response
+
                 except json.JSONDecodeError:
                     # Log the error or handle it as needed
                     continue
 
 
     def create_model_response_wrapper(self, result, model):
         response_dict = json.loads(result)
```

### Comparing `cnlitellm-0.2.1/cnlitellm/providers/xunfei.py` & `cnlitellm-0.2.2/cnlitellm/providers/xunfei.py`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.1/cnlitellm/providers/zhipu.py` & `cnlitellm-0.2.2/cnlitellm/providers/zhipu.py`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.1/cnlitellm/utils.py` & `cnlitellm-0.2.2/cnlitellm/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 from abc import ABC, abstractmethod
 from openai import OpenAIError as OriginalError
 from typing import List, Union, Optional
 
-import uuid, time, openai, random
+import uuid, time, openai, random, requests
 from openai._models import BaseModel as OpenAIObject
 
 # from .exceptions import (
 #     AuthenticationError,
 #     BadRequestError,
 #     RateLimitError,
 #     ServiceUnavailableError,
@@ -279,38 +279,97 @@
         return getattr(self, key)
 
     def __setitem__(self, key, value):
         # Allow dictionary-style assignment of attributes
         setattr(self, key, value)
 
 class ResponseModelInterface:
-    def post_stream_processing(self, response):
+    def post_stream_processing(self, response, model=None):
         for chunk in response:
-            chunk_message = chunk.choices[0].delta
-            line = {
-                "choices": [
-                    {
-                        "delta": {
-                            "role": chunk_message.role,
-                            "content": chunk_message.content,
-                        }
-                    }
-                ]
-            }
-            if (
-                hasattr(chunk.choices[0], "usage")
-                and chunk.choices[0].usage is not None
-            ):
-                chunk_usage = chunk.choices[0].usage
-                line["usage"] = {
-                    "prompt_tokens": chunk_usage["prompt_tokens"],
-                    "completion_tokens": chunk_usage["completion_tokens"],
-                    "total_tokens": chunk_usage["total_tokens"],
-                }
-            yield json.dumps(line) + "\n\n"
+            print("chunk: ", chunk)
+            data = chunk.json()
+            if isinstance(data, str):
+                data = json.loads(data)
+            if 'choices' in data:
+                choices = data['choices']
+                chunk_choices = []
+                for choice in choices:
+                    delta = choice.get("delta")
+                    if delta:
+                        chunk_delta = Delta()
+                        if "role" in choice['delta']:
+                            chunk_delta.role = choice['delta']["role"]
+                        if "content" in choice['delta']:
+                            chunk_delta.content = choice['delta']["content"]
+                        chunk_choices.append(StreamingChoices(index=choice['index'], delta=chunk_delta))
+
+            if "usage" in data:
+                chunk_usage = Usage()
+                if data["usage"]:
+                    if "prompt_tokens" in data["usage"]:
+                        chunk_usage.prompt_tokens = data["usage"]["prompt_tokens"]
+                    if "completion_tokens" in data["usage"]:
+                        chunk_usage.completion_tokens = data["usage"]["completion_tokens"]
+                    if "total_tokens" in data["usage"]:
+                        chunk_usage.total_tokens = data["usage"]["total_tokens"]
+            
+            chunk_response = ModelResponse(
+                id=data["id"],
+                choices=chunk_choices,
+                created=data["created"],
+                model=model,
+                usage=chunk_usage if "usage" in data else None,
+                stream=True
+            )
+            yield chunk_response
+
+    def post_stream_processing_wrapper(self, model, messages, **new_kwargs):
+        payload = json.dumps({"model": model, "messages": messages, **new_kwargs})
+        headers = {
+            "Authorization": f"Bearer {self.api_key}",
+            "Content-Type": "application/json",
+        }
+        response = requests.post(self.endpoint_url, headers=headers, data=payload)
+        for line in response.iter_lines():
+            print("line: ", line)
+            if line:
+                new_line = line.decode("utf-8").replace("data: ", "")
+                if new_line == "[DONE]":
+                    break
+                data = json.loads(new_line)
+                chunk_choices = []
+                for choice in data["choices"]:
+                    chunk_delta = Delta()
+                    delta = choice.get("delta")
+                    if delta:
+                        if "role" in choice['delta']:
+                            chunk_delta.role = choice['delta']["role"]
+                        if "content" in choice['delta']:
+                            chunk_delta.content = choice['delta']["content"]
+                        chunk_choices.append(StreamingChoices(index=choice['index'], delta=chunk_delta))
+
+                if "usage" in data:
+                    chunk_usage = Usage()
+                    if "prompt_tokens" in data["usage"]:
+                        chunk_usage.prompt_tokens = data["usage"]["prompt_tokens"]
+                    if "completion_tokens" in data["usage"]:
+                        chunk_usage.completion_tokens = data["usage"]["completion_tokens"]
+                    if "total_tokens" in data["usage"]:
+                        chunk_usage.total_tokens = data["usage"]["total_tokens"]
+                
+                chunk_response = ModelResponse(
+                    id=data["id"],
+                    choices=chunk_choices,
+                    created=data["created"],
+                    model=model,
+                    usage=chunk_usage if "usage" in data else None,
+                    stream=True
+                )
+                yield chunk_response
+
 
     def create_model_response(
         self, openai_response: openai.ChatCompletion, model: str
     ) -> ModelResponse:
         # print("openai_response: ", openai_response)
         choices = []
```

### Comparing `cnlitellm-0.2.1/cnlitellm.egg-info/SOURCES.txt` & `cnlitellm-0.2.2/cnlitellm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.1/setup.py` & `cnlitellm-0.2.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cnlitellm',
-    version='0.2.1',
+    version='0.2.2',
     packages=find_packages(),
     license='MIT',
     description='A Python library for unified access to Chinese domestic large language models.',
     author='everfly',
     author_email='tagriver@gmail.com',
     url='https://github.com/EvalsOne/CNLiteLLM',
     install_requires=[
```

### Comparing `cnlitellm-0.2.1/tests/test_baichuan.py` & `cnlitellm-0.2.2/tests/test_baichuan.py`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.1/tests/test_coze.py` & `cnlitellm-0.2.2/tests/test_coze.py`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.1/tests/test_fastgpt.py` & `cnlitellm-0.2.2/tests/test_fastgpt.py`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.1/tests/test_minimax.py` & `cnlitellm-0.2.2/tests/test_minimax.py`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.1/tests/test_moonshot.py` & `cnlitellm-0.2.2/tests/test_moonshot.py`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.1/tests/test_moonshot2.py` & `cnlitellm-0.2.2/tests/test_moonshot2.py`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.1/tests/test_qwen.py` & `cnlitellm-0.2.2/tests/test_qwen.py`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.1/tests/test_tiangong.py` & `cnlitellm-0.2.2/tests/test_tiangong.py`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.1/tests/test_wenxin.py` & `cnlitellm-0.2.2/tests/test_wenxin.py`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.1/tests/test_zhipu.py` & `cnlitellm-0.2.2/tests/test_zhipu.py`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.1/tests/test_zhipu2.py` & `cnlitellm-0.2.2/tests/test_zhipu2.py`

 * *Files identical despite different names*

