# Comparing `tmp/mov_cli-4.3.7.tar.gz` & `tmp/mov_cli-4.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mov_cli-4.3.7.tar", last modified: Thu Apr 25 19:50:58 2024, max compression
+gzip compressed data, was "mov_cli-4.3.8.tar", last modified: Fri Apr 26 00:23:58 2024, max compression
```

## Comparing `mov_cli-4.3.7.tar` & `mov_cli-4.3.8.tar`

### file list

```diff
@@ -1,74 +1,75 @@
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-25 19:50:58.946753 mov_cli-4.3.7/
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-25 19:50:58.940086 mov_cli-4.3.7/.github/
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-25 19:50:58.940086 mov_cli-4.3.7/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 goldy     (1000) goldy     (1000)      185 2023-12-08 21:51:24.000000 mov_cli-4.3.7/.github/ISSUE_TEMPLATE/addprovider.md
--rw-r--r--   0 goldy     (1000) goldy     (1000)      925 2023-12-08 21:51:24.000000 mov_cli-4.3.7/.github/ISSUE_TEMPLATE/bug-report.md
--rw-r--r--   0 goldy     (1000) goldy     (1000)      319 2023-12-08 21:51:24.000000 mov_cli-4.3.7/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 goldy     (1000) goldy     (1000)      300 2023-12-08 21:51:24.000000 mov_cli-4.3.7/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0 goldy     (1000) goldy     (1000)      500 2023-12-08 21:51:24.000000 mov_cli-4.3.7/.github/dependabot.yml
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-25 19:50:58.940086 mov_cli-4.3.7/.github/workflows/
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1047 2023-12-08 21:51:24.000000 mov_cli-4.3.7/.github/workflows/pypi.yml
--rw-r--r--   0 goldy     (1000) goldy     (1000)      704 2024-03-20 02:02:17.000000 mov_cli-4.3.7/.github/workflows/ruff.yml
--rw-r--r--   0 goldy     (1000) goldy     (1000)       78 2023-12-08 21:51:24.000000 mov_cli-4.3.7/.gitignore
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1064 2024-03-04 00:50:47.000000 mov_cli-4.3.7/LICENSE
--rw-r--r--   0 goldy     (1000) goldy     (1000)      296 2024-04-25 16:37:27.000000 mov_cli-4.3.7/Makefile
--rw-r--r--   0 goldy     (1000) goldy     (1000)     7990 2024-04-25 19:50:58.946753 mov_cli-4.3.7/PKG-INFO
--rw-r--r--   0 goldy     (1000) goldy     (1000)     5336 2024-04-19 20:31:56.000000 mov_cli-4.3.7/README.md
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1549 2024-04-19 20:31:56.000000 mov_cli-4.3.7/disclaimer.md
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-25 19:50:58.940086 mov_cli-4.3.7/mov_cli/
--rw-r--r--   0 goldy     (1000) goldy     (1000)      131 2024-04-25 18:30:47.000000 mov_cli-4.3.7/mov_cli/__init__.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-25 19:50:58.943420 mov_cli-4.3.7/mov_cli/cli/
--rw-r--r--   0 goldy     (1000) goldy     (1000)       17 2023-12-08 21:51:24.000000 mov_cli-4.3.7/mov_cli/cli/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     5588 2024-04-25 17:41:01.000000 mov_cli-4.3.7/mov_cli/cli/__main__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)      416 2024-04-19 20:31:56.000000 mov_cli-4.3.7/mov_cli/cli/auto_select.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2089 2024-04-19 20:31:56.000000 mov_cli-4.3.7/mov_cli/cli/configuration.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2063 2024-04-19 20:31:56.000000 mov_cli-4.3.7/mov_cli/cli/episode.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2937 2024-04-25 18:27:22.000000 mov_cli-4.3.7/mov_cli/cli/play.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1785 2024-04-25 15:53:32.000000 mov_cli-4.3.7/mov_cli/cli/plugins.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     4095 2024-04-25 18:19:14.000000 mov_cli-4.3.7/mov_cli/cli/scraper.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1259 2024-04-25 17:24:40.000000 mov_cli-4.3.7/mov_cli/cli/search.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     6946 2024-04-25 17:44:59.000000 mov_cli-4.3.7/mov_cli/cli/ui.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1320 2024-04-19 20:31:56.000000 mov_cli-4.3.7/mov_cli/cli/watch_options.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     6434 2024-04-25 18:20:55.000000 mov_cli-4.3.7/mov_cli/config.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)      585 2024-04-25 16:37:16.000000 mov_cli-4.3.7/mov_cli/config.template.toml
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1032 2024-04-19 20:31:56.000000 mov_cli-4.3.7/mov_cli/download.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1002 2024-04-19 20:51:26.000000 mov_cli-4.3.7/mov_cli/errors.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2784 2024-04-04 00:43:21.000000 mov_cli-4.3.7/mov_cli/http_client.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-25 19:50:58.943420 mov_cli-4.3.7/mov_cli/iterfzf/
--rw-r--r--   0 goldy     (1000) goldy     (1000)    35147 2024-03-10 14:47:07.000000 mov_cli-4.3.7/mov_cli/iterfzf/LICENSE.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)     4123 2024-04-04 00:43:21.000000 mov_cli-4.3.7/mov_cli/iterfzf/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)      229 2023-12-08 21:51:24.000000 mov_cli-4.3.7/mov_cli/logger.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-25 19:50:58.943420 mov_cli-4.3.7/mov_cli/media/
--rw-r--r--   0 goldy     (1000) goldy     (1000)       44 2023-12-08 21:51:24.000000 mov_cli-4.3.7/mov_cli/media/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2914 2024-04-19 20:51:26.000000 mov_cli-4.3.7/mov_cli/media/media.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1859 2024-04-19 20:31:56.000000 mov_cli-4.3.7/mov_cli/media/metadata.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-25 19:50:58.943420 mov_cli-4.3.7/mov_cli/players/
--rw-r--r--   0 goldy     (1000) goldy     (1000)      113 2024-04-25 15:53:32.000000 mov_cli-4.3.7/mov_cli/players/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1100 2024-04-04 00:43:21.000000 mov_cli-4.3.7/mov_cli/players/custom_player.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     3133 2024-04-25 18:28:29.000000 mov_cli-4.3.7/mov_cli/players/mpv.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)      551 2024-04-04 00:43:21.000000 mov_cli-4.3.7/mov_cli/players/player.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2707 2024-04-25 18:28:34.000000 mov_cli-4.3.7/mov_cli/players/syncplay.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     3868 2024-04-25 18:28:38.000000 mov_cli-4.3.7/mov_cli/players/vlc.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1369 2024-04-19 20:31:56.000000 mov_cli-4.3.7/mov_cli/plugins.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2093 2024-04-19 20:31:56.000000 mov_cli-4.3.7/mov_cli/scraper.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-25 19:50:58.946753 mov_cli-4.3.7/mov_cli/utils/
--rw-r--r--   0 goldy     (1000) goldy     (1000)       99 2024-04-22 21:39:57.000000 mov_cli-4.3.7/mov_cli/utils/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)      620 2024-04-04 00:43:21.000000 mov_cli-4.3.7/mov_cli/utils/episode_selector.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2018 2024-04-22 23:14:10.000000 mov_cli-4.3.7/mov_cli/utils/paths.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)      652 2024-03-13 15:29:53.000000 mov_cli-4.3.7/mov_cli/utils/platform.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-25 19:50:58.946753 mov_cli-4.3.7/mov_cli/utils/scraper/
--rw-r--r--   0 goldy     (1000) goldy     (1000)       69 2024-04-19 20:31:56.000000 mov_cli-4.3.7/mov_cli/utils/scraper/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     4751 2024-04-19 20:31:56.000000 mov_cli-4.3.7/mov_cli/utils/scraper/the_movie_db.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     3383 2024-04-19 20:31:56.000000 mov_cli-4.3.7/mov_cli/utils/version.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-25 19:50:58.946753 mov_cli-4.3.7/mov_cli.egg-info/
--rw-r--r--   0 goldy     (1000) goldy     (1000)     7990 2024-04-25 19:50:58.000000 mov_cli-4.3.7/mov_cli.egg-info/PKG-INFO
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1457 2024-04-25 19:50:58.000000 mov_cli-4.3.7/mov_cli.egg-info/SOURCES.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)        1 2024-04-25 19:50:58.000000 mov_cli-4.3.7/mov_cli.egg-info/dependency_links.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)       53 2024-04-25 19:50:58.000000 mov_cli-4.3.7/mov_cli.egg-info/entry_points.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)      215 2024-04-25 19:50:58.000000 mov_cli-4.3.7/mov_cli.egg-info/requires.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)        8 2024-04-25 19:50:58.000000 mov_cli-4.3.7/mov_cli.egg-info/top_level.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1733 2024-04-19 20:31:56.000000 mov_cli-4.3.7/pyproject.toml
--rw-r--r--   0 goldy     (1000) goldy     (1000)      243 2024-04-04 00:43:21.000000 mov_cli-4.3.7/ruff.toml
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-25 19:50:58.946753 mov_cli-4.3.7/scripts/
--rw-r--r--   0 goldy     (1000) goldy     (1000)      285 2023-12-08 21:51:24.000000 mov_cli-4.3.7/scripts/test_cli.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)       38 2024-04-25 19:50:58.946753 mov_cli-4.3.7/setup.cfg
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-26 00:23:58.881339 mov_cli-4.3.8/
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-26 00:23:58.871339 mov_cli-4.3.8/.github/
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-26 00:23:58.871339 mov_cli-4.3.8/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      185 2023-12-08 21:51:24.000000 mov_cli-4.3.8/.github/ISSUE_TEMPLATE/addprovider.md
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      925 2023-12-08 21:51:24.000000 mov_cli-4.3.8/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      319 2023-12-08 21:51:24.000000 mov_cli-4.3.8/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      300 2023-12-08 21:51:24.000000 mov_cli-4.3.8/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      500 2023-12-08 21:51:24.000000 mov_cli-4.3.8/.github/dependabot.yml
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-26 00:23:58.871339 mov_cli-4.3.8/.github/workflows/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1047 2023-12-08 21:51:24.000000 mov_cli-4.3.8/.github/workflows/pypi.yml
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      704 2024-03-20 02:02:17.000000 mov_cli-4.3.8/.github/workflows/ruff.yml
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       78 2023-12-08 21:51:24.000000 mov_cli-4.3.8/.gitignore
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1064 2024-03-04 00:50:47.000000 mov_cli-4.3.8/LICENSE
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      296 2024-04-25 20:43:50.000000 mov_cli-4.3.8/Makefile
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     7990 2024-04-26 00:23:58.881339 mov_cli-4.3.8/PKG-INFO
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     5336 2024-04-19 20:31:56.000000 mov_cli-4.3.8/README.md
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1549 2024-04-19 20:31:56.000000 mov_cli-4.3.8/disclaimer.md
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-26 00:23:58.874672 mov_cli-4.3.8/mov_cli/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      131 2024-04-26 00:22:56.000000 mov_cli-4.3.8/mov_cli/__init__.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-26 00:23:58.878005 mov_cli-4.3.8/mov_cli/cli/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       17 2023-12-08 21:51:24.000000 mov_cli-4.3.8/mov_cli/cli/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     5588 2024-04-25 23:19:21.000000 mov_cli-4.3.8/mov_cli/cli/__main__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      416 2024-04-19 20:31:56.000000 mov_cli-4.3.8/mov_cli/cli/auto_select.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2089 2024-04-19 20:31:56.000000 mov_cli-4.3.8/mov_cli/cli/configuration.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2063 2024-04-19 20:31:56.000000 mov_cli-4.3.8/mov_cli/cli/episode.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2937 2024-04-25 20:43:50.000000 mov_cli-4.3.8/mov_cli/cli/play.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1785 2024-04-25 15:53:32.000000 mov_cli-4.3.8/mov_cli/cli/plugins.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      159 2024-04-25 20:43:50.000000 mov_cli-4.3.8/mov_cli/cli/random_tips.json
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     4095 2024-04-26 00:20:10.000000 mov_cli-4.3.8/mov_cli/cli/scraper.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1259 2024-04-25 20:43:50.000000 mov_cli-4.3.8/mov_cli/cli/search.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     6946 2024-04-25 20:43:50.000000 mov_cli-4.3.8/mov_cli/cli/ui.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1320 2024-04-19 20:31:56.000000 mov_cli-4.3.8/mov_cli/cli/watch_options.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     6434 2024-04-25 23:19:21.000000 mov_cli-4.3.8/mov_cli/config.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      585 2024-04-25 23:19:21.000000 mov_cli-4.3.8/mov_cli/config.template.toml
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1032 2024-04-19 20:31:56.000000 mov_cli-4.3.8/mov_cli/download.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1002 2024-04-19 20:51:26.000000 mov_cli-4.3.8/mov_cli/errors.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2784 2024-04-04 00:43:21.000000 mov_cli-4.3.8/mov_cli/http_client.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-26 00:23:58.878005 mov_cli-4.3.8/mov_cli/iterfzf/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)    35147 2024-03-10 14:47:07.000000 mov_cli-4.3.8/mov_cli/iterfzf/LICENSE.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     4123 2024-04-04 00:43:21.000000 mov_cli-4.3.8/mov_cli/iterfzf/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      229 2023-12-08 21:51:24.000000 mov_cli-4.3.8/mov_cli/logger.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-26 00:23:58.878005 mov_cli-4.3.8/mov_cli/media/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       44 2023-12-08 21:51:24.000000 mov_cli-4.3.8/mov_cli/media/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2914 2024-04-19 20:51:26.000000 mov_cli-4.3.8/mov_cli/media/media.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1859 2024-04-19 20:31:56.000000 mov_cli-4.3.8/mov_cli/media/metadata.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-26 00:23:58.878005 mov_cli-4.3.8/mov_cli/players/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      113 2024-04-25 15:53:32.000000 mov_cli-4.3.8/mov_cli/players/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1100 2024-04-04 00:43:21.000000 mov_cli-4.3.8/mov_cli/players/custom_player.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     3133 2024-04-25 20:43:50.000000 mov_cli-4.3.8/mov_cli/players/mpv.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      551 2024-04-04 00:43:21.000000 mov_cli-4.3.8/mov_cli/players/player.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2707 2024-04-25 20:43:50.000000 mov_cli-4.3.8/mov_cli/players/syncplay.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     3868 2024-04-25 20:43:50.000000 mov_cli-4.3.8/mov_cli/players/vlc.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1369 2024-04-19 20:31:56.000000 mov_cli-4.3.8/mov_cli/plugins.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2093 2024-04-19 20:31:56.000000 mov_cli-4.3.8/mov_cli/scraper.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-26 00:23:58.878005 mov_cli-4.3.8/mov_cli/utils/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       99 2024-04-22 21:39:57.000000 mov_cli-4.3.8/mov_cli/utils/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      620 2024-04-04 00:43:21.000000 mov_cli-4.3.8/mov_cli/utils/episode_selector.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2018 2024-04-22 23:14:10.000000 mov_cli-4.3.8/mov_cli/utils/paths.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      652 2024-03-13 15:29:53.000000 mov_cli-4.3.8/mov_cli/utils/platform.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-26 00:23:58.881339 mov_cli-4.3.8/mov_cli/utils/scraper/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       69 2024-04-19 20:31:56.000000 mov_cli-4.3.8/mov_cli/utils/scraper/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     4751 2024-04-19 20:31:56.000000 mov_cli-4.3.8/mov_cli/utils/scraper/the_movie_db.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     3383 2024-04-19 20:31:56.000000 mov_cli-4.3.8/mov_cli/utils/version.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-26 00:23:58.881339 mov_cli-4.3.8/mov_cli.egg-info/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     7990 2024-04-26 00:23:58.000000 mov_cli-4.3.8/mov_cli.egg-info/PKG-INFO
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1486 2024-04-26 00:23:58.000000 mov_cli-4.3.8/mov_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)        1 2024-04-26 00:23:58.000000 mov_cli-4.3.8/mov_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       53 2024-04-26 00:23:58.000000 mov_cli-4.3.8/mov_cli.egg-info/entry_points.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      215 2024-04-26 00:23:58.000000 mov_cli-4.3.8/mov_cli.egg-info/requires.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)        8 2024-04-26 00:23:58.000000 mov_cli-4.3.8/mov_cli.egg-info/top_level.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1757 2024-04-26 00:22:19.000000 mov_cli-4.3.8/pyproject.toml
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      243 2024-04-04 00:43:21.000000 mov_cli-4.3.8/ruff.toml
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-26 00:23:58.881339 mov_cli-4.3.8/scripts/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      285 2023-12-08 21:51:24.000000 mov_cli-4.3.8/scripts/test_cli.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       38 2024-04-26 00:23:58.881339 mov_cli-4.3.8/setup.cfg
```

### Comparing `mov_cli-4.3.7/.github/ISSUE_TEMPLATE/bug-report.md` & `mov_cli-4.3.8/.github/ISSUE_TEMPLATE/bug-report.md`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.7/.github/workflows/pypi.yml` & `mov_cli-4.3.8/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.7/.github/workflows/ruff.yml` & `mov_cli-4.3.8/.github/workflows/ruff.yml`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.7/LICENSE` & `mov_cli-4.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.7/PKG-INFO` & `mov_cli-4.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mov-cli
-Version: 4.3.7
+Version: 4.3.8
 Summary: Watch everything from your terminal.
 Author-email: Pain <painedposeidon444@gmail.com>, Ananas <ananas@r3tr0ananas.lol>, Goldy <goldy@devgoldy.xyz>
 License: MIT License
         
         Copyright (c) 2024 mov-cli
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mov-cli Version: 4.3.7 Summary: Watch everything
+Metadata-Version: 2.1 Name: mov-cli Version: 4.3.8 Summary: Watch everything
 from your terminal. Author-email: Pain
 gmail.com>, Ananas
 r3tr0ananas.lol>, Goldy
 devgoldy.xyz> License: MIT License Copyright (c) 2024 mov-cli Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
```

### Comparing `mov_cli-4.3.7/README.md` & `mov_cli-4.3.8/README.md`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.7/disclaimer.md` & `mov_cli-4.3.8/disclaimer.md`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.7/mov_cli/cli/__main__.py` & `mov_cli-4.3.8/mov_cli/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.7/mov_cli/cli/configuration.py` & `mov_cli-4.3.8/mov_cli/cli/configuration.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.7/mov_cli/cli/episode.py` & `mov_cli-4.3.8/mov_cli/cli/episode.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.7/mov_cli/cli/play.py` & `mov_cli-4.3.8/mov_cli/cli/play.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.7/mov_cli/cli/plugins.py` & `mov_cli-4.3.8/mov_cli/cli/plugins.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.7/mov_cli/cli/scraper.py` & `mov_cli-4.3.8/mov_cli/cli/scraper.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.7/mov_cli/cli/search.py` & `mov_cli-4.3.8/mov_cli/cli/search.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.7/mov_cli/cli/ui.py` & `mov_cli-4.3.8/mov_cli/cli/ui.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.7/mov_cli/cli/watch_options.py` & `mov_cli-4.3.8/mov_cli/cli/watch_options.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.7/mov_cli/config.py` & `mov_cli-4.3.8/mov_cli/config.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.7/mov_cli/config.template.toml` & `mov_cli-4.3.8/mov_cli/config.template.toml`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.7/mov_cli/download.py` & `mov_cli-4.3.8/mov_cli/download.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.7/mov_cli/errors.py` & `mov_cli-4.3.8/mov_cli/errors.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.7/mov_cli/http_client.py` & `mov_cli-4.3.8/mov_cli/http_client.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.7/mov_cli/iterfzf/LICENSE.txt` & `mov_cli-4.3.8/mov_cli/iterfzf/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.7/mov_cli/iterfzf/__init__.py` & `mov_cli-4.3.8/mov_cli/iterfzf/__init__.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.7/mov_cli/media/media.py` & `mov_cli-4.3.8/mov_cli/media/media.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.7/mov_cli/media/metadata.py` & `mov_cli-4.3.8/mov_cli/media/metadata.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.7/mov_cli/players/custom_player.py` & `mov_cli-4.3.8/mov_cli/players/custom_player.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.7/mov_cli/players/mpv.py` & `mov_cli-4.3.8/mov_cli/players/mpv.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.7/mov_cli/players/player.py` & `mov_cli-4.3.8/mov_cli/players/player.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.7/mov_cli/players/syncplay.py` & `mov_cli-4.3.8/mov_cli/players/syncplay.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.7/mov_cli/players/vlc.py` & `mov_cli-4.3.8/mov_cli/players/vlc.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.7/mov_cli/plugins.py` & `mov_cli-4.3.8/mov_cli/plugins.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.7/mov_cli/scraper.py` & `mov_cli-4.3.8/mov_cli/scraper.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.7/mov_cli/utils/episode_selector.py` & `mov_cli-4.3.8/mov_cli/utils/episode_selector.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.7/mov_cli/utils/paths.py` & `mov_cli-4.3.8/mov_cli/utils/paths.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.7/mov_cli/utils/platform.py` & `mov_cli-4.3.8/mov_cli/utils/platform.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.7/mov_cli/utils/scraper/the_movie_db.py` & `mov_cli-4.3.8/mov_cli/utils/scraper/the_movie_db.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.7/mov_cli/utils/version.py` & `mov_cli-4.3.8/mov_cli/utils/version.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.7/mov_cli.egg-info/PKG-INFO` & `mov_cli-4.3.8/mov_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mov-cli
-Version: 4.3.7
+Version: 4.3.8
 Summary: Watch everything from your terminal.
 Author-email: Pain <painedposeidon444@gmail.com>, Ananas <ananas@r3tr0ananas.lol>, Goldy <goldy@devgoldy.xyz>
 License: MIT License
         
         Copyright (c) 2024 mov-cli
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mov-cli Version: 4.3.7 Summary: Watch everything
+Metadata-Version: 2.1 Name: mov-cli Version: 4.3.8 Summary: Watch everything
 from your terminal. Author-email: Pain
 gmail.com>, Ananas
 r3tr0ananas.lol>, Goldy
 devgoldy.xyz> License: MIT License Copyright (c) 2024 mov-cli Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
```

### Comparing `mov_cli-4.3.7/mov_cli.egg-info/SOURCES.txt` & `mov_cli-4.3.8/mov_cli.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 mov_cli/cli/__init__.py
 mov_cli/cli/__main__.py
 mov_cli/cli/auto_select.py
 mov_cli/cli/configuration.py
 mov_cli/cli/episode.py
 mov_cli/cli/play.py
 mov_cli/cli/plugins.py
+mov_cli/cli/random_tips.json
 mov_cli/cli/scraper.py
 mov_cli/cli/search.py
 mov_cli/cli/ui.py
 mov_cli/cli/watch_options.py
 mov_cli/iterfzf/LICENSE.txt
 mov_cli/iterfzf/__init__.py
 mov_cli/media/__init__.py
```

### Comparing `mov_cli-4.3.7/pyproject.toml` & `mov_cli-4.3.8/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -59,11 +59,11 @@
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 include = ["mov_cli*"]
 
 [tool.setuptools.package-data]
-"mov_cli" = ["config.template.toml"]
+"mov_cli" = ["config.template.toml", "cli/random_tips.json"]
 
 [project.scripts]
 mov-cli = "mov_cli.cli.__main__:app"
```

