# Comparing `tmp/x10_python_trading-0.1.1.tar.gz` & `tmp/x10_python_trading-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "x10_python_trading-0.1.1.tar", max compression
+gzip compressed data, was "x10_python_trading-0.1.2.tar", max compression
```

## Comparing `x10_python_trading-0.1.1.tar` & `x10_python_trading-0.1.2.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0      794 2024-04-03 15:25:46.254304 x10_python_trading-0.1.1/README.md
--rw-r--r--   0        0        0     1541 2024-04-03 15:25:46.254304 x10_python_trading-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-03 15:25:46.254304 x10_python_trading-0.1.1/starkware/crypto/__init__.py
--rw-r--r--   0        0        0     3945 2024-04-03 15:25:46.254304 x10_python_trading-0.1.1/starkware/crypto/signature/README.md
--rw-r--r--   0        0        0        0 2024-04-03 15:25:46.254304 x10_python_trading-0.1.1/starkware/crypto/signature/__init__.py
--rw-r--r--   0        0        0     1840 2024-04-03 15:25:46.254304 x10_python_trading-0.1.1/starkware/crypto/signature/fast_pedersen_hash.py
--rw-r--r--   0        0        0     3627 2024-04-03 15:25:46.254304 x10_python_trading-0.1.1/starkware/crypto/signature/math_utils.py
--rw-r--r--   0        0        0     6074 2024-04-03 15:25:46.254304 x10_python_trading-0.1.1/starkware/crypto/signature/nothing_up_my_sleeve_gen.py
--rw-r--r--   0        0        0   102708 2024-04-03 15:25:46.254304 x10_python_trading-0.1.1/starkware/crypto/signature/pedersen_params.json
--rw-r--r--   0        0        0    11728 2024-04-03 15:25:46.254304 x10_python_trading-0.1.1/starkware/crypto/signature/signature.py
--rw-r--r--   0        0        0     3759 2024-04-03 15:25:46.254304 x10_python_trading-0.1.1/starkware/crypto/signature/src/config/assets_precomputed.json
--rw-r--r--   0        0        0    70705 2024-04-03 15:25:46.254304 x10_python_trading-0.1.1/starkware/crypto/signature/src/config/constant_points.json
--rw-r--r--   0        0        0     3701 2024-04-03 15:25:46.254304 x10_python_trading-0.1.1/starkware/crypto/signature/src/config/keys_precomputed.json
--rw-r--r--   0        0        0     1955 2024-04-03 15:25:46.254304 x10_python_trading-0.1.1/starkware/python/BUILD
--rw-r--r--   0        0        0       31 2024-04-03 15:25:46.254304 x10_python_trading-0.1.1/starkware/python/CMakeLists.txt
--rw-r--r--   0        0        0     1254 2024-04-03 15:25:46.254304 x10_python_trading-0.1.1/starkware/python/CMakeLists_common.txt
--rw-r--r--   0        0        0        0 2024-04-03 15:25:46.254304 x10_python_trading-0.1.1/starkware/python/__init__.py
--rw-r--r--   0        0        0     1522 2024-04-03 15:25:46.254304 x10_python_trading-0.1.1/starkware/python/async_subprocess.py
--rw-r--r--   0        0        0     5946 2024-04-03 15:25:46.254304 x10_python_trading-0.1.1/starkware/python/expression_string.py
--rw-r--r--   0        0        0     1883 2024-04-03 15:25:46.254304 x10_python_trading-0.1.1/starkware/python/expression_string_test.py
--rw-r--r--   0        0        0     3938 2024-04-03 15:25:46.254304 x10_python_trading-0.1.1/starkware/python/fixed_point.py
--rw-r--r--   0        0        0      675 2024-04-03 15:25:46.254304 x10_python_trading-0.1.1/starkware/python/json_rpc/BUILD
--rw-r--r--   0        0        0      359 2024-04-03 15:25:46.254304 x10_python_trading-0.1.1/starkware/python/json_rpc/CMakeLists.txt
--rw-r--r--   0        0        0      812 2024-04-03 15:25:46.254304 x10_python_trading-0.1.1/starkware/python/json_rpc/client.py
--rw-r--r--   0        0        0      681 2024-04-03 15:25:46.254304 x10_python_trading-0.1.1/starkware/python/json_rpc/client_test.py
--rw-r--r--   0        0        0     8881 2024-04-03 15:25:46.254304 x10_python_trading-0.1.1/starkware/python/math_utils.py
--rw-r--r--   0        0        0     5102 2024-04-03 15:25:46.254304 x10_python_trading-0.1.1/starkware/python/math_utils_test.py
--rw-r--r--   0        0        0     1614 2024-04-03 15:25:46.258303 x10_python_trading-0.1.1/starkware/python/merkle_tree.py
--rw-r--r--   0        0        0     1796 2024-04-03 15:25:46.258303 x10_python_trading-0.1.1/starkware/python/object_utils.py
--rw-r--r--   0        0        0     1545 2024-04-03 15:25:46.258303 x10_python_trading-0.1.1/starkware/python/python_dependencies.py
--rw-r--r--   0        0        0     6247 2024-04-03 15:25:46.258303 x10_python_trading-0.1.1/starkware/python/random_test.py
--rw-r--r--   0        0        0     6247 2024-04-03 15:25:46.258303 x10_python_trading-0.1.1/starkware/python/random_test_utils.py
--rw-r--r--   0        0        0     3460 2024-04-03 15:25:46.258303 x10_python_trading-0.1.1/starkware/python/test_utils.py
--rw-r--r--   0        0        0     2783 2024-04-03 15:25:46.258303 x10_python_trading-0.1.1/starkware/python/test_utils_test.py
--rw-r--r--   0        0        0    19817 2024-04-03 15:25:46.258303 x10_python_trading-0.1.1/starkware/python/utils.py
--rw-r--r--   0        0        0      599 2024-04-03 15:25:46.258303 x10_python_trading-0.1.1/starkware/python/utils_stub_module.py
--rw-r--r--   0        0        0     1554 2024-04-03 15:25:46.258303 x10_python_trading-0.1.1/starkware/python/utils_stub_module.pyi
--rw-r--r--   0        0        0     7959 2024-04-03 15:25:46.258303 x10_python_trading-0.1.1/starkware/python/utils_test.py
--rw-r--r--   0        0        0        0 2024-04-03 15:25:46.258303 x10_python_trading-0.1.1/x10/__init__.py
--rw-r--r--   0        0        0      413 2024-04-03 15:25:46.258303 x10_python_trading-0.1.1/x10/config.py
--rw-r--r--   0        0        0       36 2024-04-03 15:25:46.258303 x10_python_trading-0.1.1/x10/errors.py
--rw-r--r--   0        0        0        0 2024-04-03 15:25:46.258303 x10_python_trading-0.1.1/x10/perpetual/__init__.py
--rw-r--r--   0        0        0     1492 2024-04-03 15:25:46.258303 x10_python_trading-0.1.1/x10/perpetual/accounts.py
--rw-r--r--   0        0        0     1618 2024-04-03 15:25:46.258303 x10_python_trading-0.1.1/x10/perpetual/amounts.py
--rw-r--r--   0        0        0     1120 2024-04-03 15:25:46.258303 x10_python_trading-0.1.1/x10/perpetual/assets.py
--rw-r--r--   0        0        0      347 2024-04-03 15:25:46.258303 x10_python_trading-0.1.1/x10/perpetual/balances.py
--rw-r--r--   0        0        0      327 2024-04-03 15:25:46.258303 x10_python_trading-0.1.1/x10/perpetual/fees.py
--rw-r--r--   0        0        0      459 2024-04-03 15:25:46.258303 x10_python_trading-0.1.1/x10/perpetual/funding_rates.py
--rw-r--r--   0        0        0     2399 2024-04-03 15:25:46.258303 x10_python_trading-0.1.1/x10/perpetual/markets.py
--rw-r--r--   0        0        0     5141 2024-04-03 15:25:46.258303 x10_python_trading-0.1.1/x10/perpetual/order_object.py
--rw-r--r--   0        0        0      739 2024-04-03 15:25:46.258303 x10_python_trading-0.1.1/x10/perpetual/orderbooks.py
--rw-r--r--   0        0        0     2207 2024-04-03 15:25:46.258303 x10_python_trading-0.1.1/x10/perpetual/orders.py
--rw-r--r--   0        0        0     1069 2024-04-03 15:25:46.258303 x10_python_trading-0.1.1/x10/perpetual/positions.py
--rw-r--r--   0        0        0       99 2024-04-03 15:25:46.258303 x10_python_trading-0.1.1/x10/perpetual/stream_client/__init__.py
--rw-r--r--   0        0        0     2974 2024-04-03 15:25:46.258303 x10_python_trading-0.1.1/x10/perpetual/stream_client/perpetual_stream_connection.py
--rw-r--r--   0        0        0     2497 2024-04-03 15:25:46.258303 x10_python_trading-0.1.1/x10/perpetual/stream_client/stream_client.py
--rw-r--r--   0        0        0     1241 2024-04-03 15:25:46.258303 x10_python_trading-0.1.1/x10/perpetual/trades.py
--rw-r--r--   0        0        0      102 2024-04-03 15:25:46.258303 x10_python_trading-0.1.1/x10/perpetual/trading_client/__init__.py
--rw-r--r--   0        0        0     4303 2024-04-03 15:25:46.258303 x10_python_trading-0.1.1/x10/perpetual/trading_client/account_module.py
--rw-r--r--   0        0        0      636 2024-04-03 15:25:46.258303 x10_python_trading-0.1.1/x10/perpetual/trading_client/base_module.py
--rw-r--r--   0        0        0     1499 2024-04-03 15:25:46.258303 x10_python_trading-0.1.1/x10/perpetual/trading_client/markets_information_module.py
--rw-r--r--   0        0        0     2831 2024-04-03 15:25:46.258303 x10_python_trading-0.1.1/x10/perpetual/trading_client/order_management_module.py
--rw-r--r--   0        0        0     1138 2024-04-03 15:25:46.258303 x10_python_trading-0.1.1/x10/perpetual/trading_client/trading_client.py
--rw-r--r--   0        0        0        0 2024-04-03 15:25:46.258303 x10_python_trading-0.1.1/x10/utils/__init__.py
--rw-r--r--   0        0        0      246 2024-04-03 15:25:46.258303 x10_python_trading-0.1.1/x10/utils/date.py
--rw-r--r--   0        0        0     5649 2024-04-03 15:25:46.258303 x10_python_trading-0.1.1/x10/utils/http.py
--rw-r--r--   0        0        0       79 2024-04-03 15:25:46.258303 x10_python_trading-0.1.1/x10/utils/log.py
--rw-r--r--   0        0        0     2336 2024-04-03 15:25:46.258303 x10_python_trading-0.1.1/x10/utils/model.py
--rw-r--r--   0        0        0    14980 2024-04-03 15:25:46.258303 x10_python_trading-0.1.1/x10/utils/starkex.py
--rw-r--r--   0        0        0      275 2024-04-03 15:25:46.258303 x10_python_trading-0.1.1/x10/utils/string.py
--rw-r--r--   0        0        0     1748 1970-01-01 00:00:00.000000 x10_python_trading-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      794 2024-04-26 19:58:17.546355 x10_python_trading-0.1.2/README.md
+-rw-r--r--   0        0        0     1541 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/crypto/__init__.py
+-rw-r--r--   0        0        0     3945 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/crypto/signature/README.md
+-rw-r--r--   0        0        0        0 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/crypto/signature/__init__.py
+-rw-r--r--   0        0        0     1840 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/crypto/signature/fast_pedersen_hash.py
+-rw-r--r--   0        0        0     3627 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/crypto/signature/math_utils.py
+-rw-r--r--   0        0        0     6074 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/crypto/signature/nothing_up_my_sleeve_gen.py
+-rw-r--r--   0        0        0   102708 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/crypto/signature/pedersen_params.json
+-rw-r--r--   0        0        0    11728 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/crypto/signature/signature.py
+-rw-r--r--   0        0        0     3759 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/crypto/signature/src/config/assets_precomputed.json
+-rw-r--r--   0        0        0    70705 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/crypto/signature/src/config/constant_points.json
+-rw-r--r--   0        0        0     3701 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/crypto/signature/src/config/keys_precomputed.json
+-rw-r--r--   0        0        0     1955 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/python/BUILD
+-rw-r--r--   0        0        0       31 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/python/CMakeLists.txt
+-rw-r--r--   0        0        0     1254 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/python/CMakeLists_common.txt
+-rw-r--r--   0        0        0        0 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/python/__init__.py
+-rw-r--r--   0        0        0     1522 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/python/async_subprocess.py
+-rw-r--r--   0        0        0     5946 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/python/expression_string.py
+-rw-r--r--   0        0        0     1883 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/python/expression_string_test.py
+-rw-r--r--   0        0        0     3938 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/python/fixed_point.py
+-rw-r--r--   0        0        0      675 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/python/json_rpc/BUILD
+-rw-r--r--   0        0        0      359 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/python/json_rpc/CMakeLists.txt
+-rw-r--r--   0        0        0      812 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/python/json_rpc/client.py
+-rw-r--r--   0        0        0      681 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/python/json_rpc/client_test.py
+-rw-r--r--   0        0        0     8881 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/python/math_utils.py
+-rw-r--r--   0        0        0     5102 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/python/math_utils_test.py
+-rw-r--r--   0        0        0     1614 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/python/merkle_tree.py
+-rw-r--r--   0        0        0     1796 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/python/object_utils.py
+-rw-r--r--   0        0        0     1545 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/python/python_dependencies.py
+-rw-r--r--   0        0        0     6247 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/python/random_test.py
+-rw-r--r--   0        0        0     6247 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/python/random_test_utils.py
+-rw-r--r--   0        0        0     3460 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/python/test_utils.py
+-rw-r--r--   0        0        0     2783 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/python/test_utils_test.py
+-rw-r--r--   0        0        0    19817 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/python/utils.py
+-rw-r--r--   0        0        0      599 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/python/utils_stub_module.py
+-rw-r--r--   0        0        0     1554 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/python/utils_stub_module.pyi
+-rw-r--r--   0        0        0     7959 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/python/utils_test.py
+-rw-r--r--   0        0        0        0 2024-04-26 19:58:17.554355 x10_python_trading-0.1.2/x10/__init__.py
+-rw-r--r--   0        0        0      413 2024-04-26 19:58:17.554355 x10_python_trading-0.1.2/x10/config.py
+-rw-r--r--   0        0        0       36 2024-04-26 19:58:17.554355 x10_python_trading-0.1.2/x10/errors.py
+-rw-r--r--   0        0        0        0 2024-04-26 19:58:17.554355 x10_python_trading-0.1.2/x10/perpetual/__init__.py
+-rw-r--r--   0        0        0     1492 2024-04-26 19:58:17.554355 x10_python_trading-0.1.2/x10/perpetual/accounts.py
+-rw-r--r--   0        0        0     1618 2024-04-26 19:58:17.554355 x10_python_trading-0.1.2/x10/perpetual/amounts.py
+-rw-r--r--   0        0        0     1120 2024-04-26 19:58:17.554355 x10_python_trading-0.1.2/x10/perpetual/assets.py
+-rw-r--r--   0        0        0      347 2024-04-26 19:58:17.554355 x10_python_trading-0.1.2/x10/perpetual/balances.py
+-rw-r--r--   0        0        0      327 2024-04-26 19:58:17.554355 x10_python_trading-0.1.2/x10/perpetual/fees.py
+-rw-r--r--   0        0        0      459 2024-04-26 19:58:17.554355 x10_python_trading-0.1.2/x10/perpetual/funding_rates.py
+-rw-r--r--   0        0        0     2702 2024-04-26 19:58:17.554355 x10_python_trading-0.1.2/x10/perpetual/markets.py
+-rw-r--r--   0        0        0     5141 2024-04-26 19:58:17.554355 x10_python_trading-0.1.2/x10/perpetual/order_object.py
+-rw-r--r--   0        0        0      739 2024-04-26 19:58:17.554355 x10_python_trading-0.1.2/x10/perpetual/orderbooks.py
+-rw-r--r--   0        0        0     2207 2024-04-26 19:58:17.554355 x10_python_trading-0.1.2/x10/perpetual/orders.py
+-rw-r--r--   0        0        0     1069 2024-04-26 19:58:17.554355 x10_python_trading-0.1.2/x10/perpetual/positions.py
+-rw-r--r--   0        0        0       99 2024-04-26 19:58:17.554355 x10_python_trading-0.1.2/x10/perpetual/stream_client/__init__.py
+-rw-r--r--   0        0        0     2974 2024-04-26 19:58:17.554355 x10_python_trading-0.1.2/x10/perpetual/stream_client/perpetual_stream_connection.py
+-rw-r--r--   0        0        0     2497 2024-04-26 19:58:17.554355 x10_python_trading-0.1.2/x10/perpetual/stream_client/stream_client.py
+-rw-r--r--   0        0        0     1241 2024-04-26 19:58:17.554355 x10_python_trading-0.1.2/x10/perpetual/trades.py
+-rw-r--r--   0        0        0      102 2024-04-26 19:58:17.554355 x10_python_trading-0.1.2/x10/perpetual/trading_client/__init__.py
+-rw-r--r--   0        0        0     4303 2024-04-26 19:58:17.554355 x10_python_trading-0.1.2/x10/perpetual/trading_client/account_module.py
+-rw-r--r--   0        0        0      636 2024-04-26 19:58:17.554355 x10_python_trading-0.1.2/x10/perpetual/trading_client/base_module.py
+-rw-r--r--   0        0        0     1499 2024-04-26 19:58:17.554355 x10_python_trading-0.1.2/x10/perpetual/trading_client/markets_information_module.py
+-rw-r--r--   0        0        0     2831 2024-04-26 19:58:17.554355 x10_python_trading-0.1.2/x10/perpetual/trading_client/order_management_module.py
+-rw-r--r--   0        0        0     1138 2024-04-26 19:58:17.554355 x10_python_trading-0.1.2/x10/perpetual/trading_client/trading_client.py
+-rw-r--r--   0        0        0        0 2024-04-26 19:58:17.554355 x10_python_trading-0.1.2/x10/utils/__init__.py
+-rw-r--r--   0        0        0      246 2024-04-26 19:58:17.554355 x10_python_trading-0.1.2/x10/utils/date.py
+-rw-r--r--   0        0        0     5649 2024-04-26 19:58:17.554355 x10_python_trading-0.1.2/x10/utils/http.py
+-rw-r--r--   0        0        0       79 2024-04-26 19:58:17.554355 x10_python_trading-0.1.2/x10/utils/log.py
+-rw-r--r--   0        0        0     2336 2024-04-26 19:58:17.554355 x10_python_trading-0.1.2/x10/utils/model.py
+-rw-r--r--   0        0        0    14980 2024-04-26 19:58:17.554355 x10_python_trading-0.1.2/x10/utils/starkex.py
+-rw-r--r--   0        0        0      275 2024-04-26 19:58:17.554355 x10_python_trading-0.1.2/x10/utils/string.py
+-rw-r--r--   0        0        0     1748 1970-01-01 00:00:00.000000 x10_python_trading-0.1.2/PKG-INFO
```

### Comparing `x10_python_trading-0.1.1/README.md` & `x10_python_trading-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.1/pyproject.toml` & `x10_python_trading-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "x10-python-trading"
-version = "0.1.1"
+version = "0.1.2"
 description = "Python client for X10 API"
 authors = ["X10 <tech@ex10.org>"]
 packages = [
     { include = "starkware" },
     { include = "x10" },
 ]
 readme = "README.md"
```

### Comparing `x10_python_trading-0.1.1/starkware/crypto/signature/README.md` & `x10_python_trading-0.1.2/starkware/crypto/signature/README.md`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.1/starkware/crypto/signature/fast_pedersen_hash.py` & `x10_python_trading-0.1.2/starkware/crypto/signature/fast_pedersen_hash.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.1/starkware/crypto/signature/math_utils.py` & `x10_python_trading-0.1.2/starkware/crypto/signature/math_utils.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.1/starkware/crypto/signature/nothing_up_my_sleeve_gen.py` & `x10_python_trading-0.1.2/starkware/crypto/signature/nothing_up_my_sleeve_gen.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.1/starkware/crypto/signature/pedersen_params.json` & `x10_python_trading-0.1.2/starkware/crypto/signature/pedersen_params.json`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.1/starkware/crypto/signature/signature.py` & `x10_python_trading-0.1.2/starkware/crypto/signature/signature.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.1/starkware/crypto/signature/src/config/assets_precomputed.json` & `x10_python_trading-0.1.2/starkware/crypto/signature/src/config/assets_precomputed.json`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.1/starkware/crypto/signature/src/config/constant_points.json` & `x10_python_trading-0.1.2/starkware/crypto/signature/src/config/constant_points.json`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.1/starkware/crypto/signature/src/config/keys_precomputed.json` & `x10_python_trading-0.1.2/starkware/crypto/signature/src/config/keys_precomputed.json`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.1/starkware/python/BUILD` & `x10_python_trading-0.1.2/starkware/python/BUILD`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.1/starkware/python/CMakeLists_common.txt` & `x10_python_trading-0.1.2/starkware/python/CMakeLists_common.txt`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.1/starkware/python/async_subprocess.py` & `x10_python_trading-0.1.2/starkware/python/async_subprocess.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.1/starkware/python/expression_string.py` & `x10_python_trading-0.1.2/starkware/python/expression_string.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.1/starkware/python/expression_string_test.py` & `x10_python_trading-0.1.2/starkware/python/expression_string_test.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.1/starkware/python/fixed_point.py` & `x10_python_trading-0.1.2/starkware/python/fixed_point.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.1/starkware/python/json_rpc/BUILD` & `x10_python_trading-0.1.2/starkware/python/json_rpc/BUILD`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.1/starkware/python/json_rpc/client.py` & `x10_python_trading-0.1.2/starkware/python/json_rpc/client.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.1/starkware/python/json_rpc/client_test.py` & `x10_python_trading-0.1.2/starkware/python/json_rpc/client_test.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.1/starkware/python/math_utils.py` & `x10_python_trading-0.1.2/starkware/python/math_utils.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.1/starkware/python/math_utils_test.py` & `x10_python_trading-0.1.2/starkware/python/math_utils_test.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.1/starkware/python/merkle_tree.py` & `x10_python_trading-0.1.2/starkware/python/merkle_tree.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.1/starkware/python/object_utils.py` & `x10_python_trading-0.1.2/starkware/python/object_utils.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.1/starkware/python/python_dependencies.py` & `x10_python_trading-0.1.2/starkware/python/python_dependencies.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.1/starkware/python/random_test.py` & `x10_python_trading-0.1.2/starkware/python/random_test.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.1/starkware/python/random_test_utils.py` & `x10_python_trading-0.1.2/starkware/python/random_test_utils.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.1/starkware/python/test_utils.py` & `x10_python_trading-0.1.2/starkware/python/test_utils.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.1/starkware/python/test_utils_test.py` & `x10_python_trading-0.1.2/starkware/python/test_utils_test.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.1/starkware/python/utils.py` & `x10_python_trading-0.1.2/starkware/python/utils.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.1/starkware/python/utils_stub_module.py` & `x10_python_trading-0.1.2/starkware/python/utils_stub_module.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.1/starkware/python/utils_stub_module.pyi` & `x10_python_trading-0.1.2/starkware/python/utils_stub_module.pyi`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.1/starkware/python/utils_test.py` & `x10_python_trading-0.1.2/starkware/python/utils_test.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.1/x10/perpetual/accounts.py` & `x10_python_trading-0.1.2/x10/perpetual/accounts.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.1/x10/perpetual/amounts.py` & `x10_python_trading-0.1.2/x10/perpetual/amounts.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.1/x10/perpetual/assets.py` & `x10_python_trading-0.1.2/x10/perpetual/assets.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.1/x10/perpetual/markets.py` & `x10_python_trading-0.1.2/x10/perpetual/markets.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,20 @@
-from decimal import Decimal
+from decimal import ROUND_CEILING, Decimal
 from functools import cached_property
+from typing import List
 
 from x10.perpetual.assets import Asset
 from x10.utils.model import X10BaseModel
 
 
+class RiskFactorConfig(X10BaseModel):
+    upper_bound: Decimal
+    risk_factor: Decimal
+
+
 class MarketStatsModel(X10BaseModel):
     daily_volume: Decimal
     daily_volume_base: Decimal
     daily_price_change: Decimal
     daily_low: Decimal
     daily_high: Decimal
     last_price: Decimal
@@ -22,25 +28,28 @@
     open_interest_base: Decimal
 
 
 class TradingConfigModel(X10BaseModel):
     min_order_size: Decimal
     min_order_size_change: Decimal
     min_price_change: Decimal
-    max_market_order_size: Decimal
-    max_limit_order_size: Decimal
-    max_position_size: Decimal
+    max_market_order_value: Decimal
+    max_limit_order_value: Decimal
+    max_position_value: Decimal
     max_leverage: Decimal
-    base_risk_limit: Decimal
-    risk_step: Decimal
-    initial_margin_fraction: Decimal
-    incremental_initial_margin_fraction: Decimal
     max_num_orders: int
     limit_price_cap: Decimal
     limit_price_floor: Decimal
+    risk_factor_config: List[RiskFactorConfig]
+
+    def price_precision(self) -> int:
+        return abs(int(self.min_price_change.log10().to_integral_exact(ROUND_CEILING)))
+
+    def quantity_precision(self) -> int:
+        return abs(int(self.min_order_size_change.log10().to_integral_exact(ROUND_CEILING)))
 
 
 class L2ConfigModel(X10BaseModel):
     type: str
     collateral_id: str
     collateral_resolution: int
     synthetic_id: str
```

### Comparing `x10_python_trading-0.1.1/x10/perpetual/order_object.py` & `x10_python_trading-0.1.2/x10/perpetual/order_object.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.1/x10/perpetual/orderbooks.py` & `x10_python_trading-0.1.2/x10/perpetual/orderbooks.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.1/x10/perpetual/orders.py` & `x10_python_trading-0.1.2/x10/perpetual/orders.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.1/x10/perpetual/positions.py` & `x10_python_trading-0.1.2/x10/perpetual/positions.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.1/x10/perpetual/stream_client/perpetual_stream_connection.py` & `x10_python_trading-0.1.2/x10/perpetual/stream_client/perpetual_stream_connection.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.1/x10/perpetual/stream_client/stream_client.py` & `x10_python_trading-0.1.2/x10/perpetual/stream_client/stream_client.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.1/x10/perpetual/trades.py` & `x10_python_trading-0.1.2/x10/perpetual/trades.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.1/x10/perpetual/trading_client/account_module.py` & `x10_python_trading-0.1.2/x10/perpetual/trading_client/account_module.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.1/x10/perpetual/trading_client/base_module.py` & `x10_python_trading-0.1.2/x10/perpetual/trading_client/base_module.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.1/x10/perpetual/trading_client/markets_information_module.py` & `x10_python_trading-0.1.2/x10/perpetual/trading_client/markets_information_module.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.1/x10/perpetual/trading_client/order_management_module.py` & `x10_python_trading-0.1.2/x10/perpetual/trading_client/order_management_module.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.1/x10/perpetual/trading_client/trading_client.py` & `x10_python_trading-0.1.2/x10/perpetual/trading_client/trading_client.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.1/x10/utils/http.py` & `x10_python_trading-0.1.2/x10/utils/http.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.1/x10/utils/model.py` & `x10_python_trading-0.1.2/x10/utils/model.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.1/x10/utils/starkex.py` & `x10_python_trading-0.1.2/x10/utils/starkex.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.1/PKG-INFO` & `x10_python_trading-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: x10-python-trading
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python client for X10 API
 Author: X10
 Author-email: tech@ex10.org
 Requires-Python: >=3.10,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

