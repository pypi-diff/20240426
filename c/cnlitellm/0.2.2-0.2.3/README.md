# Comparing `tmp/cnlitellm-0.2.2.tar.gz` & `tmp/cnlitellm-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnlitellm-0.2.2.tar", last modified: Fri Apr 26 09:53:30 2024, max compression
+gzip compressed data, was "cnlitellm-0.2.3.tar", last modified: Fri Apr 26 10:35:35 2024, max compression
```

## Comparing `cnlitellm-0.2.2.tar` & `cnlitellm-0.2.3.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-04-26 09:53:30.434846 cnlitellm-0.2.2/
--rw-r--r--   0 everfly    (501) staff       (20)       44 2024-03-19 10:47:10.000000 cnlitellm-0.2.2/LICENSE
--rw-r--r--   0 everfly    (501) staff       (20)      448 2024-04-26 09:53:30.434662 cnlitellm-0.2.2/PKG-INFO
--rw-r--r--   0 everfly    (501) staff       (20)       82 2024-03-19 10:47:10.000000 cnlitellm-0.2.2/README.md
-drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-04-26 09:53:30.428219 cnlitellm-0.2.2/cnlitellm/
--rw-r--r--   0 everfly    (501) staff       (20)        0 2024-03-19 10:47:10.000000 cnlitellm-0.2.2/cnlitellm/__init__.py
-drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-04-26 09:53:30.429457 cnlitellm-0.2.2/cnlitellm/__pycache__/
--rw-r--r--   0 everfly    (501) staff       (20)      140 2024-03-21 11:21:03.000000 cnlitellm-0.2.2/cnlitellm/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0 everfly    (501) staff       (20)     1790 2024-03-21 11:21:03.000000 cnlitellm-0.2.2/cnlitellm/__pycache__/models.cpython-312.pyc
--rw-r--r--   0 everfly    (501) staff       (20)    14486 2024-03-29 11:12:45.000000 cnlitellm-0.2.2/cnlitellm/__pycache__/utils.cpython-312.pyc
--rw-r--r--   0 everfly    (501) staff       (20)     1967 2024-04-20 11:21:30.000000 cnlitellm-0.2.2/cnlitellm/api.py
--rw-r--r--   0 everfly    (501) staff       (20)      306 2024-03-19 10:47:10.000000 cnlitellm-0.2.2/cnlitellm/exceptions.py
--rw-r--r--   0 everfly    (501) staff       (20)     1195 2024-03-19 10:47:10.000000 cnlitellm-0.2.2/cnlitellm/models.py
-drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-04-26 09:53:30.431302 cnlitellm-0.2.2/cnlitellm/providers/
--rw-r--r--   0 everfly    (501) staff       (20)        0 2024-03-19 10:47:10.000000 cnlitellm-0.2.2/cnlitellm/providers/__init__.py
-drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-04-26 09:53:30.433051 cnlitellm-0.2.2/cnlitellm/providers/__pycache__/
--rw-r--r--   0 everfly    (501) staff       (20)      150 2024-03-21 11:21:03.000000 cnlitellm-0.2.2/cnlitellm/providers/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0 everfly    (501) staff       (20)     4455 2024-03-29 11:12:45.000000 cnlitellm-0.2.2/cnlitellm/providers/__pycache__/baichuan.cpython-312.pyc
--rw-r--r--   0 everfly    (501) staff       (20)     2682 2024-03-21 11:21:03.000000 cnlitellm-0.2.2/cnlitellm/providers/__pycache__/base_provider.cpython-312.pyc
--rw-r--r--   0 everfly    (501) staff       (20)     4252 2024-03-29 11:12:45.000000 cnlitellm-0.2.2/cnlitellm/providers/__pycache__/minimax.cpython-312.pyc
--rw-r--r--   0 everfly    (501) staff       (20)     4158 2024-03-29 11:12:45.000000 cnlitellm-0.2.2/cnlitellm/providers/__pycache__/moonshot.cpython-312.pyc
--rw-r--r--   0 everfly    (501) staff       (20)     4452 2024-03-29 11:12:45.000000 cnlitellm-0.2.2/cnlitellm/providers/__pycache__/qwen.cpython-312.pyc
--rw-r--r--   0 everfly    (501) staff       (20)     5144 2024-03-29 11:12:45.000000 cnlitellm-0.2.2/cnlitellm/providers/__pycache__/tiangong.cpython-312.pyc
--rw-r--r--   0 everfly    (501) staff       (20)     5051 2024-03-29 11:12:45.000000 cnlitellm-0.2.2/cnlitellm/providers/__pycache__/wenxin.cpython-312.pyc
--rw-r--r--   0 everfly    (501) staff       (20)     3935 2024-03-29 11:12:45.000000 cnlitellm-0.2.2/cnlitellm/providers/__pycache__/zhipu.cpython-312.pyc
--rw-r--r--   0 everfly    (501) staff       (20)      462 2024-03-29 11:12:45.000000 cnlitellm-0.2.2/cnlitellm/providers/a.json
--rw-r--r--   0 everfly    (501) staff       (20)     5261 2024-04-26 05:00:16.000000 cnlitellm-0.2.2/cnlitellm/providers/baichuan.py
--rw-r--r--   0 everfly    (501) staff       (20)     1537 2024-04-26 04:45:02.000000 cnlitellm-0.2.2/cnlitellm/providers/base_provider.py
--rw-r--r--   0 everfly    (501) staff       (20)     9735 2024-04-26 09:17:08.000000 cnlitellm-0.2.2/cnlitellm/providers/coze.py
--rw-r--r--   0 everfly    (501) staff       (20)     7578 2024-04-26 09:45:14.000000 cnlitellm-0.2.2/cnlitellm/providers/dify.py
--rw-r--r--   0 everfly    (501) staff       (20)     7109 2024-04-26 09:50:55.000000 cnlitellm-0.2.2/cnlitellm/providers/fastgpt.py
--rw-r--r--   0 everfly    (501) staff       (20)     4905 2024-04-26 06:06:18.000000 cnlitellm-0.2.2/cnlitellm/providers/minimax.py
--rw-r--r--   0 everfly    (501) staff       (20)     2642 2024-04-26 07:38:29.000000 cnlitellm-0.2.2/cnlitellm/providers/moonshot.py
--rw-r--r--   0 everfly    (501) staff       (20)     6739 2024-04-26 08:29:20.000000 cnlitellm-0.2.2/cnlitellm/providers/qwen.py
--rw-r--r--   0 everfly    (501) staff       (20)     5965 2024-04-26 08:42:54.000000 cnlitellm-0.2.2/cnlitellm/providers/tiangong.py
--rw-r--r--   0 everfly    (501) staff       (20)     6421 2024-04-26 08:49:29.000000 cnlitellm-0.2.2/cnlitellm/providers/wenxin.py
--rw-r--r--   0 everfly    (501) staff       (20)     9369 2024-04-22 07:59:20.000000 cnlitellm-0.2.2/cnlitellm/providers/xunfei.py
--rw-r--r--   0 everfly    (501) staff       (20)     2367 2024-04-17 10:38:01.000000 cnlitellm-0.2.2/cnlitellm/providers/zhipu.py
--rw-r--r--   0 everfly    (501) staff       (20)    14435 2024-04-26 08:53:37.000000 cnlitellm-0.2.2/cnlitellm/utils.py
-drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-04-26 09:53:30.428805 cnlitellm-0.2.2/cnlitellm.egg-info/
--rw-r--r--   0 everfly    (501) staff       (20)      448 2024-04-26 09:53:30.000000 cnlitellm-0.2.2/cnlitellm.egg-info/PKG-INFO
--rw-r--r--   0 everfly    (501) staff       (20)     1694 2024-04-26 09:53:30.000000 cnlitellm-0.2.2/cnlitellm.egg-info/SOURCES.txt
--rw-r--r--   0 everfly    (501) staff       (20)        1 2024-04-26 09:53:30.000000 cnlitellm-0.2.2/cnlitellm.egg-info/dependency_links.txt
--rw-r--r--   0 everfly    (501) staff       (20)       69 2024-04-26 09:53:30.000000 cnlitellm-0.2.2/cnlitellm.egg-info/requires.txt
--rw-r--r--   0 everfly    (501) staff       (20)       16 2024-04-26 09:53:30.000000 cnlitellm-0.2.2/cnlitellm.egg-info/top_level.txt
-drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-04-26 09:53:30.433261 cnlitellm-0.2.2/examples/
--rw-r--r--   0 everfly    (501) staff       (20)       48 2024-03-19 10:47:10.000000 cnlitellm-0.2.2/examples/example_usage.py
--rw-r--r--   0 everfly    (501) staff       (20)      406 2024-04-07 09:48:46.000000 cnlitellm-0.2.2/pyproject.toml
--rw-r--r--   0 everfly    (501) staff       (20)      140 2024-04-07 09:38:02.000000 cnlitellm-0.2.2/requirements.txt
--rw-r--r--   0 everfly    (501) staff       (20)       38 2024-04-26 09:53:30.434880 cnlitellm-0.2.2/setup.cfg
--rw-r--r--   0 everfly    (501) staff       (20)      528 2024-04-26 09:52:38.000000 cnlitellm-0.2.2/setup.py
-drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-04-26 09:53:30.434441 cnlitellm-0.2.2/tests/
--rw-r--r--   0 everfly    (501) staff       (20)        0 2024-03-19 10:47:10.000000 cnlitellm-0.2.2/tests/__init__.py
--rw-r--r--   0 everfly    (501) staff       (20)       65 2024-03-19 10:47:10.000000 cnlitellm-0.2.2/tests/test_api.py
--rw-r--r--   0 everfly    (501) staff       (20)     2000 2024-03-29 11:12:45.000000 cnlitellm-0.2.2/tests/test_baichuan.py
--rw-r--r--   0 everfly    (501) staff       (20)      980 2024-04-20 11:40:33.000000 cnlitellm-0.2.2/tests/test_coze.py
--rw-r--r--   0 everfly    (501) staff       (20)     1416 2024-04-20 10:17:01.000000 cnlitellm-0.2.2/tests/test_fastgpt.py
--rw-r--r--   0 everfly    (501) staff       (20)     2350 2024-03-29 11:12:45.000000 cnlitellm-0.2.2/tests/test_minimax.py
--rw-r--r--   0 everfly    (501) staff       (20)     2882 2024-03-29 11:13:20.000000 cnlitellm-0.2.2/tests/test_moonshot.py
--rw-r--r--   0 everfly    (501) staff       (20)     1693 2024-04-20 03:21:10.000000 cnlitellm-0.2.2/tests/test_moonshot2.py
--rw-r--r--   0 everfly    (501) staff       (20)     1866 2024-03-29 11:12:45.000000 cnlitellm-0.2.2/tests/test_qwen.py
--rw-r--r--   0 everfly    (501) staff       (20)     1947 2024-03-29 11:12:45.000000 cnlitellm-0.2.2/tests/test_tiangong.py
--rw-r--r--   0 everfly    (501) staff       (20)     1911 2024-03-29 11:12:45.000000 cnlitellm-0.2.2/tests/test_wenxin.py
--rw-r--r--   0 everfly    (501) staff       (20)     1555 2024-04-20 09:23:11.000000 cnlitellm-0.2.2/tests/test_zhipu.py
--rw-r--r--   0 everfly    (501) staff       (20)     1405 2024-04-20 09:25:47.000000 cnlitellm-0.2.2/tests/test_zhipu2.py
+drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-04-26 10:35:35.323509 cnlitellm-0.2.3/
+-rw-r--r--   0 everfly    (501) staff       (20)       44 2024-03-19 10:47:10.000000 cnlitellm-0.2.3/LICENSE
+-rw-r--r--   0 everfly    (501) staff       (20)      448 2024-04-26 10:35:35.323325 cnlitellm-0.2.3/PKG-INFO
+-rw-r--r--   0 everfly    (501) staff       (20)       82 2024-03-19 10:47:10.000000 cnlitellm-0.2.3/README.md
+drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-04-26 10:35:35.318225 cnlitellm-0.2.3/cnlitellm/
+-rw-r--r--   0 everfly    (501) staff       (20)        0 2024-03-19 10:47:10.000000 cnlitellm-0.2.3/cnlitellm/__init__.py
+drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-04-26 10:35:35.319004 cnlitellm-0.2.3/cnlitellm/__pycache__/
+-rw-r--r--   0 everfly    (501) staff       (20)      140 2024-03-21 11:21:03.000000 cnlitellm-0.2.3/cnlitellm/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0 everfly    (501) staff       (20)     1790 2024-03-21 11:21:03.000000 cnlitellm-0.2.3/cnlitellm/__pycache__/models.cpython-312.pyc
+-rw-r--r--   0 everfly    (501) staff       (20)    14486 2024-03-29 11:12:45.000000 cnlitellm-0.2.3/cnlitellm/__pycache__/utils.cpython-312.pyc
+-rw-r--r--   0 everfly    (501) staff       (20)     1967 2024-04-20 11:21:30.000000 cnlitellm-0.2.3/cnlitellm/api.py
+-rw-r--r--   0 everfly    (501) staff       (20)      306 2024-03-19 10:47:10.000000 cnlitellm-0.2.3/cnlitellm/exceptions.py
+-rw-r--r--   0 everfly    (501) staff       (20)     1195 2024-03-19 10:47:10.000000 cnlitellm-0.2.3/cnlitellm/models.py
+drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-04-26 10:35:35.320530 cnlitellm-0.2.3/cnlitellm/providers/
+-rw-r--r--   0 everfly    (501) staff       (20)        0 2024-03-19 10:47:10.000000 cnlitellm-0.2.3/cnlitellm/providers/__init__.py
+drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-04-26 10:35:35.321594 cnlitellm-0.2.3/cnlitellm/providers/__pycache__/
+-rw-r--r--   0 everfly    (501) staff       (20)      150 2024-03-21 11:21:03.000000 cnlitellm-0.2.3/cnlitellm/providers/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0 everfly    (501) staff       (20)     4455 2024-03-29 11:12:45.000000 cnlitellm-0.2.3/cnlitellm/providers/__pycache__/baichuan.cpython-312.pyc
+-rw-r--r--   0 everfly    (501) staff       (20)     2682 2024-03-21 11:21:03.000000 cnlitellm-0.2.3/cnlitellm/providers/__pycache__/base_provider.cpython-312.pyc
+-rw-r--r--   0 everfly    (501) staff       (20)     4252 2024-03-29 11:12:45.000000 cnlitellm-0.2.3/cnlitellm/providers/__pycache__/minimax.cpython-312.pyc
+-rw-r--r--   0 everfly    (501) staff       (20)     4158 2024-03-29 11:12:45.000000 cnlitellm-0.2.3/cnlitellm/providers/__pycache__/moonshot.cpython-312.pyc
+-rw-r--r--   0 everfly    (501) staff       (20)     4452 2024-03-29 11:12:45.000000 cnlitellm-0.2.3/cnlitellm/providers/__pycache__/qwen.cpython-312.pyc
+-rw-r--r--   0 everfly    (501) staff       (20)     5144 2024-03-29 11:12:45.000000 cnlitellm-0.2.3/cnlitellm/providers/__pycache__/tiangong.cpython-312.pyc
+-rw-r--r--   0 everfly    (501) staff       (20)     5051 2024-03-29 11:12:45.000000 cnlitellm-0.2.3/cnlitellm/providers/__pycache__/wenxin.cpython-312.pyc
+-rw-r--r--   0 everfly    (501) staff       (20)     3935 2024-03-29 11:12:45.000000 cnlitellm-0.2.3/cnlitellm/providers/__pycache__/zhipu.cpython-312.pyc
+-rw-r--r--   0 everfly    (501) staff       (20)      462 2024-03-29 11:12:45.000000 cnlitellm-0.2.3/cnlitellm/providers/a.json
+-rw-r--r--   0 everfly    (501) staff       (20)     5261 2024-04-26 05:00:16.000000 cnlitellm-0.2.3/cnlitellm/providers/baichuan.py
+-rw-r--r--   0 everfly    (501) staff       (20)     1537 2024-04-26 04:45:02.000000 cnlitellm-0.2.3/cnlitellm/providers/base_provider.py
+-rw-r--r--   0 everfly    (501) staff       (20)     9735 2024-04-26 09:17:08.000000 cnlitellm-0.2.3/cnlitellm/providers/coze.py
+-rw-r--r--   0 everfly    (501) staff       (20)     7532 2024-04-26 10:28:05.000000 cnlitellm-0.2.3/cnlitellm/providers/dify.py
+-rw-r--r--   0 everfly    (501) staff       (20)     7109 2024-04-26 09:50:55.000000 cnlitellm-0.2.3/cnlitellm/providers/fastgpt.py
+-rw-r--r--   0 everfly    (501) staff       (20)     4905 2024-04-26 06:06:18.000000 cnlitellm-0.2.3/cnlitellm/providers/minimax.py
+-rw-r--r--   0 everfly    (501) staff       (20)     2642 2024-04-26 07:38:29.000000 cnlitellm-0.2.3/cnlitellm/providers/moonshot.py
+-rw-r--r--   0 everfly    (501) staff       (20)     6739 2024-04-26 08:29:20.000000 cnlitellm-0.2.3/cnlitellm/providers/qwen.py
+-rw-r--r--   0 everfly    (501) staff       (20)     5965 2024-04-26 08:42:54.000000 cnlitellm-0.2.3/cnlitellm/providers/tiangong.py
+-rw-r--r--   0 everfly    (501) staff       (20)     6421 2024-04-26 08:49:29.000000 cnlitellm-0.2.3/cnlitellm/providers/wenxin.py
+-rw-r--r--   0 everfly    (501) staff       (20)     9369 2024-04-22 07:59:20.000000 cnlitellm-0.2.3/cnlitellm/providers/xunfei.py
+-rw-r--r--   0 everfly    (501) staff       (20)     2367 2024-04-17 10:38:01.000000 cnlitellm-0.2.3/cnlitellm/providers/zhipu.py
+-rw-r--r--   0 everfly    (501) staff       (20)    14435 2024-04-26 08:53:37.000000 cnlitellm-0.2.3/cnlitellm/utils.py
+drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-04-26 10:35:35.318709 cnlitellm-0.2.3/cnlitellm.egg-info/
+-rw-r--r--   0 everfly    (501) staff       (20)      448 2024-04-26 10:35:35.000000 cnlitellm-0.2.3/cnlitellm.egg-info/PKG-INFO
+-rw-r--r--   0 everfly    (501) staff       (20)     1694 2024-04-26 10:35:35.000000 cnlitellm-0.2.3/cnlitellm.egg-info/SOURCES.txt
+-rw-r--r--   0 everfly    (501) staff       (20)        1 2024-04-26 10:35:35.000000 cnlitellm-0.2.3/cnlitellm.egg-info/dependency_links.txt
+-rw-r--r--   0 everfly    (501) staff       (20)       69 2024-04-26 10:35:35.000000 cnlitellm-0.2.3/cnlitellm.egg-info/requires.txt
+-rw-r--r--   0 everfly    (501) staff       (20)       16 2024-04-26 10:35:35.000000 cnlitellm-0.2.3/cnlitellm.egg-info/top_level.txt
+drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-04-26 10:35:35.321694 cnlitellm-0.2.3/examples/
+-rw-r--r--   0 everfly    (501) staff       (20)       48 2024-03-19 10:47:10.000000 cnlitellm-0.2.3/examples/example_usage.py
+-rw-r--r--   0 everfly    (501) staff       (20)      406 2024-04-07 09:48:46.000000 cnlitellm-0.2.3/pyproject.toml
+-rw-r--r--   0 everfly    (501) staff       (20)      140 2024-04-07 09:38:02.000000 cnlitellm-0.2.3/requirements.txt
+-rw-r--r--   0 everfly    (501) staff       (20)       38 2024-04-26 10:35:35.323544 cnlitellm-0.2.3/setup.cfg
+-rw-r--r--   0 everfly    (501) staff       (20)      528 2024-04-26 10:32:35.000000 cnlitellm-0.2.3/setup.py
+drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-04-26 10:35:35.323072 cnlitellm-0.2.3/tests/
+-rw-r--r--   0 everfly    (501) staff       (20)        0 2024-03-19 10:47:10.000000 cnlitellm-0.2.3/tests/__init__.py
+-rw-r--r--   0 everfly    (501) staff       (20)       65 2024-03-19 10:47:10.000000 cnlitellm-0.2.3/tests/test_api.py
+-rw-r--r--   0 everfly    (501) staff       (20)     2000 2024-03-29 11:12:45.000000 cnlitellm-0.2.3/tests/test_baichuan.py
+-rw-r--r--   0 everfly    (501) staff       (20)      980 2024-04-20 11:40:33.000000 cnlitellm-0.2.3/tests/test_coze.py
+-rw-r--r--   0 everfly    (501) staff       (20)     1416 2024-04-20 10:17:01.000000 cnlitellm-0.2.3/tests/test_fastgpt.py
+-rw-r--r--   0 everfly    (501) staff       (20)     2350 2024-03-29 11:12:45.000000 cnlitellm-0.2.3/tests/test_minimax.py
+-rw-r--r--   0 everfly    (501) staff       (20)     2882 2024-03-29 11:13:20.000000 cnlitellm-0.2.3/tests/test_moonshot.py
+-rw-r--r--   0 everfly    (501) staff       (20)     1693 2024-04-20 03:21:10.000000 cnlitellm-0.2.3/tests/test_moonshot2.py
+-rw-r--r--   0 everfly    (501) staff       (20)     1866 2024-03-29 11:12:45.000000 cnlitellm-0.2.3/tests/test_qwen.py
+-rw-r--r--   0 everfly    (501) staff       (20)     1947 2024-03-29 11:12:45.000000 cnlitellm-0.2.3/tests/test_tiangong.py
+-rw-r--r--   0 everfly    (501) staff       (20)     1911 2024-03-29 11:12:45.000000 cnlitellm-0.2.3/tests/test_wenxin.py
+-rw-r--r--   0 everfly    (501) staff       (20)     1555 2024-04-20 09:23:11.000000 cnlitellm-0.2.3/tests/test_zhipu.py
+-rw-r--r--   0 everfly    (501) staff       (20)     1405 2024-04-20 09:25:47.000000 cnlitellm-0.2.3/tests/test_zhipu2.py
```

### Comparing `cnlitellm-0.2.2/cnlitellm/__pycache__/models.cpython-312.pyc` & `cnlitellm-0.2.3/cnlitellm/__pycache__/models.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.2/cnlitellm/__pycache__/utils.cpython-312.pyc` & `cnlitellm-0.2.3/cnlitellm/__pycache__/utils.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.2/cnlitellm/api.py` & `cnlitellm-0.2.3/cnlitellm/api.py`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.2/cnlitellm/models.py` & `cnlitellm-0.2.3/cnlitellm/models.py`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.2/cnlitellm/providers/__pycache__/baichuan.cpython-312.pyc` & `cnlitellm-0.2.3/cnlitellm/providers/__pycache__/baichuan.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.2/cnlitellm/providers/__pycache__/base_provider.cpython-312.pyc` & `cnlitellm-0.2.3/cnlitellm/providers/__pycache__/base_provider.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.2/cnlitellm/providers/__pycache__/minimax.cpython-312.pyc` & `cnlitellm-0.2.3/cnlitellm/providers/__pycache__/minimax.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.2/cnlitellm/providers/__pycache__/moonshot.cpython-312.pyc` & `cnlitellm-0.2.3/cnlitellm/providers/__pycache__/moonshot.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.2/cnlitellm/providers/__pycache__/qwen.cpython-312.pyc` & `cnlitellm-0.2.3/cnlitellm/providers/__pycache__/qwen.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.2/cnlitellm/providers/__pycache__/tiangong.cpython-312.pyc` & `cnlitellm-0.2.3/cnlitellm/providers/__pycache__/tiangong.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.2/cnlitellm/providers/__pycache__/wenxin.cpython-312.pyc` & `cnlitellm-0.2.3/cnlitellm/providers/__pycache__/wenxin.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.2/cnlitellm/providers/__pycache__/zhipu.cpython-312.pyc` & `cnlitellm-0.2.3/cnlitellm/providers/__pycache__/zhipu.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.2/cnlitellm/providers/baichuan.py` & `cnlitellm-0.2.3/cnlitellm/providers/baichuan.py`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.2/cnlitellm/providers/base_provider.py` & `cnlitellm-0.2.3/cnlitellm/providers/base_provider.py`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.2/cnlitellm/providers/coze.py` & `cnlitellm-0.2.3/cnlitellm/providers/coze.py`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.2/cnlitellm/providers/dify.py` & `cnlitellm-0.2.3/cnlitellm/providers/dify.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,15 @@
         headers = {
             "Authorization": f"Bearer {self.api_key}",
             "Content-Type": "application/json",
         }
         response = requests.post(self.endpoint_url, headers=headers, data=payload)
         chunk_choices = []
         chunk_context = []
+        chunk_usage = Usage()
         index = 0
         for line in response.iter_lines():
             if line:
                 # judge if the new_line begins with "data:"
                 if line.startswith(b"data:"):
                     new_line = line.decode("utf-8").replace("data: ", "")
                     if new_line == "[DONE]":
@@ -76,37 +77,35 @@
                                 chunk_delta.content = chunk_message
                             chunk_choices.append(StreamingChoices(index=str(index), delta=chunk_delta))
 
                     if "metadata" in data:
                         metadata = data["metadata"]
                         if "usage" in metadata:
                             usage_info = metadata["usage"]
-                            chunk_usage = Usage()
                             if "prompt_tokens" in usage_info:
                                 chunk_usage.prompt_tokens = usage_info["prompt_tokens"]
                             if "completion_tokens" in usage_info:
                                 chunk_usage.completion_tokens = usage_info["completion_tokens"]
                             if "total_tokens" in usage_info:
                                 chunk_usage.total_tokens = usage_info["total_tokens"]
 
                         if 'retriever_resources' in metadata:
                             for resource in metadata['retriever_resources']:
                                 chunk_context.append({
                                     "id": resource["position"],
                                     "content": resource["content"],
                                     "score": resource["score"],    
                                 })
-
                     chunk_response = ModelResponse(
                         id="hello",
                         choices=chunk_choices,
                         context=chunk_context,
                         created=int(time.time()),
                         model=model,
-                        usage=chunk_usage if chunk_usage else None,
+                        usage=chunk_usage,
                         stream=True
                     )
                     index += 1
                     yield chunk_response
 
     def create_model_response_wrapper(self, result, model):
```

### Comparing `cnlitellm-0.2.2/cnlitellm/providers/fastgpt.py` & `cnlitellm-0.2.3/cnlitellm/providers/fastgpt.py`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.2/cnlitellm/providers/minimax.py` & `cnlitellm-0.2.3/cnlitellm/providers/minimax.py`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.2/cnlitellm/providers/moonshot.py` & `cnlitellm-0.2.3/cnlitellm/providers/moonshot.py`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.2/cnlitellm/providers/qwen.py` & `cnlitellm-0.2.3/cnlitellm/providers/qwen.py`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.2/cnlitellm/providers/tiangong.py` & `cnlitellm-0.2.3/cnlitellm/providers/tiangong.py`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.2/cnlitellm/providers/wenxin.py` & `cnlitellm-0.2.3/cnlitellm/providers/wenxin.py`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.2/cnlitellm/providers/xunfei.py` & `cnlitellm-0.2.3/cnlitellm/providers/xunfei.py`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.2/cnlitellm/providers/zhipu.py` & `cnlitellm-0.2.3/cnlitellm/providers/zhipu.py`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.2/cnlitellm/utils.py` & `cnlitellm-0.2.3/cnlitellm/utils.py`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.2/cnlitellm.egg-info/SOURCES.txt` & `cnlitellm-0.2.3/cnlitellm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.2/setup.py` & `cnlitellm-0.2.3/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cnlitellm',
-    version='0.2.2',
+    version='0.2.3',
     packages=find_packages(),
     license='MIT',
     description='A Python library for unified access to Chinese domestic large language models.',
     author='everfly',
     author_email='tagriver@gmail.com',
     url='https://github.com/EvalsOne/CNLiteLLM',
     install_requires=[
```

### Comparing `cnlitellm-0.2.2/tests/test_baichuan.py` & `cnlitellm-0.2.3/tests/test_baichuan.py`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.2/tests/test_coze.py` & `cnlitellm-0.2.3/tests/test_coze.py`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.2/tests/test_fastgpt.py` & `cnlitellm-0.2.3/tests/test_fastgpt.py`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.2/tests/test_minimax.py` & `cnlitellm-0.2.3/tests/test_minimax.py`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.2/tests/test_moonshot.py` & `cnlitellm-0.2.3/tests/test_moonshot.py`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.2/tests/test_moonshot2.py` & `cnlitellm-0.2.3/tests/test_moonshot2.py`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.2/tests/test_qwen.py` & `cnlitellm-0.2.3/tests/test_qwen.py`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.2/tests/test_tiangong.py` & `cnlitellm-0.2.3/tests/test_tiangong.py`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.2/tests/test_wenxin.py` & `cnlitellm-0.2.3/tests/test_wenxin.py`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.2/tests/test_zhipu.py` & `cnlitellm-0.2.3/tests/test_zhipu.py`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.2/tests/test_zhipu2.py` & `cnlitellm-0.2.3/tests/test_zhipu2.py`

 * *Files identical despite different names*
