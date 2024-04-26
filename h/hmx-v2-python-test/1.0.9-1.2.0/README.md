# Comparing `tmp/hmx-v2-python-test-1.0.9.tar.gz` & `tmp/hmx_v2_python_test-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hmx-v2-python-test-1.0.9.tar", last modified: Tue Mar 19 09:07:35 2024, max compression
+gzip compressed data, was "hmx_v2_python_test-1.2.0.tar", last modified: Fri Apr 26 19:09:44 2024, max compression
```

## Comparing `hmx-v2-python-test-1.0.9.tar` & `hmx_v2_python_test-1.2.0.tar`

### file list

```diff
@@ -1,74 +1,81 @@
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2024-03-19 09:07:35.310321 hmx-v2-python-test-1.0.9/
--rw-r--r--   0 lemon      (501) staff       (20)     1064 2023-11-29 08:33:18.000000 hmx-v2-python-test-1.0.9/LICENSE
--rw-r--r--   0 lemon      (501) staff       (20)     4561 2024-03-19 09:07:35.310270 hmx-v2-python-test-1.0.9/PKG-INFO
--rw-r--r--   0 lemon      (501) staff       (20)     3313 2024-03-19 06:20:57.000000 hmx-v2-python-test-1.0.9/README.md
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2024-03-19 09:07:35.303628 hmx-v2-python-test-1.0.9/hmx2/
--rw-r--r--   0 lemon      (501) staff       (20)       35 2023-11-29 08:33:18.000000 hmx-v2-python-test-1.0.9/hmx2/__init__.py
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2024-03-19 09:07:35.305213 hmx-v2-python-test-1.0.9/hmx2/abis/
--rw-r--r--   0 lemon      (501) staff       (20)     6094 2023-12-04 03:01:37.000000 hmx-v2-python-test-1.0.9/hmx2/abis/CIXPriceAdapter.json
--rw-r--r--   0 lemon      (501) staff       (20)    19788 2024-03-07 09:18:43.000000 hmx-v2-python-test-1.0.9/hmx2/abis/Calculator.json
--rw-r--r--   0 lemon      (501) staff       (20)    79531 2023-11-30 06:22:23.000000 hmx-v2-python-test-1.0.9/hmx2/abis/ConfigStorage.json
--rw-r--r--   0 lemon      (501) staff       (20)    23809 2024-03-05 11:40:21.000000 hmx-v2-python-test-1.0.9/hmx2/abis/CrossMarginHandler.json
--rw-r--r--   0 lemon      (501) staff       (20)     3685 2023-11-29 08:33:18.000000 hmx-v2-python-test-1.0.9/hmx2/abis/ERC20.json
--rw-r--r--   0 lemon      (501) staff       (20)    11832 2023-11-29 08:33:18.000000 hmx-v2-python-test-1.0.9/hmx2/abis/GlpManager.json
--rw-r--r--   0 lemon      (501) staff       (20)     5780 2023-12-04 03:01:37.000000 hmx-v2-python-test-1.0.9/hmx2/abis/GmPriceAdapter.json
--rw-r--r--   0 lemon      (501) staff       (20)    47380 2023-11-29 08:33:18.000000 hmx-v2-python-test-1.0.9/hmx2/abis/LimitTradeHandler.json
--rw-r--r--   0 lemon      (501) staff       (20)     2419 2024-01-18 07:42:57.000000 hmx-v2-python-test-1.0.9/hmx2/abis/OnchainPricelens.json
--rw-r--r--   0 lemon      (501) staff       (20)    26127 2023-11-29 10:08:35.000000 hmx-v2-python-test-1.0.9/hmx2/abis/PerpStorage.json
--rw-r--r--   0 lemon      (501) staff       (20)    27073 2024-01-30 10:28:55.000000 hmx-v2-python-test-1.0.9/hmx2/abis/TradeHelper.json
--rw-r--r--   0 lemon      (501) staff       (20)    24329 2023-11-29 08:33:18.000000 hmx-v2-python-test-1.0.9/hmx2/abis/VaultStorage.json
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2024-03-19 09:07:35.306047 hmx-v2-python-test-1.0.9/hmx2/constants/
--rw-r--r--   0 lemon      (501) staff       (20)       97 2024-03-19 05:22:30.000000 hmx-v2-python-test-1.0.9/hmx2/constants/__init__.py
--rw-r--r--   0 lemon      (501) staff       (20)     1917 2024-03-19 05:01:07.000000 hmx-v2-python-test-1.0.9/hmx2/constants/assets.py
--rw-r--r--   0 lemon      (501) staff       (20)      294 2024-03-19 05:01:07.000000 hmx-v2-python-test-1.0.9/hmx2/constants/common.py
--rw-r--r--   0 lemon      (501) staff       (20)     1700 2024-03-19 05:01:07.000000 hmx-v2-python-test-1.0.9/hmx2/constants/contracts.py
--rw-r--r--   0 lemon      (501) staff       (20)     7052 2024-03-19 05:01:07.000000 hmx-v2-python-test-1.0.9/hmx2/constants/markets.py
--rw-r--r--   0 lemon      (501) staff       (20)    10357 2024-03-19 05:01:07.000000 hmx-v2-python-test-1.0.9/hmx2/constants/pricefeed.py
--rw-r--r--   0 lemon      (501) staff       (20)     4970 2024-03-19 06:01:14.000000 hmx-v2-python-test-1.0.9/hmx2/constants/tokens.py
--rw-r--r--   0 lemon      (501) staff       (20)      118 2023-11-29 08:33:18.000000 hmx-v2-python-test-1.0.9/hmx2/enum.py
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2024-03-19 09:07:35.306456 hmx-v2-python-test-1.0.9/hmx2/helpers/
--rw-r--r--   0 lemon      (501) staff       (20)        0 2023-11-29 08:33:18.000000 hmx-v2-python-test-1.0.9/hmx2/helpers/__init__.py
--rw-r--r--   0 lemon      (501) staff       (20)      347 2023-11-29 08:33:18.000000 hmx-v2-python-test-1.0.9/hmx2/helpers/contract_loader.py
--rw-r--r--   0 lemon      (501) staff       (20)      519 2024-03-19 05:01:07.000000 hmx-v2-python-test-1.0.9/hmx2/helpers/mapper.py
--rw-r--r--   0 lemon      (501) staff       (20)      448 2024-03-19 05:01:07.000000 hmx-v2-python-test-1.0.9/hmx2/helpers/util.py
--rw-r--r--   0 lemon      (501) staff       (20)     2771 2024-03-19 05:01:07.000000 hmx-v2-python-test-1.0.9/hmx2/hmx_client.py
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2024-03-19 09:07:35.306810 hmx-v2-python-test-1.0.9/hmx2/modules/
--rw-r--r--   0 lemon      (501) staff       (20)        0 2023-11-29 08:33:18.000000 hmx-v2-python-test-1.0.9/hmx2/modules/__init__.py
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2024-03-19 09:07:35.307045 hmx-v2-python-test-1.0.9/hmx2/modules/calculator/
--rw-r--r--   0 lemon      (501) staff       (20)        0 2023-11-29 08:33:18.000000 hmx-v2-python-test-1.0.9/hmx2/modules/calculator/__init__.py
--rw-r--r--   0 lemon      (501) staff       (20)     6048 2024-03-19 05:01:07.000000 hmx-v2-python-test-1.0.9/hmx2/modules/calculator/calculator.py
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2024-03-19 09:07:35.307263 hmx-v2-python-test-1.0.9/hmx2/modules/oracle/
--rw-r--r--   0 lemon      (501) staff       (20)       48 2023-11-29 08:33:18.000000 hmx-v2-python-test-1.0.9/hmx2/modules/oracle/__init__.py
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2024-03-19 09:07:35.307485 hmx-v2-python-test-1.0.9/hmx2/modules/oracle/cix_oracle/
--rw-r--r--   0 lemon      (501) staff       (20)       34 2023-12-04 03:01:37.000000 hmx-v2-python-test-1.0.9/hmx2/modules/oracle/cix_oracle/__init__.py
--rw-r--r--   0 lemon      (501) staff       (20)     1315 2024-03-19 05:01:07.000000 hmx-v2-python-test-1.0.9/hmx2/modules/oracle/cix_oracle/cix_oracle.py
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2024-03-19 09:07:35.307709 hmx-v2-python-test-1.0.9/hmx2/modules/oracle/glp_oracle/
--rw-r--r--   0 lemon      (501) staff       (20)       34 2023-11-29 08:33:18.000000 hmx-v2-python-test-1.0.9/hmx2/modules/oracle/glp_oracle/__init__.py
--rw-r--r--   0 lemon      (501) staff       (20)     1003 2024-03-19 05:01:07.000000 hmx-v2-python-test-1.0.9/hmx2/modules/oracle/glp_oracle/glp_oracle.py
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2024-03-19 09:07:35.307927 hmx-v2-python-test-1.0.9/hmx2/modules/oracle/gm_oracle/
--rw-r--r--   0 lemon      (501) staff       (20)       32 2023-12-04 03:01:37.000000 hmx-v2-python-test-1.0.9/hmx2/modules/oracle/gm_oracle/__init__.py
--rw-r--r--   0 lemon      (501) staff       (20)     1169 2024-03-19 05:01:07.000000 hmx-v2-python-test-1.0.9/hmx2/modules/oracle/gm_oracle/gm_oracle.py
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2024-03-19 09:07:35.308147 hmx-v2-python-test-1.0.9/hmx2/modules/oracle/onchain_pricelens_oracle/
--rw-r--r--   0 lemon      (501) staff       (20)       59 2024-01-18 07:42:57.000000 hmx-v2-python-test-1.0.9/hmx2/modules/oracle/onchain_pricelens_oracle/__init__.py
--rw-r--r--   0 lemon      (501) staff       (20)      788 2024-03-19 05:01:07.000000 hmx-v2-python-test-1.0.9/hmx2/modules/oracle/onchain_pricelens_oracle/onchain_pricelen_oracle.py
--rw-r--r--   0 lemon      (501) staff       (20)     3180 2024-03-19 05:01:07.000000 hmx-v2-python-test-1.0.9/hmx2/modules/oracle/oracle_middleware.py
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2024-03-19 09:07:35.308373 hmx-v2-python-test-1.0.9/hmx2/modules/oracle/pyth_oracle/
--rw-r--r--   0 lemon      (501) staff       (20)       36 2023-11-29 08:33:18.000000 hmx-v2-python-test-1.0.9/hmx2/modules/oracle/pyth_oracle/__init__.py
--rw-r--r--   0 lemon      (501) staff       (20)     1302 2024-03-19 05:01:07.000000 hmx-v2-python-test-1.0.9/hmx2/modules/oracle/pyth_oracle/pyth_oracle.py
--rw-r--r--   0 lemon      (501) staff       (20)    15118 2024-03-19 05:01:07.000000 hmx-v2-python-test-1.0.9/hmx2/modules/private.py
--rw-r--r--   0 lemon      (501) staff       (20)    27327 2024-03-19 05:01:07.000000 hmx-v2-python-test-1.0.9/hmx2/modules/public.py
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2024-03-19 09:07:35.310042 hmx-v2-python-test-1.0.9/hmx_v2_python_test.egg-info/
--rw-r--r--   0 lemon      (501) staff       (20)     4561 2024-03-19 09:07:35.000000 hmx-v2-python-test-1.0.9/hmx_v2_python_test.egg-info/PKG-INFO
--rw-r--r--   0 lemon      (501) staff       (20)     1777 2024-03-19 09:07:35.000000 hmx-v2-python-test-1.0.9/hmx_v2_python_test.egg-info/SOURCES.txt
--rw-r--r--   0 lemon      (501) staff       (20)        1 2024-03-19 09:07:35.000000 hmx-v2-python-test-1.0.9/hmx_v2_python_test.egg-info/dependency_links.txt
--rw-r--r--   0 lemon      (501) staff       (20)      154 2024-03-19 09:07:35.000000 hmx-v2-python-test-1.0.9/hmx_v2_python_test.egg-info/requires.txt
--rw-r--r--   0 lemon      (501) staff       (20)       11 2024-03-19 09:07:35.000000 hmx-v2-python-test-1.0.9/hmx_v2_python_test.egg-info/top_level.txt
--rw-r--r--   0 lemon      (501) staff       (20)       79 2024-03-19 09:07:35.310507 hmx-v2-python-test-1.0.9/setup.cfg
--rw-r--r--   0 lemon      (501) staff       (20)     1461 2024-03-19 09:07:30.000000 hmx-v2-python-test-1.0.9/setup.py
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2024-03-19 09:07:35.309781 hmx-v2-python-test-1.0.9/tests/
--rw-r--r--   0 lemon      (501) staff       (20)       46 2023-11-29 08:33:18.000000 hmx-v2-python-test-1.0.9/tests/__init__.py
--rw-r--r--   0 lemon      (501) staff       (20)     5934 2024-03-19 05:01:07.000000 hmx-v2-python-test-1.0.9/tests/constants.py
--rw-r--r--   0 lemon      (501) staff       (20)     3117 2024-03-19 06:47:03.000000 hmx-v2-python-test-1.0.9/tests/test_create_market_order.py
--rw-r--r--   0 lemon      (501) staff       (20)     5393 2024-03-19 06:46:47.000000 hmx-v2-python-test-1.0.9/tests/test_deposit_collateral.py
--rw-r--r--   0 lemon      (501) staff       (20)     1307 2024-03-19 05:01:07.000000 hmx-v2-python-test-1.0.9/tests/test_get_adaptive_fee.py
--rw-r--r--   0 lemon      (501) staff       (20)     1221 2023-11-30 06:57:41.000000 hmx-v2-python-test-1.0.9/tests/test_init.py
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2024-04-26 19:09:44.518584 hmx_v2_python_test-1.2.0/
+-rw-r--r--   0 lemon      (501) staff       (20)     1064 2023-11-29 08:33:18.000000 hmx_v2_python_test-1.2.0/LICENSE
+-rw-r--r--   0 lemon      (501) staff       (20)     4642 2024-04-26 19:09:44.518509 hmx_v2_python_test-1.2.0/PKG-INFO
+-rw-r--r--   0 lemon      (501) staff       (20)     3361 2024-04-17 06:37:55.000000 hmx_v2_python_test-1.2.0/README.md
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2024-04-26 19:09:44.506010 hmx_v2_python_test-1.2.0/hmx2/
+-rw-r--r--   0 lemon      (501) staff       (20)       35 2023-11-29 08:33:18.000000 hmx_v2_python_test-1.2.0/hmx2/__init__.py
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2024-04-26 19:09:44.509275 hmx_v2_python_test-1.2.0/hmx2/abis/
+-rw-r--r--   0 lemon      (501) staff       (20)     2918 2024-04-25 10:13:28.000000 hmx_v2_python_test-1.2.0/hmx2/abis/AdaptiveFeeCalculator.json
+-rw-r--r--   0 lemon      (501) staff       (20)     6094 2023-12-04 03:01:37.000000 hmx_v2_python_test-1.2.0/hmx2/abis/CIXPriceAdapter.json
+-rw-r--r--   0 lemon      (501) staff       (20)     3332 2024-04-26 06:57:27.000000 hmx_v2_python_test-1.2.0/hmx2/abis/CalcPricelens.json
+-rw-r--r--   0 lemon      (501) staff       (20)    19788 2024-03-07 09:18:43.000000 hmx_v2_python_test-1.2.0/hmx2/abis/Calculator.json
+-rw-r--r--   0 lemon      (501) staff       (20)    79643 2024-04-25 10:13:28.000000 hmx_v2_python_test-1.2.0/hmx2/abis/ConfigStorage.json
+-rw-r--r--   0 lemon      (501) staff       (20)    23809 2024-03-05 11:40:21.000000 hmx_v2_python_test-1.2.0/hmx2/abis/CrossMarginHandler.json
+-rw-r--r--   0 lemon      (501) staff       (20)     3685 2023-11-29 08:33:18.000000 hmx_v2_python_test-1.2.0/hmx2/abis/ERC20.json
+-rw-r--r--   0 lemon      (501) staff       (20)    11832 2023-11-29 08:33:18.000000 hmx_v2_python_test-1.2.0/hmx2/abis/GlpManager.json
+-rw-r--r--   0 lemon      (501) staff       (20)     5780 2023-12-04 03:01:37.000000 hmx_v2_python_test-1.2.0/hmx2/abis/GmPriceAdapter.json
+-rw-r--r--   0 lemon      (501) staff       (20)    47380 2023-11-29 08:33:18.000000 hmx_v2_python_test-1.2.0/hmx2/abis/LimitTradeHandler.json
+-rw-r--r--   0 lemon      (501) staff       (20)     2419 2024-01-18 07:42:57.000000 hmx_v2_python_test-1.2.0/hmx2/abis/OnchainPricelens.json
+-rw-r--r--   0 lemon      (501) staff       (20)     6721 2024-04-25 10:13:28.000000 hmx_v2_python_test-1.2.0/hmx2/abis/OrderbookOracle.json
+-rw-r--r--   0 lemon      (501) staff       (20)    26489 2024-04-25 10:13:28.000000 hmx_v2_python_test-1.2.0/hmx2/abis/PerpStorage.json
+-rw-r--r--   0 lemon      (501) staff       (20)    27073 2024-01-30 10:28:55.000000 hmx_v2_python_test-1.2.0/hmx2/abis/TradeHelper.json
+-rw-r--r--   0 lemon      (501) staff       (20)    24329 2023-11-29 08:33:18.000000 hmx_v2_python_test-1.2.0/hmx2/abis/VaultStorage.json
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2024-04-26 19:09:44.510736 hmx_v2_python_test-1.2.0/hmx2/constants/
+-rw-r--r--   0 lemon      (501) staff       (20)      107 2024-04-24 05:28:38.000000 hmx_v2_python_test-1.2.0/hmx2/constants/__init__.py
+-rw-r--r--   0 lemon      (501) staff       (20)     2126 2024-04-26 06:57:27.000000 hmx_v2_python_test-1.2.0/hmx2/constants/assets.py
+-rw-r--r--   0 lemon      (501) staff       (20)      397 2024-04-26 11:31:42.000000 hmx_v2_python_test-1.2.0/hmx2/constants/common.py
+-rw-r--r--   0 lemon      (501) staff       (20)     3265 2024-04-26 12:30:21.000000 hmx_v2_python_test-1.2.0/hmx2/constants/contracts.py
+-rw-r--r--   0 lemon      (501) staff       (20)       52 2024-04-24 05:28:38.000000 hmx_v2_python_test-1.2.0/hmx2/constants/intent.py
+-rw-r--r--   0 lemon      (501) staff       (20)    14585 2024-04-26 06:57:27.000000 hmx_v2_python_test-1.2.0/hmx2/constants/markets.py
+-rw-r--r--   0 lemon      (501) staff       (20)    20697 2024-04-26 06:57:27.000000 hmx_v2_python_test-1.2.0/hmx2/constants/pricefeed.py
+-rw-r--r--   0 lemon      (501) staff       (20)    13032 2024-04-26 12:19:57.000000 hmx_v2_python_test-1.2.0/hmx2/constants/tokens.py
+-rw-r--r--   0 lemon      (501) staff       (20)      237 2024-04-24 05:28:38.000000 hmx_v2_python_test-1.2.0/hmx2/enum.py
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2024-04-26 19:09:44.511456 hmx_v2_python_test-1.2.0/hmx2/helpers/
+-rw-r--r--   0 lemon      (501) staff       (20)        0 2023-11-29 08:33:18.000000 hmx_v2_python_test-1.2.0/hmx2/helpers/__init__.py
+-rw-r--r--   0 lemon      (501) staff       (20)      347 2024-04-25 10:10:59.000000 hmx_v2_python_test-1.2.0/hmx2/helpers/contract_loader.py
+-rw-r--r--   0 lemon      (501) staff       (20)      900 2024-04-26 12:20:30.000000 hmx_v2_python_test-1.2.0/hmx2/helpers/mapper.py
+-rw-r--r--   0 lemon      (501) staff       (20)      917 2024-04-26 06:57:27.000000 hmx_v2_python_test-1.2.0/hmx2/helpers/util.py
+-rw-r--r--   0 lemon      (501) staff       (20)     3002 2024-04-26 06:57:27.000000 hmx_v2_python_test-1.2.0/hmx2/hmx_client.py
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2024-04-26 19:09:44.511964 hmx_v2_python_test-1.2.0/hmx2/modules/
+-rw-r--r--   0 lemon      (501) staff       (20)        0 2023-11-29 08:33:18.000000 hmx_v2_python_test-1.2.0/hmx2/modules/__init__.py
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2024-04-26 19:09:44.512314 hmx_v2_python_test-1.2.0/hmx2/modules/calculator/
+-rw-r--r--   0 lemon      (501) staff       (20)        0 2023-11-29 08:33:18.000000 hmx_v2_python_test-1.2.0/hmx2/modules/calculator/__init__.py
+-rw-r--r--   0 lemon      (501) staff       (20)     8423 2024-04-25 10:13:28.000000 hmx_v2_python_test-1.2.0/hmx2/modules/calculator/calculator.py
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2024-04-26 19:09:44.512767 hmx_v2_python_test-1.2.0/hmx2/modules/oracle/
+-rw-r--r--   0 lemon      (501) staff       (20)       48 2023-11-29 08:33:18.000000 hmx_v2_python_test-1.2.0/hmx2/modules/oracle/__init__.py
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2024-04-26 19:09:44.513365 hmx_v2_python_test-1.2.0/hmx2/modules/oracle/calc_pricelens_oracle/
+-rw-r--r--   0 lemon      (501) staff       (20)       55 2024-04-26 06:57:27.000000 hmx_v2_python_test-1.2.0/hmx2/modules/oracle/calc_pricelens_oracle/__init__.py
+-rw-r--r--   0 lemon      (501) staff       (20)     1209 2024-04-26 12:21:29.000000 hmx_v2_python_test-1.2.0/hmx2/modules/oracle/calc_pricelens_oracle/calc_pricelens_oracle.py
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2024-04-26 19:09:44.513712 hmx_v2_python_test-1.2.0/hmx2/modules/oracle/cix_oracle/
+-rw-r--r--   0 lemon      (501) staff       (20)       34 2023-12-04 03:01:37.000000 hmx_v2_python_test-1.2.0/hmx2/modules/oracle/cix_oracle/__init__.py
+-rw-r--r--   0 lemon      (501) staff       (20)     1315 2024-03-19 05:01:07.000000 hmx_v2_python_test-1.2.0/hmx2/modules/oracle/cix_oracle/cix_oracle.py
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2024-04-26 19:09:44.514043 hmx_v2_python_test-1.2.0/hmx2/modules/oracle/glp_oracle/
+-rw-r--r--   0 lemon      (501) staff       (20)       34 2023-11-29 08:33:18.000000 hmx_v2_python_test-1.2.0/hmx2/modules/oracle/glp_oracle/__init__.py
+-rw-r--r--   0 lemon      (501) staff       (20)     1428 2024-04-25 10:13:28.000000 hmx_v2_python_test-1.2.0/hmx2/modules/oracle/glp_oracle/glp_oracle.py
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2024-04-26 19:09:44.514554 hmx_v2_python_test-1.2.0/hmx2/modules/oracle/gm_oracle/
+-rw-r--r--   0 lemon      (501) staff       (20)       32 2023-12-04 03:01:37.000000 hmx_v2_python_test-1.2.0/hmx2/modules/oracle/gm_oracle/__init__.py
+-rw-r--r--   0 lemon      (501) staff       (20)     1169 2024-03-19 05:01:07.000000 hmx_v2_python_test-1.2.0/hmx2/modules/oracle/gm_oracle/gm_oracle.py
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2024-04-26 19:09:44.514995 hmx_v2_python_test-1.2.0/hmx2/modules/oracle/onchain_pricelens_oracle/
+-rw-r--r--   0 lemon      (501) staff       (20)       59 2024-01-18 07:42:57.000000 hmx_v2_python_test-1.2.0/hmx2/modules/oracle/onchain_pricelens_oracle/__init__.py
+-rw-r--r--   0 lemon      (501) staff       (20)      788 2024-03-19 05:01:07.000000 hmx_v2_python_test-1.2.0/hmx2/modules/oracle/onchain_pricelens_oracle/onchain_pricelen_oracle.py
+-rw-r--r--   0 lemon      (501) staff       (20)     3980 2024-04-26 11:30:15.000000 hmx_v2_python_test-1.2.0/hmx2/modules/oracle/oracle_middleware.py
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2024-04-26 19:09:44.515388 hmx_v2_python_test-1.2.0/hmx2/modules/oracle/pyth_oracle/
+-rw-r--r--   0 lemon      (501) staff       (20)       36 2023-11-29 08:33:18.000000 hmx_v2_python_test-1.2.0/hmx2/modules/oracle/pyth_oracle/__init__.py
+-rw-r--r--   0 lemon      (501) staff       (20)     1302 2024-03-19 05:01:07.000000 hmx_v2_python_test-1.2.0/hmx2/modules/oracle/pyth_oracle/pyth_oracle.py
+-rw-r--r--   0 lemon      (501) staff       (20)    19710 2024-04-26 12:39:24.000000 hmx_v2_python_test-1.2.0/hmx2/modules/private.py
+-rw-r--r--   0 lemon      (501) staff       (20)    41148 2024-04-26 11:50:34.000000 hmx_v2_python_test-1.2.0/hmx2/modules/public.py
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2024-04-26 19:09:44.518034 hmx_v2_python_test-1.2.0/hmx_v2_python_test.egg-info/
+-rw-r--r--   0 lemon      (501) staff       (20)     4642 2024-04-26 19:09:44.000000 hmx_v2_python_test-1.2.0/hmx_v2_python_test.egg-info/PKG-INFO
+-rw-r--r--   0 lemon      (501) staff       (20)     2020 2024-04-26 19:09:44.000000 hmx_v2_python_test-1.2.0/hmx_v2_python_test.egg-info/SOURCES.txt
+-rw-r--r--   0 lemon      (501) staff       (20)        1 2024-04-26 19:09:44.000000 hmx_v2_python_test-1.2.0/hmx_v2_python_test.egg-info/dependency_links.txt
+-rw-r--r--   0 lemon      (501) staff       (20)      172 2024-04-26 19:09:44.000000 hmx_v2_python_test-1.2.0/hmx_v2_python_test.egg-info/requires.txt
+-rw-r--r--   0 lemon      (501) staff       (20)       11 2024-04-26 19:09:44.000000 hmx_v2_python_test-1.2.0/hmx_v2_python_test.egg-info/top_level.txt
+-rw-r--r--   0 lemon      (501) staff       (20)       79 2024-04-26 19:09:44.518855 hmx_v2_python_test-1.2.0/setup.cfg
+-rw-r--r--   0 lemon      (501) staff       (20)     1486 2024-04-26 19:06:55.000000 hmx_v2_python_test-1.2.0/setup.py
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2024-04-26 19:09:44.517692 hmx_v2_python_test-1.2.0/tests/
+-rw-r--r--   0 lemon      (501) staff       (20)       46 2023-11-29 08:33:18.000000 hmx_v2_python_test-1.2.0/tests/__init__.py
+-rw-r--r--   0 lemon      (501) staff       (20)     5934 2024-03-19 05:01:07.000000 hmx_v2_python_test-1.2.0/tests/constants.py
+-rw-r--r--   0 lemon      (501) staff       (20)     3117 2024-04-02 05:22:20.000000 hmx_v2_python_test-1.2.0/tests/test_create_market_order.py
+-rw-r--r--   0 lemon      (501) staff       (20)     5522 2024-04-17 06:38:11.000000 hmx_v2_python_test-1.2.0/tests/test_deposit_collateral.py
+-rw-r--r--   0 lemon      (501) staff       (20)     1307 2024-03-19 05:01:07.000000 hmx_v2_python_test-1.2.0/tests/test_get_adaptive_fee.py
+-rw-r--r--   0 lemon      (501) staff       (20)     1221 2023-11-30 06:57:41.000000 hmx_v2_python_test-1.2.0/tests/test_init.py
```

### Comparing `hmx-v2-python-test-1.0.9/LICENSE` & `hmx_v2_python_test-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-test-1.0.9/PKG-INFO` & `hmx_v2_python_test-1.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hmx-v2-python-test
-Version: 1.0.9
+Version: 1.2.0
 Summary: HMXv2 Python SDK
 Home-page: https://github.com/HMXOrg/v2-sdk-python
 Author: HMXOrg
 Author-email: contact@hmx.org
 License: MIT
 Keywords: hmx exchange perp dex defi ethereum eth arbitrum
 Classifier: Intended Audience :: Developers
@@ -19,21 +19,22 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: eth_keys
-Requires-Dist: eth-account==0.11.0
+Requires-Dist: eth-account==0.10.0
 Requires-Dist: eth-abi<5.0.0,>=4.0.0
 Requires-Dist: uniswap-universal-router-decoder
 Requires-Dist: web3<7.0.0,>=6.0.0
 Requires-Dist: simple-multicall-v6
 Requires-Dist: responses
 Requires-Dist: python-dotenv>=1.0.0
+Requires-Dist: secp256k1==0.14.0
 
 # Python SDK for HMXv2
 
 This library is tested against Python versions 2.7, 3.4, 3.5, 3.9, and 3.11.
 
 ## Installation
 
@@ -57,23 +58,23 @@
 #
 # Using publicly access functions
 #
 hmx_client = Client(
     rpc_url=RPC_URL
 )
 # Get oracle price, adaptive price, and price impact of a new position
-client.public.get_price(MARKET_ETH_USD, Action.SELL, 1000)
+hmx_client.public.get_price(MARKET_ETH_USD, Action.SELL, 1000)
 # Get market information
-client.public.get_market_info(MARKET_ETH_USD)
+hmx_client.public.get_market_info(MARKET_ETH_USD)
 # Get sub account in address format
-client.public.get_sub_account(1)
+hmx_client.public.get_sub_account(1)
 # Get position ID
-client.public.get_position_id(some_account, some_sub_account_id, MARKET_ETH_USD)
+hmx_client.public.get_position_id(some_account, some_sub_account_id, MARKET_ETH_USD)
 # Get position info
-client.public.get_position_info(some_account, some_sub_account_id, MARKET_ETH_USD)
+hmx_client.public.get_position_info(some_account, some_sub_account_id, MARKET_ETH_USD)
 ```
 
 ### Private function
 
 ```python
 from hmx2.hmx_client import Client
 from hmx2.constants.markets import MARKET_ETH_USD
@@ -84,43 +85,43 @@
 # Initailized client with private key
 #
 hmx_client = Client(
     eth_private_key=PRIVATE_KEY,
     rpc_url=RPC_URL
 )
 # Get public address of the ethereum key
-client.private.get_public_address()
+hmx_client.private.get_public_address()
 # Deposit ETH as collateral
-client.private.deposit_eth_collateral(sub_account_id=0, amount=10.123)
+hmx_client.private.deposit_eth_collateral(sub_account_id=0, amount=10.123)
 # Deposit ERC20 as collateral. This function will automatically
 # approve CrossMarginHandler if needed.
-client.private.deposit_erc20_collateral(sub_account_id=0, token_address=COLLATERAL_USDCe, amount=100.10)
+hmx_client.private.deposit_erc20_collateral(sub_account_id=0, token_address=COLLATERAL_USDCe, amount=100.10)
 # Create a market order
-create_market_order = client.private.create_market_order(
+create_market_order = hmx_client.private.create_market_order(
   sub_account_id=0, market_index=MARKET_ETH_USD, buy=Action.BUY, size=100, reduce_only=False
 )
 print(create_market_order)
 # Create a trigger order
 # trigger_above_threshold = The current price must go above (if True) or below (if False)
 # the trigger price in order for the order to be executed
-create_order = client.private.create_trigger_order(
+create_order = hmx_client.private.create_trigger_order(
   sub_account_id=0,
   market_index=MARKET_ETH_USD,
   buy=Action.BUY,
   size=100,
   trigger_price=1800,
   trigger_above_threshold=True,
   reduce_only=False)
 print(create_order)
 # Update the order
-update_order = client.private.update_trigger_order(
+update_order = hmx_client.private.update_trigger_order(
   0, create_order["order"]["orderIndex"], Action.SELL, 50, 1700, True, False)
 print(update_order)
 # Cancel the order
-cancel_order = client.private.cancel_trigger_order(
+cancel_order = hmx_client.private.cancel_trigger_order(
   0, update_order["order"]["orderIndex"])
 ```
 
 ## Running Tests
 
 To run tests, you will need have to clone the repo, update .env, and run:
```

### Comparing `hmx-v2-python-test-1.0.9/README.md` & `hmx_v2_python_test-1.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -24,23 +24,23 @@
 #
 # Using publicly access functions
 #
 hmx_client = Client(
     rpc_url=RPC_URL
 )
 # Get oracle price, adaptive price, and price impact of a new position
-client.public.get_price(MARKET_ETH_USD, Action.SELL, 1000)
+hmx_client.public.get_price(MARKET_ETH_USD, Action.SELL, 1000)
 # Get market information
-client.public.get_market_info(MARKET_ETH_USD)
+hmx_client.public.get_market_info(MARKET_ETH_USD)
 # Get sub account in address format
-client.public.get_sub_account(1)
+hmx_client.public.get_sub_account(1)
 # Get position ID
-client.public.get_position_id(some_account, some_sub_account_id, MARKET_ETH_USD)
+hmx_client.public.get_position_id(some_account, some_sub_account_id, MARKET_ETH_USD)
 # Get position info
-client.public.get_position_info(some_account, some_sub_account_id, MARKET_ETH_USD)
+hmx_client.public.get_position_info(some_account, some_sub_account_id, MARKET_ETH_USD)
 ```
 
 ### Private function
 
 ```python
 from hmx2.hmx_client import Client
 from hmx2.constants.markets import MARKET_ETH_USD
@@ -51,43 +51,43 @@
 # Initailized client with private key
 #
 hmx_client = Client(
     eth_private_key=PRIVATE_KEY,
     rpc_url=RPC_URL
 )
 # Get public address of the ethereum key
-client.private.get_public_address()
+hmx_client.private.get_public_address()
 # Deposit ETH as collateral
-client.private.deposit_eth_collateral(sub_account_id=0, amount=10.123)
+hmx_client.private.deposit_eth_collateral(sub_account_id=0, amount=10.123)
 # Deposit ERC20 as collateral. This function will automatically
 # approve CrossMarginHandler if needed.
-client.private.deposit_erc20_collateral(sub_account_id=0, token_address=COLLATERAL_USDCe, amount=100.10)
+hmx_client.private.deposit_erc20_collateral(sub_account_id=0, token_address=COLLATERAL_USDCe, amount=100.10)
 # Create a market order
-create_market_order = client.private.create_market_order(
+create_market_order = hmx_client.private.create_market_order(
   sub_account_id=0, market_index=MARKET_ETH_USD, buy=Action.BUY, size=100, reduce_only=False
 )
 print(create_market_order)
 # Create a trigger order
 # trigger_above_threshold = The current price must go above (if True) or below (if False)
 # the trigger price in order for the order to be executed
-create_order = client.private.create_trigger_order(
+create_order = hmx_client.private.create_trigger_order(
   sub_account_id=0,
   market_index=MARKET_ETH_USD,
   buy=Action.BUY,
   size=100,
   trigger_price=1800,
   trigger_above_threshold=True,
   reduce_only=False)
 print(create_order)
 # Update the order
-update_order = client.private.update_trigger_order(
+update_order = hmx_client.private.update_trigger_order(
   0, create_order["order"]["orderIndex"], Action.SELL, 50, 1700, True, False)
 print(update_order)
 # Cancel the order
-cancel_order = client.private.cancel_trigger_order(
+cancel_order = hmx_client.private.cancel_trigger_order(
   0, update_order["order"]["orderIndex"])
 ```
 
 ## Running Tests
 
 To run tests, you will need have to clone the repo, update .env, and run:
```

### Comparing `hmx-v2-python-test-1.0.9/hmx2/abis/CIXPriceAdapter.json` & `hmx_v2_python_test-1.2.0/hmx2/abis/CIXPriceAdapter.json`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-test-1.0.9/hmx2/abis/Calculator.json` & `hmx_v2_python_test-1.2.0/hmx2/abis/Calculator.json`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-test-1.0.9/hmx2/abis/ConfigStorage.json` & `hmx_v2_python_test-1.2.0/hmx2/abis/ConfigStorage.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8986810551558754%*

 * *Differences: {'111': "{'inputs': {insert: [(2, OrderedDict([('name', '_isAdaptiveFeeEnabled'), ('internalType', "*

 * *        "'bool'), ('type', 'bool')]))]}}",*

 * * '46': "{'inputs': {insert: [(1, OrderedDict([('name', '_isAdaptiveFeeEnabled'), ('internalType', "*

 * *       "'bool'), ('type', 'bool')]))]}}",*

 * * 'insert': "[(30, OrderedDict([('type', 'event'), ('anonymous', False), ('inputs', "*

 * *           "[OrderedDict([('name', 'marketIndex'), ('internalType', 'uint256'), ('type', "*

 * *           "'uint256'), ('indexed', False)]), Orde […]*

```diff
@@ -782,14 +782,39 @@
             {
                 "indexed": false,
                 "internalType": "uint256",
                 "name": "marketIndex",
                 "type": "uint256"
             },
             {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "makerFee",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "takerFee",
+                "type": "uint256"
+            }
+        ],
+        "name": "LogSetMakerTakerFee",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "marketIndex",
+                "type": "uint256"
+            },
+            {
                 "components": [
                     {
                         "internalType": "bytes32",
                         "name": "assetId",
                         "type": "bytes32"
                     },
                     {
@@ -1031,14 +1056,50 @@
         "name": "LogSetServiceExecutor",
         "type": "event"
     },
     {
         "anonymous": false,
         "inputs": [
             {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "index",
+                "type": "uint256"
+            },
+            {
+                "components": [
+                    {
+                        "internalType": "uint256",
+                        "name": "fromSize",
+                        "type": "uint256"
+                    },
+                    {
+                        "internalType": "uint256",
+                        "name": "toSize",
+                        "type": "uint256"
+                    },
+                    {
+                        "internalType": "uint256",
+                        "name": "minProfitDuration",
+                        "type": "uint256"
+                    }
+                ],
+                "indexed": false,
+                "internalType": "struct IConfigStorage.StepMinProfitDuration",
+                "name": "_stepMinProfitDuration",
+                "type": "tuple"
+            }
+        ],
+        "name": "LogSetStepMinProfitDuration",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
                 "components": [
                     {
                         "internalType": "uint32",
                         "name": "stablecoinSwapFeeRateBPS",
                         "type": "uint32"
                     },
                     {
@@ -1341,14 +1402,19 @@
                         "name": "fundingRate",
                         "type": "tuple"
                     }
                 ],
                 "internalType": "struct IConfigStorage.MarketConfig",
                 "name": "_newConfig",
                 "type": "tuple"
+            },
+            {
+                "internalType": "bool",
+                "name": "_isAdaptiveFeeEnabled",
+                "type": "bool"
             }
         ],
         "name": "addMarketConfig",
         "outputs": [
             {
                 "internalType": "uint256",
                 "name": "_newMarketIndex",
@@ -1397,14 +1463,44 @@
         "outputs": [],
         "stateMutability": "nonpayable",
         "type": "function"
     },
     {
         "inputs": [
             {
+                "components": [
+                    {
+                        "internalType": "uint256",
+                        "name": "fromSize",
+                        "type": "uint256"
+                    },
+                    {
+                        "internalType": "uint256",
+                        "name": "toSize",
+                        "type": "uint256"
+                    },
+                    {
+                        "internalType": "uint256",
+                        "name": "minProfitDuration",
+                        "type": "uint256"
+                    }
+                ],
+                "internalType": "struct IConfigStorage.StepMinProfitDuration[]",
+                "name": "_stepMinProfitDurations",
+                "type": "tuple[]"
+            }
+        ],
+        "name": "addStepMinProfitDuration",
+        "outputs": [],
+        "stateMutability": "nonpayable",
+        "type": "function"
+    },
+    {
+        "inputs": [
+            {
                 "internalType": "address",
                 "name": "",
                 "type": "address"
             }
         ],
         "name": "allowedLiquidators",
         "outputs": [
@@ -2164,14 +2260,68 @@
                 "type": "uint256"
             }
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
+        "inputs": [
+            {
+                "internalType": "uint256",
+                "name": "marketIndex",
+                "type": "uint256"
+            },
+            {
+                "internalType": "uint256",
+                "name": "sizeDelta",
+                "type": "uint256"
+            }
+        ],
+        "name": "getStepMinProfitDuration",
+        "outputs": [
+            {
+                "internalType": "uint256",
+                "name": "",
+                "type": "uint256"
+            }
+        ],
+        "stateMutability": "view",
+        "type": "function"
+    },
+    {
+        "inputs": [],
+        "name": "getStepMinProfitDurations",
+        "outputs": [
+            {
+                "components": [
+                    {
+                        "internalType": "uint256",
+                        "name": "fromSize",
+                        "type": "uint256"
+                    },
+                    {
+                        "internalType": "uint256",
+                        "name": "toSize",
+                        "type": "uint256"
+                    },
+                    {
+                        "internalType": "uint256",
+                        "name": "minProfitDuration",
+                        "type": "uint256"
+                    }
+                ],
+                "internalType": "struct IConfigStorage.StepMinProfitDuration[]",
+                "name": "",
+                "type": "tuple[]"
+            }
+        ],
+        "stateMutability": "view",
+        "type": "function"
+    },
+    {
         "inputs": [],
         "name": "getTradeServiceHooks",
         "outputs": [
             {
                 "internalType": "address[]",
                 "name": "",
                 "type": "address[]"
@@ -2251,14 +2401,52 @@
         "inputs": [],
         "name": "initialize",
         "outputs": [],
         "stateMutability": "nonpayable",
         "type": "function"
     },
     {
+        "inputs": [
+            {
+                "internalType": "uint256",
+                "name": "marketIndex",
+                "type": "uint256"
+            }
+        ],
+        "name": "isAdaptiveFeeEnabledByMarketIndex",
+        "outputs": [
+            {
+                "internalType": "bool",
+                "name": "isEnabled",
+                "type": "bool"
+            }
+        ],
+        "stateMutability": "view",
+        "type": "function"
+    },
+    {
+        "inputs": [
+            {
+                "internalType": "uint256",
+                "name": "marketIndex",
+                "type": "uint256"
+            }
+        ],
+        "name": "isStepMinProfitEnabledByMarketIndex",
+        "outputs": [
+            {
+                "internalType": "bool",
+                "name": "isStepMinProfitEnabled",
+                "type": "bool"
+            }
+        ],
+        "stateMutability": "view",
+        "type": "function"
+    },
+    {
         "inputs": [],
         "name": "liquidationConfig",
         "outputs": [
             {
                 "internalType": "uint256",
                 "name": "liquidationFeeUSDE30",
                 "type": "uint256"
@@ -2320,14 +2508,33 @@
         "stateMutability": "view",
         "type": "function"
     },
     {
         "inputs": [
             {
                 "internalType": "uint256",
+                "name": "marketIndex",
+                "type": "uint256"
+            }
+        ],
+        "name": "makerFeeE8ByMarketIndex",
+        "outputs": [
+            {
+                "internalType": "uint256",
+                "name": "makerFeeE8",
+                "type": "uint256"
+            }
+        ],
+        "stateMutability": "view",
+        "type": "function"
+    },
+    {
+        "inputs": [
+            {
+                "internalType": "uint256",
                 "name": "",
                 "type": "uint256"
             }
         ],
         "name": "marketConfigs",
         "outputs": [
             {
@@ -2488,14 +2695,21 @@
         "name": "removeAcceptedToken",
         "outputs": [],
         "stateMutability": "nonpayable",
         "type": "function"
     },
     {
         "inputs": [],
+        "name": "removeLastStepMinProfitDuration",
+        "outputs": [],
+        "stateMutability": "nonpayable",
+        "type": "function"
+    },
+    {
+        "inputs": [],
         "name": "renounceOwnership",
         "outputs": [],
         "stateMutability": "nonpayable",
         "type": "function"
     },
     {
         "inputs": [
@@ -2871,14 +3085,32 @@
         ],
         "stateMutability": "nonpayable",
         "type": "function"
     },
     {
         "inputs": [
             {
+                "internalType": "uint256[]",
+                "name": "marketIndexes",
+                "type": "uint256[]"
+            },
+            {
+                "internalType": "bool[]",
+                "name": "isEnableds",
+                "type": "bool[]"
+            }
+        ],
+        "name": "setIsStepMinProfitEnabledByMarketIndex",
+        "outputs": [],
+        "stateMutability": "nonpayable",
+        "type": "function"
+    },
+    {
+        "inputs": [
+            {
                 "components": [
                     {
                         "internalType": "uint256",
                         "name": "liquidationFeeUSDE30",
                         "type": "uint256"
                     }
                 ],
@@ -2964,14 +3196,37 @@
         "outputs": [],
         "stateMutability": "nonpayable",
         "type": "function"
     },
     {
         "inputs": [
             {
+                "internalType": "uint256[]",
+                "name": "marketIndexes",
+                "type": "uint256[]"
+            },
+            {
+                "internalType": "uint256[]",
+                "name": "makerFees",
+                "type": "uint256[]"
+            },
+            {
+                "internalType": "uint256[]",
+                "name": "takerFees",
+                "type": "uint256[]"
+            }
+        ],
+        "name": "setMakerTakerFeeByMarketIndexes",
+        "outputs": [],
+        "stateMutability": "nonpayable",
+        "type": "function"
+    },
+    {
+        "inputs": [
+            {
                 "internalType": "uint256",
                 "name": "_marketIndex",
                 "type": "uint256"
             },
             {
                 "components": [
                     {
@@ -3046,14 +3301,19 @@
                         "name": "fundingRate",
                         "type": "tuple"
                     }
                 ],
                 "internalType": "struct IConfigStorage.MarketConfig",
                 "name": "_newConfig",
                 "type": "tuple"
+            },
+            {
+                "internalType": "bool",
+                "name": "_isAdaptiveFeeEnabled",
+                "type": "bool"
             }
         ],
         "name": "setMarketConfig",
         "outputs": [
             {
                 "components": [
                     {
@@ -3252,14 +3512,49 @@
         "outputs": [],
         "stateMutability": "nonpayable",
         "type": "function"
     },
     {
         "inputs": [
             {
+                "internalType": "uint256[]",
+                "name": "indexes",
+                "type": "uint256[]"
+            },
+            {
+                "components": [
+                    {
+                        "internalType": "uint256",
+                        "name": "fromSize",
+                        "type": "uint256"
+                    },
+                    {
+                        "internalType": "uint256",
+                        "name": "toSize",
+                        "type": "uint256"
+                    },
+                    {
+                        "internalType": "uint256",
+                        "name": "minProfitDuration",
+                        "type": "uint256"
+                    }
+                ],
+                "internalType": "struct IConfigStorage.StepMinProfitDuration[]",
+                "name": "_stepMinProfitDurations",
+                "type": "tuple[]"
+            }
+        ],
+        "name": "setStepMinProfitDuration",
+        "outputs": [],
+        "stateMutability": "nonpayable",
+        "type": "function"
+    },
+    {
+        "inputs": [
+            {
                 "components": [
                     {
                         "internalType": "uint32",
                         "name": "stablecoinSwapFeeRateBPS",
                         "type": "uint32"
                     },
                     {
@@ -3362,14 +3657,43 @@
                 "type": "address"
             }
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
+        "inputs": [
+            {
+                "internalType": "uint256",
+                "name": "",
+                "type": "uint256"
+            }
+        ],
+        "name": "stepMinProfitDurations",
+        "outputs": [
+            {
+                "internalType": "uint256",
+                "name": "fromSize",
+                "type": "uint256"
+            },
+            {
+                "internalType": "uint256",
+                "name": "toSize",
+                "type": "uint256"
+            },
+            {
+                "internalType": "uint256",
+                "name": "minProfitDuration",
+                "type": "uint256"
+            }
+        ],
+        "stateMutability": "view",
+        "type": "function"
+    },
+    {
         "inputs": [],
         "name": "swapConfig",
         "outputs": [
             {
                 "internalType": "uint32",
                 "name": "stablecoinSwapFeeRateBPS",
                 "type": "uint32"
@@ -3394,14 +3718,33 @@
             }
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
         "inputs": [
+            {
+                "internalType": "uint256",
+                "name": "marketIndex",
+                "type": "uint256"
+            }
+        ],
+        "name": "takerFeeE8ByMarketIndex",
+        "outputs": [
+            {
+                "internalType": "uint256",
+                "name": "takerFeeE8",
+                "type": "uint256"
+            }
+        ],
+        "stateMutability": "view",
+        "type": "function"
+    },
+    {
+        "inputs": [
             {
                 "internalType": "address",
                 "name": "",
                 "type": "address"
             }
         ],
         "name": "tokenAssetIds",
```

### Comparing `hmx-v2-python-test-1.0.9/hmx2/abis/CrossMarginHandler.json` & `hmx_v2_python_test-1.2.0/hmx2/abis/CrossMarginHandler.json`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-test-1.0.9/hmx2/abis/ERC20.json` & `hmx_v2_python_test-1.2.0/hmx2/abis/ERC20.json`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-test-1.0.9/hmx2/abis/GlpManager.json` & `hmx_v2_python_test-1.2.0/hmx2/abis/GlpManager.json`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-test-1.0.9/hmx2/abis/GmPriceAdapter.json` & `hmx_v2_python_test-1.2.0/hmx2/abis/GmPriceAdapter.json`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-test-1.0.9/hmx2/abis/LimitTradeHandler.json` & `hmx_v2_python_test-1.2.0/hmx2/abis/LimitTradeHandler.json`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-test-1.0.9/hmx2/abis/OnchainPricelens.json` & `hmx_v2_python_test-1.2.0/hmx2/abis/OnchainPricelens.json`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-test-1.0.9/hmx2/abis/PerpStorage.json` & `hmx_v2_python_test-1.2.0/hmx2/abis/PerpStorage.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8297872340425532%*

 * *Differences: {'insert': "[(4, OrderedDict([('type', 'event'), ('anonymous', False), ('inputs', "*

 * *           "[OrderedDict([('name', 'length'), ('internalType', 'uint256'), ('type', 'uint256'), "*

 * *           "('indexed', False)]), OrderedDict([('name', 'interval'), ('internalType', 'uint256'), "*

 * *           "('type', 'uint256'), ('indexed', False)])]), ('name', 'LogSetMovingWindowConfig')])), "*

 * *           "(10, OrderedDict([('stateMutability', 'view'), ('type', 'function'), ('inputs', "*

 * *           "[OrderedDict([('name', ' […]*

```diff
@@ -27,14 +27,33 @@
         "name": "Initialized",
         "type": "event"
     },
     {
         "anonymous": false,
         "inputs": [
             {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "length",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "interval",
+                "type": "uint256"
+            }
+        ],
+        "name": "LogSetMovingWindowConfig",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
                 "indexed": true,
                 "internalType": "address",
                 "name": "executorAddress",
                 "type": "address"
             },
             {
                 "indexed": false,
@@ -145,14 +164,62 @@
         "stateMutability": "nonpayable",
         "type": "function"
     },
     {
         "inputs": [
             {
                 "internalType": "uint256",
+                "name": "marketIndex",
+                "type": "uint256"
+            },
+            {
+                "internalType": "uint256",
+                "name": "timestamp",
+                "type": "uint256"
+            }
+        ],
+        "name": "epochVolumeBuy",
+        "outputs": [
+            {
+                "internalType": "uint256",
+                "name": "buyVolume",
+                "type": "uint256"
+            }
+        ],
+        "stateMutability": "view",
+        "type": "function"
+    },
+    {
+        "inputs": [
+            {
+                "internalType": "uint256",
+                "name": "marketIndex",
+                "type": "uint256"
+            },
+            {
+                "internalType": "uint256",
+                "name": "timestamp",
+                "type": "uint256"
+            }
+        ],
+        "name": "epochVolumeSell",
+        "outputs": [
+            {
+                "internalType": "uint256",
+                "name": "sellVolume",
+                "type": "uint256"
+            }
+        ],
+        "stateMutability": "view",
+        "type": "function"
+    },
+    {
+        "inputs": [
+            {
+                "internalType": "uint256",
                 "name": "_limit",
                 "type": "uint256"
             },
             {
                 "internalType": "uint256",
                 "name": "_offset",
                 "type": "uint256"
@@ -312,14 +379,38 @@
                 "type": "tuple"
             }
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
+        "inputs": [
+            {
+                "internalType": "bool",
+                "name": "isBuy",
+                "type": "bool"
+            },
+            {
+                "internalType": "uint256",
+                "name": "marketIndex",
+                "type": "uint256"
+            }
+        ],
+        "name": "getEpochVolume",
+        "outputs": [
+            {
+                "internalType": "uint256",
+                "name": "epochVolume",
+                "type": "uint256"
+            }
+        ],
+        "stateMutability": "view",
+        "type": "function"
+    },
+    {
         "inputs": [],
         "name": "getGlobalState",
         "outputs": [
             {
                 "components": [
                     {
                         "internalType": "uint256",
@@ -603,14 +694,37 @@
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
         "inputs": [
             {
+                "internalType": "bool",
+                "name": "isBuy",
+                "type": "bool"
+            },
+            {
+                "internalType": "uint256",
+                "name": "marketIndex",
+                "type": "uint256"
+            },
+            {
+                "internalType": "uint256",
+                "name": "absSizeDelta",
+                "type": "uint256"
+            }
+        ],
+        "name": "increaseEpochVolume",
+        "outputs": [],
+        "stateMutability": "nonpayable",
+        "type": "function"
+    },
+    {
+        "inputs": [
+            {
                 "internalType": "uint256",
                 "name": "_marketIndex",
                 "type": "uint256"
             },
             {
                 "internalType": "bool",
                 "name": "_isLong",
@@ -701,14 +815,40 @@
             }
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
         "inputs": [],
+        "name": "movingWindowInterval",
+        "outputs": [
+            {
+                "internalType": "uint256",
+                "name": "",
+                "type": "uint256"
+            }
+        ],
+        "stateMutability": "view",
+        "type": "function"
+    },
+    {
+        "inputs": [],
+        "name": "movingWindowLength",
+        "outputs": [
+            {
+                "internalType": "uint256",
+                "name": "",
+                "type": "uint256"
+            }
+        ],
+        "stateMutability": "view",
+        "type": "function"
+    },
+    {
+        "inputs": [],
         "name": "owner",
         "outputs": [
             {
                 "internalType": "address",
                 "name": "",
                 "type": "address"
             }
@@ -898,14 +1038,32 @@
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
         "inputs": [
             {
+                "internalType": "uint256",
+                "name": "length",
+                "type": "uint256"
+            },
+            {
+                "internalType": "uint256",
+                "name": "interval",
+                "type": "uint256"
+            }
+        ],
+        "name": "setMovingWindowConfig",
+        "outputs": [],
+        "stateMutability": "nonpayable",
+        "type": "function"
+    },
+    {
+        "inputs": [
+            {
                 "internalType": "address[]",
                 "name": "_executorAddresses",
                 "type": "address[]"
             },
             {
                 "internalType": "bool[]",
                 "name": "_isServiceExecutors",
```

### Comparing `hmx-v2-python-test-1.0.9/hmx2/abis/TradeHelper.json` & `hmx_v2_python_test-1.2.0/hmx2/abis/TradeHelper.json`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-test-1.0.9/hmx2/abis/VaultStorage.json` & `hmx_v2_python_test-1.2.0/hmx2/abis/VaultStorage.json`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-test-1.0.9/hmx2/constants/assets.py` & `hmx_v2_python_test-1.2.0/hmx2/constants/assets.py`

 * *Files 19% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 ASSET_COIN = "COIN"
 ASSET_GOOG = "GOOG"
 ASSET_BNB = "BNB"
 ASSET_SOL = "SOL"
 ASSET_QQQ = "QQQ"
 ASSET_XRP = "XRP"
 ASSET_USDC = "USDC"
+ASSET_USDCe = "USDC.e"
 ASSET_USDT = "USDT"
 ASSET_DAI = "DAI"
 ASSET_GLP = "GLP"
 ASSET_NVDA = "NVDA"
 ASSET_LINK = "LINK"
 ASSET_CHF = "CHF"
 ASSET_DOGE = "DOGE"
@@ -53,18 +54,24 @@
 ASSET_ATOM = "ATOM"
 ASSET_1000SHIB = "1000SHIB"
 ASSET_1000PEPE = "1000PEPE"
 ASSET_ICP = "ICP"
 ASSET_MANTA = "MANTA"
 ASSET_STRK = "STRK"
 ASSET_PYTH = "PYTH"
+ASSET_PENDLE = "PENDLE"
+ASSET_W = "W"
+ASSET_ENA = "ENA"
+ASSET_ybUSDB = "ybUSDB"
+ASSET_ybETH = "ybETH"
 
 ASSETS = [ASSET_ETH, ASSET_BTC, ASSET_AAPL, ASSET_JPY, ASSET_XAU, ASSET_AMZN,
           ASSET_MSFT, ASSET_TSLA, ASSET_EUR, ASSET_XAG, ASSET_AUD, ASSET_GBP,
           ASSET_ADA, ASSET_MATIC, ASSET_SUI, ASSET_ARB, ASSET_OP, ASSET_LTC,
           ASSET_COIN, ASSET_GOOG, ASSET_BNB, ASSET_SOL, ASSET_QQQ, ASSET_XRP,
           ASSET_USDC, ASSET_USDT, ASSET_DAI, ASSET_GLP, ASSET_NVDA, ASSET_LINK,
           ASSET_CHF, ASSET_DOGE, ASSET_CAD, ASSET_SGD, ASSET_CNH, ASSET_wstETH,
           ASSET_HKD, ASSET_BCH, ASSET_MEME, ASSET_gmBTC, ASSET_gmETH, ASSET_SEK,
           ASSET_DIX, ASSET_JTO, ASSET_STX, ASSET_ORDI, ASSET_TIA, ASSET_AVAX,
           ASSET_INJ, ASSET_DOT, ASSET_SEI, ASSET_ATOM, ASSET_1000SHIB, ASSET_1000PEPE,
-          ASSET_ICP, ASSET_MANTA, ASSET_STRK, ASSET_PYTH]
+          ASSET_ICP, ASSET_MANTA, ASSET_STRK, ASSET_PYTH, ASSET_USDCe, ASSET_PENDLE,
+          ASSET_W, ASSET_ENA, ASSET_ybUSDB, ASSET_ybETH]
```

### Comparing `hmx-v2-python-test-1.0.9/hmx2/constants/pricefeed.py` & `hmx_v2_python_test-1.2.0/hmx2/constants/pricefeed.py`

 * *Files 25% similar despite different names*

```diff
@@ -53,14 +53,17 @@
   ASSET_1000PEPE,
   ASSET_ICP,
   ASSET_SEK,
   ASSET_MANTA,
   ASSET_STRK,
   ASSET_PYTH,
   ASSET_wstETH,
+  ASSET_W,
+  ASSET_PENDLE,
+  ASSET_ENA,
 )
 DEFAULT_PYTH_PRICE_SERVICE_URL = "https://hermes.pyth.network"
 
 
 GET_LATEST_PRICE_FEEDS_ENDPOINT = "api/latest_price_feeds"
 
 PRICE_FEED_IDS = {
@@ -116,14 +119,17 @@
     ASSET_1000PEPE: "0xd69731a2e74ac1ce884fc3890f7ee324b6deb66147055249568869ed700882e4",
     ASSET_SEK: "0x8ccb376aa871517e807358d4e3cf0bc7fe4950474dbe6c9ffc21ef64e43fc676",
     ASSET_ICP: "0xc9907d786c5821547777780a1e4f89484f3417cb14dd244f2b0a34ea7a554d67",
     ASSET_MANTA: "0xc3883bcf1101c111e9fcfe2465703c47f2b638e21fef2cce0502e6c8f416e0e2",
     ASSET_STRK: "0x6a182399ff70ccf3e06024898942028204125a819e519a335ffa4579e66cd870",
     ASSET_PYTH: "0x0bbf28e9a841a1cc788f6a361b17ca072d0ea3098a1e5df1c3922d06719579ff",
     ASSET_wstETH: "0x6df640f3b8963d8f8358f791f352b8364513f6ab1cca5ed3f1f7b5448980e784",
+    ASSET_W: "0xeff7446475e218517566ea99e72a4abec2e1bd8498b43b7d8331e29dcb059389",
+    ASSET_PENDLE: "0x9a4df90b25497f66b1afb012467e316e801ca3d839456db028892fe8c70c8016",
+    ASSET_ENA: "0xb7910ba7322db020416fcac28b48c01212fd9cc8fbcbaf7d30477ed8605f6bd4",
   },
   421614: {
     ASSET_ETH: "0xff61491a931112ddf1bd8147cd1b641375f79f5825126d665480874634fd0ace",
     ASSET_BTC: "0xe62df6c8b4a85fe1a67db44dc12de5db330f7ac66b72dc658afedf0f4a415b43",
     ASSET_DAI: "0xb0948a5e5313200c632b51bb5ca32f6de0d36e9950a942d19751e833f70dabfd",
     ASSET_USDC: "0xeaa020c61cc479712813461ce153894a96a6c00b21ed0cfc2798d1f9a9e9c94a",
     ASSET_USDT: "0x2b89b9dc8fdf9f34709a5b106b472f0f39bb6ca9ce04b0fd7f2e971688e2e53b",
@@ -172,9 +178,130 @@
     ASSET_1000SHIB: "0xf0d57deca57b3da2fe63a493f4c25925fdfd8edf834b20f93e1f84dbd1504d4a",
     ASSET_1000PEPE: "0xd69731a2e74ac1ce884fc3890f7ee324b6deb66147055249568869ed700882e4",
     ASSET_SEK: "0x8ccb376aa871517e807358d4e3cf0bc7fe4950474dbe6c9ffc21ef64e43fc676",
     ASSET_ICP: "0xc9907d786c5821547777780a1e4f89484f3417cb14dd244f2b0a34ea7a554d67",
     ASSET_MANTA: "0xc3883bcf1101c111e9fcfe2465703c47f2b638e21fef2cce0502e6c8f416e0e2",
     ASSET_STRK: "0x6a182399ff70ccf3e06024898942028204125a819e519a335ffa4579e66cd870",
     ASSET_PYTH: "0x0bbf28e9a841a1cc788f6a361b17ca072d0ea3098a1e5df1c3922d06719579ff",
+    ASSET_W: "0xeff7446475e218517566ea99e72a4abec2e1bd8498b43b7d8331e29dcb059389",
+    ASSET_PENDLE: "0x9a4df90b25497f66b1afb012467e316e801ca3d839456db028892fe8c70c8016",
+    ASSET_ENA: "0xb7910ba7322db020416fcac28b48c01212fd9cc8fbcbaf7d30477ed8605f6bd4",
+  },
+  81457: {
+    ASSET_ETH: "0xff61491a931112ddf1bd8147cd1b641375f79f5825126d665480874634fd0ace",
+    ASSET_BTC: "0xe62df6c8b4a85fe1a67db44dc12de5db330f7ac66b72dc658afedf0f4a415b43",
+    ASSET_DAI: "0xb0948a5e5313200c632b51bb5ca32f6de0d36e9950a942d19751e833f70dabfd",
+    ASSET_USDC: "0xeaa020c61cc479712813461ce153894a96a6c00b21ed0cfc2798d1f9a9e9c94a",
+    ASSET_USDT: "0x2b89b9dc8fdf9f34709a5b106b472f0f39bb6ca9ce04b0fd7f2e971688e2e53b",
+    ASSET_AAPL: "0x49f6b65cb1de6b10eaf75e7c03ca029c306d0357e91b5311b175084a5ad55688",
+    ASSET_XAU: "0x765d2ba906dbc32ca17cc11f5310a89e9ee1f6420508c63861f2f8ba4ee34bb2",
+    ASSET_JPY: "0xef2c98c804ba503c6a707e38be4dfbb16683775f195b091252bf24693042fd52",
+    ASSET_AMZN: "0xb5d0e0fa58a1f8b81498ae670ce93c872d14434b72c364885d4fa1b257cbb07a",
+    ASSET_MSFT: "0xd0ca23c1cc005e004ccf1db5bf76aeb6a49218f43dac3d4b275e92de12ded4d1",
+    ASSET_TSLA: "0x16dad506d7db8da01c87581c87ca897a012a153557d4d578c3b9c9e1bc0632f1",
+    ASSET_EUR: "0xa995d00bb36a63cef7fd2c287dc105fc8f3d93779f062f09551b0af3e81ec30b",
+    ASSET_XAG: "0xf2fb02c32b055c805e7238d628e5e9dadef274376114eb1f012337cabe93871e",
+    ASSET_AUD: "0x67a6f93030420c1c9e3fe37c1ab6b77966af82f995944a9fefce357a22854a80",
+    ASSET_GBP: "0x84c2dde9633d93d1bcad84e7dc41c9d56578b7ec52fabedc1f335d673df0a7c1",
+    ASSET_ADA: "0x2a01deaec9e51a579277b34b122399984d0bbf57e2458a7e42fecd2829867a0d",
+    ASSET_MATIC: "0x5de33a9112c2b700b8d30b8a3402c103578ccfa2765696471cc672bd5cf6ac52",
+    ASSET_SUI: "0x23d7315113f5b1d3ba7a83604c44b94d79f4fd69af77f804fc7f920a6dc65744",
+    ASSET_ARB: "0x3fa4252848f9f0a1480be62745a4629d9eb1322aebab8a791e344b3b9c1adcf5",
+    ASSET_OP: "0x385f64d993f7b77d8182ed5003d97c60aa3361f3cecfe711544d2d59165e9bdf",
+    ASSET_LTC: "0x6e3f3fa8253588df9326580180233eb791e03b443a3ba7a1d892e73874e19a54",
+    ASSET_COIN: "0xfee33f2a978bf32dd6b662b65ba8083c6773b494f8401194ec1870c640860245",
+    ASSET_GOOG: "0xe65ff435be42630439c96396653a342829e877e2aafaeaf1a10d0ee5fd2cf3f2",
+    ASSET_BNB: "0x2f95862b045670cd22bee3114c39763a4a08beeb663b145d283c31d7d1101c4f",
+    ASSET_SOL: "0xef0d8b6fda2ceba41da15d4095d1da392a0d2f8ed0c6c7bc0f4cfac8c280b56d",
+    ASSET_QQQ: "0x9695e2b96ea7b3859da9ed25b7a46a920a776e2fdae19a7bcfdf2b219230452d",
+    ASSET_XRP: "0xec5d399846a9209f3fe5881d70aae9268c94339ff9817e8d18ff19fa05eea1c8",
+    ASSET_NVDA: "0xb1073854ed24cbc755dc527418f52b7d271f6cc967bbf8d8129112b18860a593",
+    ASSET_LINK: "0x8ac0c70fff57e9aefdf5edf44b51d62c2d433653cbb2cf5cc06bb115af04d221",
+    ASSET_CHF: "0x0b1e3297e69f162877b577b0d6a47a0d63b2392bc8499e6540da4187a63e28f8",
+    ASSET_DOGE: "0xdcef50dd0a4cd2dcc17e45df1676dcb336a11a61c69df7a0299b0150c672d25c",
+    ASSET_CAD: "0x3112b03a41c910ed446852aacf67118cb1bec67b2cd0b9a214c58cc0eaa2ecca",
+    ASSET_SGD: "0x396a969a9c1480fa15ed50bc59149e2c0075a72fe8f458ed941ddec48bdb4918",
+    ASSET_CNH: "0xeef52e09c878ad41f6a81803e3640fe04dceea727de894edd4ea117e2e332e66",
+    ASSET_HKD: "0x19d75fde7fee50fe67753fdc825e583594eb2f51ae84e114a5246c4ab23aff4c",
+    ASSET_BCH: "0x3dd2b63686a450ec7290df3a1e0b583c0481f651351edfa7636f39aed55cf8a3",
+    ASSET_MEME: "0xcd2cee36951a571e035db0dfad138e6ecdb06b517cc3373cd7db5d3609b7927c",
+    ASSET_SEK: "0x8ccb376aa871517e807358d4e3cf0bc7fe4950474dbe6c9ffc21ef64e43fc676",
+    ASSET_JTO: "0xb43660a5f790c69354b0729a5ef9d50d68f1df92107540210b9cccba1f947cc2",
+    ASSET_STX: "0xec7a775f46379b5e943c3526b1c8d54cd49749176b0b98e02dde68d1bd335c17",
+    ASSET_ORDI: "0x193c739db502aadcef37c2589738b1e37bdb257d58cf1ab3c7ebc8e6df4e3ec0",
+    ASSET_TIA: "0x09f7c1d7dfbb7df2b8fe3d3d87ee94a2259d212da4f30c1f0540d066dfa44723",
+    ASSET_AVAX: "0x93da3352f9f1d105fdfe4971cfa80e9dd777bfc5d0f683ebb6e1294b92137bb7",
+    ASSET_INJ: "0x7a5bc1d2b56ad029048cd63964b3ad2776eadf812edc1a43a31406cb54bff592",
+    ASSET_DOT: "0xca3eed9b267293f6595901c734c7525ce8ef49adafe8284606ceb307afa2ca5b",
+    ASSET_SEI: "0x53614f1cb0c031d4af66c04cb9c756234adad0e1cee85303795091499a4084eb",
+    ASSET_ATOM: "0xb00b60f88b03a6a625a8d1c048c3f66653edf217439983d037e7222c4e612819",
+    ASSET_1000SHIB: "0xf0d57deca57b3da2fe63a493f4c25925fdfd8edf834b20f93e1f84dbd1504d4a",
+    ASSET_1000PEPE: "0xd69731a2e74ac1ce884fc3890f7ee324b6deb66147055249568869ed700882e4",
+    ASSET_SEK: "0x8ccb376aa871517e807358d4e3cf0bc7fe4950474dbe6c9ffc21ef64e43fc676",
+    ASSET_ICP: "0xc9907d786c5821547777780a1e4f89484f3417cb14dd244f2b0a34ea7a554d67",
+    ASSET_MANTA: "0xc3883bcf1101c111e9fcfe2465703c47f2b638e21fef2cce0502e6c8f416e0e2",
+    ASSET_STRK: "0x6a182399ff70ccf3e06024898942028204125a819e519a335ffa4579e66cd870",
+    ASSET_PYTH: "0x0bbf28e9a841a1cc788f6a361b17ca072d0ea3098a1e5df1c3922d06719579ff",
+    ASSET_W: "0xeff7446475e218517566ea99e72a4abec2e1bd8498b43b7d8331e29dcb059389",
+    ASSET_PENDLE: "0x9a4df90b25497f66b1afb012467e316e801ca3d839456db028892fe8c70c8016",
+    ASSET_ENA: "0xb7910ba7322db020416fcac28b48c01212fd9cc8fbcbaf7d30477ed8605f6bd4",
+  },
+  168587773: {
+    ASSET_ETH: "0xff61491a931112ddf1bd8147cd1b641375f79f5825126d665480874634fd0ace",
+    ASSET_BTC: "0xe62df6c8b4a85fe1a67db44dc12de5db330f7ac66b72dc658afedf0f4a415b43",
+    ASSET_DAI: "0xb0948a5e5313200c632b51bb5ca32f6de0d36e9950a942d19751e833f70dabfd",
+    ASSET_USDC: "0xeaa020c61cc479712813461ce153894a96a6c00b21ed0cfc2798d1f9a9e9c94a",
+    ASSET_USDT: "0x2b89b9dc8fdf9f34709a5b106b472f0f39bb6ca9ce04b0fd7f2e971688e2e53b",
+    ASSET_AAPL: "0x49f6b65cb1de6b10eaf75e7c03ca029c306d0357e91b5311b175084a5ad55688",
+    ASSET_XAU: "0x765d2ba906dbc32ca17cc11f5310a89e9ee1f6420508c63861f2f8ba4ee34bb2",
+    ASSET_JPY: "0xef2c98c804ba503c6a707e38be4dfbb16683775f195b091252bf24693042fd52",
+    ASSET_AMZN: "0xb5d0e0fa58a1f8b81498ae670ce93c872d14434b72c364885d4fa1b257cbb07a",
+    ASSET_MSFT: "0xd0ca23c1cc005e004ccf1db5bf76aeb6a49218f43dac3d4b275e92de12ded4d1",
+    ASSET_TSLA: "0x16dad506d7db8da01c87581c87ca897a012a153557d4d578c3b9c9e1bc0632f1",
+    ASSET_EUR: "0xa995d00bb36a63cef7fd2c287dc105fc8f3d93779f062f09551b0af3e81ec30b",
+    ASSET_XAG: "0xf2fb02c32b055c805e7238d628e5e9dadef274376114eb1f012337cabe93871e",
+    ASSET_AUD: "0x67a6f93030420c1c9e3fe37c1ab6b77966af82f995944a9fefce357a22854a80",
+    ASSET_GBP: "0x84c2dde9633d93d1bcad84e7dc41c9d56578b7ec52fabedc1f335d673df0a7c1",
+    ASSET_ADA: "0x2a01deaec9e51a579277b34b122399984d0bbf57e2458a7e42fecd2829867a0d",
+    ASSET_MATIC: "0x5de33a9112c2b700b8d30b8a3402c103578ccfa2765696471cc672bd5cf6ac52",
+    ASSET_SUI: "0x23d7315113f5b1d3ba7a83604c44b94d79f4fd69af77f804fc7f920a6dc65744",
+    ASSET_ARB: "0x3fa4252848f9f0a1480be62745a4629d9eb1322aebab8a791e344b3b9c1adcf5",
+    ASSET_OP: "0x385f64d993f7b77d8182ed5003d97c60aa3361f3cecfe711544d2d59165e9bdf",
+    ASSET_LTC: "0x6e3f3fa8253588df9326580180233eb791e03b443a3ba7a1d892e73874e19a54",
+    ASSET_COIN: "0xfee33f2a978bf32dd6b662b65ba8083c6773b494f8401194ec1870c640860245",
+    ASSET_GOOG: "0xe65ff435be42630439c96396653a342829e877e2aafaeaf1a10d0ee5fd2cf3f2",
+    ASSET_BNB: "0x2f95862b045670cd22bee3114c39763a4a08beeb663b145d283c31d7d1101c4f",
+    ASSET_SOL: "0xef0d8b6fda2ceba41da15d4095d1da392a0d2f8ed0c6c7bc0f4cfac8c280b56d",
+    ASSET_QQQ: "0x9695e2b96ea7b3859da9ed25b7a46a920a776e2fdae19a7bcfdf2b219230452d",
+    ASSET_XRP: "0xec5d399846a9209f3fe5881d70aae9268c94339ff9817e8d18ff19fa05eea1c8",
+    ASSET_NVDA: "0xb1073854ed24cbc755dc527418f52b7d271f6cc967bbf8d8129112b18860a593",
+    ASSET_LINK: "0x8ac0c70fff57e9aefdf5edf44b51d62c2d433653cbb2cf5cc06bb115af04d221",
+    ASSET_CHF: "0x0b1e3297e69f162877b577b0d6a47a0d63b2392bc8499e6540da4187a63e28f8",
+    ASSET_DOGE: "0xdcef50dd0a4cd2dcc17e45df1676dcb336a11a61c69df7a0299b0150c672d25c",
+    ASSET_CAD: "0x3112b03a41c910ed446852aacf67118cb1bec67b2cd0b9a214c58cc0eaa2ecca",
+    ASSET_SGD: "0x396a969a9c1480fa15ed50bc59149e2c0075a72fe8f458ed941ddec48bdb4918",
+    ASSET_CNH: "0xeef52e09c878ad41f6a81803e3640fe04dceea727de894edd4ea117e2e332e66",
+    ASSET_HKD: "0x19d75fde7fee50fe67753fdc825e583594eb2f51ae84e114a5246c4ab23aff4c",
+    ASSET_BCH: "0x3dd2b63686a450ec7290df3a1e0b583c0481f651351edfa7636f39aed55cf8a3",
+    ASSET_MEME: "0xcd2cee36951a571e035db0dfad138e6ecdb06b517cc3373cd7db5d3609b7927c",
+    ASSET_SEK: "0x8ccb376aa871517e807358d4e3cf0bc7fe4950474dbe6c9ffc21ef64e43fc676",
+    ASSET_JTO: "0xb43660a5f790c69354b0729a5ef9d50d68f1df92107540210b9cccba1f947cc2",
+    ASSET_STX: "0xec7a775f46379b5e943c3526b1c8d54cd49749176b0b98e02dde68d1bd335c17",
+    ASSET_ORDI: "0x193c739db502aadcef37c2589738b1e37bdb257d58cf1ab3c7ebc8e6df4e3ec0",
+    ASSET_TIA: "0x09f7c1d7dfbb7df2b8fe3d3d87ee94a2259d212da4f30c1f0540d066dfa44723",
+    ASSET_AVAX: "0x93da3352f9f1d105fdfe4971cfa80e9dd777bfc5d0f683ebb6e1294b92137bb7",
+    ASSET_INJ: "0x7a5bc1d2b56ad029048cd63964b3ad2776eadf812edc1a43a31406cb54bff592",
+    ASSET_DOT: "0xca3eed9b267293f6595901c734c7525ce8ef49adafe8284606ceb307afa2ca5b",
+    ASSET_SEI: "0x53614f1cb0c031d4af66c04cb9c756234adad0e1cee85303795091499a4084eb",
+    ASSET_ATOM: "0xb00b60f88b03a6a625a8d1c048c3f66653edf217439983d037e7222c4e612819",
+    ASSET_1000SHIB: "0xf0d57deca57b3da2fe63a493f4c25925fdfd8edf834b20f93e1f84dbd1504d4a",
+    ASSET_1000PEPE: "0xd69731a2e74ac1ce884fc3890f7ee324b6deb66147055249568869ed700882e4",
+    ASSET_SEK: "0x8ccb376aa871517e807358d4e3cf0bc7fe4950474dbe6c9ffc21ef64e43fc676",
+    ASSET_ICP: "0xc9907d786c5821547777780a1e4f89484f3417cb14dd244f2b0a34ea7a554d67",
+    ASSET_MANTA: "0xc3883bcf1101c111e9fcfe2465703c47f2b638e21fef2cce0502e6c8f416e0e2",
+    ASSET_STRK: "0x6a182399ff70ccf3e06024898942028204125a819e519a335ffa4579e66cd870",
+    ASSET_PYTH: "0x0bbf28e9a841a1cc788f6a361b17ca072d0ea3098a1e5df1c3922d06719579ff",
+    ASSET_W: "0xeff7446475e218517566ea99e72a4abec2e1bd8498b43b7d8331e29dcb059389",
+    ASSET_PENDLE: "0x9a4df90b25497f66b1afb012467e316e801ca3d839456db028892fe8c70c8016",
+    ASSET_ENA: "0xb7910ba7322db020416fcac28b48c01212fd9cc8fbcbaf7d30477ed8605f6bd4",
   }
 }
```

### Comparing `hmx-v2-python-test-1.0.9/hmx2/hmx_client.py` & `hmx_v2_python_test-1.2.0/hmx2/hmx_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from hmx2.modules.private import Private
 from hmx2.modules.public import Public
 from hmx2.modules.oracle.pyth_oracle import PythOracle
 from hmx2.modules.oracle.glp_oracle import GlpOracle
 from hmx2.modules.oracle.cix_oracle import CixOracle
 from hmx2.modules.oracle.gm_oracle import GmOracle
 from hmx2.modules.oracle.onchain_pricelens_oracle import OnchainPricelensOracle
+from hmx2.modules.oracle.calc_pricelens_oracle import CalcPricelensOracle
 from hmx2.modules.oracle.oracle_middleware import OracleMiddleware
 
 
 class Client(object):
   def __init__(self, rpc_url, eth_private_key=None, pyth_price_service_url=DEFAULT_PYTH_PRICE_SERVICE_URL):
     self.__eth_provider = Web3(Web3.HTTPProvider(
       rpc_url, request_kwargs={'timeout': 60}))
@@ -33,16 +34,19 @@
     gm_btc_oracle = GmOracle(contract_address["GM_BTC_PRICE_ADAPTER_ADDRESS"], [
                              ASSET_BTC, ASSET_BTC, ASSET_USDC], pyth_oracle, self.__eth_provider)
     gm_eth_oracle = GmOracle(contract_address["GM_ETH_PRICE_ADAPTER_ADDRESS"], [
         ASSET_ETH, ASSET_ETH, ASSET_USDC], pyth_oracle, self.__eth_provider)
     onchain_pricelens_oracle = OnchainPricelensOracle(
       contract_address["ONCHAIN_PRICELENS_ADDRESS"], pyth_oracle, self.__eth_provider)
 
+    calc_pricelens_oracle = CalcPricelensOracle(
+      contract_address["CALC_PRICELENS_ADDRESS"], pyth_oracle, self.__eth_provider)
+
     self.__oracle_middleware = OracleMiddleware(
-      pyth_oracle, glp_oracle, dix_oracle, gm_btc_oracle, gm_eth_oracle, onchain_pricelens_oracle)
+      pyth_oracle, glp_oracle, dix_oracle, gm_btc_oracle, gm_eth_oracle, onchain_pricelens_oracle, calc_pricelens_oracle)
 
     self.__private = None
     self.__public = Public(
       self.__chain_id, self.__eth_provider, self.__oracle_middleware)
 
   @property
   def public(self):
```

### Comparing `hmx-v2-python-test-1.0.9/hmx2/modules/oracle/cix_oracle/cix_oracle.py` & `hmx_v2_python_test-1.2.0/hmx2/modules/oracle/cix_oracle/cix_oracle.py`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-test-1.0.9/hmx2/modules/oracle/gm_oracle/gm_oracle.py` & `hmx_v2_python_test-1.2.0/hmx2/modules/oracle/gm_oracle/gm_oracle.py`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-test-1.0.9/hmx2/modules/oracle/onchain_pricelens_oracle/onchain_pricelen_oracle.py` & `hmx_v2_python_test-1.2.0/hmx2/modules/oracle/onchain_pricelens_oracle/onchain_pricelen_oracle.py`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-test-1.0.9/hmx2/modules/oracle/oracle_middleware.py` & `hmx_v2_python_test-1.2.0/hmx2/modules/oracle/oracle_middleware.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,41 @@
 from hmx2.modules.oracle.pyth_oracle import PythOracle
 from hmx2.modules.oracle.glp_oracle import GlpOracle
 from hmx2.modules.oracle.cix_oracle import CixOracle
 from hmx2.modules.oracle.gm_oracle import GmOracle
 from hmx2.modules.oracle.onchain_pricelens_oracle import OnchainPricelensOracle
+from hmx2.modules.oracle.calc_pricelens_oracle import CalcPricelensOracle
 from hmx2.constants.assets import (
   ASSETS,
+  ASSET_USDCe,
   ASSET_gmBTC,
   ASSET_gmETH,
   ASSET_DIX,
   ASSET_GLP,
   ASSET_wstETH,
   ASSET_1000PEPE,
   ASSET_1000SHIB,
-  ASSET_JPY
+  ASSET_JPY,
+  ASSET_ybETH,
+  ASSET_ybUSDB,
 )
 from typing import List
 
 
 class OracleMiddleware(object):
   def __init__(self, pyth_oracle: PythOracle, glp_oracle: GlpOracle, dix_oracle: CixOracle,
-               gm_btc_oracle: GmOracle, gm_eth_oracle: GmOracle, onchain_pricelens_oracle: OnchainPricelensOracle):
+               gm_btc_oracle: GmOracle, gm_eth_oracle: GmOracle, onchain_pricelens_oracle: OnchainPricelensOracle,
+               calc_pricelens_oracle: CalcPricelensOracle):
     self.glp_oracle = glp_oracle
     self.pyth_oracle = pyth_oracle
     self.dix_oracle = dix_oracle
     self.gm_btc_oracle = gm_btc_oracle
     self.gm_eth_oracle = gm_eth_oracle
     self.onchain_pricelens_oracle = onchain_pricelens_oracle
+    self.calc_pricelens_oracle = calc_pricelens_oracle
 
   def get_price(self, asset_id: str):
     '''
     Get the latest price of the asset.
 
     :param asset_id: required
     :type asset_id: str in list ASSET_IDS
@@ -54,14 +60,17 @@
 
     if asset_id in [ASSET_1000PEPE, ASSET_1000SHIB]:
       return self.pyth_oracle.get_price(asset_id) * 1000
 
     if asset_id in [ASSET_JPY]:
       return 1 / self.pyth_oracle.get_price(asset_id)
 
+    if asset_id in [ASSET_ybETH, ASSET_ybUSDB]:
+      return self.calc_pricelens_oracle.get_price(asset_id)
+
     return self.pyth_oracle.get_price(asset_id)
 
   def get_multiple_price(self, asset_ids: List[str]):
 
     price_object = {}
 
     if set(asset_ids) - set(ASSETS):
@@ -83,14 +92,27 @@
       price_object[ASSET_gmETH] = self.gm_eth_oracle.get_price(ASSET_gmETH)
       asset_ids.remove(ASSET_gmETH)
 
     if ASSET_wstETH in asset_ids:
       price_object[ASSET_wstETH] = self.onchain_pricelens_oracle.get_price(
         ASSET_wstETH)
       asset_ids.remove(ASSET_wstETH)
+    if ASSET_USDCe in asset_ids:
+      price_object[ASSET_USDCe] = self.get_price("USDC")
+      asset_ids.remove(ASSET_USDCe)
+
+    if ASSET_ybETH in asset_ids:
+      price_object[ASSET_ybETH] = self.calc_pricelens_oracle.get_price(
+        ASSET_ybETH)
+      asset_ids.remove(ASSET_ybETH)
+
+    if ASSET_ybUSDB in asset_ids:
+      price_object[ASSET_ybUSDB] = self.calc_pricelens_oracle.get_price(
+        ASSET_ybUSDB)
+      asset_ids.remove(ASSET_ybUSDB)
 
     raw_prices = self.pyth_oracle.get_multiple_price(asset_ids)
 
     for index, asset_id in enumerate(asset_ids):
       if asset_id in [ASSET_1000PEPE, ASSET_1000SHIB]:
         price_object[asset_id] = raw_prices[index] * 1000
```

### Comparing `hmx-v2-python-test-1.0.9/hmx2/modules/oracle/pyth_oracle/pyth_oracle.py` & `hmx_v2_python_test-1.2.0/hmx2/modules/oracle/pyth_oracle/pyth_oracle.py`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-test-1.0.9/hmx2/modules/private.py` & `hmx_v2_python_test-1.2.0/hmx2/modules/private.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from eth_abi.packed import encode_packed
 from web3 import Web3, Account
 from web3.middleware.signing import construct_sign_and_send_raw_middleware
 from web3.logs import DISCARD
 from time import sleep
 from hmx2.constants.contracts import (
   CROSS_MARGIN_HANDLER_ABI_PATH,
   LIMIT_TRADE_HANDLER_ABI_PATH,
@@ -12,27 +13,44 @@
   CALCULATOR_ABI_PATH
 )
 from hmx2.constants.common import (
   ADDRESS_ZERO,
   MAX_UINT,
   EXECUTION_FEE,
   BPS,
+  MAX_UINT54,
+  MINUTES
 )
-from hmx2.enum import Cmd
+from hmx2.constants.intent import (
+  INTENT_TRADE_API,
+)
+from hmx2.enum import (
+  Action,
+  Cmd,
+)
+from eth_account import Account
+from secp256k1 import PrivateKey
+
+from eth_account.messages import encode_typed_data
+from time import time
 from hmx2.helpers.contract_loader import load_contract
 from simple_multicall_v6 import Multicall
 from hmx2.helpers.mapper import (
   get_contract_address,
   get_token_profile,
   get_collateral_address_asset_map,
   get_collateral_address_list
 )
+from hmx2.helpers.util import check_sub_account_id_param, from_number_to_e30
 from hmx2.modules.oracle.oracle_middleware import OracleMiddleware
 from eth_abi.abi import encode
 import decimal
+import math
+import requests as r
+import json
 
 decimal.getcontext().prec = 15
 decimal.getcontext().rounding = "ROUND_HALF_DOWN"
 
 
 class Private(object):
 
@@ -62,50 +80,14 @@
       self.eth_provider, self.contract_address["CROSS_MARGIN_HANDLER_ADDRESS"], CROSS_MARGIN_HANDLER_ABI_PATH)
     self.calculator_instance = load_contract(
       self.eth_provider, self.contract_address["CALCULATOR_ADDRESS"], CALCULATOR_ABI_PATH
     )
     self.multicall_instance = Multicall(w3=self.eth_provider,
                                         custom_address=self.contract_address["MULTICALL_ADDRESS"])
 
-  def get_public_address(self):
-    '''
-    Get the public address of the signer.
-    '''
-    return self.eth_signer.address
-
-  def get_collaterals(self, sub_account_id: int):
-    self.__check_sub_account_id_param(sub_account_id)
-
-    calls = [
-      self.multicall_instance.create_call(
-        self.vault_storage_instance,
-          "traderBalances",
-          [self.eth_signer.address, collateral],
-      )
-      for collateral in self.collateral_address_list
-    ]
-    collateral_usd = [
-      self.oracle_middleware.get_price(
-        self.collateral_address_asset_map[collateral])
-      for collateral in self.collateral_address_list
-    ]
-
-    results = self.multicall_instance.call(calls)
-
-    ret = {}
-    for index, collateral in enumerate(self.collateral_address_list):
-      amount = int(
-          results[1][index].hex(), 16) / 10 ** self.token_profile[collateral]["decimals"]
-      ret[self.token_profile[collateral]["symbol"]] = {
-        'amount': amount,
-        'value_usd': amount * collateral_usd[index]
-      }
-
-    return ret
-
   def deposit_erc20_collateral(self, sub_account_id: int, token_address: str, amount: float):
     '''
     Deposit ERC20 token as collateral.
 
     :param sub_account_id: required
     :type sub_account_id: int between 0 and 255
 
@@ -113,15 +95,15 @@
     :type token_address: str in list COLLATERALS
 
     :param amount: required
     :type amount: float
     '''
     if token_address not in self.collateral_address_list:
       raise Exception("Invalid collateral address")
-    self.__check_sub_account_id_param(sub_account_id)
+    check_sub_account_id_param(sub_account_id)
 
     amount_wei = int(
       amount * 10 ** self.token_profile[token_address]["decimals"])
     token_instance = load_contract(
       self.eth_provider, token_address, ERC20_ABI_PATH)
 
     CROSS_MARGIN_HANDLER_ADDRESS = self.contract_address["CROSS_MARGIN_HANDLER_ADDRESS"]
@@ -150,15 +132,15 @@
     :type token_address: str in list COLLATERALS
 
     :param amount: required
     :type amount: float
     '''
     if token_address not in self.collateral_address_list:
       raise Exception("Invalid collateral address")
-    self.__check_sub_account_id_param(sub_account_id)
+    check_sub_account_id_param(sub_account_id)
     wrap = wrap if self.token_profile[token_address]['symbol'] == "WETH" else False
 
     amount_wei = int(
       amount * 10 ** self.token_profile[token_address]["decimals"])
 
     transact_param = {"value": EXECUTION_FEE, "from": self.eth_signer.address,
                       "gas": 10000000} if self.chain_id == 421614 else {"value": EXECUTION_FEE, "from": self.eth_signer.address}
@@ -177,26 +159,28 @@
 
     :param sub_account_id: required
     :type sub_account_id: int between 0 and 255
 
     :param amount: required
     :type amount: float
     '''
-    self.__check_sub_account_id_param(sub_account_id)
+    check_sub_account_id_param(sub_account_id)
 
     amount_wei = int(amount * 10 ** 18)
 
+    eth_token = self.token_profile['WETH']['address']
+
     return self.cross_margin_handler_instance.functions.depositCollateral(
       sub_account_id,
-      self.token_profile['WETH']['address'],
+      eth_token,
       amount_wei,
       True
     ).transact({"from": self.eth_signer.address, "value": amount_wei})
 
-  def create_market_order(self, sub_account_id: int, market_index: int, buy: bool, size: float, reduce_only: bool, tp_token: str = ADDRESS_ZERO):
+  def create_market_order(self, sub_account_id: int, market_index: int, buy: bool, size: float, reduce_only: bool, tp_token: str = ADDRESS_ZERO, intent=False):
     '''
     Post a market order
 
     :param sub_account_id: required
     :type sub_account_id: int between 0 and 255
 
     :param market_index: required
@@ -210,15 +194,23 @@
 
     :param reduce_only: required
     :type reduce_only: bool
 
     :param tp_token
     :type tp_token: str in list COLLATERALS address
     '''
-    self.__check_sub_account_id_param(sub_account_id)
+    if intent:
+      while True:
+        try:
+          return self.__create_intent_trade_order(sub_account_id, market_index, buy, size, reduce_only, tp_token)
+        except Exception as e:
+          # print(e)
+          sleep(0.5)
+
+    check_sub_account_id_param(sub_account_id)
 
     order = {
       "cmd": Cmd.CREATE,
       "market_index": market_index,
       "size_delta": Web3.to_wei(size, "tether") if buy else -Web3.to_wei(size, "tether"),
       "trigger_price": 0,
       "acceptable_price": MAX_UINT if buy else 0,
@@ -237,15 +229,15 @@
 
     events = self.__parse_log(tx, "LogCreateLimitOrder")
     args = {}
     args["tx"] = events[0]["transactionHash"]
     args["order"] = events[0]["args"]
     return args
 
-  def create_trigger_order(self, sub_account_id: int, market_index: int, buy: bool, size: float, trigger_price: float, trigger_above_threshold: bool, reduce_only: bool, tp_token: str = ADDRESS_ZERO):
+  def create_trigger_order(self, sub_account_id: int, market_index: int, buy: bool, size: float, trigger_price: float, trigger_above_threshold: bool, reduce_only: bool, tp_token: str = ADDRESS_ZERO, intent: bool = False):
     '''
     Post a trigger order
 
     :param sub_account_id: required
     :type sub_account_id: int between 0 and 255
 
     :param market_index: required
@@ -265,14 +257,23 @@
 
     :param reduce_only: required
     :type reduce_only: bool
 
     :param tp_token
     :type tp_token: str in list COLLATERALS address
     '''
+
+    if intent:
+      while True:
+        try:
+          return self.__create_intent_trigger_order(sub_account_id, market_index, buy, size, trigger_price, trigger_above_threshold, reduce_only, tp_token)
+        except Exception as e:
+          # print(e)
+          sleep(0.5)
+
     order = {
       "cmd": Cmd.CREATE,
       "market_index": market_index,
       "size_delta": Web3.to_wei(size, "tether") if buy else -Web3.to_wei(size, "tether"),
       "trigger_price": Web3.to_wei(trigger_price, "tether"),
       "acceptable_price": Web3.to_wei(
         self.__add_slippage(
@@ -293,15 +294,15 @@
 
     events = self.__parse_log(tx, "LogCreateLimitOrder")
     args = {}
     args["tx"] = events[0]["transactionHash"]
     args["order"] = events[0]["args"]
     return args
 
-  def update_trigger_order(self, sub_account_id: int, order_index: int, buy: bool, size: float, trigger_price: float, trigger_above_threshold: bool, reduce_only: bool, tp_token: str = ADDRESS_ZERO):
+  def update_trigger_order(self, sub_account_id: int, order_index: int, buy: bool, size: float, trigger_price: float, trigger_above_threshold: bool, reduce_only: bool, tp_token: str = ADDRESS_ZERO, intent: bool = False):
     '''
     Update a trigger order
 
     :param sub_account_id: required
     :type sub_account_id: int between 0 and 255
 
     :param order_index: required
@@ -439,15 +440,128 @@
 
   def __prepare_cancel_order_call_data(self, order_index: int):
     return encode(
       ["uint256"],
       [order_index]
     )
 
-  def __check_sub_account_id_param(self, sub_account_id):
-    if sub_account_id not in range(0, 256):
-      raise Exception("Invalid sub account id")
-
   def __parse_log(self, tx, topic):
     receipt = self.eth_provider.eth.get_transaction_receipt(tx)
     return self.limit_trade_handler_instance.events[topic](
       ).process_receipt(receipt, DISCARD)
+
+  def __create_intent_trigger_order(self, sub_account_id: int, market_index: int, buy: bool, size: float, trigger_price: float, trigger_above_threshold: bool, reduce_only: bool, tp_token: str = ADDRESS_ZERO):
+    created_timestamp = math.floor(time())
+    expired_timestamp = created_timestamp + 240 * MINUTES
+
+    acceptable_price = self.__add_slippage(
+      trigger_price) if buy else self.__sub_slippage(trigger_price)
+    acceptable_price = from_number_to_e30(acceptable_price)
+
+    trigger_price = from_number_to_e30(trigger_price)
+
+    # trunc to e8
+    size = from_number_to_e30(size)
+
+    json_body = json_body = self.__encode_and_build_trade_order(
+      market_index, size, buy, trigger_price, acceptable_price, trigger_above_threshold, reduce_only, tp_token, created_timestamp, expired_timestamp, sub_account_id)
+
+    return self.__upsert_intent_trade_orders_api(json_body)
+
+  def __create_intent_trade_order(self, sub_account_id: int, market_index: int, buy: bool, size: float, reduce_only: bool, tp_token: str = ADDRESS_ZERO):
+    created_timestamp = math.floor(time())
+    expired_timestamp = created_timestamp + 240 * MINUTES
+
+    acceptable_price = MAX_UINT54 if buy else 0
+    trigger_price = 0
+
+    # trunc to e8
+    size = from_number_to_e30(size)
+
+    json_body = self.__encode_and_build_trade_order(
+      market_index, size, buy, trigger_price, acceptable_price, True, reduce_only, tp_token, created_timestamp, expired_timestamp, sub_account_id)
+
+    return self.__upsert_intent_trade_orders_api(json_body)
+
+  def __upsert_intent_trade_orders_api(self, req):
+    return r.post(f'{INTENT_TRADE_API}/v1/intent-handler/orders.upsert', headers={'Content-Type': 'application/json'}, data=req)
+
+  def __encode_and_build_trade_order(self, market_index: int, size: int, buy: bool, trigger_price: int, acceptable_price: int, trigger_above_threshold: bool, reduce_only: bool, tp_token: str, created_timestamp: int, expired_timestamp: int, sub_account_id: int):
+    full_message = {
+      "domain": {
+        "name": "IntentHander",
+        "version": "1.0.0",
+        "chainId": self.chain_id,
+        "verifyingContract": get_contract_address(self.chain_id)['INTENT_ADDRESS']
+      },
+      "types": {
+        "TradeOrder": [
+          {"name": "marketIndex", "type": "uint256"},
+          {"name": "sizeDelta", "type": "int256"},
+          {"name": "triggerPrice", "type": "uint256"},
+          {"name": "acceptablePrice", "type": "uint256"},
+          {"name": "triggerAboveThreshold", "type": "bool"},
+          {"name": "reduceOnly", "type": "bool"},
+          {"name": "tpToken", "type": "address"},
+          {"name": "createdTimestamp", "type": "uint256"},
+          {"name": "expiryTimestamp", "type": "uint256"},
+          {"name": "account", "type": "address"},
+          {"name": "subAccountId", "type": "uint8"}
+        ]
+      },
+      "primaryType": "TradeOrder",
+      "message": {
+        "marketIndex": market_index,
+        "sizeDelta": str(size if buy else size * -1),
+        "triggerPrice": str(trigger_price),
+        "acceptablePrice": str(acceptable_price),
+        "triggerAboveThreshold": trigger_above_threshold,
+        "reduceOnly": reduce_only,
+        "tpToken": tp_token,
+        "createdTimestamp": created_timestamp,
+        "expiryTimestamp": expired_timestamp,
+        "account": self.eth_signer.address,
+        "subAccountId": sub_account_id
+      }
+    }
+
+    encoded_data = encode_typed_data(full_message=full_message)
+
+    sign_data = Account.sign_message(encoded_data, self.eth_signer.key)
+
+    signature = encode_packed(['bytes32', 'bytes32', 'uint8'], [
+        bytes.fromhex(hex(sign_data.r)[2:]), bytes.fromhex(hex(sign_data.s)[2:]), sign_data.v])
+
+    private_key = PrivateKey(
+      bytes(bytearray.fromhex(self.eth_signer.key.hex()[2:])))
+    pubkey_ser = private_key.pubkey.serialize(compressed=False).hex()
+
+    req_body = {
+      "chainId": self.chain_id,
+      "intentTradeOrders": [
+        {
+          "marketIndex": market_index,
+          "sizeDeltaE30": str(size if buy else size * -1),
+          "triggerPriceE30": str(trigger_price),
+          "acceptablePriceE30": str(acceptable_price),
+          "triggerAboveThreshold": trigger_above_threshold,
+          "reduceOnly": reduce_only,
+          "tpToken": tp_token,
+          "createdTimestamp": created_timestamp,
+          "expiryTimestamp": expired_timestamp,
+          "account": self.eth_signer.address,
+          "subAccountId": sub_account_id,
+          "signature": "0x" + signature.hex(),
+          "digest": sign_data.messageHash.hex(),
+          "publicKey": "0x" + pubkey_ser,
+        }
+      ]
+    }
+    json_body = json.dumps(req_body)
+
+    return json_body
+
+  def get_public_address(self):
+    '''
+    Get the public address of the signer.
+    '''
+    return self.eth_signer.address
```

### Comparing `hmx-v2-python-test-1.0.9/hmx_v2_python_test.egg-info/PKG-INFO` & `hmx_v2_python_test-1.2.0/hmx_v2_python_test.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hmx-v2-python-test
-Version: 1.0.9
+Version: 1.2.0
 Summary: HMXv2 Python SDK
 Home-page: https://github.com/HMXOrg/v2-sdk-python
 Author: HMXOrg
 Author-email: contact@hmx.org
 License: MIT
 Keywords: hmx exchange perp dex defi ethereum eth arbitrum
 Classifier: Intended Audience :: Developers
@@ -19,21 +19,22 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: eth_keys
-Requires-Dist: eth-account==0.11.0
+Requires-Dist: eth-account==0.10.0
 Requires-Dist: eth-abi<5.0.0,>=4.0.0
 Requires-Dist: uniswap-universal-router-decoder
 Requires-Dist: web3<7.0.0,>=6.0.0
 Requires-Dist: simple-multicall-v6
 Requires-Dist: responses
 Requires-Dist: python-dotenv>=1.0.0
+Requires-Dist: secp256k1==0.14.0
 
 # Python SDK for HMXv2
 
 This library is tested against Python versions 2.7, 3.4, 3.5, 3.9, and 3.11.
 
 ## Installation
 
@@ -57,23 +58,23 @@
 #
 # Using publicly access functions
 #
 hmx_client = Client(
     rpc_url=RPC_URL
 )
 # Get oracle price, adaptive price, and price impact of a new position
-client.public.get_price(MARKET_ETH_USD, Action.SELL, 1000)
+hmx_client.public.get_price(MARKET_ETH_USD, Action.SELL, 1000)
 # Get market information
-client.public.get_market_info(MARKET_ETH_USD)
+hmx_client.public.get_market_info(MARKET_ETH_USD)
 # Get sub account in address format
-client.public.get_sub_account(1)
+hmx_client.public.get_sub_account(1)
 # Get position ID
-client.public.get_position_id(some_account, some_sub_account_id, MARKET_ETH_USD)
+hmx_client.public.get_position_id(some_account, some_sub_account_id, MARKET_ETH_USD)
 # Get position info
-client.public.get_position_info(some_account, some_sub_account_id, MARKET_ETH_USD)
+hmx_client.public.get_position_info(some_account, some_sub_account_id, MARKET_ETH_USD)
 ```
 
 ### Private function
 
 ```python
 from hmx2.hmx_client import Client
 from hmx2.constants.markets import MARKET_ETH_USD
@@ -84,43 +85,43 @@
 # Initailized client with private key
 #
 hmx_client = Client(
     eth_private_key=PRIVATE_KEY,
     rpc_url=RPC_URL
 )
 # Get public address of the ethereum key
-client.private.get_public_address()
+hmx_client.private.get_public_address()
 # Deposit ETH as collateral
-client.private.deposit_eth_collateral(sub_account_id=0, amount=10.123)
+hmx_client.private.deposit_eth_collateral(sub_account_id=0, amount=10.123)
 # Deposit ERC20 as collateral. This function will automatically
 # approve CrossMarginHandler if needed.
-client.private.deposit_erc20_collateral(sub_account_id=0, token_address=COLLATERAL_USDCe, amount=100.10)
+hmx_client.private.deposit_erc20_collateral(sub_account_id=0, token_address=COLLATERAL_USDCe, amount=100.10)
 # Create a market order
-create_market_order = client.private.create_market_order(
+create_market_order = hmx_client.private.create_market_order(
   sub_account_id=0, market_index=MARKET_ETH_USD, buy=Action.BUY, size=100, reduce_only=False
 )
 print(create_market_order)
 # Create a trigger order
 # trigger_above_threshold = The current price must go above (if True) or below (if False)
 # the trigger price in order for the order to be executed
-create_order = client.private.create_trigger_order(
+create_order = hmx_client.private.create_trigger_order(
   sub_account_id=0,
   market_index=MARKET_ETH_USD,
   buy=Action.BUY,
   size=100,
   trigger_price=1800,
   trigger_above_threshold=True,
   reduce_only=False)
 print(create_order)
 # Update the order
-update_order = client.private.update_trigger_order(
+update_order = hmx_client.private.update_trigger_order(
   0, create_order["order"]["orderIndex"], Action.SELL, 50, 1700, True, False)
 print(update_order)
 # Cancel the order
-cancel_order = client.private.cancel_trigger_order(
+cancel_order = hmx_client.private.cancel_trigger_order(
   0, update_order["order"]["orderIndex"])
 ```
 
 ## Running Tests
 
 To run tests, you will need have to clone the repo, update .env, and run:
```

### Comparing `hmx-v2-python-test-1.0.9/hmx_v2_python_test.egg-info/SOURCES.txt` & `hmx_v2_python_test-1.2.0/hmx_v2_python_test.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,50 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 hmx2/__init__.py
 hmx2/enum.py
 hmx2/hmx_client.py
+hmx2/abis/AdaptiveFeeCalculator.json
 hmx2/abis/CIXPriceAdapter.json
+hmx2/abis/CalcPricelens.json
 hmx2/abis/Calculator.json
 hmx2/abis/ConfigStorage.json
 hmx2/abis/CrossMarginHandler.json
 hmx2/abis/ERC20.json
 hmx2/abis/GlpManager.json
 hmx2/abis/GmPriceAdapter.json
 hmx2/abis/LimitTradeHandler.json
 hmx2/abis/OnchainPricelens.json
+hmx2/abis/OrderbookOracle.json
 hmx2/abis/PerpStorage.json
 hmx2/abis/TradeHelper.json
 hmx2/abis/VaultStorage.json
 hmx2/constants/__init__.py
 hmx2/constants/assets.py
 hmx2/constants/common.py
 hmx2/constants/contracts.py
+hmx2/constants/intent.py
 hmx2/constants/markets.py
 hmx2/constants/pricefeed.py
 hmx2/constants/tokens.py
 hmx2/helpers/__init__.py
 hmx2/helpers/contract_loader.py
 hmx2/helpers/mapper.py
 hmx2/helpers/util.py
 hmx2/modules/__init__.py
 hmx2/modules/private.py
 hmx2/modules/public.py
 hmx2/modules/calculator/__init__.py
 hmx2/modules/calculator/calculator.py
 hmx2/modules/oracle/__init__.py
 hmx2/modules/oracle/oracle_middleware.py
+hmx2/modules/oracle/calc_pricelens_oracle/__init__.py
+hmx2/modules/oracle/calc_pricelens_oracle/calc_pricelens_oracle.py
 hmx2/modules/oracle/cix_oracle/__init__.py
 hmx2/modules/oracle/cix_oracle/cix_oracle.py
 hmx2/modules/oracle/glp_oracle/__init__.py
 hmx2/modules/oracle/glp_oracle/glp_oracle.py
 hmx2/modules/oracle/gm_oracle/__init__.py
 hmx2/modules/oracle/gm_oracle/gm_oracle.py
 hmx2/modules/oracle/onchain_pricelens_oracle/__init__.py
```

### Comparing `hmx-v2-python-test-1.0.9/setup.py` & `hmx_v2_python_test-1.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from setuptools import setup, find_packages
 
 LONG_DESCRIPTION = open('README.md').read()
 
 REQUIREMENTS = [
     'eth_keys',
-    'eth-account==0.11.0',
+    'eth-account==0.10.0',
     'eth-abi>=4.0.0,<5.0.0',
     'uniswap-universal-router-decoder',
     'web3>=6.0.0,<7.0.0',
     'simple-multicall-v6',
     'responses',
-    'python-dotenv>=1.0.0'
+    'python-dotenv>=1.0.0',
+    'secp256k1==0.14.0'
 ]
 
 setup(
     name='hmx-v2-python-test',
-    version='1.0.9',
+    version='1.2.0',
     packages=find_packages(),
     package_data={
       'hmx2': ['abis/*.json'],
     },
     description='HMXv2 Python SDK',
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
```

### Comparing `hmx-v2-python-test-1.0.9/tests/constants.py` & `hmx_v2_python_test-1.2.0/tests/constants.py`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-test-1.0.9/tests/test_create_market_order.py` & `hmx_v2_python_test-1.2.0/tests/test_create_market_order.py`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-test-1.0.9/tests/test_deposit_collateral.py` & `hmx_v2_python_test-1.2.0/tests/test_deposit_collateral.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,15 +65,16 @@
     responses.add_passthru(setup_tenderly_helper.rpc_url)
 
     client = Client(
       eth_private_key=DEFAULT_KEY,
       rpc_url=setup_tenderly_helper.rpc_url
     )
     client.private.deposit_eth_collateral(0, 10)
-    my_collaterals = client.private.get_collaterals(0)
+    my_collaterals = client.public.get_collaterals(
+      client.private.get_public_address(), 0)
     assert my_collaterals["WETH"]["amount"] == 10
     assert my_collaterals["WETH"]["value_usd"] == 18500
 
   @responses.activate
   def test_correctness_when_deposit_weth_collateral_without_allowance(self, setup_tenderly_helper: TenderlyHelper):
     # mock pyth prices
     mock_pyth_price(DEFAULT_CHAIN_ID, ASSET_USDC, 1)
@@ -92,15 +93,16 @@
     action_helper = ActionHelper(
       rpc_url=setup_tenderly_helper.rpc_url,
       eth_private_key=DEFAULT_KEY
     )
     asset_map = get_token_profile(DEFAULT_CHAIN_ID)
     action_helper.wrap_eth(10)
     client.private.deposit_erc20_collateral(0, asset_map['WETH']['address'], 10)
-    my_collaterals = client.private.get_collaterals(0)
+    my_collaterals = client.public.get_collaterals(
+      client.private.get_public_address(), 0)
     assert my_collaterals["WETH"]["amount"] == 10
     assert my_collaterals["WETH"]["value_usd"] == 18500
 
   @responses.activate
   def test_correctness_when_deposit_erc20_collateral_without_allowance(self, setup_tenderly_helper: TenderlyHelper):
     # mock pyth prices
     mock_pyth_price(DEFAULT_CHAIN_ID, ASSET_USDC, 1)
@@ -126,10 +128,11 @@
     action_helper.approve(
       asset_map['WETH']['address'], UNISWAP_SWAP_ROUTER_02_ADDRESS, 10)
     action_helper.swapExactTokensForTokens(
       asset_map['WETH']['address'], asset_map['USDC.e']['address'], 500, 10)
     # deposit USDC.e as collateral
     client.private.deposit_erc20_collateral(
       0, asset_map['USDC.e']['address'], 1000)
-    my_collaterals = client.private.get_collaterals(0)
+    my_collaterals = client.public.get_collaterals(
+      client.private.get_public_address(), 0)
     assert my_collaterals["USDC.e"]["amount"] == 1000
     assert my_collaterals["USDC.e"]["value_usd"] == 1000
```

### Comparing `hmx-v2-python-test-1.0.9/tests/test_get_adaptive_fee.py` & `hmx_v2_python_test-1.2.0/tests/test_get_adaptive_fee.py`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-test-1.0.9/tests/test_init.py` & `hmx_v2_python_test-1.2.0/tests/test_init.py`

 * *Files identical despite different names*

