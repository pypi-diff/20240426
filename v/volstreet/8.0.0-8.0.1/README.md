# Comparing `tmp/volstreet-8.0.0.tar.gz` & `tmp/volstreet-8.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volstreet-8.0.0.tar", last modified: Tue Apr 23 09:02:18 2024, max compression
+gzip compressed data, was "volstreet-8.0.1.tar", last modified: Fri Apr 26 03:29:16 2024, max compression
```

## Comparing `volstreet-8.0.0.tar` & `volstreet-8.0.1.tar`

### file list

```diff
@@ -1,95 +1,97 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 09:02:18.075609 volstreet-8.0.0/
--rw-rw-rw-   0        0        0     1293 2024-04-23 09:02:18.075609 volstreet-8.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      124 2024-03-14 04:36:05.000000 volstreet-8.0.0/README.md
--rw-rw-rw-   0        0        0       91 2024-03-14 04:36:05.000000 volstreet-8.0.0/pyproject.toml
--rw-rw-rw-   0        0        0     1155 2024-04-23 09:02:18.075609 volstreet-8.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-23 09:02:17.981516 volstreet-8.0.0/volstreet/
--rw-rw-rw-   0        0        0      442 2024-03-14 09:55:16.000000 volstreet-8.0.0/volstreet/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 09:02:17.997100 volstreet-8.0.0/volstreet/angel_interface/
--rw-rw-rw-   0        0        0      247 2024-04-03 08:06:51.000000 volstreet-8.0.0/volstreet/angel_interface/__init__.py
--rw-rw-rw-   0        0        0     6878 2024-04-01 07:48:55.000000 volstreet-8.0.0/volstreet/angel_interface/access_rate_handlers.py
--rw-rw-rw-   0        0        0      274 2024-04-23 04:22:25.000000 volstreet-8.0.0/volstreet/angel_interface/active_session.py
--rw-rw-rw-   0        0        0     2713 2024-04-17 11:41:53.000000 volstreet-8.0.0/volstreet/angel_interface/async_interface.py
--rw-rw-rw-   0        0        0     7280 2024-03-14 04:36:05.000000 volstreet-8.0.0/volstreet/angel_interface/base_websocket.py
--rw-rw-rw-   0        0        0    18271 2024-04-23 04:22:25.000000 volstreet-8.0.0/volstreet/angel_interface/interface.py
--rw-rw-rw-   0        0        0     2501 2024-04-06 10:22:09.000000 volstreet-8.0.0/volstreet/angel_interface/login.py
--rw-rw-rw-   0        0        0     1988 2024-03-14 04:36:05.000000 volstreet-8.0.0/volstreet/angel_interface/order_websocket.py
--rw-rw-rw-   0        0        0    30663 2024-04-22 06:48:57.000000 volstreet-8.0.0/volstreet/angel_interface/price_websocket.py
--rw-rw-rw-   0        0        0     6661 2024-04-01 08:48:27.000000 volstreet-8.0.0/volstreet/angel_interface/smart_connect.py
-drwxrwxrwx   0        0        0        0 2024-04-23 09:02:18.013111 volstreet-8.0.0/volstreet/backtests/
--rw-rw-rw-   0        0        0      242 2024-04-23 04:22:25.000000 volstreet-8.0.0/volstreet/backtests/__init__.py
--rw-rw-rw-   0        0        0     4064 2024-04-23 04:22:25.000000 volstreet-8.0.0/volstreet/backtests/analysis.py
--rw-rw-rw-   0        0        0    11155 2024-03-14 04:36:05.000000 volstreet-8.0.0/volstreet/backtests/database.py
--rw-rw-rw-   0        0        0    38400 2024-04-03 08:06:51.000000 volstreet-8.0.0/volstreet/backtests/delta_hedging.py
--rw-rw-rw-   0        0        0     5695 2024-03-14 04:36:05.000000 volstreet-8.0.0/volstreet/backtests/delta_optimizer.py
--rw-rw-rw-   0        0        0    48672 2024-04-23 04:55:13.000000 volstreet-8.0.0/volstreet/backtests/framework.py
--rw-rw-rw-   0        0        0     5410 2024-04-13 06:57:57.000000 volstreet-8.0.0/volstreet/backtests/intraday_backtest_abc.py
--rw-rw-rw-   0        0        0     5071 2024-04-23 04:55:13.000000 volstreet-8.0.0/volstreet/backtests/proxy_functions.py
--rw-rw-rw-   0        0        0     7764 2024-04-23 08:59:42.000000 volstreet-8.0.0/volstreet/backtests/runner.py
--rw-rw-rw-   0        0        0     6446 2024-03-26 10:23:44.000000 volstreet-8.0.0/volstreet/backtests/tools.py
--rw-rw-rw-   0        0        0    15734 2024-04-13 06:57:57.000000 volstreet-8.0.0/volstreet/backtests/trend.py
--rw-rw-rw-   0        0        0     2479 2024-04-23 04:55:13.000000 volstreet-8.0.0/volstreet/backtests/underlying_info.py
--rw-rw-rw-   0        0        0    20854 2024-04-23 07:13:34.000000 volstreet-8.0.0/volstreet/blackscholes.py
--rw-rw-rw-   0        0        0     5574 2024-04-23 07:14:56.000000 volstreet-8.0.0/volstreet/config.py
--rw-rw-rw-   0        0        0     2162 2024-03-14 04:36:05.000000 volstreet-8.0.0/volstreet/database_connection.py
-drwxrwxrwx   0        0        0        0 2024-04-23 09:02:18.028745 volstreet-8.0.0/volstreet/datamodule/
--rw-rw-rw-   0        0        0      163 2024-04-13 05:46:57.000000 volstreet-8.0.0/volstreet/datamodule/__init__.py
--rw-rw-rw-   0        0        0     7358 2024-03-14 04:36:05.000000 volstreet-8.0.0/volstreet/datamodule/analysis.py
--rw-rw-rw-   0        0        0    21130 2024-03-14 04:36:05.000000 volstreet-8.0.0/volstreet/datamodule/archive.py
--rw-rw-rw-   0        0        0     8882 2024-04-13 05:28:03.000000 volstreet-8.0.0/volstreet/datamodule/data_handling.py
--rw-rw-rw-   0        0        0     4534 2024-03-14 04:36:05.000000 volstreet-8.0.0/volstreet/datamodule/eod_client.py
--rw-rw-rw-   0        0        0     5639 2024-03-14 04:36:05.000000 volstreet-8.0.0/volstreet/datamodule/gambling.py
--rw-rw-rw-   0        0        0     8098 2024-03-14 04:36:05.000000 volstreet-8.0.0/volstreet/datamodule/intraday_data.py
--rw-rw-rw-   0        0        0    15754 2024-03-26 10:23:44.000000 volstreet-8.0.0/volstreet/datamodule/stockmock.py
--rw-rw-rw-   0        0        0     1219 2024-03-14 04:36:05.000000 volstreet-8.0.0/volstreet/datamodule/trading_assistance.py
--rw-rw-rw-   0        0        0    27286 2024-03-26 10:23:44.000000 volstreet-8.0.0/volstreet/dealingroom.py
--rw-rw-rw-   0        0        0     2573 2024-04-03 08:06:51.000000 volstreet-8.0.0/volstreet/decorators.py
--rw-rw-rw-   0        0        0     1683 2024-03-14 04:36:05.000000 volstreet-8.0.0/volstreet/discord_bot.py
--rw-rw-rw-   0        0        0     1698 2024-03-14 04:36:05.000000 volstreet-8.0.0/volstreet/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-04-23 09:02:18.028745 volstreet-8.0.0/volstreet/historical_info/
--rw-rw-rw-   0        0        0      975 2024-04-23 04:55:13.000000 volstreet-8.0.0/volstreet/historical_info/__init__.py
--rw-rw-rw-   0        0        0    18590 2024-04-23 04:22:25.000000 volstreet-8.0.0/volstreet/historical_info/index_expiries.pkl
--rw-rw-rw-   0        0        0    16793 2024-04-23 04:22:25.000000 volstreet-8.0.0/volstreet/historical_info/market_days.pkl
-drwxrwxrwx   0        0        0        0 2024-04-23 09:02:18.044367 volstreet-8.0.0/volstreet/models/
--rw-rw-rw-   0        0        0      565 2024-04-23 07:16:41.000000 volstreet-8.0.0/volstreet/models/__init__.py
--rw-rw-rw-   0        0        0      772 2024-03-14 04:36:05.000000 volstreet-8.0.0/volstreet/parallelization.py
--rw-rw-rw-   0        0        0     1659 2024-04-06 06:31:33.000000 volstreet-8.0.0/volstreet/performance_tracking.py
-drwxrwxrwx   0        0        0        0 2024-04-23 09:02:18.044367 volstreet-8.0.0/volstreet/position_dashboard/
--rw-rw-rw-   0        0        0        0 2024-04-17 11:41:53.000000 volstreet-8.0.0/volstreet/position_dashboard/__init__.py
--rw-rw-rw-   0        0        0     1972 2024-04-17 11:41:53.000000 volstreet-8.0.0/volstreet/position_dashboard/app.py
--rw-rw-rw-   0        0        0      572 2024-04-17 11:41:53.000000 volstreet-8.0.0/volstreet/position_dashboard/formatting.py
-drwxrwxrwx   0        0        0        0 2024-04-23 09:02:18.059986 volstreet-8.0.0/volstreet/strategies/
--rw-rw-rw-   0        0        0      156 2024-04-17 11:41:53.000000 volstreet-8.0.0/volstreet/strategies/__init__.py
--rw-rw-rw-   0        0        0    29068 2024-04-17 11:41:53.000000 volstreet-8.0.0/volstreet/strategies/deployment.py
--rw-rw-rw-   0        0        0     5194 2024-04-17 11:41:53.000000 volstreet-8.0.0/volstreet/strategies/error_handling.py
--rw-rw-rw-   0        0        0    56703 2024-04-23 04:22:25.000000 volstreet-8.0.0/volstreet/strategies/helpers.py
--rw-rw-rw-   0        0        0     2949 2024-04-17 11:41:53.000000 volstreet-8.0.0/volstreet/strategies/monitoring.py
--rw-rw-rw-   0        0        0    17179 2024-04-10 07:52:35.000000 volstreet-8.0.0/volstreet/strategies/optimization.py
--rw-rw-rw-   0        0        0    91543 2024-04-23 04:22:25.000000 volstreet-8.0.0/volstreet/strategies/strats.py
--rw-rw-rw-   0        0        0      349 2024-04-12 11:13:05.000000 volstreet-8.0.0/volstreet/strategies/tools.py
-drwxrwxrwx   0        0        0        0 2024-04-23 09:02:18.059986 volstreet-8.0.0/volstreet/trade_interface/
--rw-rw-rw-   0        0        0      224 2024-04-17 11:41:53.000000 volstreet-8.0.0/volstreet/trade_interface/__init__.py
--rw-rw-rw-   0        0        0    26799 2024-04-23 04:22:25.000000 volstreet-8.0.0/volstreet/trade_interface/instruments.py
--rw-rw-rw-   0        0        0    19700 2024-04-22 06:48:57.000000 volstreet-8.0.0/volstreet/trade_interface/order_execution.py
--rw-rw-rw-   0        0        0    20198 2024-04-23 04:22:25.000000 volstreet-8.0.0/volstreet/trade_interface/underlyings.py
-drwxrwxrwx   0        0        0        0 2024-04-23 09:02:18.075609 volstreet-8.0.0/volstreet/utils/
--rw-rw-rw-   0        0        0      138 2024-03-14 04:36:05.000000 volstreet-8.0.0/volstreet/utils/__init__.py
--rw-rw-rw-   0        0        0      757 2024-03-14 04:36:05.000000 volstreet-8.0.0/volstreet/utils/change_config.py
--rw-rw-rw-   0        0        0     3052 2024-04-09 12:38:37.000000 volstreet-8.0.0/volstreet/utils/communication.py
--rw-rw-rw-   0        0        0    13115 2024-04-23 04:22:25.000000 volstreet-8.0.0/volstreet/utils/core.py
--rw-rw-rw-   0        0        0     4419 2024-03-14 04:36:05.000000 volstreet-8.0.0/volstreet/utils/data_io.py
--rw-rw-rw-   0        0        0     9779 2024-03-14 04:36:05.000000 volstreet-8.0.0/volstreet/utils/scrip_processing.py
--rw-rw-rw-   0        0        0     6488 2024-04-23 04:22:25.000000 volstreet-8.0.0/volstreet/vectorized_blackscholes.py
--rw-rw-rw-   0        0        0       20 2024-04-23 08:08:36.000000 volstreet-8.0.0/volstreet/volstreet_mode.json
-drwxrwxrwx   0        0        0        0 2024-04-23 09:02:18.075609 volstreet-8.0.0/volstreet/vslogging/
--rw-rw-rw-   0        0        0       81 2024-03-15 09:40:04.000000 volstreet-8.0.0/volstreet/vslogging/__init__.py
--rw-rw-rw-   0        0        0     2023 2024-03-26 10:23:44.000000 volstreet-8.0.0/volstreet/vslogging/formatters.py
--rw-rw-rw-   0        0        0     1492 2024-03-27 04:16:21.000000 volstreet-8.0.0/volstreet/vslogging/logging_config.json
--rw-rw-rw-   0        0        0      842 2024-03-26 10:23:44.000000 volstreet-8.0.0/volstreet/vslogging/logging_setup.py
--rw-rw-rw-   0        0        0     1390 2024-04-17 11:41:53.000000 volstreet-8.0.0/volstreet/vslogging/parsing.py
-drwxrwxrwx   0        0        0        0 2024-04-23 09:02:18.075609 volstreet-8.0.0/volstreet.egg-info/
--rw-rw-rw-   0        0        0     1293 2024-04-23 09:02:17.000000 volstreet-8.0.0/volstreet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2756 2024-04-23 09:02:17.000000 volstreet-8.0.0/volstreet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 09:02:17.000000 volstreet-8.0.0/volstreet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      460 2024-04-23 09:02:17.000000 volstreet-8.0.0/volstreet.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-23 09:02:17.000000 volstreet-8.0.0/volstreet.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-26 03:29:16.495072 volstreet-8.0.1/
+-rw-rw-rw-   0        0        0     1293 2024-04-26 03:29:16.494549 volstreet-8.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      124 2024-03-14 04:36:05.000000 volstreet-8.0.1/README.md
+-rw-rw-rw-   0        0        0       91 2024-03-14 04:36:05.000000 volstreet-8.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0     1155 2024-04-26 03:29:16.496603 volstreet-8.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-26 03:29:16.376282 volstreet-8.0.1/volstreet/
+-rw-rw-rw-   0        0        0      442 2024-03-14 09:55:16.000000 volstreet-8.0.1/volstreet/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 03:29:16.396590 volstreet-8.0.1/volstreet/angel_interface/
+-rw-rw-rw-   0        0        0      247 2024-04-26 02:47:59.000000 volstreet-8.0.1/volstreet/angel_interface/__init__.py
+-rw-rw-rw-   0        0        0     3726 2024-04-26 02:48:50.000000 volstreet-8.0.1/volstreet/angel_interface/access_rate_handler.py
+-rw-rw-rw-   0        0        0      274 2024-04-23 04:22:25.000000 volstreet-8.0.1/volstreet/angel_interface/active_session.py
+-rw-rw-rw-   0        0        0     2713 2024-04-17 11:41:53.000000 volstreet-8.0.1/volstreet/angel_interface/async_interface.py
+-rw-rw-rw-   0        0        0     7280 2024-03-14 04:36:05.000000 volstreet-8.0.1/volstreet/angel_interface/base_websocket.py
+-rw-rw-rw-   0        0        0    18658 2024-04-26 03:17:20.000000 volstreet-8.0.1/volstreet/angel_interface/interface.py
+-rw-rw-rw-   0        0        0     2501 2024-04-06 10:22:09.000000 volstreet-8.0.1/volstreet/angel_interface/login.py
+-rw-rw-rw-   0        0        0     1988 2024-03-14 04:36:05.000000 volstreet-8.0.1/volstreet/angel_interface/order_websocket.py
+-rw-rw-rw-   0        0        0    30663 2024-04-22 06:48:57.000000 volstreet-8.0.1/volstreet/angel_interface/price_websocket.py
+-rw-rw-rw-   0        0        0     6687 2024-04-26 02:56:08.000000 volstreet-8.0.1/volstreet/angel_interface/smart_connect.py
+drwxrwxrwx   0        0        0        0 2024-04-26 03:29:16.421529 volstreet-8.0.1/volstreet/backtests/
+-rw-rw-rw-   0        0        0      267 2024-04-24 06:53:53.000000 volstreet-8.0.1/volstreet/backtests/__init__.py
+-rw-rw-rw-   0        0        0     4064 2024-04-23 04:22:25.000000 volstreet-8.0.1/volstreet/backtests/analysis.py
+-rw-rw-rw-   0        0        0     3296 2024-04-25 15:14:45.000000 volstreet-8.0.1/volstreet/backtests/data_updation.py
+-rw-rw-rw-   0        0        0    11857 2024-04-25 10:13:39.000000 volstreet-8.0.1/volstreet/backtests/database.py
+-rw-rw-rw-   0        0        0    38400 2024-04-03 08:06:51.000000 volstreet-8.0.1/volstreet/backtests/delta_hedging.py
+-rw-rw-rw-   0        0        0     5695 2024-03-14 04:36:05.000000 volstreet-8.0.1/volstreet/backtests/delta_optimizer.py
+-rw-rw-rw-   0        0        0    48672 2024-04-24 06:53:53.000000 volstreet-8.0.1/volstreet/backtests/framework.py
+-rw-rw-rw-   0        0        0     5410 2024-04-13 06:57:57.000000 volstreet-8.0.1/volstreet/backtests/intraday_backtest_abc.py
+-rw-rw-rw-   0        0        0     6059 2024-04-25 10:23:36.000000 volstreet-8.0.1/volstreet/backtests/proxy_functions.py
+-rw-rw-rw-   0        0        0     2707 2024-04-24 14:17:18.000000 volstreet-8.0.1/volstreet/backtests/result_processing.py
+-rw-rw-rw-   0        0        0     6075 2024-04-25 10:19:27.000000 volstreet-8.0.1/volstreet/backtests/runner.py
+-rw-rw-rw-   0        0        0     6446 2024-03-26 10:23:44.000000 volstreet-8.0.1/volstreet/backtests/tools.py
+-rw-rw-rw-   0        0        0    15734 2024-04-13 06:57:57.000000 volstreet-8.0.1/volstreet/backtests/trend.py
+-rw-rw-rw-   0        0        0     1689 2024-04-25 14:52:32.000000 volstreet-8.0.1/volstreet/backtests/underlying_info.py
+-rw-rw-rw-   0        0        0    20854 2024-04-24 06:53:53.000000 volstreet-8.0.1/volstreet/blackscholes.py
+-rw-rw-rw-   0        0        0     5574 2024-04-24 06:53:53.000000 volstreet-8.0.1/volstreet/config.py
+-rw-rw-rw-   0        0        0     2162 2024-03-14 04:36:05.000000 volstreet-8.0.1/volstreet/database_connection.py
+drwxrwxrwx   0        0        0        0 2024-04-26 03:29:16.437362 volstreet-8.0.1/volstreet/datamodule/
+-rw-rw-rw-   0        0        0      163 2024-04-13 05:46:57.000000 volstreet-8.0.1/volstreet/datamodule/__init__.py
+-rw-rw-rw-   0        0        0     7358 2024-03-14 04:36:05.000000 volstreet-8.0.1/volstreet/datamodule/analysis.py
+-rw-rw-rw-   0        0        0    21130 2024-03-14 04:36:05.000000 volstreet-8.0.1/volstreet/datamodule/archive.py
+-rw-rw-rw-   0        0        0     8882 2024-04-13 05:28:03.000000 volstreet-8.0.1/volstreet/datamodule/data_handling.py
+-rw-rw-rw-   0        0        0     4534 2024-03-14 04:36:05.000000 volstreet-8.0.1/volstreet/datamodule/eod_client.py
+-rw-rw-rw-   0        0        0     5639 2024-03-14 04:36:05.000000 volstreet-8.0.1/volstreet/datamodule/gambling.py
+-rw-rw-rw-   0        0        0     8098 2024-03-14 04:36:05.000000 volstreet-8.0.1/volstreet/datamodule/intraday_data.py
+-rw-rw-rw-   0        0        0    15754 2024-03-26 10:23:44.000000 volstreet-8.0.1/volstreet/datamodule/stockmock.py
+-rw-rw-rw-   0        0        0     1219 2024-03-14 04:36:05.000000 volstreet-8.0.1/volstreet/datamodule/trading_assistance.py
+-rw-rw-rw-   0        0        0    27286 2024-03-26 10:23:44.000000 volstreet-8.0.1/volstreet/dealingroom.py
+-rw-rw-rw-   0        0        0     2573 2024-04-03 08:06:51.000000 volstreet-8.0.1/volstreet/decorators.py
+-rw-rw-rw-   0        0        0     1683 2024-03-14 04:36:05.000000 volstreet-8.0.1/volstreet/discord_bot.py
+-rw-rw-rw-   0        0        0     1698 2024-03-14 04:36:05.000000 volstreet-8.0.1/volstreet/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-26 03:29:16.437362 volstreet-8.0.1/volstreet/historical_info/
+-rw-rw-rw-   0        0        0      975 2024-04-24 06:53:53.000000 volstreet-8.0.1/volstreet/historical_info/__init__.py
+-rw-rw-rw-   0        0        0    18590 2024-04-23 04:22:25.000000 volstreet-8.0.1/volstreet/historical_info/index_expiries.pkl
+-rw-rw-rw-   0        0        0    16832 2024-04-25 14:56:47.000000 volstreet-8.0.1/volstreet/historical_info/market_days.pkl
+drwxrwxrwx   0        0        0        0 2024-04-26 03:29:16.437362 volstreet-8.0.1/volstreet/models/
+-rw-rw-rw-   0        0        0      565 2024-04-24 06:53:53.000000 volstreet-8.0.1/volstreet/models/__init__.py
+-rw-rw-rw-   0        0        0      772 2024-03-14 04:36:05.000000 volstreet-8.0.1/volstreet/parallelization.py
+-rw-rw-rw-   0        0        0     1659 2024-04-06 06:31:33.000000 volstreet-8.0.1/volstreet/performance_tracking.py
+drwxrwxrwx   0        0        0        0 2024-04-26 03:29:16.446448 volstreet-8.0.1/volstreet/position_dashboard/
+-rw-rw-rw-   0        0        0        0 2024-04-17 11:41:53.000000 volstreet-8.0.1/volstreet/position_dashboard/__init__.py
+-rw-rw-rw-   0        0        0     1972 2024-04-17 11:41:53.000000 volstreet-8.0.1/volstreet/position_dashboard/app.py
+-rw-rw-rw-   0        0        0      572 2024-04-17 11:41:53.000000 volstreet-8.0.1/volstreet/position_dashboard/formatting.py
+drwxrwxrwx   0        0        0        0 2024-04-26 03:29:16.457555 volstreet-8.0.1/volstreet/strategies/
+-rw-rw-rw-   0        0        0      156 2024-04-17 11:41:53.000000 volstreet-8.0.1/volstreet/strategies/__init__.py
+-rw-rw-rw-   0        0        0    28950 2024-04-26 03:19:34.000000 volstreet-8.0.1/volstreet/strategies/deployment.py
+-rw-rw-rw-   0        0        0     5194 2024-04-17 11:41:53.000000 volstreet-8.0.1/volstreet/strategies/error_handling.py
+-rw-rw-rw-   0        0        0    56703 2024-04-23 04:22:25.000000 volstreet-8.0.1/volstreet/strategies/helpers.py
+-rw-rw-rw-   0        0        0     2949 2024-04-17 11:41:53.000000 volstreet-8.0.1/volstreet/strategies/monitoring.py
+-rw-rw-rw-   0        0        0    17179 2024-04-10 07:52:35.000000 volstreet-8.0.1/volstreet/strategies/optimization.py
+-rw-rw-rw-   0        0        0    91543 2024-04-23 04:22:25.000000 volstreet-8.0.1/volstreet/strategies/strats.py
+-rw-rw-rw-   0        0        0      349 2024-04-12 11:13:05.000000 volstreet-8.0.1/volstreet/strategies/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-26 03:29:16.457555 volstreet-8.0.1/volstreet/trade_interface/
+-rw-rw-rw-   0        0        0      224 2024-04-17 11:41:53.000000 volstreet-8.0.1/volstreet/trade_interface/__init__.py
+-rw-rw-rw-   0        0        0    26799 2024-04-23 04:22:25.000000 volstreet-8.0.1/volstreet/trade_interface/instruments.py
+-rw-rw-rw-   0        0        0    19327 2024-04-26 03:27:47.000000 volstreet-8.0.1/volstreet/trade_interface/order_execution.py
+-rw-rw-rw-   0        0        0    20198 2024-04-23 04:22:25.000000 volstreet-8.0.1/volstreet/trade_interface/underlyings.py
+drwxrwxrwx   0        0        0        0 2024-04-26 03:29:16.476149 volstreet-8.0.1/volstreet/utils/
+-rw-rw-rw-   0        0        0      138 2024-03-14 04:36:05.000000 volstreet-8.0.1/volstreet/utils/__init__.py
+-rw-rw-rw-   0        0        0      757 2024-03-14 04:36:05.000000 volstreet-8.0.1/volstreet/utils/change_config.py
+-rw-rw-rw-   0        0        0     3052 2024-04-09 12:38:37.000000 volstreet-8.0.1/volstreet/utils/communication.py
+-rw-rw-rw-   0        0        0    13115 2024-04-23 04:22:25.000000 volstreet-8.0.1/volstreet/utils/core.py
+-rw-rw-rw-   0        0        0     4419 2024-03-14 04:36:05.000000 volstreet-8.0.1/volstreet/utils/data_io.py
+-rw-rw-rw-   0        0        0     9779 2024-03-14 04:36:05.000000 volstreet-8.0.1/volstreet/utils/scrip_processing.py
+-rw-rw-rw-   0        0        0     6488 2024-04-23 04:22:25.000000 volstreet-8.0.1/volstreet/vectorized_blackscholes.py
+-rw-rw-rw-   0        0        0       16 2024-04-26 02:35:35.000000 volstreet-8.0.1/volstreet/volstreet_mode.json
+drwxrwxrwx   0        0        0        0 2024-04-26 03:29:16.488903 volstreet-8.0.1/volstreet/vslogging/
+-rw-rw-rw-   0        0        0       81 2024-03-15 09:40:04.000000 volstreet-8.0.1/volstreet/vslogging/__init__.py
+-rw-rw-rw-   0        0        0     2023 2024-03-26 10:23:44.000000 volstreet-8.0.1/volstreet/vslogging/formatters.py
+-rw-rw-rw-   0        0        0     1492 2024-03-27 04:16:21.000000 volstreet-8.0.1/volstreet/vslogging/logging_config.json
+-rw-rw-rw-   0        0        0      842 2024-03-26 10:23:44.000000 volstreet-8.0.1/volstreet/vslogging/logging_setup.py
+-rw-rw-rw-   0        0        0     1390 2024-04-17 11:41:53.000000 volstreet-8.0.1/volstreet/vslogging/parsing.py
+drwxrwxrwx   0        0        0        0 2024-04-26 03:29:16.488903 volstreet-8.0.1/volstreet.egg-info/
+-rw-rw-rw-   0        0        0     1293 2024-04-26 03:29:16.000000 volstreet-8.0.1/volstreet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2833 2024-04-26 03:29:16.000000 volstreet-8.0.1/volstreet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 03:29:16.000000 volstreet-8.0.1/volstreet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      460 2024-04-26 03:29:16.000000 volstreet-8.0.1/volstreet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-26 03:29:16.000000 volstreet-8.0.1/volstreet.egg-info/top_level.txt
```

### Comparing `volstreet-8.0.0/PKG-INFO` & `volstreet-8.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volstreet
-Version: 8.0.0
+Version: 8.0.1
 Summary: VolStreet is a Python library for automated trading
 Home-page: https://github.com/rahulthakkr/volstreet
 Author: Rahul Thakkar
 Author-email: r.thakkar15@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `volstreet-8.0.0/setup.cfg` & `volstreet-8.0.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6f6c 7374 7265 6574 0d0a 7665   = volstreet..ve
-00000020: 7273 696f 6e20 3d20 382e 302e 300d 0a61  rsion = 8.0.0..a
+00000020: 7273 696f 6e20 3d20 382e 302e 310d 0a61  rsion = 8.0.1..a
 00000030: 7574 686f 7220 3d20 5261 6875 6c20 5468  uthor = Rahul Th
 00000040: 616b 6b61 720d 0a61 7574 686f 725f 656d  akkar..author_em
 00000050: 6169 6c20 3d20 722e 7468 616b 6b61 7231  ail = r.thakkar1
 00000060: 3540 676d 6169 6c2e 636f 6d0d 0a64 6573  5@gmail.com..des
 00000070: 6372 6970 7469 6f6e 203d 2056 6f6c 5374  cription = VolSt
 00000080: 7265 6574 2069 7320 6120 5079 7468 6f6e  reet is a Python
 00000090: 206c 6962 7261 7279 2066 6f72 2061 7574   library for aut
```

### Comparing `volstreet-8.0.0/volstreet/angel_interface/async_interface.py` & `volstreet-8.0.1/volstreet/angel_interface/async_interface.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.0/volstreet/angel_interface/base_websocket.py` & `volstreet-8.0.1/volstreet/angel_interface/base_websocket.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.0/volstreet/angel_interface/interface.py` & `volstreet-8.0.1/volstreet/angel_interface/interface.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,19 +11,39 @@
 from volstreet import config
 from volstreet.config import logger, token_exchange_dict, thread_local
 from volstreet.decorators import (
     classproperty,
     timeit,
 )
 from volstreet.utils import current_time, custom_round
-from volstreet.angel_interface.access_rate_handlers import access_rate_handler
 from volstreet.angel_interface.active_session import ActiveSession
 from volstreet.angel_interface.login import wait_for_login
 from volstreet.angel_interface.order_websocket import OrderWebsocket
 from volstreet.angel_interface.price_websocket import PriceWebsocket
+from volstreet.angel_interface.access_rate_handler import (
+    access_rate_handler,
+    limiter_1,
+    limiter_10,
+    limiter_20,
+)
+
+
+order_param_fields = [
+    "tradingsymbol",
+    "symboltoken",
+    "transactiontype",
+    "variety",
+    "exchange",
+    "producttype",
+    "duration",
+    "quantity",
+    "ordertag",
+    "ordertype",
+    "price",
+]
 
 
 class LiveFeeds:
     price_feed: PriceWebsocket = None
     order_feed: OrderWebsocket = None
     price_feed_process = None
     order_feed_process = None
@@ -75,21 +95,14 @@
         of = OrderWebsocket.from_active_session(manager, **kwargs)
         process = Process(target=of.connect)
         cls.order_feed_process = process
         cls.order_feed = of
         process.start()
 
 
-if config.backtest_mode:
-    logger.info(
-        f"Importing proxy functions in module: {__name__} since backtesting is enabled."
-    )
-    from volstreet.backtests.proxy_functions import ProxyFeeds as LiveFeeds
-
-
 def retry_angel_api(
     data_type: str | Callable = None,
     max_attempts: int = 10,
     wait_increase_factor: float = 1.1,
 ):
     def handle_retry_logic(
         function: str,
@@ -167,14 +180,22 @@
                     sleep(sleep_duration)
 
         return wrapper
 
     return decorator
 
 
+if config.backtest_mode:
+    logger.info(
+        f"Importing proxy functions in module: {__name__} since backtesting is enabled."
+    )
+    from volstreet.backtests.proxy_functions import ProxyFeeds as LiveFeeds
+    from volstreet.backtests.proxy_functions import retry_angel_api, access_rate_handler
+
+
 def increase_robustness(func):
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
         thread_local.robust_handling = True
         try:
             return func(*args, **kwargs)
         finally:
@@ -263,15 +284,15 @@
     current_params["price"] = new_price
     modified_params.pop("status")
 
     return modified_params
 
 
 @retry_angel_api(data_type=lambda x: x)
-@access_rate_handler(max_requests=20, per_seconds=1.2)
+@access_rate_handler(limiter_20, "place_order", False)
 @timeit()
 def _place_order_params(params: dict) -> str:
     return ActiveSession.obj.placeOrder(params)
 
 
 def place_order(
     symbol: str,
@@ -285,22 +306,22 @@
     params = generate_order_params(
         symbol, token, qty, action, price, order_tag, stop_loss_order
     )
     return _place_order_params(params)
 
 
 @retry_angel_api(data_type=lambda x: None)
-@access_rate_handler(max_requests=20, per_seconds=1.2)
+@access_rate_handler(limiter_20, "modify_order", False)
 @timeit()
 def modify_order(params: dict) -> None:
     return ActiveSession.obj.modifyOrder(params)
 
 
 @retry_angel_api(data_type=lambda x: x["data"]["fetched"])
-@access_rate_handler(max_requests=10, per_seconds=1.2)
+@access_rate_handler(limiter_10, "get_quotes", False)
 @timeit()
 def _fetch_quotes(tokens: list, mode: str = "FULL"):
     assert len(tokens) <= 50, "Maximum 50 tokens can be fetched at once for now."
     payload = defaultdict(list)
     for token in tokens:
         exchange = token_exchange_dict.get(token)
         if exchange:
@@ -348,15 +369,15 @@
     elif structure.lower() == "list":
         return quote_data
     else:
         raise ValueError(f"Invalid structure '{structure}'.")
 
 
 @retry_angel_api(data_type="ltp")
-@access_rate_handler(max_requests=10, per_seconds=1.2)
+@access_rate_handler(limiter_10, "get_ltp", False)
 @timeit()
 def _fetch_ltp(exchange_seg, symbol, token):
     price_data = ActiveSession.obj.ltpData(exchange_seg, symbol, token)
     return price_data
 
 
 def fetch_ltp(exchange_seg, symbol, token, field="ltp"):
@@ -367,15 +388,15 @@
         price = LiveFeeds.price_feed.data_bank[token][field]
     else:
         price = _fetch_ltp(exchange_seg, symbol, token)
     return price
 
 
 @retry_angel_api(max_attempts=10)
-@access_rate_handler(max_requests=1, per_seconds=1.05)
+@access_rate_handler(limiter_1, "get_orderbook", False)
 @timeit()
 def _fetch_book(fetch_func):
     data = fetch_func()
     return data
 
 
 def fetch_book(book: str, from_api: bool = False) -> list:
@@ -498,15 +519,15 @@
         return filter_and_return(book_data)
     else:
         logger.error(f"Invalid book type '{book}'.")
         raise ValueError("Invalid book type.")
 
 
 @retry_angel_api()
-@access_rate_handler(max_requests=3, per_seconds=1.05)
+@access_rate_handler(limiter_1, "get_historical_data", False)
 def fetch_historical_prices(
     token: str, interval: str, from_date: datetime, to_date: datetime
 ):
     from_date = pd.to_datetime(from_date) if isinstance(from_date, str) else from_date
     to_date = pd.to_datetime(to_date) if isinstance(to_date, str) else to_date
     exchange = token_exchange_dict[token]
     historic_param = {
```

### Comparing `volstreet-8.0.0/volstreet/angel_interface/login.py` & `volstreet-8.0.1/volstreet/angel_interface/login.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.0/volstreet/angel_interface/order_websocket.py` & `volstreet-8.0.1/volstreet/angel_interface/order_websocket.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.0/volstreet/angel_interface/price_websocket.py` & `volstreet-8.0.1/volstreet/angel_interface/price_websocket.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.0/volstreet/angel_interface/smart_connect.py` & `volstreet-8.0.1/volstreet/angel_interface/smart_connect.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 import aiohttp
 import json
 import functools
 from SmartApi.smartConnect import SmartConnect, urljoin
 from volstreet.config import logger
-from volstreet.angel_interface.access_rate_handlers import access_rate_handler
+from volstreet.angel_interface.access_rate_handler import (
+    access_rate_handler,
+    limiter_10,
+    limiter_20,
+)
 
 
 def log_request(func):
     """Only for async functions. Logs the request and response of the function."""
 
     @functools.wraps(func)
     async def async_wrapped(smart_connect, *args, **kwargs):
@@ -112,27 +116,27 @@
             user["data"]["jwtToken"] = "Bearer " + self.access_token
             user["data"]["refreshToken"] = self.refresh_token
             user["data"]["feedToken"] = self.feed_token
             return user
         else:
             return login_result
 
-    @access_rate_handler(max_requests=9, per_seconds=1, is_async=True)
+    @access_rate_handler(limiter_10, "get_ltp", is_async=True)
     @log_request
     async def async_get_ltp(self, params, session=None):
         response = await self.async_post_request("api.ltp.data", params, session)
         return response
 
-    @access_rate_handler(max_requests=9, per_seconds=1, is_async=True)
+    @access_rate_handler(limiter_10, "get_quotes", is_async=True)
     @log_request
     async def async_get_quotes(self, params, session=None):
         response = await self.async_post_request("api.market.data", params, session)
         return response
 
-    @access_rate_handler(max_requests=19, per_seconds=1, is_async=True)
+    @access_rate_handler(limiter_20, "place_order", is_async=True)
     @log_request
     async def async_place_order(self, order_params, session=None):
         params = {k: v for k, v in order_params.items() if v is not None}
 
         response = await self.async_post_request("api.order.place", params, session)
         if response is not None and response.get("status", False):
             if (
@@ -143,24 +147,24 @@
                 return response
             else:
                 logger.error(f"Invalid response format: {response}")
         else:
             logger.error(f"API request failed: {response}")
         return None
 
-    @access_rate_handler(max_requests=19, per_seconds=1, is_async=True)
+    @access_rate_handler(limiter_20, "modify_order", is_async=True)
     @log_request
     async def async_modify_order(self, modified_params, session=None):
         params = modified_params
         params = {k: v for k, v in params.items() if v is not None}
 
         response = await self.async_post_request("api.order.modify", params, session)
         return response
 
-    @access_rate_handler(max_requests=9, per_seconds=1, is_async=True)
+    @access_rate_handler(limiter_10, "unique_order_status", is_async=True)
     @log_request
     async def async_unique_order_status(self, unique_order_id, session=None):
         response = await self._async_request(
             "api.individual.order.details",
             "GET",
             appendage=unique_order_id,
             session=session,
```

### Comparing `volstreet-8.0.0/volstreet/backtests/analysis.py` & `volstreet-8.0.1/volstreet/backtests/analysis.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.0/volstreet/backtests/database.py` & `volstreet-8.0.1/volstreet/backtests/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from collections import defaultdict
 from sqlalchemy import create_engine, text, TextClause
 from itertools import product
 from datetime import datetime
 import numpy as np
 from typing import Optional, Iterable, List
 import os
-from volstreet import timeit
+from volstreet.decorators import timeit
 import pandas as pd
 
 
 @define
 class DataBaseConnection:
     _mode = "local"  # Set to 'timescale' for TimescaleDB
     # Database attributes
@@ -286,14 +286,37 @@
             index_prices = pd.read_sql(query, connection)
 
         # Store the query
         self._queries["index_prices"].append(query)
 
         return index_prices
 
+    @timeit()
+    def fetch_streaming_prices(self, underlying: str, date) -> pd.DataFrame:
+        """Fetch streaming prices from PostGresDB."""
+
+        query = f"""
+            SELECT *
+            FROM price_stream
+            WHERE symboltoken LIKE '{underlying}%' AND DATE(timestamp) = '{date}'
+            ORDER BY timestamp ASC;
+            """
+
+        query = text(query)
+
+        engine = create_engine(self._alchemy_engine_url)
+        with engine.connect() as connection:
+            stream_prices = pd.read_sql(query, connection)
+
+        # Store the query
+        self._queries["stream_prices"].append(query)
+
+        return stream_prices
+
+    @timeit()
     def execute_query(self, query: str | TextClause, return_type: str = "fetchall"):
         """Execute the provided query."""
         query = text(query) if isinstance(query, str) else query
         engine = create_engine(self._alchemy_engine_url)
         with engine.connect() as connection:
             result = connection.execute(query)
             result = getattr(result, return_type)()
```

### Comparing `volstreet-8.0.0/volstreet/backtests/delta_hedging.py` & `volstreet-8.0.1/volstreet/backtests/delta_hedging.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.0/volstreet/backtests/delta_optimizer.py` & `volstreet-8.0.1/volstreet/backtests/delta_optimizer.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.0/volstreet/backtests/framework.py` & `volstreet-8.0.1/volstreet/backtests/framework.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.0/volstreet/backtests/intraday_backtest_abc.py` & `volstreet-8.0.1/volstreet/backtests/intraday_backtest_abc.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.0/volstreet/backtests/proxy_functions.py` & `volstreet-8.0.1/volstreet/backtests/proxy_functions.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,15 +11,29 @@
     backtester = BackTester()
     _current_group = None
 
     @classmethod
     def request_grouped_prices_for_day(
         cls, underlying: UnderlyingInfo, day: datetime, **kwargs
     ):
-        day_prices = cls.backtester.get_prices_for_day(underlying, day, **kwargs)
+        day_prices = cls.backtester.fetch_streaming_prices(underlying.name, day)
+        if day_prices.empty:
+            config.logger.warning(
+                f"No prices found for {underlying.name} on {day} in price_stream. "
+                f"Running process to fetch prices from historical data."
+            )
+            day_prices = cls.backtester.get_prices_for_day(underlying, day, **kwargs)
+        else:
+            start_time = time(*kwargs.get("start_time", (9, 16)))
+            end_time = time(*kwargs.get("end_time", (15, 30)))
+            day_prices = day_prices[
+                (day_prices.timestamp.dt.time >= start_time)
+                & (day_prices.timestamp.dt.time <= end_time)
+            ]
+
         day_prices_grouped = day_prices.groupby(day_prices.timestamp.dt.time)
         return day_prices_grouped
 
     @classmethod
     def update_prices(cls):
         prices_at_time = cls._current_group.get_group(config.backtest_state.time())
         price_dict = prices_at_time.to_dict(orient="records")
@@ -145,7 +159,28 @@
 
 def increase_robustness(func):
     return func
 
 
 def notify_pnl(*args, **kwargs):
     pass
+
+
+def retry_angel_api(*args, **kwargs):
+    def decorator(func):
+        return func
+
+    return decorator
+
+
+def access_rate_handler(*args, **kwargs):
+    def decorator(func):
+        return func
+
+    return decorator
+
+
+def timeit(*args, **kwargs):
+    def decorator(func):
+        return func
+
+    return decorator
```

### Comparing `volstreet-8.0.0/volstreet/backtests/tools.py` & `volstreet-8.0.1/volstreet/backtests/tools.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.0/volstreet/backtests/trend.py` & `volstreet-8.0.1/volstreet/backtests/trend.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.0/volstreet/backtests/underlying_info.py` & `volstreet-8.0.1/volstreet/backtests/underlying_info.py`

 * *Files 18% similar despite different names*

```diff
@@ -46,26 +46,7 @@
 
     nearest_exp_dates = filtered_dates[valid_indices].sort_values()
 
     if n_exp == 1:
         return nearest_exp_dates[0] if len(nearest_exp_dates) != 0 else None
     else:
         return nearest_exp_dates
-
-
-def extend_expiry_dates() -> None:
-    """Extend the expiry dates which are stored in the index_expiries.pkl file."""
-
-    dbc = DataBaseConnection()
-
-    with open("volstreet\\historical_info\\index_expiries.pkl", "rb") as file:
-        all_expiry_dates = pickle.load(file)
-
-    for underlying in ["NIFTY", "BANKNIFTY", "FINNIFTY", "MIDCPNIFTY"]:
-        index_expiry_dates = all_expiry_dates[underlying]
-        new_list = dbc.fetch_historical_expiries(underlying)
-        combined_list = [*set(index_expiry_dates + new_list)]
-        all_expiry_dates[underlying] = combined_list
-        logger.info(f"Extended expiry dates for {underlying}")
-
-    with open("volstreet\\historical_info\\index_expiries.pkl", "wb") as file:
-        pickle.dump(all_expiry_dates, file)
```

### Comparing `volstreet-8.0.0/volstreet/blackscholes.py` & `volstreet-8.0.1/volstreet/blackscholes.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.0/volstreet/config.py` & `volstreet-8.0.1/volstreet/config.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.0/volstreet/database_connection.py` & `volstreet-8.0.1/volstreet/database_connection.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.0/volstreet/datamodule/analysis.py` & `volstreet-8.0.1/volstreet/datamodule/analysis.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.0/volstreet/datamodule/archive.py` & `volstreet-8.0.1/volstreet/datamodule/archive.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.0/volstreet/datamodule/data_handling.py` & `volstreet-8.0.1/volstreet/datamodule/data_handling.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.0/volstreet/datamodule/eod_client.py` & `volstreet-8.0.1/volstreet/datamodule/eod_client.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.0/volstreet/datamodule/gambling.py` & `volstreet-8.0.1/volstreet/datamodule/gambling.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.0/volstreet/datamodule/intraday_data.py` & `volstreet-8.0.1/volstreet/datamodule/intraday_data.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.0/volstreet/datamodule/stockmock.py` & `volstreet-8.0.1/volstreet/datamodule/stockmock.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.0/volstreet/datamodule/trading_assistance.py` & `volstreet-8.0.1/volstreet/datamodule/trading_assistance.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.0/volstreet/dealingroom.py` & `volstreet-8.0.1/volstreet/dealingroom.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.0/volstreet/decorators.py` & `volstreet-8.0.1/volstreet/decorators.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.0/volstreet/discord_bot.py` & `volstreet-8.0.1/volstreet/discord_bot.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.0/volstreet/exceptions.py` & `volstreet-8.0.1/volstreet/exceptions.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.0/volstreet/historical_info/__init__.py` & `volstreet-8.0.1/volstreet/historical_info/__init__.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.0/volstreet/historical_info/index_expiries.pkl` & `volstreet-8.0.1/volstreet/historical_info/index_expiries.pkl`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.0/volstreet/historical_info/market_days.pkl` & `volstreet-8.0.1/volstreet/historical_info/market_days.pkl`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 8004 958e 4100 0000 0000 005d 9428 8c08  ....A......].(..
+00000000: 8004 95b5 4100 0000 0000 005d 9428 8c08  ....A......].(..
 00000010: 6461 7465 7469 6d65 948c 0464 6174 6594  datetime...date.
 00000020: 9394 4304 07e3 0201 9485 9452 9468 0343  ..C........R.h.C
 00000030: 0407 e302 0494 8594 5294 6803 4304 07e3  ........R.h.C...
 00000040: 0205 9485 9452 9468 0343 0407 e302 0694  .....R.h.C......
 00000050: 8594 5294 6803 4304 07e3 0207 9485 9452  ..R.h.C........R
 00000060: 9468 0343 0407 e302 0894 8594 5294 6803  .h.C........R.h.
 00000070: 4304 07e3 020b 9485 9452 9468 0343 0407  C........R.h.C..
@@ -1043,8 +1043,10 @@
 00004120: 5294 6803 4304 07e8 0405 9485 9452 9468  R.h.C........R.h
 00004130: 0343 0407 e804 0894 8594 5294 6803 4304  .C........R.h.C.
 00004140: 07e8 0409 9485 9452 9468 0343 0407 e804  .......R.h.C....
 00004150: 0a94 8594 5294 6803 4304 07e8 040c 9485  ....R.h.C.......
 00004160: 9452 9468 0343 0407 e804 0f94 8594 5294  .R.h.C........R.
 00004170: 6803 4304 07e8 0410 9485 9452 9468 0343  h.C........R.h.C
 00004180: 0407 e804 1294 8594 5294 6803 4304 07e8  ........R.h.C...
-00004190: 0413 9485 9452 9465 2e                   .....R.e.
+00004190: 0413 9485 9452 9468 0343 0407 e804 1694  .....R.h.C......
+000041a0: 8594 5294 6803 4304 07e8 0417 9485 9452  ..R.h.C........R
+000041b0: 9468 0343 0407 e804 1894 8594 5294 652e  .h.C........R.e.
```

### Comparing `volstreet-8.0.0/volstreet/models/__init__.py` & `volstreet-8.0.1/volstreet/models/__init__.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.0/volstreet/parallelization.py` & `volstreet-8.0.1/volstreet/parallelization.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.0/volstreet/performance_tracking.py` & `volstreet-8.0.1/volstreet/performance_tracking.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.0/volstreet/position_dashboard/app.py` & `volstreet-8.0.1/volstreet/position_dashboard/app.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.0/volstreet/position_dashboard/formatting.py` & `volstreet-8.0.1/volstreet/position_dashboard/formatting.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.0/volstreet/strategies/deployment.py` & `volstreet-8.0.1/volstreet/strategies/deployment.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     fetch_book,
     lookup_and_return,
     modify_order,
     update_order_params,
     fetch_quotes,
 )
 from volstreet.angel_interface.active_session import ActiveSession
-from volstreet.trade_interface import Index, order_placement_lock
+from volstreet.trade_interface import Index
 from volstreet.strategies.strats import (
     intraday_strangle,
     intraday_trend,
     delta_hedged_strangle,
     overnight_straddle,
     biweekly_straddle,
     buy_weekly_hedge,
@@ -557,15 +557,14 @@
             )
             self.strategies.append(strategy)
 
     @wait_for_login
     def continuously_handle_open_orders(self):
         while not self.session_terminated:
             try:
-                order_placement_lock.acquire()
                 order_book = fetch_book("orderbook", from_api=True)
                 if not order_book:
                     continue
                 open_orders = get_open_orders(order_book, statuses=["open"])
 
                 if open_orders.size > 0:
                     order_descriptions = [
@@ -583,15 +582,14 @@
                     modify_orders(open_orders)
             except Exception as e:
                 logger.error(f"Error in continuously handling open orders: {e}")
             # In Python, the "finally" block is guaranteed to be executed regardless of how the try block is exited.
             # This includes situations where the try block is exited due to a return, break, or continue statement,
             # or even if an exception is raised. Hence, the lock gets released in the "finally" block.
             finally:
-                order_placement_lock.release()
                 sleep(3)
 
 
 def run_client(
     client: Client,
     websockets: bool = True,
     process_manager: Manager = None,
```

### Comparing `volstreet-8.0.0/volstreet/strategies/error_handling.py` & `volstreet-8.0.1/volstreet/strategies/error_handling.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.0/volstreet/strategies/helpers.py` & `volstreet-8.0.1/volstreet/strategies/helpers.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.0/volstreet/strategies/monitoring.py` & `volstreet-8.0.1/volstreet/strategies/monitoring.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.0/volstreet/strategies/optimization.py` & `volstreet-8.0.1/volstreet/strategies/optimization.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.0/volstreet/strategies/strats.py` & `volstreet-8.0.1/volstreet/strategies/strats.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.0/volstreet/trade_interface/instruments.py` & `volstreet-8.0.1/volstreet/trade_interface/instruments.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.0/volstreet/trade_interface/order_execution.py` & `volstreet-8.0.1/volstreet/trade_interface/order_execution.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,17 +27,14 @@
     Strangle,
     Straddle,
     SyntheticFuture,
     Action,
 )
 
 
-order_placement_lock = threading.Lock()
-
-
 @log_error()
 def cancel_pending_orders(order_ids, variety="STOPLOSS"):
     if isinstance(order_ids, (list, np.ndarray)):
         for order_id in order_ids:
             ActiveSession.obj.cancelOrder(order_id, variety)
     else:
         ActiveSession.obj.cancelOrder(order_ids, variety)
@@ -269,15 +266,15 @@
                 instr.generate_order_params(**params, price=(call_price, put_price))
             )
 
     return order_params
 
 
 @timeit()
-def _execute_instructions(
+def execute_instructions(
     instructions: dict[Option | Strangle | Straddle | SyntheticFuture, dict],
     at_market: bool,
 ) -> dict[Option | Strangle | Straddle | SyntheticFuture, float]:
     """Executes orders for a given set of instructions.
     Instructions is a dictionary where the keys are Instrument objects and
     the values are dictionaries containing the order parameters.
     The order parameters MUST contain the following keys:
@@ -316,14 +313,15 @@
     }
 
     average_prices = {}
 
     # If instructions has at-least one option, we need to execute the orders
     # Or else skip to the next step
     if instructions:
+        logger.info(f"{threading.current_thread().name} is executing orders.")
         if at_market:
             instructions = {
                 instr: {**params, "price": "MARKET"}
                 for instr, params in instructions.items()
             }
         order_params = generate_bulk_params(instructions)
         executed_prices = asyncio.run(execute_orders(order_params))
@@ -336,24 +334,14 @@
             for instr in og_instructions
             if instr not in instructions
         }
     )
     return average_prices
 
 
-def execute_instructions(
-    instructions: dict[Option | Strangle | Straddle | SyntheticFuture, dict],
-    at_market: bool = False,
-) -> dict[Option | Strangle | Straddle | SyntheticFuture, float]:
-    with order_placement_lock:
-        logger.info(f"{threading.current_thread().name} is executing orders.")
-        result = _execute_instructions(instructions, at_market)
-        return result
-
-
 @timeit()
 def place_option_order_and_notify(
     instrument: Option | Strangle | Straddle | SyntheticFuture,
     action: Action | str,
     qty_in_lots: int,
     prices: str | int | float | tuple | list | np.ndarray = "LIMIT",
     order_tag: str = "",
```

### Comparing `volstreet-8.0.0/volstreet/trade_interface/underlyings.py` & `volstreet-8.0.1/volstreet/trade_interface/underlyings.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.0/volstreet/utils/change_config.py` & `volstreet-8.0.1/volstreet/utils/change_config.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.0/volstreet/utils/communication.py` & `volstreet-8.0.1/volstreet/utils/communication.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.0/volstreet/utils/core.py` & `volstreet-8.0.1/volstreet/utils/core.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.0/volstreet/utils/data_io.py` & `volstreet-8.0.1/volstreet/utils/data_io.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.0/volstreet/utils/scrip_processing.py` & `volstreet-8.0.1/volstreet/utils/scrip_processing.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.0/volstreet/vectorized_blackscholes.py` & `volstreet-8.0.1/volstreet/vectorized_blackscholes.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.0/volstreet/vslogging/formatters.py` & `volstreet-8.0.1/volstreet/vslogging/formatters.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.0/volstreet/vslogging/logging_config.json` & `volstreet-8.0.1/volstreet/vslogging/logging_config.json`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.0/volstreet/vslogging/logging_setup.py` & `volstreet-8.0.1/volstreet/vslogging/logging_setup.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.0/volstreet/vslogging/parsing.py` & `volstreet-8.0.1/volstreet/vslogging/parsing.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.0/volstreet.egg-info/PKG-INFO` & `volstreet-8.0.1/volstreet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volstreet
-Version: 8.0.0
+Version: 8.0.1
 Summary: VolStreet is a Python library for automated trading
 Home-page: https://github.com/rahulthakkr/volstreet
 Author: Rahul Thakkar
 Author-email: r.thakkar15@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `volstreet-8.0.0/volstreet.egg-info/SOURCES.txt` & `volstreet-8.0.1/volstreet.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -15,31 +15,33 @@
 volstreet/volstreet_mode.json
 volstreet.egg-info/PKG-INFO
 volstreet.egg-info/SOURCES.txt
 volstreet.egg-info/dependency_links.txt
 volstreet.egg-info/requires.txt
 volstreet.egg-info/top_level.txt
 volstreet/angel_interface/__init__.py
-volstreet/angel_interface/access_rate_handlers.py
+volstreet/angel_interface/access_rate_handler.py
 volstreet/angel_interface/active_session.py
 volstreet/angel_interface/async_interface.py
 volstreet/angel_interface/base_websocket.py
 volstreet/angel_interface/interface.py
 volstreet/angel_interface/login.py
 volstreet/angel_interface/order_websocket.py
 volstreet/angel_interface/price_websocket.py
 volstreet/angel_interface/smart_connect.py
 volstreet/backtests/__init__.py
 volstreet/backtests/analysis.py
+volstreet/backtests/data_updation.py
 volstreet/backtests/database.py
 volstreet/backtests/delta_hedging.py
 volstreet/backtests/delta_optimizer.py
 volstreet/backtests/framework.py
 volstreet/backtests/intraday_backtest_abc.py
 volstreet/backtests/proxy_functions.py
+volstreet/backtests/result_processing.py
 volstreet/backtests/runner.py
 volstreet/backtests/tools.py
 volstreet/backtests/trend.py
 volstreet/backtests/underlying_info.py
 volstreet/datamodule/__init__.py
 volstreet/datamodule/analysis.py
 volstreet/datamodule/archive.py
```

