# Comparing `tmp/qstrader-0.2.6.tar.gz` & `tmp/qstrader-0.2.7.tar.gz`

## Comparing `qstrader-0.2.6.tar` & `qstrader-0.2.7.tar`

### file list

```diff
@@ -1,137 +1,138 @@
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 qstrader-0.2.6/.coveragerc
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 qstrader-0.2.6/.travis.yml
--rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 qstrader-0.2.6/CHANGELOG.md
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 qstrader-0.2.6/MANIFEST.in
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 qstrader-0.2.6/dockerfiles/bionic/Dockerfile
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 qstrader-0.2.6/dockerfiles/centos8/Dockerfile
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 qstrader-0.2.6/dockerfiles/fedora33/Dockerfile
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 qstrader-0.2.6/dockerfiles/focal/Dockerfile
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 qstrader-0.2.6/examples/buy_and_hold.py
--rw-r--r--   0        0        0     2962 2020-02-02 00:00:00.000000 qstrader-0.2.6/examples/long_short.py
--rw-r--r--   0        0        0     8160 2020-02-02 00:00:00.000000 qstrader-0.2.6/examples/momentum_taa.py
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 qstrader-0.2.6/examples/sixty_forty.py
--rw-r--r--   0        0        0     2766 2020-02-02 00:00:00.000000 qstrader-0.2.6/examples/sixty_forty_fees.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/__init__.py
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/alpha_model/__init__.py
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/alpha_model/alpha_model.py
--rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/alpha_model/fixed_signals.py
--rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/alpha_model/single_signal.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/asset/__init__.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/asset/asset.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/asset/cash.py
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/asset/equity.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/asset/universe/__init__.py
--rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/asset/universe/dynamic.py
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/asset/universe/static.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/asset/universe/universe.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/broker/__init__.py
--rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/broker/broker.py
--rw-r--r--   0        0        0    23497 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/broker/simulated_broker.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/broker/fee_model/__init__.py
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/broker/fee_model/fee_model.py
--rw-r--r--   0        0        0     2927 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/broker/fee_model/percent_fee_model.py
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/broker/fee_model/zero_fee_model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/broker/portfolio/__init__.py
--rw-r--r--   0        0        0    10994 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/broker/portfolio/portfolio.py
--rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/broker/portfolio/portfolio_event.py
--rw-r--r--   0        0        0    11917 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/broker/portfolio/position.py
--rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/broker/portfolio/position_handler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/broker/transaction/__init__.py
--rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/broker/transaction/transaction.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/data/__init__.py
--rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/data/backtest_data_handler.py
--rw-r--r--   0        0        0     9475 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/data/daily_bar_csv.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/exchange/__init__.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/exchange/exchange.py
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/exchange/simulated_exchange.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/execution/__init__.py
--rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/execution/execution_handler.py
--rw-r--r--   0        0        0     3037 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/execution/order.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/execution/execution_algo/__init__.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/execution/execution_algo/execution_algo.py
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/execution/execution_algo/market_order.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/portcon/__init__.py
--rw-r--r--   0        0        0    10458 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/portcon/pcm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/portcon/optimiser/__init__.py
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/portcon/optimiser/equal_weight.py
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/portcon/optimiser/fixed_weight.py
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/portcon/optimiser/optimiser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/portcon/order_sizer/__init__.py
--rw-r--r--   0        0        0     6032 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/portcon/order_sizer/dollar_weighted.py
--rw-r--r--   0        0        0     5641 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/portcon/order_sizer/long_short.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/portcon/order_sizer/order_sizer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/risk_model/__init__.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/risk_model/risk_model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/signals/__init__.py
--rw-r--r--   0        0        0     3712 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/signals/buffer.py
--rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/signals/momentum.py
--rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/signals/signal.py
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/signals/signals_collection.py
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/signals/sma.py
--rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/signals/vol.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/simulation/__init__.py
--rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/simulation/daily_bday.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/simulation/event.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/simulation/sim_engine.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/statistics/__init__.py
--rw-r--r--   0        0        0    13429 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/statistics/json_statistics.py
--rw-r--r--   0        0        0     3155 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/statistics/performance.py
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/statistics/statistics.py
--rw-r--r--   0        0        0    12593 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/statistics/tearsheet.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/system/__init__.py
--rw-r--r--   0        0        0     5779 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/system/qts.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/system/rebalance/__init__.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/system/rebalance/buy_and_hold.py
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/system/rebalance/daily.py
--rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/system/rebalance/end_of_month.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/system/rebalance/rebalance.py
--rw-r--r--   0        0        0     3003 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/system/rebalance/weekly.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/trading/__init__.py
--rw-r--r--   0        0        0    15331 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/trading/backtest.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/trading/trading_session.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/utils/__init__.py
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 qstrader-0.2.6/qstrader/utils/console.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 qstrader-0.2.6/requirements/base.txt
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 qstrader-0.2.6/requirements/tests.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qstrader-0.2.6/scripts/__init__.py
--rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 qstrader-0.2.6/scripts/static_backtest.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 qstrader-0.2.6/tests/conftest.py
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 qstrader-0.2.6/tests/integration/portcon/test_pcm_e2e.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 qstrader-0.2.6/tests/integration/trading/conftest.py
--rw-r--r--   0        0        0     4224 2020-02-02 00:00:00.000000 qstrader-0.2.6/tests/integration/trading/test_backtest_e2e.py
--rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 qstrader-0.2.6/tests/integration/trading/fixtures/ABC.csv
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 qstrader-0.2.6/tests/integration/trading/fixtures/DEF.csv
--rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 qstrader-0.2.6/tests/integration/trading/fixtures/long_short_history.dat
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 qstrader-0.2.6/tests/integration/trading/fixtures/sixty_forty_history.dat
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 qstrader-0.2.6/tests/unit/alpha_model/test_fixed_signals.py
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 qstrader-0.2.6/tests/unit/alpha_model/test_single_signal.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 qstrader-0.2.6/tests/unit/asset/test_cash.py
--rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 qstrader-0.2.6/tests/unit/asset/universe/test_dynamic_universe.py
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 qstrader-0.2.6/tests/unit/asset/universe/test_static_universe.py
--rw-r--r--   0        0        0    21014 2020-02-02 00:00:00.000000 qstrader-0.2.6/tests/unit/broker/test_simulated_broker.py
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 qstrader-0.2.6/tests/unit/broker/fee_model/test_percent_fee_model.py
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 qstrader-0.2.6/tests/unit/broker/fee_model/test_zero_fee_model.py
--rw-r--r--   0        0        0    12720 2020-02-02 00:00:00.000000 qstrader-0.2.6/tests/unit/broker/portfolio/test_portfolio.py
--rw-r--r--   0        0        0    21930 2020-02-02 00:00:00.000000 qstrader-0.2.6/tests/unit/broker/portfolio/test_position.py
--rw-r--r--   0        0        0     4684 2020-02-02 00:00:00.000000 qstrader-0.2.6/tests/unit/broker/portfolio/test_position_handler.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 qstrader-0.2.6/tests/unit/broker/transaction/test_transaction.py
--rw-r--r--   0        0        0     6764 2020-02-02 00:00:00.000000 qstrader-0.2.6/tests/unit/portcon/test_pcm.py
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 qstrader-0.2.6/tests/unit/portcon/optimiser/test_equal_weight.py
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 qstrader-0.2.6/tests/unit/portcon/optimiser/test_fixed_weight.py
--rw-r--r--   0        0        0     4264 2020-02-02 00:00:00.000000 qstrader-0.2.6/tests/unit/portcon/order_sizer/test_dollar_weighted.py
--rw-r--r--   0        0        0     5612 2020-02-02 00:00:00.000000 qstrader-0.2.6/tests/unit/portcon/order_sizer/test_long_short.py
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 qstrader-0.2.6/tests/unit/signals/test_momentum.py
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 qstrader-0.2.6/tests/unit/signals/test_sma.py
--rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 qstrader-0.2.6/tests/unit/simulation/test_daily_bday.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 qstrader-0.2.6/tests/unit/simulation/test_event.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 qstrader-0.2.6/tests/unit/system/rebalance/test_buy_and_hold_rebalance.py
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 qstrader-0.2.6/tests/unit/system/rebalance/test_daily_rebalance.py
--rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 qstrader-0.2.6/tests/unit/system/rebalance/test_end_of_month_rebalance.py
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 qstrader-0.2.6/tests/unit/system/rebalance/test_weekly_rebalance.py
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 qstrader-0.2.6/tests/unit/utils/test_console.py
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 qstrader-0.2.6/.gitignore
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 qstrader-0.2.6/LICENSE
--rw-r--r--   0        0        0     8740 2020-02-02 00:00:00.000000 qstrader-0.2.6/README.md
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 qstrader-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     9901 2020-02-02 00:00:00.000000 qstrader-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 qstrader-0.2.7/.coveragerc
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 qstrader-0.2.7/.travis.yml
+-rw-r--r--   0        0        0     4267 2020-02-02 00:00:00.000000 qstrader-0.2.7/CHANGELOG.md
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 qstrader-0.2.7/MANIFEST.in
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 qstrader-0.2.7/dockerfiles/bionic/Dockerfile
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 qstrader-0.2.7/dockerfiles/centos8/Dockerfile
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 qstrader-0.2.7/dockerfiles/fedora33/Dockerfile
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 qstrader-0.2.7/dockerfiles/focal/Dockerfile
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 qstrader-0.2.7/examples/buy_and_hold.py
+-rw-r--r--   0        0        0     2962 2020-02-02 00:00:00.000000 qstrader-0.2.7/examples/long_short.py
+-rw-r--r--   0        0        0     8160 2020-02-02 00:00:00.000000 qstrader-0.2.7/examples/momentum_taa.py
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 qstrader-0.2.7/examples/sixty_forty.py
+-rw-r--r--   0        0        0     2766 2020-02-02 00:00:00.000000 qstrader-0.2.7/examples/sixty_forty_fees.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/__init__.py
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/alpha_model/__init__.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/alpha_model/alpha_model.py
+-rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/alpha_model/fixed_signals.py
+-rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/alpha_model/single_signal.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/asset/__init__.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/asset/asset.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/asset/cash.py
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/asset/equity.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/asset/universe/__init__.py
+-rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/asset/universe/dynamic.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/asset/universe/static.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/asset/universe/universe.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/broker/__init__.py
+-rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/broker/broker.py
+-rw-r--r--   0        0        0    23497 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/broker/simulated_broker.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/broker/fee_model/__init__.py
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/broker/fee_model/fee_model.py
+-rw-r--r--   0        0        0     2927 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/broker/fee_model/percent_fee_model.py
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/broker/fee_model/zero_fee_model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/broker/portfolio/__init__.py
+-rw-r--r--   0        0        0    10994 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/broker/portfolio/portfolio.py
+-rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/broker/portfolio/portfolio_event.py
+-rw-r--r--   0        0        0    11917 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/broker/portfolio/position.py
+-rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/broker/portfolio/position_handler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/broker/transaction/__init__.py
+-rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/broker/transaction/transaction.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/data/__init__.py
+-rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/data/backtest_data_handler.py
+-rw-r--r--   0        0        0     9475 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/data/daily_bar_csv.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/exchange/__init__.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/exchange/exchange.py
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/exchange/simulated_exchange.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/execution/__init__.py
+-rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/execution/execution_handler.py
+-rw-r--r--   0        0        0     3037 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/execution/order.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/execution/execution_algo/__init__.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/execution/execution_algo/execution_algo.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/execution/execution_algo/market_order.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/portcon/__init__.py
+-rw-r--r--   0        0        0    10458 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/portcon/pcm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/portcon/optimiser/__init__.py
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/portcon/optimiser/equal_weight.py
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/portcon/optimiser/fixed_weight.py
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/portcon/optimiser/optimiser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/portcon/order_sizer/__init__.py
+-rw-r--r--   0        0        0     6032 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/portcon/order_sizer/dollar_weighted.py
+-rw-r--r--   0        0        0     5641 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/portcon/order_sizer/long_short.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/portcon/order_sizer/order_sizer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/risk_model/__init__.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/risk_model/risk_model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/signals/__init__.py
+-rw-r--r--   0        0        0     3712 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/signals/buffer.py
+-rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/signals/momentum.py
+-rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/signals/signal.py
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/signals/signals_collection.py
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/signals/sma.py
+-rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/signals/vol.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/simulation/__init__.py
+-rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/simulation/daily_bday.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/simulation/event.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/simulation/sim_engine.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/statistics/__init__.py
+-rw-r--r--   0        0        0    13429 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/statistics/json_statistics.py
+-rw-r--r--   0        0        0     3155 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/statistics/performance.py
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/statistics/statistics.py
+-rw-r--r--   0        0        0    12593 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/statistics/tearsheet.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/system/__init__.py
+-rw-r--r--   0        0        0     5779 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/system/qts.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/system/rebalance/__init__.py
+-rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/system/rebalance/buy_and_hold.py
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/system/rebalance/daily.py
+-rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/system/rebalance/end_of_month.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/system/rebalance/rebalance.py
+-rw-r--r--   0        0        0     3003 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/system/rebalance/weekly.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/trading/__init__.py
+-rw-r--r--   0        0        0    15331 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/trading/backtest.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/trading/trading_session.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/utils/__init__.py
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 qstrader-0.2.7/qstrader/utils/console.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 qstrader-0.2.7/requirements/base.txt
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 qstrader-0.2.7/requirements/tests.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qstrader-0.2.7/scripts/__init__.py
+-rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 qstrader-0.2.7/scripts/static_backtest.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 qstrader-0.2.7/tests/conftest.py
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 qstrader-0.2.7/tests/integration/portcon/test_pcm_e2e.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 qstrader-0.2.7/tests/integration/trading/conftest.py
+-rw-r--r--   0        0        0     5233 2020-02-02 00:00:00.000000 qstrader-0.2.7/tests/integration/trading/test_backtest_e2e.py
+-rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 qstrader-0.2.7/tests/integration/trading/fixtures/ABC.csv
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 qstrader-0.2.7/tests/integration/trading/fixtures/DEF.csv
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 qstrader-0.2.7/tests/integration/trading/fixtures/GHI.csv
+-rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 qstrader-0.2.7/tests/integration/trading/fixtures/long_short_history.dat
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 qstrader-0.2.7/tests/integration/trading/fixtures/sixty_forty_history.dat
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 qstrader-0.2.7/tests/unit/alpha_model/test_fixed_signals.py
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 qstrader-0.2.7/tests/unit/alpha_model/test_single_signal.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 qstrader-0.2.7/tests/unit/asset/test_cash.py
+-rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 qstrader-0.2.7/tests/unit/asset/universe/test_dynamic_universe.py
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 qstrader-0.2.7/tests/unit/asset/universe/test_static_universe.py
+-rw-r--r--   0        0        0    21014 2020-02-02 00:00:00.000000 qstrader-0.2.7/tests/unit/broker/test_simulated_broker.py
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 qstrader-0.2.7/tests/unit/broker/fee_model/test_percent_fee_model.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 qstrader-0.2.7/tests/unit/broker/fee_model/test_zero_fee_model.py
+-rw-r--r--   0        0        0    12720 2020-02-02 00:00:00.000000 qstrader-0.2.7/tests/unit/broker/portfolio/test_portfolio.py
+-rw-r--r--   0        0        0    21930 2020-02-02 00:00:00.000000 qstrader-0.2.7/tests/unit/broker/portfolio/test_position.py
+-rw-r--r--   0        0        0     4684 2020-02-02 00:00:00.000000 qstrader-0.2.7/tests/unit/broker/portfolio/test_position_handler.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 qstrader-0.2.7/tests/unit/broker/transaction/test_transaction.py
+-rw-r--r--   0        0        0     6764 2020-02-02 00:00:00.000000 qstrader-0.2.7/tests/unit/portcon/test_pcm.py
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 qstrader-0.2.7/tests/unit/portcon/optimiser/test_equal_weight.py
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 qstrader-0.2.7/tests/unit/portcon/optimiser/test_fixed_weight.py
+-rw-r--r--   0        0        0     4264 2020-02-02 00:00:00.000000 qstrader-0.2.7/tests/unit/portcon/order_sizer/test_dollar_weighted.py
+-rw-r--r--   0        0        0     5612 2020-02-02 00:00:00.000000 qstrader-0.2.7/tests/unit/portcon/order_sizer/test_long_short.py
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 qstrader-0.2.7/tests/unit/signals/test_momentum.py
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 qstrader-0.2.7/tests/unit/signals/test_sma.py
+-rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 qstrader-0.2.7/tests/unit/simulation/test_daily_bday.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 qstrader-0.2.7/tests/unit/simulation/test_event.py
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 qstrader-0.2.7/tests/unit/system/rebalance/test_buy_and_hold_rebalance.py
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 qstrader-0.2.7/tests/unit/system/rebalance/test_daily_rebalance.py
+-rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 qstrader-0.2.7/tests/unit/system/rebalance/test_end_of_month_rebalance.py
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 qstrader-0.2.7/tests/unit/system/rebalance/test_weekly_rebalance.py
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 qstrader-0.2.7/tests/unit/utils/test_console.py
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 qstrader-0.2.7/.gitignore
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 qstrader-0.2.7/LICENSE
+-rw-r--r--   0        0        0     8740 2020-02-02 00:00:00.000000 qstrader-0.2.7/README.md
+-rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 qstrader-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     9901 2020-02-02 00:00:00.000000 qstrader-0.2.7/PKG-INFO
```

### Comparing `qstrader-0.2.6/CHANGELOG.md` & `qstrader-0.2.7/CHANGELOG.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+# 0.2.7
+
+* Updates the execution handler to update final orders ensuring an execution order is created in the event of a single submission without a further rebalance.
+* Updates rebalance_buy_and_hold to check if the start_dt is a business day
+    If start_dt is a business day rebalance_dates =  [start_dt]
+    If start_dt is a weekend rebalance_dates = [next business day]
+* Adds a unit test to check that the buisness day calculation is correct
+* Adds an integration test to check that a backtest using buy_and_hold_rebalance generates execution orders on the correct dates
+
+
 # 0.2.6
 
 * Removed get_portfolio_total_non_cash_equity and get_account_total_non_cash_equity from broker/broker.py abstract base class. These methods are not implemented.
 * Added save option to TearsheetStatistics class in statistics/tearsheet.py. The tearsheet output can now be saved to a given filename by passing the optional filename parameter as a string when calling the plot_results function.
 
 
 # 0.2.5
```

### Comparing `qstrader-0.2.6/examples/buy_and_hold.py` & `qstrader-0.2.7/examples/buy_and_hold.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/examples/long_short.py` & `qstrader-0.2.7/examples/long_short.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/examples/momentum_taa.py` & `qstrader-0.2.7/examples/momentum_taa.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/examples/sixty_forty.py` & `qstrader-0.2.7/examples/sixty_forty.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/examples/sixty_forty_fees.py` & `qstrader-0.2.7/examples/sixty_forty_fees.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/qstrader/alpha_model/alpha_model.py` & `qstrader-0.2.7/qstrader/alpha_model/alpha_model.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/qstrader/alpha_model/fixed_signals.py` & `qstrader-0.2.7/qstrader/alpha_model/fixed_signals.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/qstrader/alpha_model/single_signal.py` & `qstrader-0.2.7/qstrader/alpha_model/single_signal.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/qstrader/asset/equity.py` & `qstrader-0.2.7/qstrader/asset/equity.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/qstrader/asset/universe/dynamic.py` & `qstrader-0.2.7/qstrader/asset/universe/dynamic.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/qstrader/asset/universe/static.py` & `qstrader-0.2.7/qstrader/asset/universe/static.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/qstrader/broker/broker.py` & `qstrader-0.2.7/qstrader/broker/broker.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/qstrader/broker/simulated_broker.py` & `qstrader-0.2.7/qstrader/broker/simulated_broker.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/qstrader/broker/fee_model/fee_model.py` & `qstrader-0.2.7/qstrader/broker/fee_model/fee_model.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/qstrader/broker/fee_model/percent_fee_model.py` & `qstrader-0.2.7/qstrader/broker/fee_model/percent_fee_model.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/qstrader/broker/fee_model/zero_fee_model.py` & `qstrader-0.2.7/qstrader/broker/fee_model/zero_fee_model.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/qstrader/broker/portfolio/portfolio.py` & `qstrader-0.2.7/qstrader/broker/portfolio/portfolio.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/qstrader/broker/portfolio/portfolio_event.py` & `qstrader-0.2.7/qstrader/broker/portfolio/portfolio_event.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/qstrader/broker/portfolio/position.py` & `qstrader-0.2.7/qstrader/broker/portfolio/position.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/qstrader/broker/portfolio/position_handler.py` & `qstrader-0.2.7/qstrader/broker/portfolio/position_handler.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/qstrader/broker/transaction/transaction.py` & `qstrader-0.2.7/qstrader/broker/transaction/transaction.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/qstrader/data/backtest_data_handler.py` & `qstrader-0.2.7/qstrader/data/backtest_data_handler.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/qstrader/data/daily_bar_csv.py` & `qstrader-0.2.7/qstrader/data/daily_bar_csv.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/qstrader/exchange/exchange.py` & `qstrader-0.2.7/qstrader/exchange/exchange.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/qstrader/exchange/simulated_exchange.py` & `qstrader-0.2.7/qstrader/exchange/simulated_exchange.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/qstrader/execution/execution_handler.py` & `qstrader-0.2.7/qstrader/execution/execution_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,7 +79,8 @@
         )
 
         # If order submission is specified then send the
         # individual order items to the Broker instance
         if self.submit_orders:
             for order in final_orders:
                 self.broker.submit_order(self.broker_portfolio_id, order)
+                self.broker.update(dt)
```

### Comparing `qstrader-0.2.6/qstrader/execution/order.py` & `qstrader-0.2.7/qstrader/execution/order.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/qstrader/execution/execution_algo/market_order.py` & `qstrader-0.2.7/qstrader/execution/execution_algo/market_order.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/qstrader/portcon/pcm.py` & `qstrader-0.2.7/qstrader/portcon/pcm.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/qstrader/portcon/optimiser/equal_weight.py` & `qstrader-0.2.7/qstrader/portcon/optimiser/equal_weight.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/qstrader/portcon/optimiser/fixed_weight.py` & `qstrader-0.2.7/qstrader/portcon/optimiser/fixed_weight.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/qstrader/portcon/optimiser/optimiser.py` & `qstrader-0.2.7/qstrader/portcon/optimiser/optimiser.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/qstrader/portcon/order_sizer/dollar_weighted.py` & `qstrader-0.2.7/qstrader/portcon/order_sizer/dollar_weighted.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/qstrader/portcon/order_sizer/long_short.py` & `qstrader-0.2.7/qstrader/portcon/order_sizer/long_short.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/qstrader/risk_model/risk_model.py` & `qstrader-0.2.7/qstrader/risk_model/risk_model.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/qstrader/signals/buffer.py` & `qstrader-0.2.7/qstrader/signals/buffer.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/qstrader/signals/momentum.py` & `qstrader-0.2.7/qstrader/signals/momentum.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/qstrader/signals/signal.py` & `qstrader-0.2.7/qstrader/signals/signal.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/qstrader/signals/signals_collection.py` & `qstrader-0.2.7/qstrader/signals/signals_collection.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/qstrader/signals/sma.py` & `qstrader-0.2.7/qstrader/signals/sma.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/qstrader/signals/vol.py` & `qstrader-0.2.7/qstrader/signals/vol.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/qstrader/simulation/daily_bday.py` & `qstrader-0.2.7/qstrader/simulation/daily_bday.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/qstrader/simulation/event.py` & `qstrader-0.2.7/qstrader/simulation/event.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/qstrader/simulation/sim_engine.py` & `qstrader-0.2.7/qstrader/simulation/sim_engine.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/qstrader/statistics/json_statistics.py` & `qstrader-0.2.7/qstrader/statistics/json_statistics.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/qstrader/statistics/performance.py` & `qstrader-0.2.7/qstrader/statistics/performance.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/qstrader/statistics/statistics.py` & `qstrader-0.2.7/qstrader/statistics/statistics.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/qstrader/statistics/tearsheet.py` & `qstrader-0.2.7/qstrader/statistics/tearsheet.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/qstrader/system/qts.py` & `qstrader-0.2.7/qstrader/system/qts.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/qstrader/system/rebalance/daily.py` & `qstrader-0.2.7/qstrader/system/rebalance/daily.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/qstrader/system/rebalance/end_of_month.py` & `qstrader-0.2.7/qstrader/system/rebalance/end_of_month.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/qstrader/system/rebalance/weekly.py` & `qstrader-0.2.7/qstrader/system/rebalance/weekly.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/qstrader/trading/backtest.py` & `qstrader-0.2.7/qstrader/trading/backtest.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/scripts/static_backtest.py` & `qstrader-0.2.7/scripts/static_backtest.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/tests/conftest.py` & `qstrader-0.2.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/tests/integration/portcon/test_pcm_e2e.py` & `qstrader-0.2.7/tests/integration/portcon/test_pcm_e2e.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/tests/integration/trading/test_backtest_e2e.py` & `qstrader-0.2.7/tests/integration/trading/test_backtest_e2e.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 import pytz
 import pytest
 
 from qstrader.alpha_model.fixed_signals import FixedSignalsAlphaModel
 from qstrader.asset.universe.static import StaticUniverse
 from qstrader.trading.backtest import BacktestTradingSession
 
+from qstrader import settings
+
 
 def test_backtest_sixty_forty(etf_filepath):
     """
     Ensures that a full end-to-end weekly rebalanced backtested
     trading session with fixed proportion weights produces the
     correct rebalance orders as well as correctly calculated
     market values after a single month's worth of daily
@@ -123,7 +125,38 @@
     }
 
     history_df = portfolio.history_to_df().reset_index()
     expected_df = pd.read_csv(os.path.join(etf_filepath, 'long_short_history.dat'))
 
     pd.testing.assert_frame_equal(history_df, expected_df)
     assert portfolio_dict == expected_dict
+
+
+def test_backtest_buy_and_hold(etf_filepath, capsys):
+    """
+    Ensures a backtest with a buy and hold rebalance calculates
+    the correct dates for execution orders when the start date is not
+    a business day.
+    """
+    settings.print_events=True
+    os.environ['QSTRADER_CSV_DATA_DIR'] = etf_filepath
+    assets = ['EQ:GHI']
+    universe = StaticUniverse(assets)
+    alpha_model = FixedSignalsAlphaModel({'EQ:GHI':1.0})
+    
+    start_dt = pd.Timestamp('2015-11-07 14:30:00', tz=pytz.UTC)
+    end_dt = pd.Timestamp('2015-11-10 14:30:00', tz=pytz.UTC)
+
+    backtest = BacktestTradingSession(
+        start_dt,
+        end_dt,
+        universe,
+        alpha_model,
+        rebalance='buy_and_hold',
+        long_only=True,
+        cash_buffer_percentage=0.01,
+    )
+    backtest.run(results=False)
+    
+    expected_execution_text = "(2015-11-09 14:30:00+00:00) - executed order:"
+    captured = capsys.readouterr()
+    assert expected_execution_text in captured.out
```

### Comparing `qstrader-0.2.6/tests/integration/trading/fixtures/ABC.csv` & `qstrader-0.2.7/tests/integration/trading/fixtures/ABC.csv`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/tests/integration/trading/fixtures/DEF.csv` & `qstrader-0.2.7/tests/integration/trading/fixtures/DEF.csv`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/tests/integration/trading/fixtures/long_short_history.dat` & `qstrader-0.2.7/tests/integration/trading/fixtures/long_short_history.dat`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/tests/integration/trading/fixtures/sixty_forty_history.dat` & `qstrader-0.2.7/tests/integration/trading/fixtures/sixty_forty_history.dat`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/tests/unit/alpha_model/test_fixed_signals.py` & `qstrader-0.2.7/tests/unit/alpha_model/test_fixed_signals.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/tests/unit/alpha_model/test_single_signal.py` & `qstrader-0.2.7/tests/unit/alpha_model/test_single_signal.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/tests/unit/asset/universe/test_dynamic_universe.py` & `qstrader-0.2.7/tests/unit/asset/universe/test_dynamic_universe.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/tests/unit/asset/universe/test_static_universe.py` & `qstrader-0.2.7/tests/unit/asset/universe/test_static_universe.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/tests/unit/broker/test_simulated_broker.py` & `qstrader-0.2.7/tests/unit/broker/test_simulated_broker.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/tests/unit/broker/fee_model/test_percent_fee_model.py` & `qstrader-0.2.7/tests/unit/broker/fee_model/test_percent_fee_model.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/tests/unit/broker/fee_model/test_zero_fee_model.py` & `qstrader-0.2.7/tests/unit/broker/fee_model/test_zero_fee_model.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/tests/unit/broker/portfolio/test_portfolio.py` & `qstrader-0.2.7/tests/unit/broker/portfolio/test_portfolio.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/tests/unit/broker/portfolio/test_position.py` & `qstrader-0.2.7/tests/unit/broker/portfolio/test_position.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/tests/unit/broker/portfolio/test_position_handler.py` & `qstrader-0.2.7/tests/unit/broker/portfolio/test_position_handler.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/tests/unit/broker/transaction/test_transaction.py` & `qstrader-0.2.7/tests/unit/broker/transaction/test_transaction.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/tests/unit/portcon/test_pcm.py` & `qstrader-0.2.7/tests/unit/portcon/test_pcm.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/tests/unit/portcon/optimiser/test_equal_weight.py` & `qstrader-0.2.7/tests/unit/portcon/optimiser/test_equal_weight.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/tests/unit/portcon/optimiser/test_fixed_weight.py` & `qstrader-0.2.7/tests/unit/portcon/optimiser/test_fixed_weight.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/tests/unit/portcon/order_sizer/test_dollar_weighted.py` & `qstrader-0.2.7/tests/unit/portcon/order_sizer/test_dollar_weighted.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/tests/unit/portcon/order_sizer/test_long_short.py` & `qstrader-0.2.7/tests/unit/portcon/order_sizer/test_long_short.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/tests/unit/signals/test_momentum.py` & `qstrader-0.2.7/tests/unit/signals/test_momentum.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/tests/unit/signals/test_sma.py` & `qstrader-0.2.7/tests/unit/signals/test_sma.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/tests/unit/simulation/test_daily_bday.py` & `qstrader-0.2.7/tests/unit/simulation/test_daily_bday.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/tests/unit/simulation/test_event.py` & `qstrader-0.2.7/tests/unit/simulation/test_event.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/tests/unit/system/rebalance/test_daily_rebalance.py` & `qstrader-0.2.7/tests/unit/system/rebalance/test_daily_rebalance.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/tests/unit/system/rebalance/test_end_of_month_rebalance.py` & `qstrader-0.2.7/tests/unit/system/rebalance/test_end_of_month_rebalance.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/tests/unit/system/rebalance/test_weekly_rebalance.py` & `qstrader-0.2.7/tests/unit/system/rebalance/test_weekly_rebalance.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/tests/unit/utils/test_console.py` & `qstrader-0.2.7/tests/unit/utils/test_console.py`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/LICENSE` & `qstrader-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/README.md` & `qstrader-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `qstrader-0.2.6/pyproject.toml` & `qstrader-0.2.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "qstrader"
-version = "0.2.6"
+version = "0.2.7"
 dependencies = [
     "click>=8.1",
     "matplotlib>=3.8",
     "numpy>=1.26",
     "pandas>=2.2",
     "seaborn>=0.13",
 ]
```

### Comparing `qstrader-0.2.6/PKG-INFO` & `qstrader-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: qstrader
-Version: 0.2.6
+Version: 0.2.7
 Summary: QSTrader backtesting simulation engine
 Project-URL: Homepage, https://github.com/mhallsmoore/qstrader
 Project-URL: Issues, https://github.com/mhallsmoore/qstrader/issues
 Project-URL: Documentation, https://www.quantstart.com/qstrader/
 Project-URL: Website, https://www.quantstart.com
 Author-email: Michael Halls-Moore <support@quantstart.com>
 Maintainer-email: Juliette James <juliette.james@quantstart.com>
```

