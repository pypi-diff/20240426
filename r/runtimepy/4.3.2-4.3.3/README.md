# Comparing `tmp/runtimepy-4.3.2.tar.gz` & `tmp/runtimepy-4.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runtimepy-4.3.2.tar", last modified: Thu Apr 25 21:06:42 2024, max compression
+gzip compressed data, was "runtimepy-4.3.3.tar", last modified: Fri Apr 26 15:59:27 2024, max compression
```

## Comparing `runtimepy-4.3.2.tar` & `runtimepy-4.3.3.tar`

### file list

```diff
@@ -1,306 +1,307 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:06:42.486411 runtimepy-4.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-25 21:04:20.000000 runtimepy-4.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7055 2024-04-25 21:06:42.486411 runtimepy-4.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-04-25 21:04:20.000000 runtimepy-4.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-25 21:04:20.000000 runtimepy-4.3.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:06:42.450411 runtimepy-4.3.2/runtimepy/
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:06:42.450411 runtimepy-4.3.2/runtimepy/channel/
--rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/channel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:06:42.454411 runtimepy-4.3.2/runtimepy/channel/environment/
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/channel/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/channel/environment/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     9835 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/channel/environment/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:06:42.454411 runtimepy-4.3.2/runtimepy/channel/environment/command/
--rw-r--r--   0 runner    (1001) docker     (127)     8162 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/channel/environment/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/channel/environment/command/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5984 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/channel/environment/command/processor.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/channel/environment/command/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/channel/environment/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     6949 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/channel/environment/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/channel/environment/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     5341 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/channel/environment/telemetry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:06:42.454411 runtimepy-4.3.2/runtimepy/channel/event/
--rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/channel/event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/channel/event/header.py
--rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/channel/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:06:42.454411 runtimepy-4.3.2/runtimepy/codec/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/codec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:06:42.454411 runtimepy-4.3.2/runtimepy/codec/protocol/
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/codec/protocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/codec/protocol/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/codec/protocol/json.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:06:42.454411 runtimepy-4.3.2/runtimepy/codec/system/
--rw-r--r--   0 runner    (1001) docker     (127)     6939 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/codec/system/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:06:42.454411 runtimepy-4.3.2/runtimepy/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/commands/all.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/commands/arbiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/commands/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/commands/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/commands/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/commands/tui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:06:42.458411 runtimepy-4.3.2/runtimepy/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:06:42.458411 runtimepy-4.3.2/runtimepy/data/css/
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/data/css/bootstrap_extra.css
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/data/css/main.css
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/data/dummy_load.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/data/factories.yaml
--rw-r--r--   0 runner    (1001) docker     (127)   362870 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/data/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:06:42.458411 runtimepy-4.3.2/runtimepy/data/js/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/data/js/DataConnection.js
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/data/js/JsonConnection.js
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/data/js/audio.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:06:42.462411 runtimepy-4.3.2/runtimepy/data/js/classes/
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/data/js/classes/App.js
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/data/js/classes/ChannelTable.js
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/data/js/classes/DataConnection.js
--rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/data/js/classes/JsonConnection.js
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/data/js/classes/Plot.js
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/data/js/classes/PlotManager.js
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/data/js/classes/PlotModalManager.js
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/data/js/classes/TabFilter.js
--rw-r--r--   0 runner    (1001) docker     (127)     7620 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/data/js/classes/TabInterface.js
--rw-r--r--   0 runner    (1001) docker     (127)     5233 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/data/js/classes/WindowHashManager.js
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/data/js/classes/WorkerInterface.js
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/data/js/init.js
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/data/js/main.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:06:42.462411 runtimepy-4.3.2/runtimepy/data/js/tab/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/data/js/tab/env.js
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/data/js/tab/sound.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:06:42.462411 runtimepy-4.3.2/runtimepy/data/js/unused/
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/data/js/unused/pyodide.js
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/data/js/util.js
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/data/js/worker.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:06:42.462411 runtimepy-4.3.2/runtimepy/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/data/schemas/BitFields.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/data/schemas/Channel.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/data/schemas/ChannelCommand.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/data/schemas/ChannelRegistry.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/data/schemas/ClientConnectionConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/data/schemas/ConnectionArbiterConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/data/schemas/EnumRegistry.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/data/schemas/FindFile.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/data/schemas/PeerProcessConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/data/schemas/RuntimeEnum.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/data/schemas/ServerConnectionConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/data/schemas/StructConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/data/schemas/TaskConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/data/schemas/has_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/data/schemas/has_factory.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/data/schemas/has_name.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/data/schemas/has_request_flag.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/data/server.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/data/server_base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/data/server_dev.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:06:42.462411 runtimepy-4.3.2/runtimepy/enum/
--rw-r--r--   0 runner    (1001) docker     (127)     5819 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/enum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/enum/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/enum/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5091 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:06:42.466411 runtimepy-4.3.2/runtimepy/message/
--rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/message/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3775 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/message/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11285 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/message/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/message/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:06:42.466411 runtimepy-4.3.2/runtimepy/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/metrics/channel.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/metrics/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/metrics/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:06:42.466411 runtimepy-4.3.2/runtimepy/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/mixins/async_command.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/mixins/enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/mixins/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/mixins/finalize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/mixins/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/mixins/psutil.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/mixins/regex.py
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/mixins/trig.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:06:42.466411 runtimepy-4.3.2/runtimepy/net/
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:06:42.466411 runtimepy-4.3.2/runtimepy/net/apps/
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:06:42.470411 runtimepy-4.3.2/runtimepy/net/arbiter/
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/arbiter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14523 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/arbiter/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:06:42.470411 runtimepy-4.3.2/runtimepy/net/arbiter/config/
--rw-r--r--   0 runner    (1001) docker     (127)     7990 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/arbiter/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/arbiter/config/codec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/arbiter/config/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:06:42.470411 runtimepy-4.3.2/runtimepy/net/arbiter/factory/
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/arbiter/factory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/arbiter/factory/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/arbiter/factory/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:06:42.470411 runtimepy-4.3.2/runtimepy/net/arbiter/housekeeping/
--rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/arbiter/housekeeping/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:06:42.470411 runtimepy-4.3.2/runtimepy/net/arbiter/imports/
--rw-r--r--   0 runner    (1001) docker     (127)     4980 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/arbiter/imports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/arbiter/imports/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     8350 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/arbiter/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/arbiter/result.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/arbiter/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:06:42.470411 runtimepy-4.3.2/runtimepy/net/arbiter/tcp/
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/arbiter/tcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/arbiter/tcp/json.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/arbiter/udp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/arbiter/websocket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/backoff.py
--rw-r--r--   0 runner    (1001) docker     (127)    11894 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:06:42.470411 runtimepy-4.3.2/runtimepy/net/factories/
--rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/factories/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:06:42.470411 runtimepy-4.3.2/runtimepy/net/http/
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/http/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/http/header.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/http/request_target.py
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/http/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/http/state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/http/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:06:42.470411 runtimepy-4.3.2/runtimepy/net/server/
--rw-r--r--   0 runner    (1001) docker     (127)     5178 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:06:42.474411 runtimepy-4.3.2/runtimepy/net/server/app/
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/server/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/server/app/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:06:42.474411 runtimepy-4.3.2/runtimepy/net/server/app/bootstrap/
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/server/app/bootstrap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/server/app/bootstrap/elements.py
--rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/server/app/bootstrap/tabs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/server/app/create.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/server/app/elements.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:06:42.474411 runtimepy-4.3.2/runtimepy/net/server/app/env/
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/server/app/env/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/server/app/env/modal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:06:42.474411 runtimepy-4.3.2/runtimepy/net/server/app/env/tab/
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/server/app/env/tab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/server/app/env/tab/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7408 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/server/app/env/tab/html.py
--rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/server/app/env/tab/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/server/app/env/widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/server/app/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/server/app/placeholder.py
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/server/app/pyodide.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/server/app/sound.py
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/server/app/tab.py
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/server/html.py
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/server/json.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:06:42.474411 runtimepy-4.3.2/runtimepy/net/server/struct/
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/server/struct/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:06:42.474411 runtimepy-4.3.2/runtimepy/net/server/websocket/
--rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/server/websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/server/websocket/state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:06:42.474411 runtimepy-4.3.2/runtimepy/net/stream/
--rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/stream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/stream/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:06:42.474411 runtimepy-4.3.2/runtimepy/net/stream/json/
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/stream/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/stream/string.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:06:42.478412 runtimepy-4.3.2/runtimepy/net/tcp/
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/tcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7377 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/tcp/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/tcp/create.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:06:42.478412 runtimepy-4.3.2/runtimepy/net/tcp/http/
--rw-r--r--   0 runner    (1001) docker     (127)     5236 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/tcp/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/tcp/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:06:42.478412 runtimepy-4.3.2/runtimepy/net/tcp/telnet/
--rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/tcp/telnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/tcp/telnet/codes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:06:42.478412 runtimepy-4.3.2/runtimepy/net/udp/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/udp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7485 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/udp/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/udp/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/udp/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:06:42.478412 runtimepy-4.3.2/runtimepy/net/websocket/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8068 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/net/websocket/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:06:42.478412 runtimepy-4.3.2/runtimepy/primitives/
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/primitives/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:06:42.478412 runtimepy-4.3.2/runtimepy/primitives/array/
--rw-r--r--   0 runner    (1001) docker     (127)     8239 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/primitives/array/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7715 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/primitives/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/primitives/bool.py
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/primitives/byte_order.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:06:42.478412 runtimepy-4.3.2/runtimepy/primitives/field/
--rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/primitives/field/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7481 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/primitives/field/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:06:42.478412 runtimepy-4.3.2/runtimepy/primitives/field/manager/
--rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/primitives/field/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6705 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/primitives/field/manager/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/primitives/float.py
--rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/primitives/int.py
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/primitives/scaling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:06:42.482411 runtimepy-4.3.2/runtimepy/primitives/serializable/
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/primitives/serializable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/primitives/serializable/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/primitives/serializable/fixed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/primitives/serializable/prefixed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/primitives/string.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:06:42.482411 runtimepy-4.3.2/runtimepy/primitives/types/
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/primitives/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/primitives/types/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/primitives/types/bool.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/primitives/types/bounds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/primitives/types/float.py
--rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/primitives/types/int.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:06:42.482411 runtimepy-4.3.2/runtimepy/registry/
--rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/registry/bool.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/registry/item.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/registry/name.py
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:06:42.482411 runtimepy-4.3.2/runtimepy/sample/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/sample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/sample/peer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/sample/program.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:06:42.482411 runtimepy-4.3.2/runtimepy/struct/
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/struct/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:06:42.482411 runtimepy-4.3.2/runtimepy/subprocess/
--rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/subprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7441 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/subprocess/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     6335 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/subprocess/peer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6792 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/subprocess/program.py
--rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/subprocess/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:06:42.482411 runtimepy-4.3.2/runtimepy/task/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5947 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/task/asynchronous.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:06:42.482411 runtimepy-4.3.2/runtimepy/task/basic/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/task/basic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/task/basic/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6388 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/task/basic/periodic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/task/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:06:42.486411 runtimepy-4.3.2/runtimepy/task/trig/
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/task/trig/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:06:42.486411 runtimepy-4.3.2/runtimepy/telemetry/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/telemetry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:06:42.486411 runtimepy-4.3.2/runtimepy/tui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/tui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:06:42.486411 runtimepy-4.3.2/runtimepy/tui/channels/
--rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/tui/channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/tui/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/tui/mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/tui/mock.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/tui/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-04-25 21:04:20.000000 runtimepy-4.3.2/runtimepy/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:06:42.486411 runtimepy-4.3.2/runtimepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7055 2024-04-25 21:06:42.000000 runtimepy-4.3.2/runtimepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8012 2024-04-25 21:06:42.000000 runtimepy-4.3.2/runtimepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 21:06:42.000000 runtimepy-4.3.2/runtimepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-25 21:06:42.000000 runtimepy-4.3.2/runtimepy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-25 21:06:42.000000 runtimepy-4.3.2/runtimepy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-25 21:06:42.000000 runtimepy-4.3.2/runtimepy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 21:06:42.486411 runtimepy-4.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-25 21:04:20.000000 runtimepy-4.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:06:42.486411 runtimepy-4.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-25 21:04:20.000000 runtimepy-4.3.2/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-25 21:04:20.000000 runtimepy-4.3.2/tests/test_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-25 21:04:20.000000 runtimepy-4.3.2/tests/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:27.505902 runtimepy-4.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-26 15:56:56.000000 runtimepy-4.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7055 2024-04-26 15:59:27.505902 runtimepy-4.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-04-26 15:56:56.000000 runtimepy-4.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-26 15:56:56.000000 runtimepy-4.3.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:27.465901 runtimepy-4.3.3/runtimepy/
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:27.465901 runtimepy-4.3.3/runtimepy/channel/
+-rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/channel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:27.465901 runtimepy-4.3.3/runtimepy/channel/environment/
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/channel/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/channel/environment/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9835 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/channel/environment/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:27.465901 runtimepy-4.3.3/runtimepy/channel/environment/command/
+-rw-r--r--   0 runner    (1001) docker     (127)     8162 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/channel/environment/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/channel/environment/command/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5984 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/channel/environment/command/processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/channel/environment/command/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/channel/environment/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6949 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/channel/environment/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/channel/environment/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5341 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/channel/environment/telemetry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:27.465901 runtimepy-4.3.3/runtimepy/channel/event/
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/channel/event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/channel/event/header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/channel/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:27.469901 runtimepy-4.3.3/runtimepy/codec/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/codec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:27.469901 runtimepy-4.3.3/runtimepy/codec/protocol/
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/codec/protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/codec/protocol/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/codec/protocol/json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:27.469901 runtimepy-4.3.3/runtimepy/codec/system/
+-rw-r--r--   0 runner    (1001) docker     (127)     6939 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/codec/system/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:27.469901 runtimepy-4.3.3/runtimepy/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/commands/all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/commands/arbiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/commands/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/commands/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/commands/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/commands/tui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:27.469901 runtimepy-4.3.3/runtimepy/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:27.469901 runtimepy-4.3.3/runtimepy/data/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/data/css/bootstrap_extra.css
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/data/css/main.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/data/dummy_load.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/data/factories.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)   362870 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/data/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:27.473901 runtimepy-4.3.3/runtimepy/data/js/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/data/js/DataConnection.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/data/js/JsonConnection.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/data/js/audio.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:27.473901 runtimepy-4.3.3/runtimepy/data/js/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/data/js/classes/App.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/data/js/classes/ChannelTable.js
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/data/js/classes/DataConnection.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/data/js/classes/JsonConnection.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/data/js/classes/Plot.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/data/js/classes/PlotManager.js
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/data/js/classes/PlotModalManager.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/data/js/classes/TabFilter.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7620 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/data/js/classes/TabInterface.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5233 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/data/js/classes/WindowHashManager.js
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/data/js/classes/WorkerInterface.js
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/data/js/init.js
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/data/js/main.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:27.473901 runtimepy-4.3.3/runtimepy/data/js/tab/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/data/js/tab/env.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/data/js/tab/sound.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:27.473901 runtimepy-4.3.3/runtimepy/data/js/unused/
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/data/js/unused/pyodide.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/data/js/util.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/data/js/worker.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:27.477902 runtimepy-4.3.3/runtimepy/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/data/schemas/BitFields.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/data/schemas/Channel.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/data/schemas/ChannelCommand.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/data/schemas/ChannelRegistry.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/data/schemas/ClientConnectionConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/data/schemas/ConnectionArbiterConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/data/schemas/EnumRegistry.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/data/schemas/FindFile.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/data/schemas/PeerProcessConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/data/schemas/RuntimeEnum.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/data/schemas/ServerConnectionConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/data/schemas/StructConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/data/schemas/TaskConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/data/schemas/has_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/data/schemas/has_factory.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/data/schemas/has_name.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/data/schemas/has_request_flag.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/data/server.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/data/server_base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/data/server_dev.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:27.477902 runtimepy-4.3.3/runtimepy/enum/
+-rw-r--r--   0 runner    (1001) docker     (127)     5819 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/enum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/enum/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/enum/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5091 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:27.477902 runtimepy-4.3.3/runtimepy/message/
+-rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/message/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3775 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/message/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11285 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/message/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/message/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:27.481902 runtimepy-4.3.3/runtimepy/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/metrics/channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/metrics/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/metrics/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:27.481902 runtimepy-4.3.3/runtimepy/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/mixins/async_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/mixins/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/mixins/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/mixins/finalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/mixins/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/mixins/psutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/mixins/regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/mixins/trig.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:27.481902 runtimepy-4.3.3/runtimepy/net/
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:27.481902 runtimepy-4.3.3/runtimepy/net/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:27.485901 runtimepy-4.3.3/runtimepy/net/arbiter/
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/arbiter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14523 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/arbiter/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:27.485901 runtimepy-4.3.3/runtimepy/net/arbiter/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     7990 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/arbiter/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/arbiter/config/codec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/arbiter/config/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:27.485901 runtimepy-4.3.3/runtimepy/net/arbiter/factory/
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/arbiter/factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/arbiter/factory/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/arbiter/factory/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:27.485901 runtimepy-4.3.3/runtimepy/net/arbiter/housekeeping/
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/arbiter/housekeeping/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:27.485901 runtimepy-4.3.3/runtimepy/net/arbiter/imports/
+-rw-r--r--   0 runner    (1001) docker     (127)     4980 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/arbiter/imports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/arbiter/imports/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8350 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/arbiter/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/arbiter/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/arbiter/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:27.485901 runtimepy-4.3.3/runtimepy/net/arbiter/tcp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/arbiter/tcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/arbiter/tcp/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/arbiter/udp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/arbiter/websocket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/backoff.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11894 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:27.485901 runtimepy-4.3.3/runtimepy/net/factories/
+-rw-r--r--   0 runner    (1001) docker     (127)     4316 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/factories/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:27.485901 runtimepy-4.3.3/runtimepy/net/http/
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/http/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/http/header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/http/request_target.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/http/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/http/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/http/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:27.485901 runtimepy-4.3.3/runtimepy/net/server/
+-rw-r--r--   0 runner    (1001) docker     (127)     5178 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:27.489901 runtimepy-4.3.3/runtimepy/net/server/app/
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/server/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/server/app/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:27.489901 runtimepy-4.3.3/runtimepy/net/server/app/bootstrap/
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/server/app/bootstrap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/server/app/bootstrap/elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/server/app/bootstrap/tabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/server/app/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/server/app/elements.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:27.489901 runtimepy-4.3.3/runtimepy/net/server/app/env/
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/server/app/env/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/server/app/env/modal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:27.489901 runtimepy-4.3.3/runtimepy/net/server/app/env/tab/
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/server/app/env/tab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/server/app/env/tab/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7408 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/server/app/env/tab/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/server/app/env/tab/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/server/app/env/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/server/app/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/server/app/placeholder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/server/app/pyodide.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/server/app/sound.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/server/app/tab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/server/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/server/json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:27.489901 runtimepy-4.3.3/runtimepy/net/server/struct/
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/server/struct/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:27.489901 runtimepy-4.3.3/runtimepy/net/server/websocket/
+-rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/server/websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/server/websocket/state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:27.493902 runtimepy-4.3.3/runtimepy/net/stream/
+-rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/stream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/stream/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:27.493902 runtimepy-4.3.3/runtimepy/net/stream/json/
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/stream/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/stream/string.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:27.493902 runtimepy-4.3.3/runtimepy/net/tcp/
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/tcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7377 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/tcp/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/tcp/create.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:27.493902 runtimepy-4.3.3/runtimepy/net/tcp/http/
+-rw-r--r--   0 runner    (1001) docker     (127)     5236 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/tcp/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/tcp/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:27.493902 runtimepy-4.3.3/runtimepy/net/tcp/telnet/
+-rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/tcp/telnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/tcp/telnet/codes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:27.493902 runtimepy-4.3.3/runtimepy/net/udp/
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/udp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7485 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/udp/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/udp/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/udp/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/udp/queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:27.493902 runtimepy-4.3.3/runtimepy/net/websocket/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8068 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/net/websocket/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:27.493902 runtimepy-4.3.3/runtimepy/primitives/
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/primitives/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:27.497902 runtimepy-4.3.3/runtimepy/primitives/array/
+-rw-r--r--   0 runner    (1001) docker     (127)     8239 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/primitives/array/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7715 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/primitives/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/primitives/bool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/primitives/byte_order.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:27.497902 runtimepy-4.3.3/runtimepy/primitives/field/
+-rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/primitives/field/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7481 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/primitives/field/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:27.497902 runtimepy-4.3.3/runtimepy/primitives/field/manager/
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/primitives/field/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6705 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/primitives/field/manager/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/primitives/float.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/primitives/int.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/primitives/scaling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:27.497902 runtimepy-4.3.3/runtimepy/primitives/serializable/
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/primitives/serializable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/primitives/serializable/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/primitives/serializable/fixed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/primitives/serializable/prefixed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/primitives/string.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:27.497902 runtimepy-4.3.3/runtimepy/primitives/types/
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/primitives/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/primitives/types/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/primitives/types/bool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/primitives/types/bounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/primitives/types/float.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/primitives/types/int.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:27.497902 runtimepy-4.3.3/runtimepy/registry/
+-rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/registry/bool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/registry/item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/registry/name.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:27.497902 runtimepy-4.3.3/runtimepy/sample/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/sample/peer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/sample/program.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:27.497902 runtimepy-4.3.3/runtimepy/struct/
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/struct/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:27.501901 runtimepy-4.3.3/runtimepy/subprocess/
+-rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/subprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7441 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/subprocess/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6335 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/subprocess/peer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6792 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/subprocess/program.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/subprocess/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:27.501901 runtimepy-4.3.3/runtimepy/task/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5947 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/task/asynchronous.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:27.501901 runtimepy-4.3.3/runtimepy/task/basic/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/task/basic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/task/basic/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6388 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/task/basic/periodic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/task/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:27.501901 runtimepy-4.3.3/runtimepy/task/trig/
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/task/trig/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:27.501901 runtimepy-4.3.3/runtimepy/telemetry/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/telemetry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:27.501901 runtimepy-4.3.3/runtimepy/tui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/tui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:27.501901 runtimepy-4.3.3/runtimepy/tui/channels/
+-rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/tui/channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/tui/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/tui/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/tui/mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/tui/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-04-26 15:56:56.000000 runtimepy-4.3.3/runtimepy/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:27.501901 runtimepy-4.3.3/runtimepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7055 2024-04-26 15:59:27.000000 runtimepy-4.3.3/runtimepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8039 2024-04-26 15:59:27.000000 runtimepy-4.3.3/runtimepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 15:59:27.000000 runtimepy-4.3.3/runtimepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-26 15:59:27.000000 runtimepy-4.3.3/runtimepy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-26 15:59:27.000000 runtimepy-4.3.3/runtimepy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-26 15:59:27.000000 runtimepy-4.3.3/runtimepy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 15:59:27.505902 runtimepy-4.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-26 15:56:56.000000 runtimepy-4.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:27.501901 runtimepy-4.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-26 15:56:56.000000 runtimepy-4.3.3/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-26 15:56:56.000000 runtimepy-4.3.3/tests/test_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-26 15:56:56.000000 runtimepy-4.3.3/tests/test_resources.py
```

### Comparing `runtimepy-4.3.2/LICENSE` & `runtimepy-4.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/PKG-INFO` & `runtimepy-4.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runtimepy
-Version: 4.3.2
+Version: 4.3.3
 Summary: A framework for implementing Python services.
 Home-page: https://github.com/vkottler/runtimepy
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -40,19 +40,19 @@
 Requires-Dist: types-setuptools; extra == "test"
 Requires-Dist: uvloop; (sys_platform != "win32" and sys_platform != "cygwin") and extra == "test"
 
 <!--
     =====================================
     generator=datazen
     version=3.1.4
-    hash=8ff56133d99744aa32cb4ab0d35d6e3b
+    hash=9bf8999fe73a97ce64d0a8d517418872
     =====================================
 -->
 
-# runtimepy ([4.3.2](https://pypi.org/project/runtimepy/))
+# runtimepy ([4.3.3](https://pypi.org/project/runtimepy/))
 
 [![python](https://img.shields.io/pypi/pyversions/runtimepy.svg)](https://pypi.org/project/runtimepy/)
 ![Build Status](https://github.com/vkottler/runtimepy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/runtimepy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/runtimepy)
 ![PyPI - Status](https://img.shields.io/pypi/status/runtimepy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/runtimepy)
```

### Comparing `runtimepy-4.3.2/README.md` & `runtimepy-4.3.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.4
-    hash=8ff56133d99744aa32cb4ab0d35d6e3b
+    hash=9bf8999fe73a97ce64d0a8d517418872
     =====================================
 -->
 
-# runtimepy ([4.3.2](https://pypi.org/project/runtimepy/))
+# runtimepy ([4.3.3](https://pypi.org/project/runtimepy/))
 
 [![python](https://img.shields.io/pypi/pyversions/runtimepy.svg)](https://pypi.org/project/runtimepy/)
 ![Build Status](https://github.com/vkottler/runtimepy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/runtimepy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/runtimepy)
 ![PyPI - Status](https://img.shields.io/pypi/status/runtimepy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/runtimepy)
```

### Comparing `runtimepy-4.3.2/pyproject.toml` & `runtimepy-4.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "runtimepy"
-version = "4.3.2"
+version = "4.3.3"
 description = "A framework for implementing Python services."
 readme = "README.md"
 requires-python = ">=3.11"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
```

### Comparing `runtimepy-4.3.2/runtimepy/app.py` & `runtimepy-4.3.3/runtimepy/app.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/channel/__init__.py` & `runtimepy-4.3.3/runtimepy/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/channel/environment/__init__.py` & `runtimepy-4.3.3/runtimepy/channel/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/channel/environment/array.py` & `runtimepy-4.3.3/runtimepy/channel/environment/array.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/channel/environment/base.py` & `runtimepy-4.3.3/runtimepy/channel/environment/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/channel/environment/command/__init__.py` & `runtimepy-4.3.3/runtimepy/channel/environment/command/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/channel/environment/command/parser.py` & `runtimepy-4.3.3/runtimepy/channel/environment/command/parser.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/channel/environment/command/processor.py` & `runtimepy-4.3.3/runtimepy/channel/environment/command/processor.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/channel/environment/command/result.py` & `runtimepy-4.3.3/runtimepy/channel/environment/command/result.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/channel/environment/create.py` & `runtimepy-4.3.3/runtimepy/channel/environment/create.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/channel/environment/file.py` & `runtimepy-4.3.3/runtimepy/channel/environment/file.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/channel/environment/sample.py` & `runtimepy-4.3.3/runtimepy/channel/environment/sample.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/channel/environment/telemetry.py` & `runtimepy-4.3.3/runtimepy/channel/environment/telemetry.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/channel/event/__init__.py` & `runtimepy-4.3.3/runtimepy/channel/event/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/channel/event/header.py` & `runtimepy-4.3.3/runtimepy/channel/event/header.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/channel/registry.py` & `runtimepy-4.3.3/runtimepy/channel/registry.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/codec/protocol/__init__.py` & `runtimepy-4.3.3/runtimepy/codec/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/codec/protocol/base.py` & `runtimepy-4.3.3/runtimepy/codec/protocol/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/codec/protocol/json.py` & `runtimepy-4.3.3/runtimepy/codec/protocol/json.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/codec/system/__init__.py` & `runtimepy-4.3.3/runtimepy/codec/system/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/commands/all.py` & `runtimepy-4.3.3/runtimepy/commands/all.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/commands/arbiter.py` & `runtimepy-4.3.3/runtimepy/commands/arbiter.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/commands/common.py` & `runtimepy-4.3.3/runtimepy/commands/common.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/commands/server.py` & `runtimepy-4.3.3/runtimepy/commands/server.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/commands/task.py` & `runtimepy-4.3.3/runtimepy/commands/task.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/commands/tui.py` & `runtimepy-4.3.3/runtimepy/commands/tui.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/data/css/bootstrap_extra.css` & `runtimepy-4.3.3/runtimepy/data/css/bootstrap_extra.css`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/data/dummy_load.yaml` & `runtimepy-4.3.3/runtimepy/data/dummy_load.yaml`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/data/factories.yaml` & `runtimepy-4.3.3/runtimepy/data/factories.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 # Connection factories.
 factories:
   # JSON messaging.
   - {name: runtimepy.net.factories.TcpJson}
   - {name: runtimepy.net.factories.UdpJson}
   - {name: runtimepy.net.factories.WebsocketJson}
 
+  # Queue wrappers.
+  - {name: runtimepy.net.factories.UdpQueue}
+
   # Echo and null connections (useful for testing and debugging).
   - {name: runtimepy.net.factories.TcpEcho, namespaces: [tcp, echo]}
   - {name: runtimepy.net.factories.UdpEcho, namespaces: [udp, echo]}
   - name: runtimepy.net.factories.WebsocketEcho
     namespaces: [websocket, echo]
   - {name: runtimepy.net.factories.TcpNull, namespaces: [tcp, "null"]}
   - {name: runtimepy.net.factories.UdpNull, namespaces: [udp, "null"]}
```

### Comparing `runtimepy-4.3.2/runtimepy/data/favicon.ico` & `runtimepy-4.3.3/runtimepy/data/favicon.ico`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/data/js/JsonConnection.js` & `runtimepy-4.3.3/runtimepy/data/js/JsonConnection.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/data/js/audio.js` & `runtimepy-4.3.3/runtimepy/data/js/audio.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/data/js/classes/App.js` & `runtimepy-4.3.3/runtimepy/data/js/classes/App.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/data/js/classes/ChannelTable.js` & `runtimepy-4.3.3/runtimepy/data/js/classes/ChannelTable.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/data/js/classes/JsonConnection.js` & `runtimepy-4.3.3/runtimepy/data/js/classes/JsonConnection.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/data/js/classes/Plot.js` & `runtimepy-4.3.3/runtimepy/data/js/classes/Plot.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/data/js/classes/PlotManager.js` & `runtimepy-4.3.3/runtimepy/data/js/classes/PlotManager.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/data/js/classes/PlotModalManager.js` & `runtimepy-4.3.3/runtimepy/data/js/classes/PlotModalManager.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/data/js/classes/TabFilter.js` & `runtimepy-4.3.3/runtimepy/data/js/classes/TabFilter.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/data/js/classes/TabInterface.js` & `runtimepy-4.3.3/runtimepy/data/js/classes/TabInterface.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/data/js/classes/WindowHashManager.js` & `runtimepy-4.3.3/runtimepy/data/js/classes/WindowHashManager.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/data/js/tab/sound.js` & `runtimepy-4.3.3/runtimepy/data/js/tab/sound.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/data/js/unused/pyodide.js` & `runtimepy-4.3.3/runtimepy/data/js/unused/pyodide.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/data/js/util.js` & `runtimepy-4.3.3/runtimepy/data/js/util.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/data/js/worker.js` & `runtimepy-4.3.3/runtimepy/data/js/worker.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/data/schemas/BitFields.yaml` & `runtimepy-4.3.3/runtimepy/data/schemas/BitFields.yaml`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/data/schemas/ConnectionArbiterConfig.yaml` & `runtimepy-4.3.3/runtimepy/data/schemas/ConnectionArbiterConfig.yaml`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/data/schemas/FindFile.yaml` & `runtimepy-4.3.3/runtimepy/data/schemas/FindFile.yaml`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/data/server_base.yaml` & `runtimepy-4.3.3/runtimepy/data/server_base.yaml`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/entry.py` & `runtimepy-4.3.3/runtimepy/entry.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/enum/__init__.py` & `runtimepy-4.3.3/runtimepy/enum/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/enum/registry.py` & `runtimepy-4.3.3/runtimepy/enum/registry.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/enum/types.py` & `runtimepy-4.3.3/runtimepy/enum/types.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/mapping.py` & `runtimepy-4.3.3/runtimepy/mapping.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/message/__init__.py` & `runtimepy-4.3.3/runtimepy/message/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/message/handlers.py` & `runtimepy-4.3.3/runtimepy/message/handlers.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/message/interface.py` & `runtimepy-4.3.3/runtimepy/message/interface.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/message/types.py` & `runtimepy-4.3.3/runtimepy/message/types.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/metrics/channel.py` & `runtimepy-4.3.3/runtimepy/metrics/channel.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/metrics/connection.py` & `runtimepy-4.3.3/runtimepy/metrics/connection.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/metrics/task.py` & `runtimepy-4.3.3/runtimepy/metrics/task.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/mixins/async_command.py` & `runtimepy-4.3.3/runtimepy/mixins/async_command.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/mixins/enum.py` & `runtimepy-4.3.3/runtimepy/mixins/enum.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/mixins/environment.py` & `runtimepy-4.3.3/runtimepy/mixins/environment.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/mixins/finalize.py` & `runtimepy-4.3.3/runtimepy/mixins/finalize.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/mixins/logging.py` & `runtimepy-4.3.3/runtimepy/mixins/logging.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/mixins/psutil.py` & `runtimepy-4.3.3/runtimepy/mixins/psutil.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/mixins/regex.py` & `runtimepy-4.3.3/runtimepy/mixins/regex.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/mixins/trig.py` & `runtimepy-4.3.3/runtimepy/mixins/trig.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/__init__.py` & `runtimepy-4.3.3/runtimepy/net/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/apps/__init__.py` & `runtimepy-4.3.3/runtimepy/net/apps/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/arbiter/__init__.py` & `runtimepy-4.3.3/runtimepy/net/arbiter/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/arbiter/base.py` & `runtimepy-4.3.3/runtimepy/net/arbiter/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/arbiter/config/__init__.py` & `runtimepy-4.3.3/runtimepy/net/arbiter/config/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/arbiter/config/codec.py` & `runtimepy-4.3.3/runtimepy/net/arbiter/config/codec.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/arbiter/config/util.py` & `runtimepy-4.3.3/runtimepy/net/arbiter/config/util.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/arbiter/factory/connection.py` & `runtimepy-4.3.3/runtimepy/net/arbiter/factory/connection.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/arbiter/factory/task.py` & `runtimepy-4.3.3/runtimepy/net/arbiter/factory/task.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/arbiter/housekeeping/__init__.py` & `runtimepy-4.3.3/runtimepy/net/arbiter/housekeeping/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/arbiter/imports/__init__.py` & `runtimepy-4.3.3/runtimepy/net/arbiter/imports/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/arbiter/imports/util.py` & `runtimepy-4.3.3/runtimepy/net/arbiter/imports/util.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/arbiter/info.py` & `runtimepy-4.3.3/runtimepy/net/arbiter/info.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/arbiter/result.py` & `runtimepy-4.3.3/runtimepy/net/arbiter/result.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/arbiter/task.py` & `runtimepy-4.3.3/runtimepy/net/arbiter/task.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/arbiter/tcp/__init__.py` & `runtimepy-4.3.3/runtimepy/net/arbiter/tcp/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/arbiter/tcp/json.py` & `runtimepy-4.3.3/runtimepy/net/arbiter/tcp/json.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/arbiter/udp.py` & `runtimepy-4.3.3/runtimepy/net/arbiter/udp.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/arbiter/websocket.py` & `runtimepy-4.3.3/runtimepy/net/arbiter/websocket.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/backoff.py` & `runtimepy-4.3.3/runtimepy/net/backoff.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/connection.py` & `runtimepy-4.3.3/runtimepy/net/connection.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/factories/__init__.py` & `runtimepy-4.3.3/runtimepy/net/factories/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     NullTcpConnection,
     TcpConnection,
 )
 from runtimepy.net.tcp.http import HttpConnection
 from runtimepy.net.udp import (
     EchoUdpConnection,
     NullUdpConnection,
+    QueueUdpConnection,
     UdpConnection,
 )
 from runtimepy.net.websocket import (
     EchoWebsocketConnection,
     NullWebsocketConnection,
     WebsocketConnection,
 )
@@ -89,14 +90,20 @@
 
 class UdpJson(UdpConnectionFactory[UdpJsonMessageConnection]):
     """UDP JSON-connection factory."""
 
     kind = UdpJsonMessageConnection
 
 
+class UdpQueue(UdpConnectionFactory[QueueUdpConnection]):
+    """UDP queue-connection factory."""
+
+    kind = QueueUdpConnection
+
+
 class TcpEcho(TcpConnectionFactory[EchoTcpConnection]):
     """TCP echo-connection factory."""
 
     kind = EchoTcpConnection
 
 
 class TcpMessage(TcpConnectionFactory[TcpPrefixedMessageConnection]):
```

### Comparing `runtimepy-4.3.2/runtimepy/net/http/__init__.py` & `runtimepy-4.3.3/runtimepy/net/http/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/http/common.py` & `runtimepy-4.3.3/runtimepy/net/http/common.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/http/header.py` & `runtimepy-4.3.3/runtimepy/net/http/header.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/http/request_target.py` & `runtimepy-4.3.3/runtimepy/net/http/request_target.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/http/response.py` & `runtimepy-4.3.3/runtimepy/net/http/response.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/http/state.py` & `runtimepy-4.3.3/runtimepy/net/http/state.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/http/version.py` & `runtimepy-4.3.3/runtimepy/net/http/version.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/manager.py` & `runtimepy-4.3.3/runtimepy/net/manager.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/mixin.py` & `runtimepy-4.3.3/runtimepy/net/mixin.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/server/__init__.py` & `runtimepy-4.3.3/runtimepy/net/server/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/server/app/__init__.py` & `runtimepy-4.3.3/runtimepy/net/server/app/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/server/app/base.py` & `runtimepy-4.3.3/runtimepy/net/server/app/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/server/app/bootstrap/__init__.py` & `runtimepy-4.3.3/runtimepy/net/server/app/bootstrap/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/server/app/bootstrap/elements.py` & `runtimepy-4.3.3/runtimepy/net/server/app/bootstrap/elements.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/server/app/bootstrap/tabs.py` & `runtimepy-4.3.3/runtimepy/net/server/app/bootstrap/tabs.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/server/app/create.py` & `runtimepy-4.3.3/runtimepy/net/server/app/create.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/server/app/env/__init__.py` & `runtimepy-4.3.3/runtimepy/net/server/app/env/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/server/app/env/modal.py` & `runtimepy-4.3.3/runtimepy/net/server/app/env/modal.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/server/app/env/tab/__init__.py` & `runtimepy-4.3.3/runtimepy/net/server/app/env/tab/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/server/app/env/tab/base.py` & `runtimepy-4.3.3/runtimepy/net/server/app/env/tab/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/server/app/env/tab/html.py` & `runtimepy-4.3.3/runtimepy/net/server/app/env/tab/html.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/server/app/env/tab/message.py` & `runtimepy-4.3.3/runtimepy/net/server/app/env/tab/message.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/server/app/env/widgets.py` & `runtimepy-4.3.3/runtimepy/net/server/app/env/widgets.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/server/app/files.py` & `runtimepy-4.3.3/runtimepy/net/server/app/files.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/server/app/placeholder.py` & `runtimepy-4.3.3/runtimepy/net/server/app/placeholder.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/server/app/sound.py` & `runtimepy-4.3.3/runtimepy/net/server/app/sound.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/server/app/tab.py` & `runtimepy-4.3.3/runtimepy/net/server/app/tab.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/server/html.py` & `runtimepy-4.3.3/runtimepy/net/server/html.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/server/json.py` & `runtimepy-4.3.3/runtimepy/net/server/json.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/server/struct/__init__.py` & `runtimepy-4.3.3/runtimepy/net/server/struct/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/server/websocket/__init__.py` & `runtimepy-4.3.3/runtimepy/net/server/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/server/websocket/state.py` & `runtimepy-4.3.3/runtimepy/net/server/websocket/state.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/stream/__init__.py` & `runtimepy-4.3.3/runtimepy/net/stream/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/stream/base.py` & `runtimepy-4.3.3/runtimepy/net/stream/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/stream/json/__init__.py` & `runtimepy-4.3.3/runtimepy/net/stream/json/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/stream/string.py` & `runtimepy-4.3.3/runtimepy/net/stream/string.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/tcp/connection.py` & `runtimepy-4.3.3/runtimepy/net/tcp/connection.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/tcp/create.py` & `runtimepy-4.3.3/runtimepy/net/tcp/create.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/tcp/http/__init__.py` & `runtimepy-4.3.3/runtimepy/net/tcp/http/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/tcp/protocol.py` & `runtimepy-4.3.3/runtimepy/net/tcp/protocol.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/tcp/telnet/__init__.py` & `runtimepy-4.3.3/runtimepy/net/tcp/telnet/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/tcp/telnet/codes.py` & `runtimepy-4.3.3/runtimepy/net/tcp/telnet/codes.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/udp/connection.py` & `runtimepy-4.3.3/runtimepy/net/udp/connection.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/udp/create.py` & `runtimepy-4.3.3/runtimepy/net/udp/create.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/udp/protocol.py` & `runtimepy-4.3.3/runtimepy/net/udp/protocol.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/util.py` & `runtimepy-4.3.3/runtimepy/net/util.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/net/websocket/connection.py` & `runtimepy-4.3.3/runtimepy/net/websocket/connection.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/primitives/__init__.py` & `runtimepy-4.3.3/runtimepy/primitives/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/primitives/array/__init__.py` & `runtimepy-4.3.3/runtimepy/primitives/array/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/primitives/base.py` & `runtimepy-4.3.3/runtimepy/primitives/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/primitives/bool.py` & `runtimepy-4.3.3/runtimepy/primitives/bool.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/primitives/byte_order.py` & `runtimepy-4.3.3/runtimepy/primitives/byte_order.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/primitives/field/__init__.py` & `runtimepy-4.3.3/runtimepy/primitives/field/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/primitives/field/fields.py` & `runtimepy-4.3.3/runtimepy/primitives/field/fields.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/primitives/field/manager/__init__.py` & `runtimepy-4.3.3/runtimepy/primitives/field/manager/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/primitives/field/manager/base.py` & `runtimepy-4.3.3/runtimepy/primitives/field/manager/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/primitives/float.py` & `runtimepy-4.3.3/runtimepy/primitives/float.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/primitives/int.py` & `runtimepy-4.3.3/runtimepy/primitives/int.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/primitives/scaling.py` & `runtimepy-4.3.3/runtimepy/primitives/scaling.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/primitives/serializable/base.py` & `runtimepy-4.3.3/runtimepy/primitives/serializable/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/primitives/serializable/fixed.py` & `runtimepy-4.3.3/runtimepy/primitives/serializable/fixed.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/primitives/serializable/prefixed.py` & `runtimepy-4.3.3/runtimepy/primitives/serializable/prefixed.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/primitives/string.py` & `runtimepy-4.3.3/runtimepy/primitives/string.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/primitives/types/__init__.py` & `runtimepy-4.3.3/runtimepy/primitives/types/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/primitives/types/base.py` & `runtimepy-4.3.3/runtimepy/primitives/types/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/primitives/types/bool.py` & `runtimepy-4.3.3/runtimepy/primitives/types/bool.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/primitives/types/bounds.py` & `runtimepy-4.3.3/runtimepy/primitives/types/bounds.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/primitives/types/float.py` & `runtimepy-4.3.3/runtimepy/primitives/types/float.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/primitives/types/int.py` & `runtimepy-4.3.3/runtimepy/primitives/types/int.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/registry/__init__.py` & `runtimepy-4.3.3/runtimepy/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/registry/bool.py` & `runtimepy-4.3.3/runtimepy/registry/bool.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/registry/item.py` & `runtimepy-4.3.3/runtimepy/registry/item.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/registry/name.py` & `runtimepy-4.3.3/runtimepy/registry/name.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/sample/peer.py` & `runtimepy-4.3.3/runtimepy/sample/peer.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/sample/program.py` & `runtimepy-4.3.3/runtimepy/sample/program.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/schemas.py` & `runtimepy-4.3.3/runtimepy/schemas.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/struct/__init__.py` & `runtimepy-4.3.3/runtimepy/struct/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/subprocess/__init__.py` & `runtimepy-4.3.3/runtimepy/subprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/subprocess/interface.py` & `runtimepy-4.3.3/runtimepy/subprocess/interface.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/subprocess/peer.py` & `runtimepy-4.3.3/runtimepy/subprocess/peer.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/subprocess/program.py` & `runtimepy-4.3.3/runtimepy/subprocess/program.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/subprocess/protocol.py` & `runtimepy-4.3.3/runtimepy/subprocess/protocol.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/task/asynchronous.py` & `runtimepy-4.3.3/runtimepy/task/asynchronous.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/task/basic/manager.py` & `runtimepy-4.3.3/runtimepy/task/basic/manager.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/task/basic/periodic.py` & `runtimepy-4.3.3/runtimepy/task/basic/periodic.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/task/sample.py` & `runtimepy-4.3.3/runtimepy/task/sample.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/task/trig/__init__.py` & `runtimepy-4.3.3/runtimepy/task/trig/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/tui/channels/__init__.py` & `runtimepy-4.3.3/runtimepy/tui/channels/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/tui/cursor.py` & `runtimepy-4.3.3/runtimepy/tui/cursor.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/tui/mixin.py` & `runtimepy-4.3.3/runtimepy/tui/mixin.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/tui/mock.py` & `runtimepy-4.3.3/runtimepy/tui/mock.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/tui/task.py` & `runtimepy-4.3.3/runtimepy/tui/task.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy/util.py` & `runtimepy-4.3.3/runtimepy/util.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/runtimepy.egg-info/PKG-INFO` & `runtimepy-4.3.3/runtimepy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runtimepy
-Version: 4.3.2
+Version: 4.3.3
 Summary: A framework for implementing Python services.
 Home-page: https://github.com/vkottler/runtimepy
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -40,19 +40,19 @@
 Requires-Dist: types-setuptools; extra == "test"
 Requires-Dist: uvloop; (sys_platform != "win32" and sys_platform != "cygwin") and extra == "test"
 
 <!--
     =====================================
     generator=datazen
     version=3.1.4
-    hash=8ff56133d99744aa32cb4ab0d35d6e3b
+    hash=9bf8999fe73a97ce64d0a8d517418872
     =====================================
 -->
 
-# runtimepy ([4.3.2](https://pypi.org/project/runtimepy/))
+# runtimepy ([4.3.3](https://pypi.org/project/runtimepy/))
 
 [![python](https://img.shields.io/pypi/pyversions/runtimepy.svg)](https://pypi.org/project/runtimepy/)
 ![Build Status](https://github.com/vkottler/runtimepy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/runtimepy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/runtimepy)
 ![PyPI - Status](https://img.shields.io/pypi/status/runtimepy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/runtimepy)
```

### Comparing `runtimepy-4.3.2/runtimepy.egg-info/SOURCES.txt` & `runtimepy-4.3.3/runtimepy.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -180,14 +180,15 @@
 runtimepy/net/tcp/http/__init__.py
 runtimepy/net/tcp/telnet/__init__.py
 runtimepy/net/tcp/telnet/codes.py
 runtimepy/net/udp/__init__.py
 runtimepy/net/udp/connection.py
 runtimepy/net/udp/create.py
 runtimepy/net/udp/protocol.py
+runtimepy/net/udp/queue.py
 runtimepy/net/websocket/__init__.py
 runtimepy/net/websocket/connection.py
 runtimepy/primitives/__init__.py
 runtimepy/primitives/base.py
 runtimepy/primitives/bool.py
 runtimepy/primitives/byte_order.py
 runtimepy/primitives/float.py
```

### Comparing `runtimepy-4.3.2/setup.py` & `runtimepy-4.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/tests/test_entry.py` & `runtimepy-4.3.3/tests/test_entry.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.3.2/tests/test_mapping.py` & `runtimepy-4.3.3/tests/test_mapping.py`

 * *Files identical despite different names*
