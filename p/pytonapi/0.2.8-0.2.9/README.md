# Comparing `tmp/pytonapi-0.2.8.tar.gz` & `tmp/pytonapi-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytonapi-0.2.8.tar", last modified: Thu Apr 25 11:24:44 2024, max compression
+gzip compressed data, was "pytonapi-0.2.9.tar", last modified: Fri Apr 26 19:28:07 2024, max compression
```

## Comparing `pytonapi-0.2.8.tar` & `pytonapi-0.2.9.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-25 11:24:44.729197 pytonapi-0.2.8/
--rw-rw-r--   0 ness      (1000) ness      (1000)     1060 2024-04-04 18:07:04.000000 pytonapi-0.2.8/LICENSE
--rw-r--r--   0 ness      (1000) ness      (1000)     5377 2024-04-25 11:24:44.729197 pytonapi-0.2.8/PKG-INFO
--rw-rw-r--   0 ness      (1000) ness      (1000)     4653 2024-04-04 18:07:04.000000 pytonapi-0.2.8/README.md
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-25 11:24:44.717196 pytonapi-0.2.8/pytonapi/
--rw-rw-r--   0 ness      (1000) ness      (1000)      129 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/__init__.py
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-25 11:24:44.717196 pytonapi-0.2.8/pytonapi/async_tonapi/
--rw-rw-r--   0 ness      (1000) ness      (1000)     3349 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/async_tonapi/__init__.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     9657 2024-04-22 23:59:07.000000 pytonapi-0.2.8/pytonapi/async_tonapi/client.py
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-25 11:24:44.721197 pytonapi-0.2.8/pytonapi/async_tonapi/methods/
--rw-rw-r--   0 ness      (1000) ness      (1000)      967 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/async_tonapi/methods/__init__.py
--rw-rw-r--   0 ness      (1000) ness      (1000)    14416 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/async_tonapi/methods/accounts.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     9152 2024-04-20 19:32:54.000000 pytonapi-0.2.8/pytonapi/async_tonapi/methods/blockchain.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     1655 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/async_tonapi/methods/dns.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     4670 2024-04-20 20:11:38.000000 pytonapi-0.2.8/pytonapi/async_tonapi/methods/emulate.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     1347 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/async_tonapi/methods/events.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     4176 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/async_tonapi/methods/inscriptions.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     2633 2024-04-11 12:27:47.000000 pytonapi-0.2.8/pytonapi/async_tonapi/methods/jettons.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     8021 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/async_tonapi/methods/liteserver.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     4509 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/async_tonapi/methods/nft.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     1791 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/async_tonapi/methods/rates.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     3798 2024-04-25 11:21:31.000000 pytonapi-0.2.8/pytonapi/async_tonapi/methods/sse.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     2455 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/async_tonapi/methods/staking.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      476 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/async_tonapi/methods/storage.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      895 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/async_tonapi/methods/tonconnect.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      768 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/async_tonapi/methods/traces.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     2343 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/async_tonapi/methods/wallet.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     2367 2024-04-25 11:21:42.000000 pytonapi-0.2.8/pytonapi/async_tonapi/methods/websocket.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     2279 2024-04-22 23:25:05.000000 pytonapi-0.2.8/pytonapi/exceptions.py
--rw-rw-r--   0 ness      (1000) ness      (1000)        0 2024-04-25 11:21:31.000000 pytonapi-0.2.8/pytonapi/py.typed
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-25 11:24:44.725196 pytonapi-0.2.8/pytonapi/schema/
--rw-rw-r--   0 ness      (1000) ness      (1000)      735 2024-04-25 11:21:31.000000 pytonapi-0.2.8/pytonapi/schema/__init__.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      874 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/schema/_address.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      896 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/schema/_balance.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     1787 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/schema/accounts.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     7591 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/schema/blockchain.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      575 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/schema/dns.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      500 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/schema/domains.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     6158 2024-04-25 11:21:31.000000 pytonapi-0.2.8/pytonapi/schema/events.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      245 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/schema/inscriptions.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     1486 2024-04-11 13:28:19.000000 pytonapi-0.2.8/pytonapi/schema/jettons.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     1856 2024-04-25 11:21:31.000000 pytonapi-0.2.8/pytonapi/schema/liteserver.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     1164 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/schema/nft.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      369 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/schema/rates.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     1152 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/schema/staking.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      364 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/schema/storage.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      169 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/schema/tonconnect.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     3133 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/schema/traces.py
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-25 11:24:44.725196 pytonapi-0.2.8/pytonapi/tonapi/
--rw-rw-r--   0 ness      (1000) ness      (1000)     3028 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/tonapi/__init__.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     7813 2024-04-18 22:10:30.000000 pytonapi-0.2.8/pytonapi/tonapi/client.py
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-25 11:24:44.729197 pytonapi-0.2.8/pytonapi/tonapi/methods/
--rw-rw-r--   0 ness      (1000) ness      (1000)      905 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/tonapi/methods/__init__.py
--rw-rw-r--   0 ness      (1000) ness      (1000)    14172 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/tonapi/methods/accounts.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     8771 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/tonapi/methods/blockchain.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     1592 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/tonapi/methods/dns.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     4594 2024-04-20 20:13:33.000000 pytonapi-0.2.8/pytonapi/tonapi/methods/emulate.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     1310 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/tonapi/methods/events.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     4112 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/tonapi/methods/inscriptions.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     2568 2024-04-11 12:29:15.000000 pytonapi-0.2.8/pytonapi/tonapi/methods/jettons.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     7825 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/tonapi/methods/liteserver.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     4330 2024-04-25 11:21:31.000000 pytonapi-0.2.8/pytonapi/tonapi/methods/nft.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     1680 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/tonapi/methods/rates.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     2553 2024-04-25 11:21:31.000000 pytonapi-0.2.8/pytonapi/tonapi/methods/sse.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     2325 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/tonapi/methods/staking.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      448 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/tonapi/methods/storage.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      855 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/tonapi/methods/tonconnect.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      731 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/tonapi/methods/traces.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     2279 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/tonapi/methods/wallet.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     3256 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/utils.py
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-25 11:24:44.717196 pytonapi-0.2.8/pytonapi.egg-info/
--rw-r--r--   0 ness      (1000) ness      (1000)     5377 2024-04-25 11:24:44.000000 pytonapi-0.2.8/pytonapi.egg-info/PKG-INFO
--rw-rw-r--   0 ness      (1000) ness      (1000)     2183 2024-04-25 11:24:44.000000 pytonapi-0.2.8/pytonapi.egg-info/SOURCES.txt
--rw-rw-r--   0 ness      (1000) ness      (1000)        1 2024-04-25 11:24:44.000000 pytonapi-0.2.8/pytonapi.egg-info/dependency_links.txt
--rw-rw-r--   0 ness      (1000) ness      (1000)       45 2024-04-25 11:24:44.000000 pytonapi-0.2.8/pytonapi.egg-info/requires.txt
--rw-rw-r--   0 ness      (1000) ness      (1000)        9 2024-04-25 11:24:44.000000 pytonapi-0.2.8/pytonapi.egg-info/top_level.txt
--rw-rw-r--   0 ness      (1000) ness      (1000)       38 2024-04-25 11:24:44.729197 pytonapi-0.2.8/setup.cfg
--rw-rw-r--   0 ness      (1000) ness      (1000)     1023 2024-04-25 11:24:37.000000 pytonapi-0.2.8/setup.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-26 19:28:07.264086 pytonapi-0.2.9/
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1060 2024-04-04 18:07:04.000000 pytonapi-0.2.9/LICENSE
+-rw-r--r--   0 ness      (1000) ness      (1000)     5377 2024-04-26 19:28:07.264086 pytonapi-0.2.9/PKG-INFO
+-rw-rw-r--   0 ness      (1000) ness      (1000)     4653 2024-04-04 18:07:04.000000 pytonapi-0.2.9/README.md
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-26 19:28:07.252086 pytonapi-0.2.9/pytonapi/
+-rw-rw-r--   0 ness      (1000) ness      (1000)      129 2024-04-04 18:07:04.000000 pytonapi-0.2.9/pytonapi/__init__.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-26 19:28:07.256086 pytonapi-0.2.9/pytonapi/async_tonapi/
+-rw-rw-r--   0 ness      (1000) ness      (1000)     3349 2024-04-04 18:07:04.000000 pytonapi-0.2.9/pytonapi/async_tonapi/__init__.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     9657 2024-04-26 19:21:14.000000 pytonapi-0.2.9/pytonapi/async_tonapi/client.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-26 19:28:07.256086 pytonapi-0.2.9/pytonapi/async_tonapi/methods/
+-rw-rw-r--   0 ness      (1000) ness      (1000)      967 2024-04-04 18:07:04.000000 pytonapi-0.2.9/pytonapi/async_tonapi/methods/__init__.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)    14416 2024-04-04 18:07:04.000000 pytonapi-0.2.9/pytonapi/async_tonapi/methods/accounts.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     9152 2024-04-20 19:32:54.000000 pytonapi-0.2.9/pytonapi/async_tonapi/methods/blockchain.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1655 2024-04-04 18:07:04.000000 pytonapi-0.2.9/pytonapi/async_tonapi/methods/dns.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     4670 2024-04-20 20:11:38.000000 pytonapi-0.2.9/pytonapi/async_tonapi/methods/emulate.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1347 2024-04-04 18:07:04.000000 pytonapi-0.2.9/pytonapi/async_tonapi/methods/events.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     4176 2024-04-04 18:07:04.000000 pytonapi-0.2.9/pytonapi/async_tonapi/methods/inscriptions.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2633 2024-04-11 12:27:47.000000 pytonapi-0.2.9/pytonapi/async_tonapi/methods/jettons.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     8021 2024-04-04 18:07:04.000000 pytonapi-0.2.9/pytonapi/async_tonapi/methods/liteserver.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     4509 2024-04-04 18:07:04.000000 pytonapi-0.2.9/pytonapi/async_tonapi/methods/nft.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1791 2024-04-04 18:07:04.000000 pytonapi-0.2.9/pytonapi/async_tonapi/methods/rates.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     3798 2024-04-25 11:21:31.000000 pytonapi-0.2.9/pytonapi/async_tonapi/methods/sse.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2455 2024-04-04 18:07:04.000000 pytonapi-0.2.9/pytonapi/async_tonapi/methods/staking.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      476 2024-04-04 18:07:04.000000 pytonapi-0.2.9/pytonapi/async_tonapi/methods/storage.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      895 2024-04-04 18:07:04.000000 pytonapi-0.2.9/pytonapi/async_tonapi/methods/tonconnect.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      768 2024-04-04 18:07:04.000000 pytonapi-0.2.9/pytonapi/async_tonapi/methods/traces.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2343 2024-04-04 18:07:04.000000 pytonapi-0.2.9/pytonapi/async_tonapi/methods/wallet.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2367 2024-04-25 11:21:42.000000 pytonapi-0.2.9/pytonapi/async_tonapi/methods/websocket.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2279 2024-04-22 23:25:05.000000 pytonapi-0.2.9/pytonapi/exceptions.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)        0 2024-04-25 11:21:31.000000 pytonapi-0.2.9/pytonapi/py.typed
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-26 19:28:07.260086 pytonapi-0.2.9/pytonapi/schema/
+-rw-rw-r--   0 ness      (1000) ness      (1000)      735 2024-04-25 11:21:31.000000 pytonapi-0.2.9/pytonapi/schema/__init__.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      874 2024-04-04 18:07:04.000000 pytonapi-0.2.9/pytonapi/schema/_address.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      896 2024-04-04 18:07:04.000000 pytonapi-0.2.9/pytonapi/schema/_balance.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1787 2024-04-04 18:07:04.000000 pytonapi-0.2.9/pytonapi/schema/accounts.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     7591 2024-04-04 18:07:04.000000 pytonapi-0.2.9/pytonapi/schema/blockchain.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      575 2024-04-04 18:07:04.000000 pytonapi-0.2.9/pytonapi/schema/dns.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      500 2024-04-04 18:07:04.000000 pytonapi-0.2.9/pytonapi/schema/domains.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     6158 2024-04-25 11:21:31.000000 pytonapi-0.2.9/pytonapi/schema/events.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      245 2024-04-04 18:07:04.000000 pytonapi-0.2.9/pytonapi/schema/inscriptions.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1486 2024-04-11 13:28:19.000000 pytonapi-0.2.9/pytonapi/schema/jettons.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1856 2024-04-25 11:21:31.000000 pytonapi-0.2.9/pytonapi/schema/liteserver.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1164 2024-04-04 18:07:04.000000 pytonapi-0.2.9/pytonapi/schema/nft.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      369 2024-04-04 18:07:04.000000 pytonapi-0.2.9/pytonapi/schema/rates.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1152 2024-04-04 18:07:04.000000 pytonapi-0.2.9/pytonapi/schema/staking.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      364 2024-04-04 18:07:04.000000 pytonapi-0.2.9/pytonapi/schema/storage.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      169 2024-04-04 18:07:04.000000 pytonapi-0.2.9/pytonapi/schema/tonconnect.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     3070 2024-04-26 19:13:54.000000 pytonapi-0.2.9/pytonapi/schema/traces.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-26 19:28:07.260086 pytonapi-0.2.9/pytonapi/tonapi/
+-rw-rw-r--   0 ness      (1000) ness      (1000)     3028 2024-04-04 18:07:04.000000 pytonapi-0.2.9/pytonapi/tonapi/__init__.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     7813 2024-04-18 22:10:30.000000 pytonapi-0.2.9/pytonapi/tonapi/client.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-26 19:28:07.264086 pytonapi-0.2.9/pytonapi/tonapi/methods/
+-rw-rw-r--   0 ness      (1000) ness      (1000)      905 2024-04-04 18:07:04.000000 pytonapi-0.2.9/pytonapi/tonapi/methods/__init__.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)    14172 2024-04-04 18:07:04.000000 pytonapi-0.2.9/pytonapi/tonapi/methods/accounts.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     8771 2024-04-04 18:07:04.000000 pytonapi-0.2.9/pytonapi/tonapi/methods/blockchain.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1592 2024-04-04 18:07:04.000000 pytonapi-0.2.9/pytonapi/tonapi/methods/dns.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     4594 2024-04-20 20:13:33.000000 pytonapi-0.2.9/pytonapi/tonapi/methods/emulate.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1310 2024-04-04 18:07:04.000000 pytonapi-0.2.9/pytonapi/tonapi/methods/events.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     4112 2024-04-04 18:07:04.000000 pytonapi-0.2.9/pytonapi/tonapi/methods/inscriptions.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2568 2024-04-11 12:29:15.000000 pytonapi-0.2.9/pytonapi/tonapi/methods/jettons.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     7825 2024-04-04 18:07:04.000000 pytonapi-0.2.9/pytonapi/tonapi/methods/liteserver.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     4330 2024-04-25 11:21:31.000000 pytonapi-0.2.9/pytonapi/tonapi/methods/nft.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1680 2024-04-04 18:07:04.000000 pytonapi-0.2.9/pytonapi/tonapi/methods/rates.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2553 2024-04-25 11:21:31.000000 pytonapi-0.2.9/pytonapi/tonapi/methods/sse.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2325 2024-04-04 18:07:04.000000 pytonapi-0.2.9/pytonapi/tonapi/methods/staking.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      448 2024-04-04 18:07:04.000000 pytonapi-0.2.9/pytonapi/tonapi/methods/storage.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      855 2024-04-04 18:07:04.000000 pytonapi-0.2.9/pytonapi/tonapi/methods/tonconnect.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      731 2024-04-04 18:07:04.000000 pytonapi-0.2.9/pytonapi/tonapi/methods/traces.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2279 2024-04-04 18:07:04.000000 pytonapi-0.2.9/pytonapi/tonapi/methods/wallet.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     3256 2024-04-04 18:07:04.000000 pytonapi-0.2.9/pytonapi/utils.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-26 19:28:07.256086 pytonapi-0.2.9/pytonapi.egg-info/
+-rw-r--r--   0 ness      (1000) ness      (1000)     5377 2024-04-26 19:28:07.000000 pytonapi-0.2.9/pytonapi.egg-info/PKG-INFO
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2183 2024-04-26 19:28:07.000000 pytonapi-0.2.9/pytonapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 ness      (1000) ness      (1000)        1 2024-04-26 19:28:07.000000 pytonapi-0.2.9/pytonapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 ness      (1000) ness      (1000)       45 2024-04-26 19:28:07.000000 pytonapi-0.2.9/pytonapi.egg-info/requires.txt
+-rw-rw-r--   0 ness      (1000) ness      (1000)        9 2024-04-26 19:28:07.000000 pytonapi-0.2.9/pytonapi.egg-info/top_level.txt
+-rw-rw-r--   0 ness      (1000) ness      (1000)       38 2024-04-26 19:28:07.264086 pytonapi-0.2.9/setup.cfg
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1023 2024-04-26 19:27:34.000000 pytonapi-0.2.9/setup.py
```

### Comparing `pytonapi-0.2.8/LICENSE` & `pytonapi-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.8/PKG-INFO` & `pytonapi-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytonapi
-Version: 0.2.8
+Version: 0.2.9
 Summary: Provide access to indexed TON blockchain.
 Home-page: https://github.com/tonkeeper/pytonapi/
 Author: nessshon
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pytonapi-0.2.8/README.md` & `pytonapi-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.8/pytonapi/async_tonapi/__init__.py` & `pytonapi-0.2.9/pytonapi/async_tonapi/__init__.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.8/pytonapi/async_tonapi/client.py` & `pytonapi-0.2.9/pytonapi/async_tonapi/client.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.8/pytonapi/async_tonapi/methods/__init__.py` & `pytonapi-0.2.9/pytonapi/async_tonapi/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.8/pytonapi/async_tonapi/methods/accounts.py` & `pytonapi-0.2.9/pytonapi/async_tonapi/methods/accounts.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.8/pytonapi/async_tonapi/methods/blockchain.py` & `pytonapi-0.2.9/pytonapi/async_tonapi/methods/blockchain.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.8/pytonapi/async_tonapi/methods/dns.py` & `pytonapi-0.2.9/pytonapi/async_tonapi/methods/dns.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.8/pytonapi/async_tonapi/methods/emulate.py` & `pytonapi-0.2.9/pytonapi/async_tonapi/methods/emulate.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.8/pytonapi/async_tonapi/methods/events.py` & `pytonapi-0.2.9/pytonapi/async_tonapi/methods/events.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.8/pytonapi/async_tonapi/methods/inscriptions.py` & `pytonapi-0.2.9/pytonapi/async_tonapi/methods/inscriptions.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.8/pytonapi/async_tonapi/methods/jettons.py` & `pytonapi-0.2.9/pytonapi/async_tonapi/methods/jettons.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.8/pytonapi/async_tonapi/methods/liteserver.py` & `pytonapi-0.2.9/pytonapi/async_tonapi/methods/liteserver.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.8/pytonapi/async_tonapi/methods/nft.py` & `pytonapi-0.2.9/pytonapi/async_tonapi/methods/nft.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.8/pytonapi/async_tonapi/methods/rates.py` & `pytonapi-0.2.9/pytonapi/async_tonapi/methods/rates.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.8/pytonapi/async_tonapi/methods/sse.py` & `pytonapi-0.2.9/pytonapi/async_tonapi/methods/sse.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.8/pytonapi/async_tonapi/methods/staking.py` & `pytonapi-0.2.9/pytonapi/async_tonapi/methods/staking.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.8/pytonapi/async_tonapi/methods/tonconnect.py` & `pytonapi-0.2.9/pytonapi/async_tonapi/methods/tonconnect.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.8/pytonapi/async_tonapi/methods/traces.py` & `pytonapi-0.2.9/pytonapi/async_tonapi/methods/traces.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.8/pytonapi/async_tonapi/methods/wallet.py` & `pytonapi-0.2.9/pytonapi/async_tonapi/methods/wallet.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.8/pytonapi/async_tonapi/methods/websocket.py` & `pytonapi-0.2.9/pytonapi/async_tonapi/methods/websocket.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.8/pytonapi/exceptions.py` & `pytonapi-0.2.9/pytonapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.8/pytonapi/schema/__init__.py` & `pytonapi-0.2.9/pytonapi/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.8/pytonapi/schema/_address.py` & `pytonapi-0.2.9/pytonapi/schema/_address.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.8/pytonapi/schema/_balance.py` & `pytonapi-0.2.9/pytonapi/schema/_balance.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.8/pytonapi/schema/accounts.py` & `pytonapi-0.2.9/pytonapi/schema/accounts.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.8/pytonapi/schema/blockchain.py` & `pytonapi-0.2.9/pytonapi/schema/blockchain.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.8/pytonapi/schema/dns.py` & `pytonapi-0.2.9/pytonapi/schema/dns.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.8/pytonapi/schema/events.py` & `pytonapi-0.2.9/pytonapi/schema/events.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.8/pytonapi/schema/jettons.py` & `pytonapi-0.2.9/pytonapi/schema/jettons.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.8/pytonapi/schema/liteserver.py` & `pytonapi-0.2.9/pytonapi/schema/liteserver.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.8/pytonapi/schema/nft.py` & `pytonapi-0.2.9/pytonapi/schema/nft.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.8/pytonapi/schema/staking.py` & `pytonapi-0.2.9/pytonapi/schema/staking.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.8/pytonapi/schema/traces.py` & `pytonapi-0.2.9/pytonapi/schema/traces.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,17 +69,15 @@
     gas_fees: Optional[int]
     gas_used: Optional[int]
     vm_steps: Optional[int]
     exit_code: Optional[int]
 
 
 class StateInit(BaseModel):
-    code: Optional[str]
-    data: Optional[str]
-    library: Dict[str, str]
+    boc: str
 
 
 class Message(BaseModel):
     created_lt: int
     ihr_disabled: bool
     bounce: bool
     bounced: bool
```

### Comparing `pytonapi-0.2.8/pytonapi/tonapi/__init__.py` & `pytonapi-0.2.9/pytonapi/tonapi/__init__.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.8/pytonapi/tonapi/client.py` & `pytonapi-0.2.9/pytonapi/tonapi/client.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.8/pytonapi/tonapi/methods/__init__.py` & `pytonapi-0.2.9/pytonapi/tonapi/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.8/pytonapi/tonapi/methods/accounts.py` & `pytonapi-0.2.9/pytonapi/tonapi/methods/accounts.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.8/pytonapi/tonapi/methods/blockchain.py` & `pytonapi-0.2.9/pytonapi/tonapi/methods/blockchain.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.8/pytonapi/tonapi/methods/dns.py` & `pytonapi-0.2.9/pytonapi/tonapi/methods/dns.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.8/pytonapi/tonapi/methods/emulate.py` & `pytonapi-0.2.9/pytonapi/tonapi/methods/emulate.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.8/pytonapi/tonapi/methods/events.py` & `pytonapi-0.2.9/pytonapi/tonapi/methods/events.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.8/pytonapi/tonapi/methods/inscriptions.py` & `pytonapi-0.2.9/pytonapi/tonapi/methods/inscriptions.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.8/pytonapi/tonapi/methods/jettons.py` & `pytonapi-0.2.9/pytonapi/tonapi/methods/jettons.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.8/pytonapi/tonapi/methods/liteserver.py` & `pytonapi-0.2.9/pytonapi/tonapi/methods/liteserver.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.8/pytonapi/tonapi/methods/nft.py` & `pytonapi-0.2.9/pytonapi/tonapi/methods/nft.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.8/pytonapi/tonapi/methods/rates.py` & `pytonapi-0.2.9/pytonapi/tonapi/methods/rates.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.8/pytonapi/tonapi/methods/sse.py` & `pytonapi-0.2.9/pytonapi/tonapi/methods/sse.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.8/pytonapi/tonapi/methods/staking.py` & `pytonapi-0.2.9/pytonapi/tonapi/methods/staking.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.8/pytonapi/tonapi/methods/tonconnect.py` & `pytonapi-0.2.9/pytonapi/tonapi/methods/tonconnect.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.8/pytonapi/tonapi/methods/traces.py` & `pytonapi-0.2.9/pytonapi/tonapi/methods/traces.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.8/pytonapi/tonapi/methods/wallet.py` & `pytonapi-0.2.9/pytonapi/tonapi/methods/wallet.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.8/pytonapi/utils.py` & `pytonapi-0.2.9/pytonapi/utils.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.8/pytonapi.egg-info/PKG-INFO` & `pytonapi-0.2.9/pytonapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytonapi
-Version: 0.2.8
+Version: 0.2.9
 Summary: Provide access to indexed TON blockchain.
 Home-page: https://github.com/tonkeeper/pytonapi/
 Author: nessshon
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pytonapi-0.2.8/pytonapi.egg-info/SOURCES.txt` & `pytonapi-0.2.9/pytonapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.8/setup.py` & `pytonapi-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pytonapi",
-    version="0.2.8",
+    version="0.2.9",
     author="nessshon",
     description="Provide access to indexed TON blockchain.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/tonkeeper/pytonapi/",
     packages=setuptools.find_packages(exclude=["examples", "tests"]),
     install_requires=[
```
