# Comparing `tmp/benchmarl-1.1.1.tar.gz` & `tmp/benchmarl-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "benchmarl-1.1.1.tar", last modified: Mon Mar  4 10:04:08 2024, max compression
+gzip compressed data, was "benchmarl-1.2.0.tar", last modified: Fri Apr 26 10:59:25 2024, max compression
```

## Comparing `benchmarl-1.1.1.tar` & `benchmarl-1.2.0.tar`

### file list

```diff
@@ -1,160 +1,219 @@
-drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-03-04 10:04:08.382219 benchmarl-1.1.1/
--rw-r--r--   0 Matteo     (501) staff       (20)     1088 2023-10-20 08:48:13.000000 benchmarl-1.1.1/LICENSE
--rw-r--r--   0 Matteo     (501) staff       (20)      276 2024-03-04 10:04:08.382300 benchmarl-1.1.1/PKG-INFO
--rw-r--r--   0 Matteo     (501) staff       (20)    29313 2024-02-23 11:14:35.000000 benchmarl-1.1.1/README.md
-drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-03-04 10:04:08.317512 benchmarl-1.1.1/benchmarl/
--rw-r--r--   0 Matteo     (501) staff       (20)     1312 2024-03-04 10:02:48.000000 benchmarl-1.1.1/benchmarl/__init__.py
-drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-03-04 10:04:08.321508 benchmarl-1.1.1/benchmarl/algorithms/
--rw-r--r--   0 Matteo     (501) staff       (20)     1208 2023-11-28 10:20:07.000000 benchmarl-1.1.1/benchmarl/algorithms/__init__.py
--rw-r--r--   0 Matteo     (501) staff       (20)    15198 2023-11-28 10:20:07.000000 benchmarl-1.1.1/benchmarl/algorithms/common.py
--rw-r--r--   0 Matteo     (501) staff       (20)     9637 2024-02-29 12:42:04.000000 benchmarl-1.1.1/benchmarl/algorithms/iddpg.py
--rw-r--r--   0 Matteo     (501) staff       (20)    11400 2024-02-02 14:35:11.000000 benchmarl-1.1.1/benchmarl/algorithms/ippo.py
--rw-r--r--   0 Matteo     (501) staff       (20)     7147 2023-11-28 10:20:07.000000 benchmarl-1.1.1/benchmarl/algorithms/iql.py
--rw-r--r--   0 Matteo     (501) staff       (20)    15299 2024-02-24 13:54:54.000000 benchmarl-1.1.1/benchmarl/algorithms/isac.py
--rw-r--r--   0 Matteo     (501) staff       (20)    11762 2024-02-24 13:54:54.000000 benchmarl-1.1.1/benchmarl/algorithms/maddpg.py
--rw-r--r--   0 Matteo     (501) staff       (20)    12711 2024-02-02 14:35:11.000000 benchmarl-1.1.1/benchmarl/algorithms/mappo.py
--rw-r--r--   0 Matteo     (501) staff       (20)    18722 2024-02-24 13:54:54.000000 benchmarl-1.1.1/benchmarl/algorithms/masac.py
--rw-r--r--   0 Matteo     (501) staff       (20)     7752 2023-11-28 10:20:07.000000 benchmarl-1.1.1/benchmarl/algorithms/qmix.py
--rw-r--r--   0 Matteo     (501) staff       (20)     7176 2023-11-28 10:20:07.000000 benchmarl-1.1.1/benchmarl/algorithms/vdn.py
-drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-03-04 10:04:08.343045 benchmarl-1.1.1/benchmarl/benchmark/
--rw-r--r--   0 Matteo     (501) staff       (20)      214 2023-11-28 10:20:07.000000 benchmarl-1.1.1/benchmarl/benchmark/__init__.py
--rw-r--r--   0 Matteo     (501) staff       (20)     2946 2023-11-28 10:20:07.000000 benchmarl-1.1.1/benchmarl/benchmark/benchmark.py
-drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-03-04 10:04:08.322214 benchmarl-1.1.1/benchmarl/conf/
--rw-r--r--   0 Matteo     (501) staff       (20)     6148 2024-01-18 11:10:46.000000 benchmarl-1.1.1/benchmarl/conf/.DS_Store
--rw-r--r--   0 Matteo     (501) staff       (20)      180 2023-10-20 08:48:13.000000 benchmarl-1.1.1/benchmarl/conf/__init__.py
-drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-03-04 10:04:08.322538 benchmarl-1.1.1/benchmarl/conf/__pycache__/
--rw-r--r--   0 Matteo     (501) staff       (20)      157 2023-11-27 09:02:40.000000 benchmarl-1.1.1/benchmarl/conf/__pycache__/__init__.cpython-39.pyc
-drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-03-04 10:04:08.324498 benchmarl-1.1.1/benchmarl/conf/algorithm/
--rw-r--r--   0 Matteo     (501) staff       (20)      126 2024-01-17 10:12:32.000000 benchmarl-1.1.1/benchmarl/conf/algorithm/iddpg.yaml
--rw-r--r--   0 Matteo     (501) staff       (20)      210 2024-01-17 10:12:32.000000 benchmarl-1.1.1/benchmarl/conf/algorithm/ippo.yaml
--rw-r--r--   0 Matteo     (501) staff       (20)       76 2023-10-14 08:15:47.000000 benchmarl-1.1.1/benchmarl/conf/algorithm/iql.yaml
--rw-r--r--   0 Matteo     (501) staff       (20)      311 2024-01-17 10:29:41.000000 benchmarl-1.1.1/benchmarl/conf/algorithm/isac.yaml
--rw-r--r--   0 Matteo     (501) staff       (20)      127 2024-01-17 10:12:32.000000 benchmarl-1.1.1/benchmarl/conf/algorithm/maddpg.yaml
--rw-r--r--   0 Matteo     (501) staff       (20)      212 2024-01-17 10:12:32.000000 benchmarl-1.1.1/benchmarl/conf/algorithm/mappo.yaml
--rw-r--r--   0 Matteo     (501) staff       (20)      307 2024-02-23 15:25:15.000000 benchmarl-1.1.1/benchmarl/conf/algorithm/masac.yaml
--rw-r--r--   0 Matteo     (501) staff       (20)       98 2023-10-14 08:15:47.000000 benchmarl-1.1.1/benchmarl/conf/algorithm/qmix.yaml
--rw-r--r--   0 Matteo     (501) staff       (20)       75 2023-10-14 08:15:47.000000 benchmarl-1.1.1/benchmarl/conf/algorithm/vdn.yaml
--rw-r--r--   0 Matteo     (501) staff       (20)      152 2024-01-17 09:09:44.000000 benchmarl-1.1.1/benchmarl/conf/config.yaml
-drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-03-04 10:04:08.324678 benchmarl-1.1.1/benchmarl/conf/experiment/
--rw-r--r--   0 Matteo     (501) staff       (20)     4274 2024-01-19 11:33:16.000000 benchmarl-1.1.1/benchmarl/conf/experiment/base_experiment.yaml
-drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-03-04 10:04:08.324980 benchmarl-1.1.1/benchmarl/conf/model/
-drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-03-04 10:04:08.325337 benchmarl-1.1.1/benchmarl/conf/model/layers/
--rw-r--r--   0 Matteo     (501) staff       (20)      116 2023-11-28 10:20:07.000000 benchmarl-1.1.1/benchmarl/conf/model/layers/gnn.yaml
--rw-r--r--   0 Matteo     (501) staff       (20)      156 2023-11-28 10:20:07.000000 benchmarl-1.1.1/benchmarl/conf/model/layers/mlp.yaml
--rw-r--r--   0 Matteo     (501) staff       (20)      433 2023-10-14 08:15:47.000000 benchmarl-1.1.1/benchmarl/conf/model/sequence.yaml
-drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-03-04 10:04:08.314304 benchmarl-1.1.1/benchmarl/conf/task/
-drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-03-04 10:04:08.327037 benchmarl-1.1.1/benchmarl/conf/task/pettingzoo/
--rw-r--r--   0 Matteo     (501) staff       (20)     1135 2023-10-20 08:48:13.000000 benchmarl-1.1.1/benchmarl/conf/task/pettingzoo/multiwalker.yaml
--rw-r--r--   0 Matteo     (501) staff       (20)      110 2023-10-20 08:48:13.000000 benchmarl-1.1.1/benchmarl/conf/task/pettingzoo/simple_adversary.yaml
--rw-r--r--   0 Matteo     (501) staff       (20)       99 2023-10-20 08:48:13.000000 benchmarl-1.1.1/benchmarl/conf/task/pettingzoo/simple_crypto.yaml
--rw-r--r--   0 Matteo     (501) staff       (20)       95 2023-10-20 08:48:13.000000 benchmarl-1.1.1/benchmarl/conf/task/pettingzoo/simple_push.yaml
--rw-r--r--   0 Matteo     (501) staff       (20)      122 2023-10-20 08:48:13.000000 benchmarl-1.1.1/benchmarl/conf/task/pettingzoo/simple_reference.yaml
--rw-r--r--   0 Matteo     (501) staff       (20)      119 2023-10-20 08:48:13.000000 benchmarl-1.1.1/benchmarl/conf/task/pettingzoo/simple_speaker_listener.yaml
--rw-r--r--   0 Matteo     (501) staff       (20)      121 2023-10-20 08:48:13.000000 benchmarl-1.1.1/benchmarl/conf/task/pettingzoo/simple_spread.yaml
--rw-r--r--   0 Matteo     (501) staff       (20)      141 2023-10-20 08:48:13.000000 benchmarl-1.1.1/benchmarl/conf/task/pettingzoo/simple_tag.yaml
--rw-r--r--   0 Matteo     (501) staff       (20)      182 2023-10-20 08:48:13.000000 benchmarl-1.1.1/benchmarl/conf/task/pettingzoo/simple_world_comm.yaml
--rw-r--r--   0 Matteo     (501) staff       (20)      424 2023-10-20 08:48:13.000000 benchmarl-1.1.1/benchmarl/conf/task/pettingzoo/waterworld.yaml
-drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-03-04 10:04:08.329144 benchmarl-1.1.1/benchmarl/conf/task/smacv2/
--rw-r--r--   0 Matteo     (501) staff       (20)     1152 2023-10-20 08:48:13.000000 benchmarl-1.1.1/benchmarl/conf/task/smacv2/protoss_10_vs_10.yaml
--rw-r--r--   0 Matteo     (501) staff       (20)     1152 2023-10-20 08:48:13.000000 benchmarl-1.1.1/benchmarl/conf/task/smacv2/protoss_10_vs_11.yaml
--rw-r--r--   0 Matteo     (501) staff       (20)     1152 2023-10-20 08:48:13.000000 benchmarl-1.1.1/benchmarl/conf/task/smacv2/protoss_20_vs_20.yaml
--rw-r--r--   0 Matteo     (501) staff       (20)     1152 2023-10-20 08:48:13.000000 benchmarl-1.1.1/benchmarl/conf/task/smacv2/protoss_20_vs_23.yaml
--rw-r--r--   0 Matteo     (501) staff       (20)     1150 2023-10-14 08:15:47.000000 benchmarl-1.1.1/benchmarl/conf/task/smacv2/protoss_5_vs_5.yaml
--rw-r--r--   0 Matteo     (501) staff       (20)     1195 2023-10-20 08:48:13.000000 benchmarl-1.1.1/benchmarl/conf/task/smacv2/terran_10_vs_10.yaml
--rw-r--r--   0 Matteo     (501) staff       (20)     1195 2023-10-20 08:48:13.000000 benchmarl-1.1.1/benchmarl/conf/task/smacv2/terran_10_vs_11.yaml
--rw-r--r--   0 Matteo     (501) staff       (20)     1195 2023-10-20 08:48:13.000000 benchmarl-1.1.1/benchmarl/conf/task/smacv2/terran_20_vs_20.yaml
--rw-r--r--   0 Matteo     (501) staff       (20)     1195 2023-10-20 08:48:13.000000 benchmarl-1.1.1/benchmarl/conf/task/smacv2/terran_20_vs_23.yaml
--rw-r--r--   0 Matteo     (501) staff       (20)     1193 2023-10-20 08:48:13.000000 benchmarl-1.1.1/benchmarl/conf/task/smacv2/terran_5_vs_5.yaml
--rw-r--r--   0 Matteo     (501) staff       (20)     1198 2023-10-20 08:48:13.000000 benchmarl-1.1.1/benchmarl/conf/task/smacv2/zerg_10_vs_10.yaml
--rw-r--r--   0 Matteo     (501) staff       (20)     1198 2023-10-20 08:48:13.000000 benchmarl-1.1.1/benchmarl/conf/task/smacv2/zerg_10_vs_11.yaml
--rw-r--r--   0 Matteo     (501) staff       (20)     1198 2023-10-20 08:48:13.000000 benchmarl-1.1.1/benchmarl/conf/task/smacv2/zerg_20_vs_20.yaml
--rw-r--r--   0 Matteo     (501) staff       (20)     1198 2023-10-20 08:48:13.000000 benchmarl-1.1.1/benchmarl/conf/task/smacv2/zerg_20_vs_23.yaml
--rw-r--r--   0 Matteo     (501) staff       (20)     1196 2023-10-20 08:48:13.000000 benchmarl-1.1.1/benchmarl/conf/task/smacv2/zerg_5_vs_5.yaml
-drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-03-04 10:04:08.342627 benchmarl-1.1.1/benchmarl/conf/task/vmas/
--rw-r--r--   0 Matteo     (501) staff       (20)      123 2023-10-20 08:48:13.000000 benchmarl-1.1.1/benchmarl/conf/task/vmas/balance.yaml
--rw-r--r--   0 Matteo     (501) staff       (20)      145 2024-02-01 15:20:17.000000 benchmarl-1.1.1/benchmarl/conf/task/vmas/dispersion.yaml
--rw-r--r--   0 Matteo     (501) staff       (20)      117 2024-02-01 15:20:17.000000 benchmarl-1.1.1/benchmarl/conf/task/vmas/dropout.yaml
--rw-r--r--   0 Matteo     (501) staff       (20)      152 2024-02-01 15:20:17.000000 benchmarl-1.1.1/benchmarl/conf/task/vmas/give_way.yaml
--rw-r--r--   0 Matteo     (501) staff       (20)      217 2024-01-17 09:20:02.000000 benchmarl-1.1.1/benchmarl/conf/task/vmas/navigation.yaml
--rw-r--r--   0 Matteo     (501) staff       (20)      139 2024-02-01 15:20:17.000000 benchmarl-1.1.1/benchmarl/conf/task/vmas/reverse_transport.yaml
--rw-r--r--   0 Matteo     (501) staff       (20)      174 2024-02-01 15:20:17.000000 benchmarl-1.1.1/benchmarl/conf/task/vmas/sampling.yaml
--rw-r--r--   0 Matteo     (501) staff       (20)       99 2023-12-26 13:20:37.000000 benchmarl-1.1.1/benchmarl/conf/task/vmas/simple_adversary.yaml
--rw-r--r--   0 Matteo     (501) staff       (20)       76 2023-12-26 13:20:37.000000 benchmarl-1.1.1/benchmarl/conf/task/vmas/simple_crypto.yaml
--rw-r--r--   0 Matteo     (501) staff       (20)       65 2023-12-26 13:20:37.000000 benchmarl-1.1.1/benchmarl/conf/task/vmas/simple_push.yaml
--rw-r--r--   0 Matteo     (501) staff       (20)       70 2023-12-26 13:20:32.000000 benchmarl-1.1.1/benchmarl/conf/task/vmas/simple_reference.yaml
--rw-r--r--   0 Matteo     (501) staff       (20)       77 2023-12-26 13:20:37.000000 benchmarl-1.1.1/benchmarl/conf/task/vmas/simple_speaker_listener.yaml
--rw-r--r--   0 Matteo     (501) staff       (20)       96 2023-12-26 13:20:37.000000 benchmarl-1.1.1/benchmarl/conf/task/vmas/simple_spread.yaml
--rw-r--r--   0 Matteo     (501) staff       (20)      316 2023-12-26 13:20:32.000000 benchmarl-1.1.1/benchmarl/conf/task/vmas/simple_tag.yaml
--rw-r--r--   0 Matteo     (501) staff       (20)      153 2023-12-26 13:20:37.000000 benchmarl-1.1.1/benchmarl/conf/task/vmas/simple_world_comm.yaml
--rw-r--r--   0 Matteo     (501) staff       (20)      148 2023-10-20 08:48:13.000000 benchmarl-1.1.1/benchmarl/conf/task/vmas/transport.yaml
--rw-r--r--   0 Matteo     (501) staff       (20)      123 2023-10-20 08:48:13.000000 benchmarl-1.1.1/benchmarl/conf/task/vmas/wheel.yaml
--rw-r--r--   0 Matteo     (501) staff       (20)      330 2024-02-01 15:20:17.000000 benchmarl-1.1.1/benchmarl/conf/task/vmas/wind_flocking.yaml
-drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-03-04 10:04:08.346505 benchmarl-1.1.1/benchmarl/environments/
--rw-r--r--   0 Matteo     (501) staff       (20)     4437 2024-02-01 15:20:17.000000 benchmarl-1.1.1/benchmarl/environments/__init__.py
--rw-r--r--   0 Matteo     (501) staff       (20)     8830 2023-12-26 12:06:50.000000 benchmarl-1.1.1/benchmarl/environments/common.py
-drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-03-04 10:04:08.350421 benchmarl-1.1.1/benchmarl/environments/pettingzoo/
--rw-r--r--   0 Matteo     (501) staff       (20)      180 2023-10-20 08:48:13.000000 benchmarl-1.1.1/benchmarl/environments/pettingzoo/__init__.py
--rw-r--r--   0 Matteo     (501) staff       (20)     5015 2023-12-26 12:06:50.000000 benchmarl-1.1.1/benchmarl/environments/pettingzoo/common.py
--rw-r--r--   0 Matteo     (501) staff       (20)      655 2024-01-19 11:33:16.000000 benchmarl-1.1.1/benchmarl/environments/pettingzoo/multiwalker.py
--rw-r--r--   0 Matteo     (501) staff       (20)      330 2023-12-26 12:20:31.000000 benchmarl-1.1.1/benchmarl/environments/pettingzoo/simple_adverasary.py
--rw-r--r--   0 Matteo     (501) staff       (20)      309 2023-10-20 08:48:13.000000 benchmarl-1.1.1/benchmarl/environments/pettingzoo/simple_crypto.py
--rw-r--r--   0 Matteo     (501) staff       (20)      309 2023-11-28 10:20:07.000000 benchmarl-1.1.1/benchmarl/environments/pettingzoo/simple_push.py
--rw-r--r--   0 Matteo     (501) staff       (20)      309 2023-10-20 08:48:13.000000 benchmarl-1.1.1/benchmarl/environments/pettingzoo/simple_reference.py
--rw-r--r--   0 Matteo     (501) staff       (20)      309 2023-10-20 08:48:13.000000 benchmarl-1.1.1/benchmarl/environments/pettingzoo/simple_speaker_listener.py
--rw-r--r--   0 Matteo     (501) staff       (20)      363 2023-10-20 08:48:13.000000 benchmarl-1.1.1/benchmarl/environments/pettingzoo/simple_spread.py
--rw-r--r--   0 Matteo     (501) staff       (20)      405 2023-10-20 08:48:13.000000 benchmarl-1.1.1/benchmarl/environments/pettingzoo/simple_tag.py
--rw-r--r--   0 Matteo     (501) staff       (20)      464 2023-10-20 08:48:13.000000 benchmarl-1.1.1/benchmarl/environments/pettingzoo/simple_world_comm.py
--rw-r--r--   0 Matteo     (501) staff       (20)      934 2023-11-28 10:20:07.000000 benchmarl-1.1.1/benchmarl/environments/pettingzoo/waterworld.py
-drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-03-04 10:04:08.352458 benchmarl-1.1.1/benchmarl/environments/smacv2/
--rw-r--r--   0 Matteo     (501) staff       (20)      180 2023-10-20 08:48:13.000000 benchmarl-1.1.1/benchmarl/environments/smacv2/__init__.py
--rw-r--r--   0 Matteo     (501) staff       (20)     3378 2023-11-28 10:20:07.000000 benchmarl-1.1.1/benchmarl/environments/smacv2/common.py
-drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-03-04 10:04:08.372466 benchmarl-1.1.1/benchmarl/environments/vmas/
--rw-r--r--   0 Matteo     (501) staff       (20)      180 2023-11-23 12:19:19.000000 benchmarl-1.1.1/benchmarl/environments/vmas/__init__.py
--rw-r--r--   0 Matteo     (501) staff       (20)      393 2023-10-20 08:48:13.000000 benchmarl-1.1.1/benchmarl/environments/vmas/balance.py
--rw-r--r--   0 Matteo     (501) staff       (20)     2947 2024-02-02 14:56:04.000000 benchmarl-1.1.1/benchmarl/environments/vmas/common.py
--rw-r--r--   0 Matteo     (501) staff       (20)      438 2024-02-01 15:20:17.000000 benchmarl-1.1.1/benchmarl/environments/vmas/dispersion.py
--rw-r--r--   0 Matteo     (501) staff       (20)      383 2024-02-01 15:20:17.000000 benchmarl-1.1.1/benchmarl/environments/vmas/dropout.py
--rw-r--r--   0 Matteo     (501) staff       (20)      428 2024-02-01 15:20:17.000000 benchmarl-1.1.1/benchmarl/environments/vmas/give_way.py
--rw-r--r--   0 Matteo     (501) staff       (20)      552 2023-10-20 08:48:13.000000 benchmarl-1.1.1/benchmarl/environments/vmas/navigation.py
--rw-r--r--   0 Matteo     (501) staff       (20)      417 2024-02-01 15:20:17.000000 benchmarl-1.1.1/benchmarl/environments/vmas/reverse_transport.py
--rw-r--r--   0 Matteo     (501) staff       (20)      498 2024-02-01 15:20:17.000000 benchmarl-1.1.1/benchmarl/environments/vmas/sampling.py
--rw-r--r--   0 Matteo     (501) staff       (20)      345 2023-12-26 13:20:37.000000 benchmarl-1.1.1/benchmarl/environments/vmas/simple_adverasary.py
--rw-r--r--   0 Matteo     (501) staff       (20)      309 2023-12-26 13:20:37.000000 benchmarl-1.1.1/benchmarl/environments/vmas/simple_crypto.py
--rw-r--r--   0 Matteo     (501) staff       (20)      284 2023-12-26 13:20:37.000000 benchmarl-1.1.1/benchmarl/environments/vmas/simple_push.py
--rw-r--r--   0 Matteo     (501) staff       (20)      284 2023-12-26 13:20:32.000000 benchmarl-1.1.1/benchmarl/environments/vmas/simple_reference.py
--rw-r--r--   0 Matteo     (501) staff       (20)      284 2023-12-26 13:20:37.000000 benchmarl-1.1.1/benchmarl/environments/vmas/simple_speaker_listener.py
--rw-r--r--   0 Matteo     (501) staff       (20)      343 2023-12-26 13:20:37.000000 benchmarl-1.1.1/benchmarl/environments/vmas/simple_spread.py
--rw-r--r--   0 Matteo     (501) staff       (20)      708 2023-12-26 13:20:32.000000 benchmarl-1.1.1/benchmarl/environments/vmas/simple_tag.py
--rw-r--r--   0 Matteo     (501) staff       (20)      446 2023-12-26 13:20:37.000000 benchmarl-1.1.1/benchmarl/environments/vmas/simple_world_comm.py
--rw-r--r--   0 Matteo     (501) staff       (20)      447 2023-10-20 08:48:13.000000 benchmarl-1.1.1/benchmarl/environments/vmas/transport.py
--rw-r--r--   0 Matteo     (501) staff       (20)      414 2023-10-20 08:48:13.000000 benchmarl-1.1.1/benchmarl/environments/vmas/wheel.py
--rw-r--r--   0 Matteo     (501) staff       (20)      762 2024-02-01 15:20:17.000000 benchmarl-1.1.1/benchmarl/environments/vmas/wind_flocking.py
--rw-r--r--   0 Matteo     (501) staff       (20)     7619 2023-11-28 10:20:07.000000 benchmarl-1.1.1/benchmarl/eval_results.py
-drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-03-04 10:04:08.375779 benchmarl-1.1.1/benchmarl/experiment/
--rw-r--r--   0 Matteo     (501) staff       (20)      265 2023-11-28 10:20:07.000000 benchmarl-1.1.1/benchmarl/experiment/__init__.py
--rw-r--r--   0 Matteo     (501) staff       (20)     3045 2024-01-17 09:07:49.000000 benchmarl-1.1.1/benchmarl/experiment/callback.py
--rw-r--r--   0 Matteo     (501) staff       (20)    28853 2024-02-24 13:09:13.000000 benchmarl-1.1.1/benchmarl/experiment/experiment.py
--rw-r--r--   0 Matteo     (501) staff       (20)    13138 2023-12-26 12:06:50.000000 benchmarl-1.1.1/benchmarl/experiment/logger.py
--rw-r--r--   0 Matteo     (501) staff       (20)     3613 2023-11-28 10:20:07.000000 benchmarl-1.1.1/benchmarl/hydra_config.py
-drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-03-04 10:04:08.378413 benchmarl-1.1.1/benchmarl/models/
--rw-r--r--   0 Matteo     (501) staff       (20)      434 2023-11-28 10:20:07.000000 benchmarl-1.1.1/benchmarl/models/__init__.py
--rw-r--r--   0 Matteo     (501) staff       (20)    16029 2023-11-28 10:20:07.000000 benchmarl-1.1.1/benchmarl/models/common.py
--rw-r--r--   0 Matteo     (501) staff       (20)     9209 2023-11-28 10:20:07.000000 benchmarl-1.1.1/benchmarl/models/gnn.py
--rw-r--r--   0 Matteo     (501) staff       (20)     4760 2024-02-24 13:08:47.000000 benchmarl-1.1.1/benchmarl/models/mlp.py
--rw-r--r--   0 Matteo     (501) staff       (20)     1182 2023-11-28 10:20:07.000000 benchmarl-1.1.1/benchmarl/run.py
--rw-r--r--   0 Matteo     (501) staff       (20)     1406 2023-12-26 12:06:50.000000 benchmarl-1.1.1/benchmarl/utils.py
-drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-03-04 10:04:08.318353 benchmarl-1.1.1/benchmarl.egg-info/
--rw-r--r--   0 Matteo     (501) staff       (20)      276 2024-03-04 10:04:08.000000 benchmarl-1.1.1/benchmarl.egg-info/PKG-INFO
--rw-r--r--   0 Matteo     (501) staff       (20)    34857 2024-03-04 10:04:08.000000 benchmarl-1.1.1/benchmarl.egg-info/SOURCES.txt
--rw-r--r--   0 Matteo     (501) staff       (20)        1 2024-03-04 10:04:08.000000 benchmarl-1.1.1/benchmarl.egg-info/dependency_links.txt
--rw-r--r--   0 Matteo     (501) staff       (20)      112 2024-03-04 10:04:08.000000 benchmarl-1.1.1/benchmarl.egg-info/requires.txt
--rw-r--r--   0 Matteo     (501) staff       (20)       10 2024-03-04 10:04:08.000000 benchmarl-1.1.1/benchmarl.egg-info/top_level.txt
--rw-r--r--   0 Matteo     (501) staff       (20)      432 2024-03-04 10:04:08.382723 benchmarl-1.1.1/setup.cfg
--rw-r--r--   0 Matteo     (501) staff       (20)     1143 2024-03-04 10:02:48.000000 benchmarl-1.1.1/setup.py
-drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-03-04 10:04:08.381955 benchmarl-1.1.1/test/
--rw-r--r--   0 Matteo     (501) staff       (20)      959 2023-10-20 08:48:13.000000 benchmarl-1.1.1/test/test_algorithm.py
--rw-r--r--   0 Matteo     (501) staff       (20)     2043 2023-11-27 13:14:07.000000 benchmarl-1.1.1/test/test_models.py
--rw-r--r--   0 Matteo     (501) staff       (20)     5022 2024-02-24 13:44:46.000000 benchmarl-1.1.1/test/test_pettingzoo.py
--rw-r--r--   0 Matteo     (501) staff       (20)     2462 2023-12-26 12:06:29.000000 benchmarl-1.1.1/test/test_smacv2.py
--rw-r--r--   0 Matteo     (501) staff       (20)      966 2023-10-20 08:48:13.000000 benchmarl-1.1.1/test/test_task.py
--rw-r--r--   0 Matteo     (501) staff       (20)     4678 2024-02-24 13:54:54.000000 benchmarl-1.1.1/test/test_vmas.py
+drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-04-26 10:59:25.165416 benchmarl-1.2.0/
+-rw-r--r--   0 Matteo     (501) staff       (20)     1088 2023-10-20 08:48:13.000000 benchmarl-1.2.0/LICENSE
+-rw-r--r--   0 Matteo     (501) staff       (20)      739 2024-04-26 10:59:25.165328 benchmarl-1.2.0/PKG-INFO
+-rw-r--r--   0 Matteo     (501) staff       (20)    29627 2024-04-23 09:25:28.000000 benchmarl-1.2.0/README.md
+drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-04-26 10:59:24.904828 benchmarl-1.2.0/benchmarl/
+-rw-r--r--   0 Matteo     (501) staff       (20)     1312 2024-04-26 10:59:00.000000 benchmarl-1.2.0/benchmarl/__init__.py
+drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-04-26 10:59:24.907510 benchmarl-1.2.0/benchmarl/algorithms/
+-rw-r--r--   0 Matteo     (501) staff       (20)     1208 2023-11-28 10:20:07.000000 benchmarl-1.2.0/benchmarl/algorithms/__init__.py
+-rw-r--r--   0 Matteo     (501) staff       (20)    15228 2024-04-23 09:25:28.000000 benchmarl-1.2.0/benchmarl/algorithms/common.py
+-rw-r--r--   0 Matteo     (501) staff       (20)     8688 2024-04-23 09:25:28.000000 benchmarl-1.2.0/benchmarl/algorithms/iddpg.py
+-rw-r--r--   0 Matteo     (501) staff       (20)    10898 2024-04-26 10:59:00.000000 benchmarl-1.2.0/benchmarl/algorithms/ippo.py
+-rw-r--r--   0 Matteo     (501) staff       (20)     6896 2024-04-23 09:25:28.000000 benchmarl-1.2.0/benchmarl/algorithms/iql.py
+-rw-r--r--   0 Matteo     (501) staff       (20)    14135 2024-04-23 09:25:28.000000 benchmarl-1.2.0/benchmarl/algorithms/isac.py
+-rw-r--r--   0 Matteo     (501) staff       (20)    10483 2024-04-23 09:25:28.000000 benchmarl-1.2.0/benchmarl/algorithms/maddpg.py
+-rw-r--r--   0 Matteo     (501) staff       (20)    12173 2024-04-23 09:25:28.000000 benchmarl-1.2.0/benchmarl/algorithms/mappo.py
+-rw-r--r--   0 Matteo     (501) staff       (20)    17192 2024-04-23 09:25:28.000000 benchmarl-1.2.0/benchmarl/algorithms/masac.py
+-rw-r--r--   0 Matteo     (501) staff       (20)     7675 2024-04-23 09:25:28.000000 benchmarl-1.2.0/benchmarl/algorithms/qmix.py
+-rw-r--r--   0 Matteo     (501) staff       (20)     6925 2024-04-23 09:25:28.000000 benchmarl-1.2.0/benchmarl/algorithms/vdn.py
+drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-04-26 10:59:24.932896 benchmarl-1.2.0/benchmarl/benchmark/
+-rw-r--r--   0 Matteo     (501) staff       (20)      214 2023-11-28 10:20:07.000000 benchmarl-1.2.0/benchmarl/benchmark/__init__.py
+-rw-r--r--   0 Matteo     (501) staff       (20)     2946 2023-11-28 10:20:07.000000 benchmarl-1.2.0/benchmarl/benchmark/benchmark.py
+drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-04-26 10:59:25.142125 benchmarl-1.2.0/benchmarl/conf/
+-rw-r--r--   0 Matteo     (501) staff       (20)    10244 2024-04-19 07:45:52.000000 benchmarl-1.2.0/benchmarl/conf/.DS_Store
+-rw-r--r--   0 Matteo     (501) staff       (20)      180 2023-10-20 08:48:13.000000 benchmarl-1.2.0/benchmarl/conf/__init__.py
+drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-04-26 10:59:25.142453 benchmarl-1.2.0/benchmarl/conf/__pycache__/
+-rw-r--r--   0 Matteo     (501) staff       (20)      175 2024-04-24 14:11:36.000000 benchmarl-1.2.0/benchmarl/conf/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 Matteo     (501) staff       (20)      157 2023-11-27 09:02:40.000000 benchmarl-1.2.0/benchmarl/conf/__pycache__/__init__.cpython-39.pyc
+drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-04-26 10:59:25.143813 benchmarl-1.2.0/benchmarl/conf/algorithm/
+-rw-r--r--   0 Matteo     (501) staff       (20)      126 2024-01-17 10:12:32.000000 benchmarl-1.2.0/benchmarl/conf/algorithm/iddpg.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)      210 2024-01-17 10:12:32.000000 benchmarl-1.2.0/benchmarl/conf/algorithm/ippo.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)       76 2023-10-14 08:15:47.000000 benchmarl-1.2.0/benchmarl/conf/algorithm/iql.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)      311 2024-01-17 10:29:41.000000 benchmarl-1.2.0/benchmarl/conf/algorithm/isac.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)      127 2024-01-17 10:12:32.000000 benchmarl-1.2.0/benchmarl/conf/algorithm/maddpg.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)      212 2024-01-17 10:12:32.000000 benchmarl-1.2.0/benchmarl/conf/algorithm/mappo.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)      307 2024-02-23 15:25:15.000000 benchmarl-1.2.0/benchmarl/conf/algorithm/masac.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)       98 2023-10-14 08:15:47.000000 benchmarl-1.2.0/benchmarl/conf/algorithm/qmix.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)       75 2023-10-14 08:15:47.000000 benchmarl-1.2.0/benchmarl/conf/algorithm/vdn.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)      152 2024-04-26 08:20:02.000000 benchmarl-1.2.0/benchmarl/conf/config.yaml
+drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-04-26 10:59:25.143965 benchmarl-1.2.0/benchmarl/conf/experiment/
+-rw-r--r--   0 Matteo     (501) staff       (20)     4263 2024-04-23 09:25:28.000000 benchmarl-1.2.0/benchmarl/conf/experiment/base_experiment.yaml
+drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-04-26 10:59:25.144122 benchmarl-1.2.0/benchmarl/conf/model/
+drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-04-26 10:59:25.144578 benchmarl-1.2.0/benchmarl/conf/model/layers/
+-rw-r--r--   0 Matteo     (501) staff       (20)      359 2024-04-23 09:25:28.000000 benchmarl-1.2.0/benchmarl/conf/model/layers/cnn.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)      116 2023-11-28 10:20:07.000000 benchmarl-1.2.0/benchmarl/conf/model/layers/gnn.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)      156 2023-11-28 10:20:07.000000 benchmarl-1.2.0/benchmarl/conf/model/layers/mlp.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)      433 2023-10-14 08:15:47.000000 benchmarl-1.2.0/benchmarl/conf/model/sequence.yaml
+drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-04-26 10:59:25.144738 benchmarl-1.2.0/benchmarl/conf/task/
+-rw-r--r--   0 Matteo     (501) staff       (20)     6148 2024-04-18 10:23:56.000000 benchmarl-1.2.0/benchmarl/conf/task/.DS_Store
+drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-04-26 10:59:25.156035 benchmarl-1.2.0/benchmarl/conf/task/meltingpot/
+-rw-r--r--   0 Matteo     (501) staff       (20)        0 2024-04-23 09:25:28.000000 benchmarl-1.2.0/benchmarl/conf/task/meltingpot/allelopathic_harvest__open.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)        0 2024-04-23 09:25:28.000000 benchmarl-1.2.0/benchmarl/conf/task/meltingpot/bach_or_stravinsky_in_the_matrix__arena.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)        0 2024-04-23 09:25:28.000000 benchmarl-1.2.0/benchmarl/conf/task/meltingpot/bach_or_stravinsky_in_the_matrix__repeated.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)        0 2024-04-23 09:25:28.000000 benchmarl-1.2.0/benchmarl/conf/task/meltingpot/boat_race__eight_races.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)        0 2024-04-23 09:25:28.000000 benchmarl-1.2.0/benchmarl/conf/task/meltingpot/chemistry__three_metabolic_cycles.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)        0 2024-04-23 09:25:28.000000 benchmarl-1.2.0/benchmarl/conf/task/meltingpot/chemistry__three_metabolic_cycles_with_plentiful_distractors.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)        0 2024-04-23 09:25:28.000000 benchmarl-1.2.0/benchmarl/conf/task/meltingpot/chemistry__two_metabolic_cycles.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)        0 2024-04-23 09:25:28.000000 benchmarl-1.2.0/benchmarl/conf/task/meltingpot/chemistry__two_metabolic_cycles_with_distractors.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)        0 2024-04-23 09:25:28.000000 benchmarl-1.2.0/benchmarl/conf/task/meltingpot/chicken_in_the_matrix__arena.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)        0 2024-04-23 09:25:28.000000 benchmarl-1.2.0/benchmarl/conf/task/meltingpot/chicken_in_the_matrix__repeated.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)        0 2024-04-23 09:25:28.000000 benchmarl-1.2.0/benchmarl/conf/task/meltingpot/clean_up.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)        0 2024-04-23 09:25:28.000000 benchmarl-1.2.0/benchmarl/conf/task/meltingpot/coins.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)        0 2024-04-23 09:25:28.000000 benchmarl-1.2.0/benchmarl/conf/task/meltingpot/collaborative_cooking__asymmetric.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)        0 2024-04-23 09:25:28.000000 benchmarl-1.2.0/benchmarl/conf/task/meltingpot/collaborative_cooking__circuit.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)        0 2024-04-23 09:25:28.000000 benchmarl-1.2.0/benchmarl/conf/task/meltingpot/collaborative_cooking__cramped.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)        0 2024-04-23 09:25:28.000000 benchmarl-1.2.0/benchmarl/conf/task/meltingpot/collaborative_cooking__crowded.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)        0 2024-04-23 09:25:28.000000 benchmarl-1.2.0/benchmarl/conf/task/meltingpot/collaborative_cooking__figure_eight.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)        0 2024-04-23 09:25:28.000000 benchmarl-1.2.0/benchmarl/conf/task/meltingpot/collaborative_cooking__forced.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)        0 2024-04-23 09:25:28.000000 benchmarl-1.2.0/benchmarl/conf/task/meltingpot/collaborative_cooking__ring.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)        0 2024-04-23 09:25:28.000000 benchmarl-1.2.0/benchmarl/conf/task/meltingpot/commons_harvest__closed.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)        0 2024-04-23 09:25:28.000000 benchmarl-1.2.0/benchmarl/conf/task/meltingpot/commons_harvest__open.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)        0 2024-04-23 09:25:28.000000 benchmarl-1.2.0/benchmarl/conf/task/meltingpot/commons_harvest__partnership.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)        0 2024-04-23 09:25:28.000000 benchmarl-1.2.0/benchmarl/conf/task/meltingpot/coop_mining.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)        0 2024-04-23 09:25:28.000000 benchmarl-1.2.0/benchmarl/conf/task/meltingpot/daycare.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)        0 2024-04-23 09:25:28.000000 benchmarl-1.2.0/benchmarl/conf/task/meltingpot/externality_mushrooms__dense.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)        0 2024-04-23 09:25:28.000000 benchmarl-1.2.0/benchmarl/conf/task/meltingpot/factory_commons__either_or.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)        0 2024-04-23 09:25:28.000000 benchmarl-1.2.0/benchmarl/conf/task/meltingpot/fruit_market__concentric_rivers.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)        0 2024-04-23 09:25:28.000000 benchmarl-1.2.0/benchmarl/conf/task/meltingpot/gift_refinements.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)        0 2024-04-23 09:25:28.000000 benchmarl-1.2.0/benchmarl/conf/task/meltingpot/hidden_agenda.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)        0 2024-04-23 09:25:28.000000 benchmarl-1.2.0/benchmarl/conf/task/meltingpot/paintball__capture_the_flag.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)        0 2024-04-23 09:25:28.000000 benchmarl-1.2.0/benchmarl/conf/task/meltingpot/paintball__king_of_the_hill.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)        0 2024-04-23 09:25:28.000000 benchmarl-1.2.0/benchmarl/conf/task/meltingpot/predator_prey__alley_hunt.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)        0 2024-04-23 09:25:28.000000 benchmarl-1.2.0/benchmarl/conf/task/meltingpot/predator_prey__open.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)        0 2024-04-23 09:25:28.000000 benchmarl-1.2.0/benchmarl/conf/task/meltingpot/predator_prey__orchard.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)        0 2024-04-23 09:25:28.000000 benchmarl-1.2.0/benchmarl/conf/task/meltingpot/predator_prey__random_forest.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)        0 2024-04-23 09:25:28.000000 benchmarl-1.2.0/benchmarl/conf/task/meltingpot/prisoners_dilemma_in_the_matrix__arena.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)        0 2024-04-23 09:25:28.000000 benchmarl-1.2.0/benchmarl/conf/task/meltingpot/prisoners_dilemma_in_the_matrix__repeated.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)        0 2024-04-23 09:25:28.000000 benchmarl-1.2.0/benchmarl/conf/task/meltingpot/pure_coordination_in_the_matrix__arena.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)        0 2024-04-23 09:25:28.000000 benchmarl-1.2.0/benchmarl/conf/task/meltingpot/pure_coordination_in_the_matrix__repeated.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)        0 2024-04-23 09:25:28.000000 benchmarl-1.2.0/benchmarl/conf/task/meltingpot/rationalizable_coordination_in_the_matrix__arena.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)        0 2024-04-23 09:25:28.000000 benchmarl-1.2.0/benchmarl/conf/task/meltingpot/rationalizable_coordination_in_the_matrix__repeated.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)        0 2024-04-23 09:25:28.000000 benchmarl-1.2.0/benchmarl/conf/task/meltingpot/running_with_scissors_in_the_matrix__arena.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)        0 2024-04-23 09:25:28.000000 benchmarl-1.2.0/benchmarl/conf/task/meltingpot/running_with_scissors_in_the_matrix__one_shot.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)        0 2024-04-23 09:25:28.000000 benchmarl-1.2.0/benchmarl/conf/task/meltingpot/running_with_scissors_in_the_matrix__repeated.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)        0 2024-04-23 09:25:28.000000 benchmarl-1.2.0/benchmarl/conf/task/meltingpot/stag_hunt_in_the_matrix__arena.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)        0 2024-04-23 09:25:28.000000 benchmarl-1.2.0/benchmarl/conf/task/meltingpot/stag_hunt_in_the_matrix__repeated.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)        0 2024-04-23 09:25:28.000000 benchmarl-1.2.0/benchmarl/conf/task/meltingpot/territory__inside_out.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)        0 2024-04-23 09:25:28.000000 benchmarl-1.2.0/benchmarl/conf/task/meltingpot/territory__open.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)        0 2024-04-23 09:25:28.000000 benchmarl-1.2.0/benchmarl/conf/task/meltingpot/territory__rooms.yaml
+drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-04-26 10:59:25.157739 benchmarl-1.2.0/benchmarl/conf/task/pettingzoo/
+-rw-r--r--   0 Matteo     (501) staff       (20)     1135 2023-10-20 08:48:13.000000 benchmarl-1.2.0/benchmarl/conf/task/pettingzoo/multiwalker.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)      110 2023-10-20 08:48:13.000000 benchmarl-1.2.0/benchmarl/conf/task/pettingzoo/simple_adversary.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)       99 2023-10-20 08:48:13.000000 benchmarl-1.2.0/benchmarl/conf/task/pettingzoo/simple_crypto.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)       95 2023-10-20 08:48:13.000000 benchmarl-1.2.0/benchmarl/conf/task/pettingzoo/simple_push.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)      122 2023-10-20 08:48:13.000000 benchmarl-1.2.0/benchmarl/conf/task/pettingzoo/simple_reference.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)      119 2023-10-20 08:48:13.000000 benchmarl-1.2.0/benchmarl/conf/task/pettingzoo/simple_speaker_listener.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)      121 2023-10-20 08:48:13.000000 benchmarl-1.2.0/benchmarl/conf/task/pettingzoo/simple_spread.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)      141 2023-10-20 08:48:13.000000 benchmarl-1.2.0/benchmarl/conf/task/pettingzoo/simple_tag.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)      182 2023-10-20 08:48:13.000000 benchmarl-1.2.0/benchmarl/conf/task/pettingzoo/simple_world_comm.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)      424 2023-10-20 08:48:13.000000 benchmarl-1.2.0/benchmarl/conf/task/pettingzoo/waterworld.yaml
+drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-04-26 10:59:25.160228 benchmarl-1.2.0/benchmarl/conf/task/smacv2/
+-rw-r--r--   0 Matteo     (501) staff       (20)     1152 2023-10-20 08:48:13.000000 benchmarl-1.2.0/benchmarl/conf/task/smacv2/protoss_10_vs_10.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)     1152 2023-10-20 08:48:13.000000 benchmarl-1.2.0/benchmarl/conf/task/smacv2/protoss_10_vs_11.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)     1152 2023-10-20 08:48:13.000000 benchmarl-1.2.0/benchmarl/conf/task/smacv2/protoss_20_vs_20.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)     1152 2023-10-20 08:48:13.000000 benchmarl-1.2.0/benchmarl/conf/task/smacv2/protoss_20_vs_23.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)     1150 2023-10-14 08:15:47.000000 benchmarl-1.2.0/benchmarl/conf/task/smacv2/protoss_5_vs_5.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)     1195 2023-10-20 08:48:13.000000 benchmarl-1.2.0/benchmarl/conf/task/smacv2/terran_10_vs_10.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)     1195 2023-10-20 08:48:13.000000 benchmarl-1.2.0/benchmarl/conf/task/smacv2/terran_10_vs_11.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)     1195 2023-10-20 08:48:13.000000 benchmarl-1.2.0/benchmarl/conf/task/smacv2/terran_20_vs_20.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)     1195 2023-10-20 08:48:13.000000 benchmarl-1.2.0/benchmarl/conf/task/smacv2/terran_20_vs_23.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)     1193 2023-10-20 08:48:13.000000 benchmarl-1.2.0/benchmarl/conf/task/smacv2/terran_5_vs_5.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)     1198 2023-10-20 08:48:13.000000 benchmarl-1.2.0/benchmarl/conf/task/smacv2/zerg_10_vs_10.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)     1198 2023-10-20 08:48:13.000000 benchmarl-1.2.0/benchmarl/conf/task/smacv2/zerg_10_vs_11.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)     1198 2023-10-20 08:48:13.000000 benchmarl-1.2.0/benchmarl/conf/task/smacv2/zerg_20_vs_20.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)     1198 2023-10-20 08:48:13.000000 benchmarl-1.2.0/benchmarl/conf/task/smacv2/zerg_20_vs_23.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)     1196 2023-10-20 08:48:13.000000 benchmarl-1.2.0/benchmarl/conf/task/smacv2/zerg_5_vs_5.yaml
+drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-04-26 10:59:25.162983 benchmarl-1.2.0/benchmarl/conf/task/vmas/
+-rw-r--r--   0 Matteo     (501) staff       (20)      123 2023-10-20 08:48:13.000000 benchmarl-1.2.0/benchmarl/conf/task/vmas/balance.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)      145 2024-02-01 15:20:17.000000 benchmarl-1.2.0/benchmarl/conf/task/vmas/dispersion.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)      117 2024-02-01 15:20:17.000000 benchmarl-1.2.0/benchmarl/conf/task/vmas/dropout.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)      152 2024-02-01 15:20:17.000000 benchmarl-1.2.0/benchmarl/conf/task/vmas/give_way.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)      217 2024-04-26 10:59:00.000000 benchmarl-1.2.0/benchmarl/conf/task/vmas/navigation.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)      139 2024-02-01 15:20:17.000000 benchmarl-1.2.0/benchmarl/conf/task/vmas/reverse_transport.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)      174 2024-02-01 15:20:17.000000 benchmarl-1.2.0/benchmarl/conf/task/vmas/sampling.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)       99 2023-12-26 13:20:37.000000 benchmarl-1.2.0/benchmarl/conf/task/vmas/simple_adversary.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)       76 2023-12-26 13:20:37.000000 benchmarl-1.2.0/benchmarl/conf/task/vmas/simple_crypto.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)       65 2023-12-26 13:20:37.000000 benchmarl-1.2.0/benchmarl/conf/task/vmas/simple_push.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)       70 2023-12-26 13:20:32.000000 benchmarl-1.2.0/benchmarl/conf/task/vmas/simple_reference.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)       77 2023-12-26 13:20:37.000000 benchmarl-1.2.0/benchmarl/conf/task/vmas/simple_speaker_listener.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)       96 2023-12-26 13:20:37.000000 benchmarl-1.2.0/benchmarl/conf/task/vmas/simple_spread.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)      316 2023-12-26 13:20:32.000000 benchmarl-1.2.0/benchmarl/conf/task/vmas/simple_tag.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)      153 2023-12-26 13:20:37.000000 benchmarl-1.2.0/benchmarl/conf/task/vmas/simple_world_comm.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)      148 2023-10-20 08:48:13.000000 benchmarl-1.2.0/benchmarl/conf/task/vmas/transport.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)      123 2023-10-20 08:48:13.000000 benchmarl-1.2.0/benchmarl/conf/task/vmas/wheel.yaml
+-rw-r--r--   0 Matteo     (501) staff       (20)      330 2024-02-01 15:20:17.000000 benchmarl-1.2.0/benchmarl/conf/task/vmas/wind_flocking.yaml
+drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-04-26 10:59:24.979868 benchmarl-1.2.0/benchmarl/environments/
+-rw-r--r--   0 Matteo     (501) staff       (20)     4499 2024-04-26 10:59:00.000000 benchmarl-1.2.0/benchmarl/environments/__init__.py
+-rw-r--r--   0 Matteo     (501) staff       (20)     9447 2024-04-26 10:59:00.000000 benchmarl-1.2.0/benchmarl/environments/common.py
+drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-04-26 10:59:25.005770 benchmarl-1.2.0/benchmarl/environments/meltingpot/
+-rw-r--r--   0 Matteo     (501) staff       (20)        0 2024-04-23 09:25:28.000000 benchmarl-1.2.0/benchmarl/environments/meltingpot/__init__.py
+-rw-r--r--   0 Matteo     (501) staff       (20)     6024 2024-04-25 10:07:27.000000 benchmarl-1.2.0/benchmarl/environments/meltingpot/common.py
+drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-04-26 10:59:25.033204 benchmarl-1.2.0/benchmarl/environments/pettingzoo/
+-rw-r--r--   0 Matteo     (501) staff       (20)      180 2023-10-20 08:48:13.000000 benchmarl-1.2.0/benchmarl/environments/pettingzoo/__init__.py
+-rw-r--r--   0 Matteo     (501) staff       (20)     5177 2024-04-23 09:25:28.000000 benchmarl-1.2.0/benchmarl/environments/pettingzoo/common.py
+-rw-r--r--   0 Matteo     (501) staff       (20)      655 2024-01-19 11:33:16.000000 benchmarl-1.2.0/benchmarl/environments/pettingzoo/multiwalker.py
+-rw-r--r--   0 Matteo     (501) staff       (20)      330 2023-12-26 12:20:31.000000 benchmarl-1.2.0/benchmarl/environments/pettingzoo/simple_adverasary.py
+-rw-r--r--   0 Matteo     (501) staff       (20)      309 2023-10-20 08:48:13.000000 benchmarl-1.2.0/benchmarl/environments/pettingzoo/simple_crypto.py
+-rw-r--r--   0 Matteo     (501) staff       (20)      309 2023-11-28 10:20:07.000000 benchmarl-1.2.0/benchmarl/environments/pettingzoo/simple_push.py
+-rw-r--r--   0 Matteo     (501) staff       (20)      309 2023-10-20 08:48:13.000000 benchmarl-1.2.0/benchmarl/environments/pettingzoo/simple_reference.py
+-rw-r--r--   0 Matteo     (501) staff       (20)      309 2023-10-20 08:48:13.000000 benchmarl-1.2.0/benchmarl/environments/pettingzoo/simple_speaker_listener.py
+-rw-r--r--   0 Matteo     (501) staff       (20)      363 2023-10-20 08:48:13.000000 benchmarl-1.2.0/benchmarl/environments/pettingzoo/simple_spread.py
+-rw-r--r--   0 Matteo     (501) staff       (20)      405 2023-10-20 08:48:13.000000 benchmarl-1.2.0/benchmarl/environments/pettingzoo/simple_tag.py
+-rw-r--r--   0 Matteo     (501) staff       (20)      464 2023-10-20 08:48:13.000000 benchmarl-1.2.0/benchmarl/environments/pettingzoo/simple_world_comm.py
+-rw-r--r--   0 Matteo     (501) staff       (20)      934 2023-11-28 10:20:07.000000 benchmarl-1.2.0/benchmarl/environments/pettingzoo/waterworld.py
+drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-04-26 10:59:25.056800 benchmarl-1.2.0/benchmarl/environments/smacv2/
+-rw-r--r--   0 Matteo     (501) staff       (20)      180 2023-10-20 08:48:13.000000 benchmarl-1.2.0/benchmarl/environments/smacv2/__init__.py
+-rw-r--r--   0 Matteo     (501) staff       (20)     3364 2024-04-23 09:25:28.000000 benchmarl-1.2.0/benchmarl/environments/smacv2/common.py
+drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-04-26 10:59:25.091753 benchmarl-1.2.0/benchmarl/environments/vmas/
+-rw-r--r--   0 Matteo     (501) staff       (20)      180 2023-11-23 12:19:19.000000 benchmarl-1.2.0/benchmarl/environments/vmas/__init__.py
+-rw-r--r--   0 Matteo     (501) staff       (20)      393 2023-10-20 08:48:13.000000 benchmarl-1.2.0/benchmarl/environments/vmas/balance.py
+-rw-r--r--   0 Matteo     (501) staff       (20)     2947 2024-04-26 10:59:00.000000 benchmarl-1.2.0/benchmarl/environments/vmas/common.py
+-rw-r--r--   0 Matteo     (501) staff       (20)      438 2024-02-01 15:20:17.000000 benchmarl-1.2.0/benchmarl/environments/vmas/dispersion.py
+-rw-r--r--   0 Matteo     (501) staff       (20)      383 2024-02-01 15:20:17.000000 benchmarl-1.2.0/benchmarl/environments/vmas/dropout.py
+-rw-r--r--   0 Matteo     (501) staff       (20)      428 2024-02-01 15:20:17.000000 benchmarl-1.2.0/benchmarl/environments/vmas/give_way.py
+-rw-r--r--   0 Matteo     (501) staff       (20)      552 2024-04-26 10:59:00.000000 benchmarl-1.2.0/benchmarl/environments/vmas/navigation.py
+-rw-r--r--   0 Matteo     (501) staff       (20)      417 2024-02-01 15:20:17.000000 benchmarl-1.2.0/benchmarl/environments/vmas/reverse_transport.py
+-rw-r--r--   0 Matteo     (501) staff       (20)      498 2024-02-01 15:20:17.000000 benchmarl-1.2.0/benchmarl/environments/vmas/sampling.py
+-rw-r--r--   0 Matteo     (501) staff       (20)      345 2023-12-26 13:20:37.000000 benchmarl-1.2.0/benchmarl/environments/vmas/simple_adverasary.py
+-rw-r--r--   0 Matteo     (501) staff       (20)      309 2023-12-26 13:20:37.000000 benchmarl-1.2.0/benchmarl/environments/vmas/simple_crypto.py
+-rw-r--r--   0 Matteo     (501) staff       (20)      284 2023-12-26 13:20:37.000000 benchmarl-1.2.0/benchmarl/environments/vmas/simple_push.py
+-rw-r--r--   0 Matteo     (501) staff       (20)      284 2023-12-26 13:20:32.000000 benchmarl-1.2.0/benchmarl/environments/vmas/simple_reference.py
+-rw-r--r--   0 Matteo     (501) staff       (20)      284 2023-12-26 13:20:37.000000 benchmarl-1.2.0/benchmarl/environments/vmas/simple_speaker_listener.py
+-rw-r--r--   0 Matteo     (501) staff       (20)      343 2023-12-26 13:20:37.000000 benchmarl-1.2.0/benchmarl/environments/vmas/simple_spread.py
+-rw-r--r--   0 Matteo     (501) staff       (20)      708 2023-12-26 13:20:32.000000 benchmarl-1.2.0/benchmarl/environments/vmas/simple_tag.py
+-rw-r--r--   0 Matteo     (501) staff       (20)      446 2023-12-26 13:20:37.000000 benchmarl-1.2.0/benchmarl/environments/vmas/simple_world_comm.py
+-rw-r--r--   0 Matteo     (501) staff       (20)      447 2023-10-20 08:48:13.000000 benchmarl-1.2.0/benchmarl/environments/vmas/transport.py
+-rw-r--r--   0 Matteo     (501) staff       (20)      414 2023-10-20 08:48:13.000000 benchmarl-1.2.0/benchmarl/environments/vmas/wheel.py
+-rw-r--r--   0 Matteo     (501) staff       (20)      762 2024-02-01 15:20:17.000000 benchmarl-1.2.0/benchmarl/environments/vmas/wind_flocking.py
+-rw-r--r--   0 Matteo     (501) staff       (20)     7619 2023-11-28 10:20:07.000000 benchmarl-1.2.0/benchmarl/eval_results.py
+drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-04-26 10:59:25.118686 benchmarl-1.2.0/benchmarl/experiment/
+-rw-r--r--   0 Matteo     (501) staff       (20)      265 2023-11-28 10:20:07.000000 benchmarl-1.2.0/benchmarl/experiment/__init__.py
+-rw-r--r--   0 Matteo     (501) staff       (20)     3045 2024-01-17 09:07:49.000000 benchmarl-1.2.0/benchmarl/experiment/callback.py
+-rw-r--r--   0 Matteo     (501) staff       (20)    29228 2024-04-26 10:59:00.000000 benchmarl-1.2.0/benchmarl/experiment/experiment.py
+-rw-r--r--   0 Matteo     (501) staff       (20)    13188 2024-04-26 10:59:00.000000 benchmarl-1.2.0/benchmarl/experiment/logger.py
+-rw-r--r--   0 Matteo     (501) staff       (20)     3613 2023-11-28 10:20:07.000000 benchmarl-1.2.0/benchmarl/hydra_config.py
+drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-04-26 10:59:25.141544 benchmarl-1.2.0/benchmarl/models/
+-rw-r--r--   0 Matteo     (501) staff       (20)      504 2024-04-26 10:59:00.000000 benchmarl-1.2.0/benchmarl/models/__init__.py
+-rw-r--r--   0 Matteo     (501) staff       (20)    13947 2024-04-24 09:11:37.000000 benchmarl-1.2.0/benchmarl/models/cnn.py
+-rw-r--r--   0 Matteo     (501) staff       (20)    16158 2024-04-23 09:25:28.000000 benchmarl-1.2.0/benchmarl/models/common.py
+-rw-r--r--   0 Matteo     (501) staff       (20)    10128 2024-04-23 09:25:28.000000 benchmarl-1.2.0/benchmarl/models/gnn.py
+-rw-r--r--   0 Matteo     (501) staff       (20)     5723 2024-04-23 09:25:28.000000 benchmarl-1.2.0/benchmarl/models/mlp.py
+-rw-r--r--   0 Matteo     (501) staff       (20)     1182 2023-11-28 10:20:07.000000 benchmarl-1.2.0/benchmarl/run.py
+-rw-r--r--   0 Matteo     (501) staff       (20)     1459 2024-04-23 09:25:28.000000 benchmarl-1.2.0/benchmarl/utils.py
+drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-04-26 10:59:25.164597 benchmarl-1.2.0/benchmarl.egg-info/
+-rw-r--r--   0 Matteo     (501) staff       (20)      739 2024-04-26 10:59:24.000000 benchmarl-1.2.0/benchmarl.egg-info/PKG-INFO
+-rw-r--r--   0 Matteo     (501) staff       (20)    82358 2024-04-26 10:59:24.000000 benchmarl-1.2.0/benchmarl.egg-info/SOURCES.txt
+-rw-r--r--   0 Matteo     (501) staff       (20)        1 2024-04-26 10:59:24.000000 benchmarl-1.2.0/benchmarl.egg-info/dependency_links.txt
+-rw-r--r--   0 Matteo     (501) staff       (20)      177 2024-04-26 10:59:24.000000 benchmarl-1.2.0/benchmarl.egg-info/requires.txt
+-rw-r--r--   0 Matteo     (501) staff       (20)       10 2024-04-26 10:59:24.000000 benchmarl-1.2.0/benchmarl.egg-info/top_level.txt
+-rw-r--r--   0 Matteo     (501) staff       (20)       82 2024-04-25 10:18:10.000000 benchmarl-1.2.0/pyproject.toml
+-rw-r--r--   0 Matteo     (501) staff       (20)      432 2024-04-26 10:59:25.165689 benchmarl-1.2.0/setup.cfg
+-rw-r--r--   0 Matteo     (501) staff       (20)     1647 2024-04-26 10:59:00.000000 benchmarl-1.2.0/setup.py
+drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-04-26 10:59:25.164299 benchmarl-1.2.0/test/
+-rw-r--r--   0 Matteo     (501) staff       (20)      959 2023-10-20 08:48:13.000000 benchmarl-1.2.0/test/test_algorithm.py
+-rw-r--r--   0 Matteo     (501) staff       (20)     3866 2024-04-26 10:59:00.000000 benchmarl-1.2.0/test/test_meltingpot.py
+-rw-r--r--   0 Matteo     (501) staff       (20)     5893 2024-04-26 10:59:00.000000 benchmarl-1.2.0/test/test_models.py
+-rw-r--r--   0 Matteo     (501) staff       (20)     4838 2024-04-23 09:25:28.000000 benchmarl-1.2.0/test/test_pettingzoo.py
+-rw-r--r--   0 Matteo     (501) staff       (20)     2462 2023-12-26 12:06:29.000000 benchmarl-1.2.0/test/test_smacv2.py
+-rw-r--r--   0 Matteo     (501) staff       (20)      966 2023-10-20 08:48:13.000000 benchmarl-1.2.0/test/test_task.py
+-rw-r--r--   0 Matteo     (501) staff       (20)     4494 2024-04-23 09:25:28.000000 benchmarl-1.2.0/test/test_vmas.py
```

### Comparing `benchmarl-1.1.1/LICENSE` & `benchmarl-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `benchmarl-1.1.1/README.md` & `benchmarl-1.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ![BenchMARL](https://raw.githubusercontent.com/matteobettini/benchmarl_sphinx_theme/master/benchmarl_sphinx_theme/static/img/benchmarl.png?raw=true)
 
 
 # BenchMARL
 [![tests](https://github.com/facebookresearch/BenchMARL/actions/workflows/unit_tests.yml/badge.svg)](test)
 [![codecov](https://codecov.io/github/facebookresearch/BenchMARL/coverage.svg?branch=main)](https://codecov.io/gh/facebookresearch/BenchMARL)
 [![Documentation Status](https://readthedocs.org/projects/benchmarl/badge/?version=latest)](https://benchmarl.readthedocs.io/en/latest/?badge=latest)
-[![Python](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue.svg)](https://www.python.org/downloads/)
+[![Python](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue.svg)](https://www.python.org/downloads/)
 <a href="https://pypi.org/project/benchmarl"><img src="https://img.shields.io/pypi/v/benchmarl" alt="pypi version"></a>
 [![Downloads](https://static.pepy.tech/personalized-badge/benchmarl?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads)](https://pepy.tech/project/benchmarl)
 [![Discord Shield](https://dcbadge.vercel.app/api/server/jEEWCn6T3p?style=flat)](https://discord.gg/jEEWCn6T3p)
 [![arXiv](https://img.shields.io/badge/arXiv-2312.01472-b31b1b.svg)](https://arxiv.org/abs/2312.01472)
 
 ```bash
 python benchmarl/run.py algorithm=mappo task=vmas/balance
@@ -109,14 +109,18 @@
 ```
 
 ##### PettingZoo
 ```bash
 pip install "pettingzoo[all]"
 ```
 
+##### MeltingPot
+```bash
+pip install dm-meltingpot
+```
 ##### SMACv2
 
 Follow the instructions on the environment [repository](https://github.com/oxwhirl/smacv2).
 
 [Here](.github/unittest/install_smacv2.sh) is how we install it on linux.
 
 ### Run
@@ -232,20 +236,22 @@
 | [IQL](https://www.semanticscholar.org/paper/Multi-Agent-Reinforcement-Learning%3A-Independent-Tan/59de874c1e547399b695337bcff23070664fa66e) | Off           | No           | NA                           | Discrete              | No                  |  
 
 
 **Tasks**. Tasks are scenarios from a specific environment which constitute the MARL
 challenge to solve.
 They differ based on many aspects, here is a table with the current environments in BenchMARL
 
-| Environment                                                        | Tasks                               | Cooperation               | Global state | Reward function               | Action space          |    Vectorized    |
-|--------------------------------------------------------------------|-------------------------------------|---------------------------|--------------|-------------------------------|-----------------------|:----------------:|
-| [VMAS](https://github.com/proroklab/VectorizedMultiAgentSimulator) | [18](benchmarl/conf/task/vmas)      | Cooperative + Competitive | No           | Shared + Independent + Global | Continuous + Discrete |       Yes        |    
-| [SMACv2](https://github.com/oxwhirl/smacv2)                        | [15](benchmarl/conf/task/smacv2)    | Cooperative               | Yes          | Global                        | Discrete              |        No        |
-| [MPE](https://github.com/openai/multiagent-particle-envs)          | [8](benchmarl/conf/task/pettingzoo) | Cooperative + Competitive | Yes          | Shared + Independent          | Continuous + Discrete |        No        |
-| [SISL](https://github.com/sisl/MADRL)                              | [2](benchmarl/conf/task/pettingzoo) | Cooperative               | No           | Shared                        | Continuous            |        No        |
+| Environment                                                        | Tasks                                | Cooperation               | Global state | Reward function               | Action space          |    Vectorized    |
+|--------------------------------------------------------------------|--------------------------------------|---------------------------|--------------|-------------------------------|-----------------------|:----------------:|
+| [VMAS](https://github.com/proroklab/VectorizedMultiAgentSimulator) | [18](benchmarl/conf/task/vmas)       | Cooperative + Competitive | No           | Shared + Independent + Global | Continuous + Discrete |       Yes        |    
+| [SMACv2](https://github.com/oxwhirl/smacv2)                        | [15](benchmarl/conf/task/smacv2)     | Cooperative               | Yes          | Global                        | Discrete              |        No        |
+| [MPE](https://github.com/openai/multiagent-particle-envs)          | [8](benchmarl/conf/task/pettingzoo)  | Cooperative + Competitive | Yes          | Shared + Independent          | Continuous + Discrete |        No        |
+| [SISL](https://github.com/sisl/MADRL)                              | [2](benchmarl/conf/task/pettingzoo)  | Cooperative               | No           | Shared                        | Continuous            |        No        |
+| [MeltingPot](https://github.com/google-deepmind/meltingpot)        | [49](benchmarl/conf/task/meltingpot) | Cooperative + Competitive | Yes          | Independent                   | Discrete              |        No        |
+
 
 > [!NOTE]  
 > BenchMARL uses the [TorchRL MARL API](https://github.com/pytorch/rl/issues/1463) for grouping agents.
 > In competitive environments like MPE, for example, teams will be in different groups. Each group has its own loss,
 > models, buffers, and so on. Parameter sharing options refer to sharing within the group. See the example on [creating
 > a custom algorithm](examples/extending/algorithm/custom_algorithm.py) for more info.
 
@@ -254,20 +260,20 @@
 different layers. All the models can be used with or without parameter sharing within an 
 agent group. Here is a table of the models implemented in BenchMARL
 
 | Name                           | Decentralized | Centralized with local inputs | Centralized with global input | 
 |--------------------------------|:-------------:|:-----------------------------:|:-----------------------------:|
 | [MLP](benchmarl/models/mlp.py) |      Yes      |              Yes              |              Yes              |
 | [GNN](benchmarl/models/gnn.py) |      Yes      |              No               |              No               |
+| [CNN](benchmarl/models/cnn.py) |      Yes      |              Yes              |              Yes              |
 
 And the ones that are _work in progress_
 
 | Name               | Decentralized | Centralized with local inputs | Centralized with global input | 
 |--------------------|:-------------:|:-----------------------------:|:-----------------------------:|
-| CNN                |      Yes      |              Yes              |              Yes              | 
 | RNN (GRU and LSTM) |      Yes      |              Yes              |              Yes              | 
 
 
 ## Fine-tuned public benchmarks
 > [!WARNING]  
 > This section is under a work in progress. We are constantly working on fine-tuning
 > our experiments to enable our users to have access to state-of-the-art benchmarks.
```

#### html2text {}

```diff
@@ -2,17 +2,18 @@
 benchmarl_sphinx_theme/master/benchmarl_sphinx_theme/static/img/
 benchmarl.png?raw=true) # BenchMARL [![tests](https://github.com/
 facebookresearch/BenchMARL/actions/workflows/unit_tests.yml/badge.svg)](test)
 [![codecov](https://codecov.io/github/facebookresearch/BenchMARL/
 coverage.svg?branch=main)](https://codecov.io/gh/facebookresearch/BenchMARL) [!
 [Documentation Status](https://readthedocs.org/projects/benchmarl/badge/
 ?version=latest)](https://benchmarl.readthedocs.io/en/latest/?badge=latest) [!
-[Python](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-
-blue.svg)](https://www.python.org/downloads/) _[_p_y_p_i_ _v_e_r_s_i_o_n_][![Downloads]
-(https://static.pepy.tech/personalized-badge/
+[Python](https://img.shields.io/badge/python-
+3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue.svg)](https://www.python.org/
+downloads/) _[_p_y_p_i_ _v_e_r_s_i_o_n_][![Downloads](https://static.pepy.tech/personalized-
+badge/
 benchmarl?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads)]
 (https://pepy.tech/project/benchmarl) [![Discord Shield](https://
 dcbadge.vercel.app/api/server/jEEWCn6T3p?style=flat)](https://discord.gg/
 jEEWCn6T3p) [![arXiv](https://img.shields.io/badge/arXiv-2312.01472-
 b31b1b.svg)](https://arxiv.org/abs/2312.01472) ```bash python benchmarl/run.py
 algorithm=mappo task=vmas/balance ``` [![Examples](https://img.shields.io/
 badge/Examples-blue.svg)](examples) [![Open In Colab](https://
@@ -58,25 +59,26 @@
 ``` For more details, or for installing nightly versions, see the [TorchRL
 installation guide](https://github.com/pytorch/rl#installation). #### Install
 BenchMARL You can just install it from github ```bash pip install benchmarl ```
 Or also clone it locally to access the configs and scripts ```bash git clone
 https://github.com/facebookresearch/BenchMARL.git pip install -e BenchMARL ```
 #### Install environments All enviornment dependencies are optional in
 BenchMARL and can be installed separately. ##### VMAS ```bash pip install vmas
-``` ##### PettingZoo ```bash pip install "pettingzoo[all]" ``` ##### SMACv2
-Follow the instructions on the environment [repository](https://github.com/
-oxwhirl/smacv2). [Here](.github/unittest/install_smacv2.sh) is how we install
-it on linux. ### Run Experiments are launched with a [default configuration]
-(benchmarl/conf) that can be overridden in many ways. To learn how to customize
-and override configurations please refer to the [configuring section]
-(#configuring). #### Command line To launch an experiment from the command line
-you can do ```bash python benchmarl/run.py algorithm=mappo task=vmas/balance
-``` [![Example](https://img.shields.io/badge/Example-blue.svg)](examples/
-running/run_experiment.sh) Thanks to [hydra](https://hydra.cc/docs/intro/), you
-can run benchmarks as multi-runs like: ```bash python benchmarl/run.py -
+``` ##### PettingZoo ```bash pip install "pettingzoo[all]" ``` ##### MeltingPot
+```bash pip install dm-meltingpot ``` ##### SMACv2 Follow the instructions on
+the environment [repository](https://github.com/oxwhirl/smacv2). [Here]
+(.github/unittest/install_smacv2.sh) is how we install it on linux. ### Run
+Experiments are launched with a [default configuration](benchmarl/conf) that
+can be overridden in many ways. To learn how to customize and override
+configurations please refer to the [configuring section](#configuring). ####
+Command line To launch an experiment from the command line you can do ```bash
+python benchmarl/run.py algorithm=mappo task=vmas/balance ``` [![Example]
+(https://img.shields.io/badge/Example-blue.svg)](examples/running/
+run_experiment.sh) Thanks to [hydra](https://hydra.cc/docs/intro/), you can run
+benchmarks as multi-runs like: ```bash python benchmarl/run.py -
 m algorithm=mappo,qmix,masac task=vmas/balance,vmas/sampling seed=0,1 ``` [!
 [Example](https://img.shields.io/badge/Example-blue.svg)](examples/running/
 run_benchmark.sh) The default implementation for hydra multi-runs is
 sequential, but [parallel](https://hydra.cc/docs/plugins/joblib_launcher/) and
 [slurm](https://hydra.cc/docs/plugins/submitit_launcher/) launchers are also
 available. #### Script You can also load and launch your experiments from
 within a script ```python experiment = Experiment
@@ -139,56 +141,59 @@
 Reinforcement-Learning%3A-Independent-Tan/
 59de874c1e547399b695337bcff23070664fa66e) | Off | No | NA | Discrete | No |
 **Tasks**. Tasks are scenarios from a specific environment which constitute the
 MARL challenge to solve. They differ based on many aspects, here is a table
 with the current environments in BenchMARL | Environment | Tasks | Cooperation
 | Global state | Reward function | Action space | Vectorized | |---------------
 -----------------------------------------------------|-------------------------
-------------|---------------------------|--------------|-----------------------
---------|-----------------------|:----------------:| | [VMAS](https://
+-------------|---------------------------|--------------|----------------------
+---------|-----------------------|:----------------:| | [VMAS](https://
 github.com/proroklab/VectorizedMultiAgentSimulator) | [18](benchmarl/conf/task/
 vmas) | Cooperative + Competitive | No | Shared + Independent + Global |
 Continuous + Discrete | Yes | | [SMACv2](https://github.com/oxwhirl/smacv2) |
 [15](benchmarl/conf/task/smacv2) | Cooperative | Yes | Global | Discrete | No |
 | [MPE](https://github.com/openai/multiagent-particle-envs) | [8](benchmarl/
 conf/task/pettingzoo) | Cooperative + Competitive | Yes | Shared + Independent
 | Continuous + Discrete | No | | [SISL](https://github.com/sisl/MADRL) | [2]
 (benchmarl/conf/task/pettingzoo) | Cooperative | No | Shared | Continuous | No
-| > [!NOTE] > BenchMARL uses the [TorchRL MARL API](https://github.com/pytorch/
-rl/issues/1463) for grouping agents. > In competitive environments like MPE,
-for example, teams will be in different groups. Each group has its own loss, >
-models, buffers, and so on. Parameter sharing options refer to sharing within
-the group. See the example on [creating > a custom algorithm](examples/
-extending/algorithm/custom_algorithm.py) for more info. **Models**. Models are
-neural networks used to process data. They can be used as actors (policies) or,
-when requested, as critics. We provide a set of base models (layers) and a
-SequenceModel to concatenate different layers. All the models can be used with
-or without parameter sharing within an agent group. Here is a table of the
-models implemented in BenchMARL | Name | Decentralized | Centralized with local
-inputs | Centralized with global input | |--------------------------------|:---
-----------:|:-----------------------------:|:-----------------------------:| |
-[MLP](benchmarl/models/mlp.py) | Yes | Yes | Yes | | [GNN](benchmarl/models/
-gnn.py) | Yes | No | No | And the ones that are _work in progress_ | Name |
+| | [MeltingPot](https://github.com/google-deepmind/meltingpot) | [49]
+(benchmarl/conf/task/meltingpot) | Cooperative + Competitive | Yes |
+Independent | Discrete | No | > [!NOTE] > BenchMARL uses the [TorchRL MARL API]
+(https://github.com/pytorch/rl/issues/1463) for grouping agents. > In
+competitive environments like MPE, for example, teams will be in different
+groups. Each group has its own loss, > models, buffers, and so on. Parameter
+sharing options refer to sharing within the group. See the example on [creating
+> a custom algorithm](examples/extending/algorithm/custom_algorithm.py) for
+more info. **Models**. Models are neural networks used to process data. They
+can be used as actors (policies) or, when requested, as critics. We provide a
+set of base models (layers) and a SequenceModel to concatenate different
+layers. All the models can be used with or without parameter sharing within an
+agent group. Here is a table of the models implemented in BenchMARL | Name |
 Decentralized | Centralized with local inputs | Centralized with global input |
-|--------------------|:-------------:|:-----------------------------:|:--------
----------------------:| | CNN | Yes | Yes | Yes | | RNN (GRU and LSTM) | Yes |
-Yes | Yes | ## Fine-tuned public benchmarks > [!WARNING] > This section is
-under a work in progress. We are constantly working on fine-tuning > our
-experiments to enable our users to have access to state-of-the-art benchmarks.
-> If you would like to collaborate in this effort, please reach out to us. In
-the [fine_tuned](fine_tuned) folder we are collecting some tested
-hyperparameters for specific environments to enable users to bootstrap their
-benchmarking. You can just run the scripts in this folder to automatically use
-the proposed hyperparameters. We will tune benchmarks for you and publish the
-config and benchmarking plots on [Wandb](https://wandb.ai/matteobettini/
-benchmarl-public/reportlist) publicly Currently available ones are: - **VMAS**:
-[![Conf](https://img.shields.io/badge/Conf-purple.svg)](fine_tuned/vmas/conf/
-config.yaml) [![Static Badge](https://img.shields.io/badge/Benchmarks-Wandb-
-yellow)](https://api.wandb.ai/links/matteobettini/r5744vas) In the following,
-we report a table of the results: | **
+|--------------------------------|:-------------:|:----------------------------
+-:|:-----------------------------:| | [MLP](benchmarl/models/mlp.py) | Yes |
+Yes | Yes | | [GNN](benchmarl/models/gnn.py) | Yes | No | No | | [CNN]
+(benchmarl/models/cnn.py) | Yes | Yes | Yes | And the ones that are _work in
+progress_ | Name | Decentralized | Centralized with local inputs | Centralized
+with global input | |--------------------|:-------------:|:--------------------
+---------:|:-----------------------------:| | RNN (GRU and LSTM) | Yes | Yes |
+Yes | ## Fine-tuned public benchmarks > [!WARNING] > This section is under a
+work in progress. We are constantly working on fine-tuning > our experiments to
+enable our users to have access to state-of-the-art benchmarks. > If you would
+like to collaborate in this effort, please reach out to us. In the [fine_tuned]
+(fine_tuned) folder we are collecting some tested hyperparameters for specific
+environments to enable users to bootstrap their benchmarking. You can just run
+the scripts in this folder to automatically use the proposed hyperparameters.
+We will tune benchmarks for you and publish the config and benchmarking plots
+on [Wandb](https://wandb.ai/matteobettini/benchmarl-public/reportlist) publicly
+Currently available ones are: - **VMAS**: [![Conf](https://img.shields.io/
+badge/Conf-purple.svg)](fine_tuned/vmas/conf/config.yaml) [![Static Badge]
+(https://img.shields.io/badge/Benchmarks-Wandb-yellow)](https://api.wandb.ai/
+links/matteobettini/r5744vas) In the following, we report a table of the
+results: | **
                                   Environment
 ** | **
                      Sample efficiency curves (all tasks)
 ** | **
                               Performance profile
 ** | **
                                Aggregate scores
```

### Comparing `benchmarl-1.1.1/benchmarl/__init__.py` & `benchmarl-1.2.0/benchmarl/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #  Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 #  This source code is licensed under the license found in the
 #  LICENSE file in the root directory of this source tree.
 #
 
 
-__version__ = "1.1.1"
+__version__ = "1.2.0"
 
 import importlib
 
 import benchmarl.algorithms
 import benchmarl.benchmark
 import benchmarl.environments
 import benchmarl.experiment
```

### Comparing `benchmarl-1.1.1/benchmarl/algorithms/__init__.py` & `benchmarl-1.2.0/benchmarl/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `benchmarl-1.1.1/benchmarl/algorithms/common.py` & `benchmarl-1.2.0/benchmarl/algorithms/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,26 +3,27 @@
 #  This source code is licensed under the license found in the
 #  LICENSE file in the root directory of this source tree.
 #
 
 import pathlib
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
-from typing import Any, Dict, Iterable, Optional, Tuple, Type
+from typing import Any, Dict, Iterable, List, Optional, Tuple, Type
 
 from tensordict import TensorDictBase
 from tensordict.nn import TensorDictModule, TensorDictSequential
 from torchrl.data import (
     DiscreteTensorSpec,
     LazyTensorStorage,
     OneHotDiscreteTensorSpec,
     ReplayBuffer,
     TensorDictReplayBuffer,
 )
 from torchrl.data.replay_buffers import RandomSampler, SamplerWithoutReplacement
+from torchrl.envs import Compose, Transform
 from torchrl.objectives import LossModule
 from torchrl.objectives.utils import HardUpdate, SoftUpdate, TargetNetUpdater
 
 from benchmarl.models.common import ModelConfig
 from benchmarl.utils import _read_yaml_config, DEVICE_TYPING
 
 
@@ -55,30 +56,24 @@
         self._policies_for_loss = {}
         self._policies_for_collection = {}
 
         self._check_specs()
 
     def _check_specs(self):
         if self.state_spec is not None:
-            if (
-                len(self.state_spec.keys(True, True)) != 1
-                or list(self.state_spec.keys())[0] != "state"
-            ):
+            if len(self.state_spec.keys(True, True)) != 1:
                 raise ValueError(
-                    "State spec must contain one entry per group named 'state'"
+                    "State spec must contain one entry per group"
                     " to follow the library conventions, "
                     "you can apply a transform to your environment to satisfy this criteria."
                 )
         for group in self.group_map.keys():
-            if (
-                len(self.observation_spec[group].keys(True, True)) != 1
-                or list(self.observation_spec[group].keys())[0] != "observation"
-            ):
+            if len(self.observation_spec[group].keys(True, True)) != 1:
                 raise ValueError(
-                    "Observation spec must contain one entry per group named 'observation'"
+                    "Observation spec must contain one entry per group"
                     " to follow the library conventions, "
                     "you can apply a transform to your environment to satisfy this criteria."
                 )
             if (
                 len(self.action_spec[group].keys(True, True)) != 1
                 or list(self.action_spec[group].keys())[0] != "action"
             ):
@@ -134,36 +129,37 @@
                     )
             else:
                 target_net_updater = None
             self._losses_and_updaters.update({group: (loss, target_net_updater)})
         return self._losses_and_updaters[group]
 
     def get_replay_buffer(
-        self,
-        group: str,
+        self, group: str, transforms: List[Transform] = None
     ) -> ReplayBuffer:
         """
         Get the ReplayBuffer for a specific group.
         This function will check ``self.on_policy`` and create the buffer accordingly
 
         Args:
             group (str): agent group of the loss and updater
+            transforms (optional, list of Transform): Transforms to apply to the replay buffer ``.sample()`` call
 
         Returns: ReplayBuffer the group
         """
         memory_size = self.experiment_config.replay_buffer_memory_size(self.on_policy)
         sampling_size = self.experiment_config.train_minibatch_size(self.on_policy)
         storing_device = self.device
         sampler = SamplerWithoutReplacement() if self.on_policy else RandomSampler()
 
         return TensorDictReplayBuffer(
             storage=LazyTensorStorage(memory_size, device=storing_device),
             sampler=sampler,
             batch_size=sampling_size,
             priority_key=(group, "td_error"),
+            transform=Compose(*transforms) if transforms is not None else None,
         )
 
     def get_policy_for_loss(self, group: str) -> TensorDictModule:
         """
         Get the non-explorative policy for a specific group loss.
         This function calls the abstract :class:`~benchmarl.algorithms.Algorithm._get_policy_for_loss()` which needs to be implemented.
         The function will cache the output at the first call and return the cached values in future calls.
```

### Comparing `benchmarl-1.1.1/benchmarl/algorithms/iddpg.py` & `benchmarl-1.2.0/benchmarl/algorithms/maddpg.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 #  This source code is licensed under the license found in the
 #  LICENSE file in the root directory of this source tree.
 #
 
 from dataclasses import dataclass, MISSING
 from typing import Dict, Iterable, Tuple, Type
 
-import torch
 from tensordict import TensorDictBase
 from tensordict.nn import TensorDictModule, TensorDictSequential
 from torchrl.data import CompositeSpec, UnboundedContinuousTensorSpec
 from torchrl.modules import (
     AdditiveGaussianWrapper,
     Delta,
     ProbabilisticActor,
@@ -19,34 +18,33 @@
 )
 from torchrl.objectives import DDPGLoss, LossModule, ValueEstimators
 
 from benchmarl.algorithms.common import Algorithm, AlgorithmConfig
 from benchmarl.models.common import ModelConfig
 
 
-class Iddpg(Algorithm):
-    """Same as :class:`~benchmarl.algorithms.Maddpg` (from `https://arxiv.org/abs/1706.02275 <https://arxiv.org/abs/1706.02275>`__) but with decentralized critics.
+class Maddpg(Algorithm):
+    """Multi Agent DDPG (from `https://arxiv.org/abs/1706.02275 <https://arxiv.org/abs/1706.02275>`__).
 
     Args:
         share_param_critic (bool): Whether to share the parameters of the critics withing agent groups
         loss_function (str): loss function for the value discrepancy. Can be one of "l1", "l2" or "smooth_l1".
         delay_value (bool): whether to separate the target value networks from the value networks used for
             data collection.
         use_tanh_mapping (bool): if ``True``, use squash actions (output by the policy) into the action range, otherwise
             clip them.
-
     """
 
     def __init__(
         self,
         share_param_critic: bool,
         loss_function: str,
         delay_value: bool,
         use_tanh_mapping: bool,
-        **kwargs
+        **kwargs,
     ):
         super().__init__(**kwargs)
 
         self.share_param_critic = share_param_critic
         self.delay_value = delay_value
         self.loss_function = loss_function
         self.use_tanh_mapping = use_tanh_mapping
@@ -73,18 +71,19 @@
                 done=(group, "done"),
                 terminated=(group, "terminated"),
             )
 
             loss_module.make_value_estimator(
                 ValueEstimators.TD0, gamma=self.experiment_config.gamma
             )
+
             return loss_module, True
         else:
             raise NotImplementedError(
-                "Iddpg is not compatible with discrete actions yet"
+                "MADDPG is not compatible with discrete actions yet"
             )
 
     def _get_parameters(self, group: str, loss: LossModule) -> Dict[str, Iterable]:
         return {
             "loss_actor": list(loss.actor_network_params.flatten_keys().values()),
             "loss_value": list(loss.value_network_params.flatten_keys().values()),
         }
@@ -92,24 +91,15 @@
     def _get_policy_for_loss(
         self, group: str, model_config: ModelConfig, continuous: bool
     ) -> TensorDictModule:
         if continuous:
             n_agents = len(self.group_map[group])
             logits_shape = list(self.action_spec[group, "action"].shape)
             actor_input_spec = CompositeSpec(
-                {
-                    group: CompositeSpec(
-                        {
-                            "observation": self.observation_spec[group]["observation"]
-                            .clone()
-                            .to(self.device)
-                        },
-                        shape=(n_agents,),
-                    )
-                }
+                {group: self.observation_spec[group].clone().to(self.device)}
             )
             actor_output_spec = CompositeSpec(
                 {
                     group: CompositeSpec(
                         {"param": UnboundedContinuousTensorSpec(shape=logits_shape)},
                         shape=(n_agents,),
                     )
@@ -141,15 +131,15 @@
                 else {},
                 return_log_prob=False,
                 safe=not self.use_tanh_mapping,
             )
             return policy
         else:
             raise NotImplementedError(
-                "Iddpg is not compatible with discrete actions yet"
+                "MADDPG is not compatible with discrete actions yet"
             )
 
     def _get_policy_for_collection(
         self, policy_for_loss: TensorDictModule, group: str, continuous: bool
     ) -> TensorDictModule:
         return AdditiveGaussianWrapper(
             policy_for_loss,
@@ -194,79 +184,113 @@
     # Custom new methods
     #####################
 
     def get_value_module(self, group: str) -> TensorDictModule:
         n_agents = len(self.group_map[group])
         modules = []
 
-        modules.append(
-            TensorDictModule(
-                lambda obs, action: torch.cat([obs, action], dim=-1),
-                in_keys=[(group, "observation"), (group, "action")],
-                out_keys=[(group, "obs_action")],
+        if self.share_param_critic:
+            critic_output_spec = CompositeSpec(
+                {"state_action_value": UnboundedContinuousTensorSpec(shape=(1,))}
             )
-        )
-        critic_input_spec = CompositeSpec(
-            {
-                group: CompositeSpec(
-                    {
-                        "obs_action": UnboundedContinuousTensorSpec(
-                            shape=(
-                                n_agents,
-                                self.observation_spec[group, "observation"].shape[-1]
-                                + self.action_spec[group, "action"].shape[-1],
+        else:
+            critic_output_spec = CompositeSpec(
+                {
+                    group: CompositeSpec(
+                        {
+                            "state_action_value": UnboundedContinuousTensorSpec(
+                                shape=(n_agents, 1)
                             )
-                        )
-                    },
-                    shape=(n_agents,),
+                        },
+                        shape=(n_agents,),
+                    )
+                }
+            )
+
+        if self.state_spec is not None:
+            modules.append(
+                TensorDictModule(
+                    lambda action: action.reshape(*action.shape[:-2], -1),
+                    in_keys=[(group, "action")],
+                    out_keys=["global_action"],
                 )
-            }
-        )
-        critic_output_spec = CompositeSpec(
-            {
-                group: CompositeSpec(
-                    {
-                        "state_action_value": UnboundedContinuousTensorSpec(
-                            shape=(n_agents, 1)
-                        )
-                    },
-                    shape=(n_agents,),
+            )
+
+            critic_input_spec = self.state_spec.clone().update(
+                {
+                    "global_action": UnboundedContinuousTensorSpec(
+                        shape=(self.action_spec[group, "action"].shape[-1] * n_agents,)
+                    )
+                }
+            )
+
+            modules.append(
+                self.critic_model_config.get_model(
+                    input_spec=critic_input_spec,
+                    output_spec=critic_output_spec,
+                    n_agents=n_agents,
+                    centralised=True,
+                    input_has_agent_dim=False,
+                    agent_group=group,
+                    share_params=self.share_param_critic,
+                    device=self.device,
+                    action_spec=self.action_spec,
                 )
-            }
-        )
+            )
 
-        modules.append(
-            self.critic_model_config.get_model(
-                input_spec=critic_input_spec,
-                output_spec=critic_output_spec,
-                n_agents=n_agents,
-                centralised=False,
-                input_has_agent_dim=True,
-                agent_group=group,
-                share_params=self.share_param_critic,
-                device=self.device,
-                action_spec=self.action_spec,
+        else:
+            critic_input_spec = CompositeSpec(
+                {
+                    group: self.observation_spec[group]
+                    .clone()
+                    .update(self.action_spec[group])
+                }
+            )
+
+            modules.append(
+                self.critic_model_config.get_model(
+                    input_spec=critic_input_spec,
+                    output_spec=critic_output_spec,
+                    n_agents=n_agents,
+                    centralised=True,
+                    input_has_agent_dim=True,
+                    agent_group=group,
+                    share_params=self.share_param_critic,
+                    device=self.device,
+                    action_spec=self.action_spec,
+                )
+            )
+
+        if self.share_param_critic:
+            modules.append(
+                TensorDictModule(
+                    lambda value: value.unsqueeze(-2).expand(
+                        *value.shape[:-1], n_agents, 1
+                    ),
+                    in_keys=["state_action_value"],
+                    out_keys=[(group, "state_action_value")],
+                )
             )
-        )
 
         return TensorDictSequential(*modules)
 
 
 @dataclass
-class IddpgConfig(AlgorithmConfig):
-    """Configuration dataclass for :class:`~benchmarl.algorithms.Iddpg`."""
+class MaddpgConfig(AlgorithmConfig):
+    """Configuration dataclass for :class:`~benchmarl.algorithms.Maddpg`."""
 
     share_param_critic: bool = MISSING
+
     loss_function: str = MISSING
     delay_value: bool = MISSING
     use_tanh_mapping: bool = MISSING
 
     @staticmethod
     def associated_class() -> Type[Algorithm]:
-        return Iddpg
+        return Maddpg
 
     @staticmethod
     def supports_continuous_actions() -> bool:
         return True
 
     @staticmethod
     def supports_discrete_actions() -> bool:
```

### Comparing `benchmarl-1.1.1/benchmarl/algorithms/ippo.py` & `benchmarl-1.2.0/benchmarl/algorithms/ippo.py`

 * *Files 3% similar despite different names*

```diff
@@ -110,24 +110,15 @@
         else:
             logits_shape = [
                 *self.action_spec[group, "action"].shape,
                 self.action_spec[group, "action"].space.n,
             ]
 
         actor_input_spec = CompositeSpec(
-            {
-                group: CompositeSpec(
-                    {
-                        "observation": self.observation_spec[group]["observation"]
-                        .clone()
-                        .to(self.device)
-                    },
-                    shape=(n_agents,),
-                )
-            }
+            {group: self.observation_spec[group].clone().to(self.device)}
         )
 
         actor_output_spec = CompositeSpec(
             {
                 group: CompositeSpec(
                     {"logits": UnboundedContinuousTensorSpec(shape=logits_shape)},
                     shape=(n_agents,),
@@ -253,24 +244,15 @@
     # Custom new methods
     #####################
 
     def get_critic(self, group: str) -> TensorDictModule:
         n_agents = len(self.group_map[group])
 
         critic_input_spec = CompositeSpec(
-            {
-                group: CompositeSpec(
-                    {
-                        "observation": self.observation_spec[group]["observation"]
-                        .clone()
-                        .to(self.device)
-                    },
-                    shape=(n_agents,),
-                )
-            }
+            {group: self.observation_spec[group].clone().to(self.device)}
         )
         critic_output_spec = CompositeSpec(
             {
                 group: CompositeSpec(
                     {"state_value": UnboundedContinuousTensorSpec(shape=(n_agents, 1))},
                     shape=(n_agents,),
                 )
```

### Comparing `benchmarl-1.1.1/benchmarl/algorithms/iql.py` & `benchmarl-1.2.0/benchmarl/algorithms/iql.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,24 +74,15 @@
         n_agents = len(self.group_map[group])
         logits_shape = [
             *self.action_spec[group, "action"].shape,
             self.action_spec[group, "action"].space.n,
         ]
 
         actor_input_spec = CompositeSpec(
-            {
-                group: CompositeSpec(
-                    {
-                        "observation": self.observation_spec[group]["observation"]
-                        .clone()
-                        .to(self.device)
-                    },
-                    shape=(n_agents,),
-                )
-            }
+            {group: self.observation_spec[group].clone().to(self.device)}
         )
 
         actor_output_spec = CompositeSpec(
             {
                 group: CompositeSpec(
                     {"action_value": UnboundedContinuousTensorSpec(shape=logits_shape)},
                     shape=(n_agents,),
```

### Comparing `benchmarl-1.1.1/benchmarl/algorithms/isac.py` & `benchmarl-1.2.0/benchmarl/algorithms/isac.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 #  This source code is licensed under the license found in the
 #  LICENSE file in the root directory of this source tree.
 #
 
 from dataclasses import dataclass, MISSING
 from typing import Dict, Iterable, Optional, Tuple, Type, Union
 
-import torch
 from tensordict import TensorDictBase
 from tensordict.nn import NormalParamExtractor, TensorDictModule, TensorDictSequential
 from torch.distributions import Categorical
 from torchrl.data import CompositeSpec, UnboundedContinuousTensorSpec
 from torchrl.modules import (
     IndependentNormal,
     MaskedCategorical,
@@ -162,24 +161,15 @@
         else:
             logits_shape = [
                 *self.action_spec[group, "action"].shape,
                 self.action_spec[group, "action"].space.n,
             ]
 
         actor_input_spec = CompositeSpec(
-            {
-                group: CompositeSpec(
-                    {
-                        "observation": self.observation_spec[group]["observation"]
-                        .clone()
-                        .to(self.device)
-                    },
-                    shape=(n_agents,),
-                )
-            }
+            {group: self.observation_spec[group].clone().to(self.device)}
         )
 
         actor_output_spec = CompositeSpec(
             {
                 group: CompositeSpec(
                     {"logits": UnboundedContinuousTensorSpec(shape=logits_shape)},
                     shape=(n_agents,),
@@ -288,24 +278,15 @@
     #####################
 
     def get_discrete_value_module(self, group: str) -> TensorDictModule:
         n_agents = len(self.group_map[group])
         n_actions = self.action_spec[group, "action"].space.n
 
         critic_input_spec = CompositeSpec(
-            {
-                group: CompositeSpec(
-                    {
-                        "observation": self.observation_spec[group]["observation"]
-                        .clone()
-                        .to(self.device)
-                    },
-                    shape=(n_agents,),
-                )
-            }
+            {group: self.observation_spec[group].clone().to(self.device)}
         )
 
         critic_output_spec = CompositeSpec(
             {
                 group: CompositeSpec(
                     {
                         "action_value": UnboundedContinuousTensorSpec(
@@ -330,35 +311,19 @@
 
         return value_module
 
     def get_continuous_value_module(self, group: str) -> TensorDictModule:
         n_agents = len(self.group_map[group])
         modules = []
 
-        modules.append(
-            TensorDictModule(
-                lambda obs, action: torch.cat([obs, action], dim=-1),
-                in_keys=[(group, "observation"), (group, "action")],
-                out_keys=[(group, "obs_action")],
-            )
-        )
         critic_input_spec = CompositeSpec(
             {
-                group: CompositeSpec(
-                    {
-                        "obs_action": UnboundedContinuousTensorSpec(
-                            shape=(
-                                n_agents,
-                                self.observation_spec[group, "observation"].shape[-1]
-                                + self.action_spec[group, "action"].shape[-1],
-                            )
-                        )
-                    },
-                    shape=(n_agents,),
-                )
+                group: self.observation_spec[group]
+                .clone()
+                .update(self.action_spec[group])
             }
         )
 
         critic_output_spec = CompositeSpec(
             {
                 group: CompositeSpec(
                     {
```

### Comparing `benchmarl-1.1.1/benchmarl/algorithms/maddpg.py` & `benchmarl-1.2.0/benchmarl/algorithms/mappo.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,164 +6,201 @@
 
 from dataclasses import dataclass, MISSING
 from typing import Dict, Iterable, Tuple, Type
 
 import torch
 from tensordict import TensorDictBase
 from tensordict.nn import TensorDictModule, TensorDictSequential
+from tensordict.nn.distributions import NormalParamExtractor
+from torch.distributions import Categorical
 from torchrl.data import CompositeSpec, UnboundedContinuousTensorSpec
 from torchrl.modules import (
-    AdditiveGaussianWrapper,
-    Delta,
+    IndependentNormal,
+    MaskedCategorical,
     ProbabilisticActor,
-    TanhDelta,
+    TanhNormal,
 )
-from torchrl.objectives import DDPGLoss, LossModule, ValueEstimators
+from torchrl.objectives import ClipPPOLoss, LossModule, ValueEstimators
 
 from benchmarl.algorithms.common import Algorithm, AlgorithmConfig
 from benchmarl.models.common import ModelConfig
 
 
-class Maddpg(Algorithm):
-    """Multi Agent DDPG (from `https://arxiv.org/abs/1706.02275 <https://arxiv.org/abs/1706.02275>`__).
+class Mappo(Algorithm):
+    """Multi Agent PPO (from `https://arxiv.org/abs/2103.01955 <https://arxiv.org/abs/2103.01955>`__).
 
     Args:
         share_param_critic (bool): Whether to share the parameters of the critics withing agent groups
-        loss_function (str): loss function for the value discrepancy. Can be one of "l1", "l2" or "smooth_l1".
-        delay_value (bool): whether to separate the target value networks from the value networks used for
-            data collection.
-        use_tanh_mapping (bool): if ``True``, use squash actions (output by the policy) into the action range, otherwise
-            clip them.
+        clip_epsilon (scalar): weight clipping threshold in the clipped PPO loss equation.
+        entropy_coef (scalar): entropy multiplier when computing the total loss.
+        critic_coef (scalar): critic loss multiplier when computing the total
+        loss_critic_type (str): loss function for the value discrepancy.
+            Can be one of "l1", "l2" or "smooth_l1".
+        lmbda (float): The GAE lambda
+        scale_mapping (str): positive mapping function to be used with the std.
+            choices: "softplus", "exp", "relu", "biased_softplus_1";
+        use_tanh_normal (bool): if ``True``, use TanhNormal as the continuyous action distribution with support bound
+            to the action domain. Otherwise, an IndependentNormal is used.
+
     """
 
     def __init__(
         self,
         share_param_critic: bool,
-        loss_function: str,
-        delay_value: bool,
-        use_tanh_mapping: bool,
+        clip_epsilon: float,
+        entropy_coef: bool,
+        critic_coef: float,
+        loss_critic_type: str,
+        lmbda: float,
+        scale_mapping: str,
+        use_tanh_normal: bool,
         **kwargs
     ):
         super().__init__(**kwargs)
 
         self.share_param_critic = share_param_critic
-        self.delay_value = delay_value
-        self.loss_function = loss_function
-        self.use_tanh_mapping = use_tanh_mapping
+        self.clip_epsilon = clip_epsilon
+        self.entropy_coef = entropy_coef
+        self.critic_coef = critic_coef
+        self.loss_critic_type = loss_critic_type
+        self.lmbda = lmbda
+        self.scale_mapping = scale_mapping
+        self.use_tanh_normal = use_tanh_normal
 
     #############################
     # Overridden abstract methods
     #############################
 
     def _get_loss(
         self, group: str, policy_for_loss: TensorDictModule, continuous: bool
     ) -> Tuple[LossModule, bool]:
-        if continuous:
-            # Loss
-            loss_module = DDPGLoss(
-                actor_network=policy_for_loss,
-                value_network=self.get_value_module(group),
-                delay_value=self.delay_value,
-                loss_function=self.loss_function,
-            )
-            loss_module.set_keys(
-                state_action_value=(group, "state_action_value"),
-                reward=(group, "reward"),
-                priority=(group, "td_error"),
-                done=(group, "done"),
-                terminated=(group, "terminated"),
-            )
-
-            loss_module.make_value_estimator(
-                ValueEstimators.TD0, gamma=self.experiment_config.gamma
-            )
-
-            return loss_module, True
-        else:
-            raise NotImplementedError(
-                "MADDPG is not compatible with discrete actions yet"
-            )
+        # Loss
+        loss_module = ClipPPOLoss(
+            actor=policy_for_loss,
+            critic=self.get_critic(group),
+            clip_epsilon=self.clip_epsilon,
+            entropy_coef=self.entropy_coef,
+            critic_coef=self.critic_coef,
+            loss_critic_type=self.loss_critic_type,
+            normalize_advantage=False,
+        )
+        loss_module.set_keys(
+            reward=(group, "reward"),
+            action=(group, "action"),
+            done=(group, "done"),
+            terminated=(group, "terminated"),
+            advantage=(group, "advantage"),
+            value_target=(group, "value_target"),
+            value=(group, "state_value"),
+            sample_log_prob=(group, "log_prob"),
+        )
+        loss_module.make_value_estimator(
+            ValueEstimators.GAE, gamma=self.experiment_config.gamma, lmbda=self.lmbda
+        )
+        return loss_module, False
 
-    def _get_parameters(self, group: str, loss: LossModule) -> Dict[str, Iterable]:
+    def _get_parameters(self, group: str, loss: ClipPPOLoss) -> Dict[str, Iterable]:
         return {
-            "loss_actor": list(loss.actor_network_params.flatten_keys().values()),
-            "loss_value": list(loss.value_network_params.flatten_keys().values()),
+            "loss_objective": list(loss.actor_network_params.flatten_keys().values()),
+            "loss_critic": list(loss.critic_network_params.flatten_keys().values()),
         }
 
     def _get_policy_for_loss(
         self, group: str, model_config: ModelConfig, continuous: bool
     ) -> TensorDictModule:
+        n_agents = len(self.group_map[group])
         if continuous:
-            n_agents = len(self.group_map[group])
             logits_shape = list(self.action_spec[group, "action"].shape)
-            actor_input_spec = CompositeSpec(
-                {
-                    group: CompositeSpec(
-                        {
-                            "observation": self.observation_spec[group]["observation"]
-                            .clone()
-                            .to(self.device)
-                        },
-                        shape=(n_agents,),
-                    )
-                }
-            )
-            actor_output_spec = CompositeSpec(
-                {
-                    group: CompositeSpec(
-                        {"param": UnboundedContinuousTensorSpec(shape=logits_shape)},
-                        shape=(n_agents,),
-                    )
-                }
-            )
-            actor_module = model_config.get_model(
-                input_spec=actor_input_spec,
-                output_spec=actor_output_spec,
-                agent_group=group,
-                input_has_agent_dim=True,
-                n_agents=n_agents,
-                centralised=False,
-                share_params=self.experiment_config.share_policy_params,
-                device=self.device,
-                action_spec=self.action_spec,
-            )
+            logits_shape[-1] *= 2
+        else:
+            logits_shape = [
+                *self.action_spec[group, "action"].shape,
+                self.action_spec[group, "action"].space.n,
+            ]
 
+        actor_input_spec = CompositeSpec(
+            {group: self.observation_spec[group].clone().to(self.device)}
+        )
+
+        actor_output_spec = CompositeSpec(
+            {
+                group: CompositeSpec(
+                    {"logits": UnboundedContinuousTensorSpec(shape=logits_shape)},
+                    shape=(n_agents,),
+                )
+            }
+        )
+        actor_module = model_config.get_model(
+            input_spec=actor_input_spec,
+            output_spec=actor_output_spec,
+            agent_group=group,
+            input_has_agent_dim=True,
+            n_agents=n_agents,
+            centralised=False,
+            share_params=self.experiment_config.share_policy_params,
+            device=self.device,
+            action_spec=self.action_spec,
+        )
+
+        if continuous:
+            extractor_module = TensorDictModule(
+                NormalParamExtractor(scale_mapping=self.scale_mapping),
+                in_keys=[(group, "logits")],
+                out_keys=[(group, "loc"), (group, "scale")],
+            )
             policy = ProbabilisticActor(
-                module=actor_module,
+                module=TensorDictSequential(actor_module, extractor_module),
                 spec=self.action_spec[group, "action"],
-                in_keys=[(group, "param")],
+                in_keys=[(group, "loc"), (group, "scale")],
                 out_keys=[(group, "action")],
-                distribution_class=TanhDelta if self.use_tanh_mapping else Delta,
+                distribution_class=IndependentNormal
+                if not self.use_tanh_normal
+                else TanhNormal,
                 distribution_kwargs={
                     "min": self.action_spec[(group, "action")].space.low,
                     "max": self.action_spec[(group, "action")].space.high,
                 }
-                if self.use_tanh_mapping
+                if self.use_tanh_normal
                 else {},
-                return_log_prob=False,
-                safe=not self.use_tanh_mapping,
+                return_log_prob=True,
+                log_prob_key=(group, "log_prob"),
             )
-            return policy
+
         else:
-            raise NotImplementedError(
-                "MADDPG is not compatible with discrete actions yet"
-            )
+            if self.action_mask_spec is None:
+                policy = ProbabilisticActor(
+                    module=actor_module,
+                    spec=self.action_spec[group, "action"],
+                    in_keys=[(group, "logits")],
+                    out_keys=[(group, "action")],
+                    distribution_class=Categorical,
+                    return_log_prob=True,
+                    log_prob_key=(group, "log_prob"),
+                )
+            else:
+                policy = ProbabilisticActor(
+                    module=actor_module,
+                    spec=self.action_spec[group, "action"],
+                    in_keys={
+                        "logits": (group, "logits"),
+                        "mask": (group, "action_mask"),
+                    },
+                    out_keys=[(group, "action")],
+                    distribution_class=MaskedCategorical,
+                    return_log_prob=True,
+                    log_prob_key=(group, "log_prob"),
+                )
+
+        return policy
 
     def _get_policy_for_collection(
         self, policy_for_loss: TensorDictModule, group: str, continuous: bool
     ) -> TensorDictModule:
-        return AdditiveGaussianWrapper(
-            policy_for_loss,
-            annealing_num_steps=self.experiment_config.get_exploration_anneal_frames(
-                self.on_policy
-            ),
-            action_key=(group, "action"),
-            sigma_init=self.experiment_config.exploration_eps_init,
-            sigma_end=self.experiment_config.exploration_eps_end,
-        )
+        # MAPPO uses the same stochastic actor for collection
+        return policy_for_loss
 
     def process_batch(self, group: str, batch: TensorDictBase) -> TensorDictBase:
         keys = list(batch.keys(True, True))
         group_shape = batch.get(group).shape
 
         nested_done_key = ("next", group, "done")
         nested_terminated_key = ("next", group, "terminated")
@@ -184,150 +221,119 @@
 
         if nested_reward_key not in keys:
             batch.set(
                 nested_reward_key,
                 batch.get(("next", "reward")).unsqueeze(-1).expand((*group_shape, 1)),
             )
 
+        with torch.no_grad():
+            loss = self.get_loss_and_updater(group)[0]
+            loss.value_estimator(
+                batch,
+                params=loss.critic_network_params,
+                target_params=loss.target_critic_network_params,
+            )
+
         return batch
 
+    def process_loss_vals(
+        self, group: str, loss_vals: TensorDictBase
+    ) -> TensorDictBase:
+        loss_vals.set(
+            "loss_objective", loss_vals["loss_objective"] + loss_vals["loss_entropy"]
+        )
+        del loss_vals["loss_entropy"]
+        return loss_vals
+
     #####################
     # Custom new methods
     #####################
 
-    def get_value_module(self, group: str) -> TensorDictModule:
+    def get_critic(self, group: str) -> TensorDictModule:
         n_agents = len(self.group_map[group])
-        modules = []
-
         if self.share_param_critic:
             critic_output_spec = CompositeSpec(
-                {"state_action_value": UnboundedContinuousTensorSpec(shape=(1,))}
+                {"state_value": UnboundedContinuousTensorSpec(shape=(1,))}
             )
         else:
             critic_output_spec = CompositeSpec(
                 {
                     group: CompositeSpec(
                         {
-                            "state_action_value": UnboundedContinuousTensorSpec(
+                            "state_value": UnboundedContinuousTensorSpec(
                                 shape=(n_agents, 1)
                             )
                         },
                         shape=(n_agents,),
                     )
                 }
             )
 
         if self.state_spec is not None:
-            modules.append(
-                TensorDictModule(
-                    lambda state, action: torch.cat(
-                        [state, action.reshape(*action.shape[:-2], -1)], dim=-1
-                    ),
-                    in_keys=["state", (group, "action")],
-                    out_keys=["state_action"],
-                )
-            )
-            critic_input_spec = CompositeSpec(
-                {
-                    "state_action": UnboundedContinuousTensorSpec(
-                        shape=(
-                            self.state_spec["state"].shape[-1]
-                            + self.action_spec[group, "action"].shape[-1] * n_agents,
-                        )
-                    )
-                }
-            )
-
-            modules.append(
-                self.critic_model_config.get_model(
-                    input_spec=critic_input_spec,
-                    output_spec=critic_output_spec,
-                    n_agents=n_agents,
-                    centralised=True,
-                    input_has_agent_dim=False,
-                    agent_group=group,
-                    share_params=self.share_param_critic,
-                    device=self.device,
-                    action_spec=self.action_spec,
-                )
+            value_module = self.critic_model_config.get_model(
+                input_spec=self.state_spec,
+                output_spec=critic_output_spec,
+                n_agents=n_agents,
+                centralised=True,
+                input_has_agent_dim=False,
+                agent_group=group,
+                share_params=self.share_param_critic,
+                device=self.device,
+                action_spec=self.action_spec,
             )
 
         else:
-            modules.append(
-                TensorDictModule(
-                    lambda obs, action: torch.cat([obs, action], dim=-1),
-                    in_keys=[(group, "observation"), (group, "action")],
-                    out_keys=[(group, "obs_action")],
-                )
-            )
             critic_input_spec = CompositeSpec(
-                {
-                    group: CompositeSpec(
-                        {
-                            "obs_action": UnboundedContinuousTensorSpec(
-                                shape=(
-                                    n_agents,
-                                    self.observation_spec[group, "observation"].shape[
-                                        -1
-                                    ]
-                                    + self.action_spec[group, "action"].shape[-1],
-                                )
-                            )
-                        },
-                        shape=(n_agents,),
-                    )
-                }
+                {group: self.observation_spec[group].clone().to(self.device)}
             )
-
-            modules.append(
-                self.critic_model_config.get_model(
-                    input_spec=critic_input_spec,
-                    output_spec=critic_output_spec,
-                    n_agents=n_agents,
-                    centralised=True,
-                    input_has_agent_dim=True,
-                    agent_group=group,
-                    share_params=self.share_param_critic,
-                    device=self.device,
-                    action_spec=self.action_spec,
-                )
+            value_module = self.critic_model_config.get_model(
+                input_spec=critic_input_spec,
+                output_spec=critic_output_spec,
+                n_agents=n_agents,
+                centralised=True,
+                input_has_agent_dim=True,
+                agent_group=group,
+                share_params=self.share_param_critic,
+                device=self.device,
+                action_spec=self.action_spec,
             )
-
         if self.share_param_critic:
-            modules.append(
-                TensorDictModule(
-                    lambda value: value.unsqueeze(-2).expand(
-                        *value.shape[:-1], n_agents, 1
-                    ),
-                    in_keys=["state_action_value"],
-                    out_keys=[(group, "state_action_value")],
-                )
+            expand_module = TensorDictModule(
+                lambda value: value.unsqueeze(-2).expand(
+                    *value.shape[:-1], n_agents, 1
+                ),
+                in_keys=["state_value"],
+                out_keys=[(group, "state_value")],
             )
+            value_module = TensorDictSequential(value_module, expand_module)
 
-        return TensorDictSequential(*modules)
+        return value_module
 
 
 @dataclass
-class MaddpgConfig(AlgorithmConfig):
-    """Configuration dataclass for :class:`~benchmarl.algorithms.Maddpg`."""
+class MappoConfig(AlgorithmConfig):
+    """Configuration dataclass for :class:`~benchmarl.algorithms.Mappo`."""
 
     share_param_critic: bool = MISSING
-
-    loss_function: str = MISSING
-    delay_value: bool = MISSING
-    use_tanh_mapping: bool = MISSING
+    clip_epsilon: float = MISSING
+    entropy_coef: float = MISSING
+    critic_coef: float = MISSING
+    loss_critic_type: str = MISSING
+    lmbda: float = MISSING
+    scale_mapping: str = MISSING
+    use_tanh_normal: bool = MISSING
 
     @staticmethod
     def associated_class() -> Type[Algorithm]:
-        return Maddpg
+        return Mappo
 
     @staticmethod
     def supports_continuous_actions() -> bool:
         return True
 
     @staticmethod
     def supports_discrete_actions() -> bool:
-        return False
+        return True
 
     @staticmethod
     def on_policy() -> bool:
-        return False
+        return True
```

### Comparing `benchmarl-1.1.1/benchmarl/algorithms/mappo.py` & `benchmarl-1.2.0/benchmarl/algorithms/masac.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,112 +1,159 @@
 #  Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 #  This source code is licensed under the license found in the
 #  LICENSE file in the root directory of this source tree.
 #
 
 from dataclasses import dataclass, MISSING
-from typing import Dict, Iterable, Tuple, Type
+from typing import Dict, Iterable, Optional, Tuple, Type, Union
 
-import torch
 from tensordict import TensorDictBase
-from tensordict.nn import TensorDictModule, TensorDictSequential
-from tensordict.nn.distributions import NormalParamExtractor
+from tensordict.nn import NormalParamExtractor, TensorDictModule, TensorDictSequential
 from torch.distributions import Categorical
 from torchrl.data import CompositeSpec, UnboundedContinuousTensorSpec
 from torchrl.modules import (
     IndependentNormal,
     MaskedCategorical,
     ProbabilisticActor,
     TanhNormal,
 )
-from torchrl.objectives import ClipPPOLoss, LossModule, ValueEstimators
+from torchrl.objectives import DiscreteSACLoss, LossModule, SACLoss, ValueEstimators
 
 from benchmarl.algorithms.common import Algorithm, AlgorithmConfig
 from benchmarl.models.common import ModelConfig
 
 
-class Mappo(Algorithm):
-    """Multi Agent PPO (from `https://arxiv.org/abs/2103.01955 <https://arxiv.org/abs/2103.01955>`__).
+class Masac(Algorithm):
+    """Multi Agent Soft Actor Critic.
 
     Args:
         share_param_critic (bool): Whether to share the parameters of the critics withing agent groups
-        clip_epsilon (scalar): weight clipping threshold in the clipped PPO loss equation.
-        entropy_coef (scalar): entropy multiplier when computing the total loss.
-        critic_coef (scalar): critic loss multiplier when computing the total
-        loss_critic_type (str): loss function for the value discrepancy.
-            Can be one of "l1", "l2" or "smooth_l1".
-        lmbda (float): The GAE lambda
+        num_qvalue_nets (integer): number of Q-Value networks used.
+        loss_function (str): loss function to be used with
+            the value function loss.
+        delay_qvalue (bool): Whether to separate the target Q value
+            networks from the Q value networks used for data collection.
+        target_entropy (float or str, optional): Target entropy for the
+            stochastic policy. Default is "auto", where target entropy is
+            computed as :obj:`-prod(n_actions)`.
+        discrete_target_entropy_weight (float): weight for the target entropy term when actions are discrete
+        alpha_init (float): initial entropy multiplier.
+        min_alpha (float): min value of alpha.
+        max_alpha (float): max value of alpha.
+        fixed_alpha (bool): if ``True``, alpha will be fixed to its
+            initial value. Otherwise, alpha will be optimized to
+            match the 'target_entropy' value.
         scale_mapping (str): positive mapping function to be used with the std.
             choices: "softplus", "exp", "relu", "biased_softplus_1";
         use_tanh_normal (bool): if ``True``, use TanhNormal as the continuyous action distribution with support bound
             to the action domain. Otherwise, an IndependentNormal is used.
-
     """
 
     def __init__(
         self,
         share_param_critic: bool,
-        clip_epsilon: float,
-        entropy_coef: bool,
-        critic_coef: float,
-        loss_critic_type: str,
-        lmbda: float,
+        num_qvalue_nets: int,
+        loss_function: str,
+        delay_qvalue: bool,
+        target_entropy: Union[float, str],
+        discrete_target_entropy_weight: float,
+        alpha_init: float,
+        min_alpha: Optional[float],
+        max_alpha: Optional[float],
+        fixed_alpha: bool,
         scale_mapping: str,
         use_tanh_normal: bool,
         **kwargs
     ):
         super().__init__(**kwargs)
 
         self.share_param_critic = share_param_critic
-        self.clip_epsilon = clip_epsilon
-        self.entropy_coef = entropy_coef
-        self.critic_coef = critic_coef
-        self.loss_critic_type = loss_critic_type
-        self.lmbda = lmbda
+        self.delay_qvalue = delay_qvalue
+        self.num_qvalue_nets = num_qvalue_nets
+        self.loss_function = loss_function
+        self.target_entropy = target_entropy
+        self.discrete_target_entropy_weight = discrete_target_entropy_weight
+        self.alpha_init = alpha_init
+        self.min_alpha = min_alpha
+        self.max_alpha = max_alpha
+        self.fixed_alpha = fixed_alpha
         self.scale_mapping = scale_mapping
         self.use_tanh_normal = use_tanh_normal
 
     #############################
     # Overridden abstract methods
     #############################
 
     def _get_loss(
         self, group: str, policy_for_loss: TensorDictModule, continuous: bool
     ) -> Tuple[LossModule, bool]:
-        # Loss
-        loss_module = ClipPPOLoss(
-            actor=policy_for_loss,
-            critic=self.get_critic(group),
-            clip_epsilon=self.clip_epsilon,
-            entropy_coef=self.entropy_coef,
-            critic_coef=self.critic_coef,
-            loss_critic_type=self.loss_critic_type,
-            normalize_advantage=False,
-        )
-        loss_module.set_keys(
-            reward=(group, "reward"),
-            action=(group, "action"),
-            done=(group, "done"),
-            terminated=(group, "terminated"),
-            advantage=(group, "advantage"),
-            value_target=(group, "value_target"),
-            value=(group, "state_value"),
-            sample_log_prob=(group, "log_prob"),
-        )
+        if continuous:
+            # Loss
+            loss_module = SACLoss(
+                actor_network=policy_for_loss,
+                qvalue_network=self.get_continuous_value_module(group),
+                num_qvalue_nets=self.num_qvalue_nets,
+                loss_function=self.loss_function,
+                alpha_init=self.alpha_init,
+                min_alpha=self.min_alpha,
+                max_alpha=self.max_alpha,
+                action_spec=self.action_spec,
+                fixed_alpha=self.fixed_alpha,
+                target_entropy=self.target_entropy,
+                delay_qvalue=self.delay_qvalue,
+            )
+            loss_module.set_keys(
+                state_action_value=(group, "state_action_value"),
+                action=(group, "action"),
+                reward=(group, "reward"),
+                priority=(group, "td_error"),
+                done=(group, "done"),
+                terminated=(group, "terminated"),
+            )
+
+        else:
+            loss_module = DiscreteSACLoss(
+                actor_network=policy_for_loss,
+                qvalue_network=self.get_discrete_value_module(group),
+                num_qvalue_nets=self.num_qvalue_nets,
+                loss_function=self.loss_function,
+                alpha_init=self.alpha_init,
+                min_alpha=self.min_alpha,
+                max_alpha=self.max_alpha,
+                action_space=self.action_spec,
+                fixed_alpha=self.fixed_alpha,
+                target_entropy=self.target_entropy,
+                target_entropy_weight=self.discrete_target_entropy_weight,
+                delay_qvalue=self.delay_qvalue,
+                num_actions=self.action_spec[group, "action"].space.n,
+            )
+            loss_module.set_keys(
+                action_value=(group, "action_value"),
+                action=(group, "action"),
+                reward=(group, "reward"),
+                priority=(group, "td_error"),
+                done=(group, "done"),
+                terminated=(group, "terminated"),
+            )
+
         loss_module.make_value_estimator(
-            ValueEstimators.GAE, gamma=self.experiment_config.gamma, lmbda=self.lmbda
+            ValueEstimators.TD0, gamma=self.experiment_config.gamma
         )
-        return loss_module, False
 
-    def _get_parameters(self, group: str, loss: ClipPPOLoss) -> Dict[str, Iterable]:
-        return {
-            "loss_objective": list(loss.actor_network_params.flatten_keys().values()),
-            "loss_critic": list(loss.critic_network_params.flatten_keys().values()),
+        return loss_module, True
+
+    def _get_parameters(self, group: str, loss: LossModule) -> Dict[str, Iterable]:
+        items = {
+            "loss_actor": list(loss.actor_network_params.flatten_keys().values()),
+            "loss_qvalue": list(loss.qvalue_network_params.flatten_keys().values()),
         }
+        if not self.fixed_alpha:
+            items.update({"loss_alpha": [loss.log_alpha]})
+        return items
 
     def _get_policy_for_loss(
         self, group: str, model_config: ModelConfig, continuous: bool
     ) -> TensorDictModule:
         n_agents = len(self.group_map[group])
         if continuous:
             logits_shape = list(self.action_spec[group, "action"].shape)
@@ -114,24 +161,15 @@
         else:
             logits_shape = [
                 *self.action_spec[group, "action"].shape,
                 self.action_spec[group, "action"].space.n,
             ]
 
         actor_input_spec = CompositeSpec(
-            {
-                group: CompositeSpec(
-                    {
-                        "observation": self.observation_spec[group]["observation"]
-                        .clone()
-                        .to(self.device)
-                    },
-                    shape=(n_agents,),
-                )
-            }
+            {group: self.observation_spec[group].clone().to(self.device)}
         )
 
         actor_output_spec = CompositeSpec(
             {
                 group: CompositeSpec(
                     {"logits": UnboundedContinuousTensorSpec(shape=logits_shape)},
                     shape=(n_agents,),
@@ -190,25 +228,24 @@
                     module=actor_module,
                     spec=self.action_spec[group, "action"],
                     in_keys={
                         "logits": (group, "logits"),
                         "mask": (group, "action_mask"),
                     },
                     out_keys=[(group, "action")],
+                    distribution_kwargs={"neg_inf": -18.0},
                     distribution_class=MaskedCategorical,
                     return_log_prob=True,
                     log_prob_key=(group, "log_prob"),
                 )
-
         return policy
 
     def _get_policy_for_collection(
         self, policy_for_loss: TensorDictModule, group: str, continuous: bool
     ) -> TensorDictModule:
-        # MAPPO uses the same stochastic actor for collection
         return policy_for_loss
 
     def process_batch(self, group: str, batch: TensorDictBase) -> TensorDictBase:
         keys = list(batch.keys(True, True))
         group_shape = batch.get(group).shape
 
         nested_done_key = ("next", group, "done")
@@ -230,50 +267,34 @@
 
         if nested_reward_key not in keys:
             batch.set(
                 nested_reward_key,
                 batch.get(("next", "reward")).unsqueeze(-1).expand((*group_shape, 1)),
             )
 
-        with torch.no_grad():
-            loss = self.get_loss_and_updater(group)[0]
-            loss.value_estimator(
-                batch,
-                params=loss.critic_network_params,
-                target_params=loss.target_critic_network_params,
-            )
-
         return batch
 
-    def process_loss_vals(
-        self, group: str, loss_vals: TensorDictBase
-    ) -> TensorDictBase:
-        loss_vals.set(
-            "loss_objective", loss_vals["loss_objective"] + loss_vals["loss_entropy"]
-        )
-        del loss_vals["loss_entropy"]
-        return loss_vals
-
     #####################
     # Custom new methods
     #####################
 
-    def get_critic(self, group: str) -> TensorDictModule:
+    def get_discrete_value_module(self, group: str) -> TensorDictModule:
         n_agents = len(self.group_map[group])
+        n_actions = self.action_spec[group, "action"].space.n
         if self.share_param_critic:
             critic_output_spec = CompositeSpec(
-                {"state_value": UnboundedContinuousTensorSpec(shape=(1,))}
+                {"action_value": UnboundedContinuousTensorSpec(shape=(n_actions,))}
             )
         else:
             critic_output_spec = CompositeSpec(
                 {
                     group: CompositeSpec(
                         {
-                            "state_value": UnboundedContinuousTensorSpec(
-                                shape=(n_agents, 1)
+                            "action_value": UnboundedContinuousTensorSpec(
+                                shape=(n_agents, n_actions)
                             )
                         },
                         shape=(n_agents,),
                     )
                 }
             )
 
@@ -288,24 +309,15 @@
                 share_params=self.share_param_critic,
                 device=self.device,
                 action_spec=self.action_spec,
             )
 
         else:
             critic_input_spec = CompositeSpec(
-                {
-                    group: CompositeSpec(
-                        {
-                            "observation": self.observation_spec[group]["observation"]
-                            .clone()
-                            .to(self.device)
-                        },
-                        shape=(n_agents,),
-                    )
-                }
+                {group: self.observation_spec[group].clone().to(self.device)}
             )
             value_module = self.critic_model_config.get_model(
                 input_spec=critic_input_spec,
                 output_spec=critic_output_spec,
                 n_agents=n_agents,
                 centralised=True,
                 input_has_agent_dim=True,
@@ -313,45 +325,139 @@
                 share_params=self.share_param_critic,
                 device=self.device,
                 action_spec=self.action_spec,
             )
         if self.share_param_critic:
             expand_module = TensorDictModule(
                 lambda value: value.unsqueeze(-2).expand(
-                    *value.shape[:-1], n_agents, 1
+                    *value.shape[:-1], n_agents, n_actions
                 ),
-                in_keys=["state_value"],
-                out_keys=[(group, "state_value")],
+                in_keys=["action_value"],
+                out_keys=[(group, "action_value")],
             )
             value_module = TensorDictSequential(value_module, expand_module)
 
         return value_module
 
+    def get_continuous_value_module(self, group: str) -> TensorDictModule:
+        n_agents = len(self.group_map[group])
+        modules = []
+
+        if self.share_param_critic:
+            critic_output_spec = CompositeSpec(
+                {"state_action_value": UnboundedContinuousTensorSpec(shape=(1,))}
+            )
+        else:
+            critic_output_spec = CompositeSpec(
+                {
+                    group: CompositeSpec(
+                        {
+                            "state_action_value": UnboundedContinuousTensorSpec(
+                                shape=(n_agents, 1)
+                            )
+                        },
+                        shape=(n_agents,),
+                    )
+                }
+            )
+
+        if self.state_spec is not None:
+
+            modules.append(
+                TensorDictModule(
+                    lambda action: action.reshape(*action.shape[:-2], -1),
+                    in_keys=[(group, "action")],
+                    out_keys=["global_action"],
+                )
+            )
+
+            critic_input_spec = self.state_spec.clone().update(
+                {
+                    "global_action": UnboundedContinuousTensorSpec(
+                        shape=(self.action_spec[group, "action"].shape[-1] * n_agents,)
+                    )
+                }
+            )
+
+            modules.append(
+                self.critic_model_config.get_model(
+                    input_spec=critic_input_spec,
+                    output_spec=critic_output_spec,
+                    n_agents=n_agents,
+                    centralised=True,
+                    input_has_agent_dim=False,
+                    agent_group=group,
+                    share_params=self.share_param_critic,
+                    device=self.device,
+                    action_spec=self.action_spec,
+                )
+            )
+
+        else:
+            critic_input_spec = CompositeSpec(
+                {
+                    group: self.observation_spec[group]
+                    .clone()
+                    .update(self.action_spec[group])
+                }
+            )
+
+            modules.append(
+                self.critic_model_config.get_model(
+                    input_spec=critic_input_spec,
+                    output_spec=critic_output_spec,
+                    n_agents=n_agents,
+                    centralised=True,
+                    input_has_agent_dim=True,
+                    agent_group=group,
+                    share_params=self.share_param_critic,
+                    device=self.device,
+                    action_spec=self.action_spec,
+                )
+            )
+
+        if self.share_param_critic:
+            modules.append(
+                TensorDictModule(
+                    lambda value: value.unsqueeze(-2).expand(
+                        *value.shape[:-1], n_agents, 1
+                    ),
+                    in_keys=["state_action_value"],
+                    out_keys=[(group, "state_action_value")],
+                )
+            )
+
+        return TensorDictSequential(*modules)
+
 
 @dataclass
-class MappoConfig(AlgorithmConfig):
-    """Configuration dataclass for :class:`~benchmarl.algorithms.Mappo`."""
+class MasacConfig(AlgorithmConfig):
+    """Configuration dataclass for :class:`~benchmarl.algorithms.Masac`."""
 
     share_param_critic: bool = MISSING
-    clip_epsilon: float = MISSING
-    entropy_coef: float = MISSING
-    critic_coef: float = MISSING
-    loss_critic_type: str = MISSING
-    lmbda: float = MISSING
+    num_qvalue_nets: int = MISSING
+    loss_function: str = MISSING
+    delay_qvalue: bool = MISSING
+    target_entropy: Union[float, str] = MISSING
+    discrete_target_entropy_weight: float = MISSING
+    alpha_init: float = MISSING
+    min_alpha: Optional[float] = MISSING
+    max_alpha: Optional[float] = MISSING
+    fixed_alpha: bool = MISSING
     scale_mapping: str = MISSING
     use_tanh_normal: bool = MISSING
 
     @staticmethod
     def associated_class() -> Type[Algorithm]:
-        return Mappo
+        return Masac
 
     @staticmethod
     def supports_continuous_actions() -> bool:
         return True
 
     @staticmethod
     def supports_discrete_actions() -> bool:
         return True
 
     @staticmethod
     def on_policy() -> bool:
-        return True
+        return False
```

### Comparing `benchmarl-1.1.1/benchmarl/algorithms/qmix.py` & `benchmarl-1.2.0/benchmarl/algorithms/qmix.py`

 * *Files 6% similar despite different names*

```diff
@@ -80,24 +80,15 @@
         n_agents = len(self.group_map[group])
         logits_shape = [
             *self.action_spec[group, "action"].shape,
             self.action_spec[group, "action"].space.n,
         ]
 
         actor_input_spec = CompositeSpec(
-            {
-                group: CompositeSpec(
-                    {
-                        "observation": self.observation_spec[group]["observation"]
-                        .clone()
-                        .to(self.device)
-                    },
-                    shape=(n_agents,),
-                )
-            }
+            {group: self.observation_spec[group].clone().to(self.device)}
         )
 
         actor_output_spec = CompositeSpec(
             {
                 group: CompositeSpec(
                     {"action_value": UnboundedContinuousTensorSpec(shape=logits_shape)},
                     shape=(n_agents,),
@@ -182,21 +173,23 @@
 
     #####################
     # Custom new methods
     #####################
 
     def get_mixer(self, group: str) -> TensorDictModule:
         n_agents = len(self.group_map[group])
+        group_observation_key = list(self.observation_spec[group].keys())[0]
 
         if self.state_spec is not None:
-            state_shape = self.state_spec["state"].shape
-            in_keys = [(group, "chosen_action_value"), "state"]
+            global_state_key = list(self.state_spec.keys())[0]
+            state_shape = self.state_spec[global_state_key].shape
+            in_keys = [(group, "chosen_action_value"), global_state_key]
         else:
-            state_shape = self.observation_spec[group, "observation"].shape
-            in_keys = [(group, "chosen_action_value"), (group, "observation")]
+            state_shape = self.observation_spec[group, group_observation_key].shape
+            in_keys = [(group, "chosen_action_value"), (group, group_observation_key)]
 
         mixer = TensorDictModule(
             module=QMixer(
                 state_shape=state_shape,
                 mixing_embed_dim=self.mixing_embed_dim,
                 n_agents=n_agents,
                 device=self.device,
```

### Comparing `benchmarl-1.1.1/benchmarl/algorithms/vdn.py` & `benchmarl-1.2.0/benchmarl/algorithms/vdn.py`

 * *Files 9% similar despite different names*

```diff
@@ -78,24 +78,15 @@
         n_agents = len(self.group_map[group])
         logits_shape = [
             *self.action_spec[group, "action"].shape,
             self.action_spec[group, "action"].space.n,
         ]
 
         actor_input_spec = CompositeSpec(
-            {
-                group: CompositeSpec(
-                    {
-                        "observation": self.observation_spec[group]["observation"]
-                        .clone()
-                        .to(self.device)
-                    },
-                    shape=(n_agents,),
-                )
-            }
+            {group: self.observation_spec[group].clone().to(self.device)}
         )
 
         actor_output_spec = CompositeSpec(
             {
                 group: CompositeSpec(
                     {"action_value": UnboundedContinuousTensorSpec(shape=logits_shape)},
                     shape=(n_agents,),
```

### Comparing `benchmarl-1.1.1/benchmarl/benchmark/benchmark.py` & `benchmarl-1.2.0/benchmarl/benchmark/benchmark.py`

 * *Files identical despite different names*

### Comparing `benchmarl-1.1.1/benchmarl/conf/experiment/base_experiment.yaml` & `benchmarl-1.2.0/benchmarl/conf/experiment/base_experiment.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -78,19 +78,19 @@
 evaluation_interval: 120_000
 # Number of episodes that evaluation is run on
 evaluation_episodes: 10
 # If True, when stochastic policies are evaluated, their mode is taken, otherwise, if False, they are sampled
 evaluation_deterministic_actions: True
 
 # List of loggers to use, options are: wandb, csv, tensorboard, mflow
-loggers: [wandb]
+loggers: []
 # Create a json folder as part of the output in the format of marl-eval
 create_json: True
 
 # Absolute path to the folder where the experiment will log.
 # If null, this will default to the hydra output dir (if using hydra) or to the current folder when the script is run (if not).
 save_folder: null
 # Absolute path to a checkpoint file where the experiment was saved. If null the experiment is started fresh.
 restore_file: null
 # Interval for experiment saving in terms of collected frames (this should be a multiple of on/off_policy_collected_frames_per_batch).
 # Set it to 0 to disable checkpointing
-checkpoint_interval: 300_000
+checkpoint_interval: 0
```

### Comparing `benchmarl-1.1.1/benchmarl/conf/task/pettingzoo/multiwalker.yaml` & `benchmarl-1.2.0/benchmarl/conf/task/pettingzoo/multiwalker.yaml`

 * *Files identical despite different names*

### Comparing `benchmarl-1.1.1/benchmarl/conf/task/smacv2/protoss_10_vs_10.yaml` & `benchmarl-1.2.0/benchmarl/conf/task/smacv2/protoss_10_vs_10.yaml`

 * *Files identical despite different names*

### Comparing `benchmarl-1.1.1/benchmarl/conf/task/smacv2/protoss_10_vs_11.yaml` & `benchmarl-1.2.0/benchmarl/conf/task/smacv2/protoss_10_vs_11.yaml`

 * *Files identical despite different names*

### Comparing `benchmarl-1.1.1/benchmarl/conf/task/smacv2/protoss_20_vs_20.yaml` & `benchmarl-1.2.0/benchmarl/conf/task/smacv2/protoss_20_vs_20.yaml`

 * *Files identical despite different names*

### Comparing `benchmarl-1.1.1/benchmarl/conf/task/smacv2/protoss_20_vs_23.yaml` & `benchmarl-1.2.0/benchmarl/conf/task/smacv2/protoss_20_vs_23.yaml`

 * *Files identical despite different names*

### Comparing `benchmarl-1.1.1/benchmarl/conf/task/smacv2/protoss_5_vs_5.yaml` & `benchmarl-1.2.0/benchmarl/conf/task/smacv2/protoss_5_vs_5.yaml`

 * *Files identical despite different names*

### Comparing `benchmarl-1.1.1/benchmarl/conf/task/smacv2/terran_10_vs_10.yaml` & `benchmarl-1.2.0/benchmarl/conf/task/smacv2/terran_10_vs_10.yaml`

 * *Files identical despite different names*

### Comparing `benchmarl-1.1.1/benchmarl/conf/task/smacv2/terran_10_vs_11.yaml` & `benchmarl-1.2.0/benchmarl/conf/task/smacv2/terran_10_vs_11.yaml`

 * *Files identical despite different names*

### Comparing `benchmarl-1.1.1/benchmarl/conf/task/smacv2/terran_20_vs_20.yaml` & `benchmarl-1.2.0/benchmarl/conf/task/smacv2/terran_20_vs_20.yaml`

 * *Files identical despite different names*

### Comparing `benchmarl-1.1.1/benchmarl/conf/task/smacv2/terran_20_vs_23.yaml` & `benchmarl-1.2.0/benchmarl/conf/task/smacv2/terran_20_vs_23.yaml`

 * *Files identical despite different names*

### Comparing `benchmarl-1.1.1/benchmarl/conf/task/smacv2/terran_5_vs_5.yaml` & `benchmarl-1.2.0/benchmarl/conf/task/smacv2/terran_5_vs_5.yaml`

 * *Files identical despite different names*

### Comparing `benchmarl-1.1.1/benchmarl/conf/task/smacv2/zerg_10_vs_10.yaml` & `benchmarl-1.2.0/benchmarl/conf/task/smacv2/zerg_10_vs_10.yaml`

 * *Files identical despite different names*

### Comparing `benchmarl-1.1.1/benchmarl/conf/task/smacv2/zerg_10_vs_11.yaml` & `benchmarl-1.2.0/benchmarl/conf/task/smacv2/zerg_10_vs_11.yaml`

 * *Files identical despite different names*

### Comparing `benchmarl-1.1.1/benchmarl/conf/task/smacv2/zerg_20_vs_20.yaml` & `benchmarl-1.2.0/benchmarl/conf/task/smacv2/zerg_20_vs_20.yaml`

 * *Files identical despite different names*

### Comparing `benchmarl-1.1.1/benchmarl/conf/task/smacv2/zerg_20_vs_23.yaml` & `benchmarl-1.2.0/benchmarl/conf/task/smacv2/zerg_20_vs_23.yaml`

 * *Files identical despite different names*

### Comparing `benchmarl-1.1.1/benchmarl/conf/task/smacv2/zerg_5_vs_5.yaml` & `benchmarl-1.2.0/benchmarl/conf/task/smacv2/zerg_5_vs_5.yaml`

 * *Files identical despite different names*

### Comparing `benchmarl-1.1.1/benchmarl/environments/__init__.py` & `benchmarl-1.2.0/benchmarl/environments/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 #  Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 #  This source code is licensed under the license found in the
 #  LICENSE file in the root directory of this source tree.
 #
 
 from .common import Task
+from .meltingpot.common import MeltingPotTask
 from .pettingzoo.common import PettingZooTask
 from .smacv2.common import Smacv2Task
 from .vmas.common import VmasTask
 
 # This is a registry mapping "envname/task_name" to the EnvNameTask.TASK_NAME enum
 # It is used by automatically load task enums from yaml files
 task_config_registry = {}
-for env in [VmasTask, Smacv2Task, PettingZooTask]:
+for env in [VmasTask, Smacv2Task, PettingZooTask, MeltingPotTask]:
     env_config_registry = {
         f"{env.env_name()}/{task.name.lower()}": task for task in env
     }
     task_config_registry.update(env_config_registry)
 
 
 from .pettingzoo.multiwalker import TaskConfig as MultiwalkerConfig
@@ -27,22 +28,22 @@
 from .pettingzoo.simple_speaker_listener import (
     TaskConfig as SimpleSpeakerListenerConfig,
 )
 from .pettingzoo.simple_spread import TaskConfig as SimpleSpreadConfig
 from .pettingzoo.simple_tag import TaskConfig as SimpleTagConfig
 from .pettingzoo.simple_world_comm import TaskConfig as SimpleWorldComm
 from .pettingzoo.waterworld import TaskConfig as WaterworldConfig
+
 from .vmas.balance import TaskConfig as BalanceConfig
 from .vmas.dispersion import TaskConfig as DispersionConfig
 from .vmas.dropout import TaskConfig as DropoutConfig
 from .vmas.give_way import TaskConfig as GiveWayConfig
 from .vmas.navigation import TaskConfig as NavigationConfig
 from .vmas.reverse_transport import TaskConfig as ReverseTransportConfig
 from .vmas.sampling import TaskConfig as SamplingConfig
-
 from .vmas.simple_adverasary import TaskConfig as VmasSimpleAdversaryConfig
 from .vmas.simple_crypto import TaskConfig as VmasSimpleCryptoConfig
 from .vmas.simple_push import TaskConfig as VmasSimplePushConfig
 from .vmas.simple_reference import TaskConfig as VmasSimpleReferenceConfig
 from .vmas.simple_speaker_listener import TaskConfig as VmasSimpleSpeakerListenerConfig
 from .vmas.simple_spread import TaskConfig as VmasSimpleSpreadConfig
 from .vmas.simple_tag import TaskConfig as VmasSimpleTagConfig
```

### Comparing `benchmarl-1.1.1/benchmarl/environments/common.py` & `benchmarl-1.2.0/benchmarl/environments/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,21 +92,21 @@
         """
         This function is used to obtain a TorchRL object from the enum Task.
 
         Args:
             num_envs (int): The number of envs that should be in the batch_size of the returned env.
                 In vectorized envs, this can be used to set the number of batched environments.
                 If your environment is not vectorized, you can just ignore this, and it will be
-                wrapped in a torchrl.envs.SerialEnv with num_envs automatically.
+                wrapped in a :class:`torchrl.envs.SerialEnv` with num_envs automatically.
             continuous_actions (bool): Whether your environment should have continuous or discrete actions.
                 If your environment does not support both, ignore this and refer to the supports_x_actions methods.
             seed (optional, int): The seed of your env
             device (str): the device of your env, you can pass this to any torchrl env constructor
 
-        Returns: a function that takes no arguments and returns a torchrl.envs.EnvBase object
+        Returns: a function that takes no arguments and returns a :class:`torchrl.envs.EnvBase` object
 
         """
         raise NotImplementedError
 
     def supports_continuous_actions(self) -> bool:
         """
         Return true if your task supports continuous actions.
@@ -152,15 +152,15 @@
 
         """
         raise NotImplementedError
 
     def observation_spec(self, env: EnvBase) -> CompositeSpec:
         """
         A spec for the observation.
-        Must be a CompositeSpec with one (group_name, "observation") entry per group.
+        Must be a CompositeSpec with one (group_name, observation_key) entry per group.
 
         Args:
             env (EnvBase): An environment created via self.get_env_fun
 
         """
         raise NotImplementedError
 
@@ -175,15 +175,15 @@
 
         """
         raise NotImplementedError
 
     def state_spec(self, env: EnvBase) -> Optional[CompositeSpec]:
         """
         A spec for the state.
-        If provided, must be a CompositeSpec with one "state" entry.
+        If provided, must be a CompositeSpec with one entry.
 
         Args:
             env (EnvBase): An environment created via self.get_env_fun
 
         """
         raise NotImplementedError
 
@@ -238,14 +238,36 @@
         """
         if "_reset" in env.reset_keys:
             reset_keys = ["_reset"] * len(self.group_map(env).keys())
         else:
             reset_keys = env.reset_keys
         return RewardSum(reset_keys=reset_keys)
 
+    def get_env_transforms(self, env: EnvBase) -> List[Transform]:
+        """
+        Returns a list of :class:`torchrl.envs.Transform` to be applied to the env.
+
+        Args:
+            env (EnvBase): An environment created via self.get_env_fun
+
+
+        """
+        return []
+
+    def get_replay_buffer_transforms(self, env: EnvBase) -> List[Transform]:
+        """
+        Returns a list of :class:`torchrl.envs.Transform` to be applied to the :class:`torchrl.data.ReplayBuffer`.
+
+        Args:
+            env (EnvBase): An environment created via self.get_env_fun
+
+
+        """
+        return []
+
     @staticmethod
     def render_callback(experiment, env: EnvBase, data: TensorDictBase):
         try:
             return env.render(mode="rgb_array")
         except TypeError:
             return env.render()
```

### Comparing `benchmarl-1.1.1/benchmarl/environments/pettingzoo/common.py` & `benchmarl-1.2.0/benchmarl/environments/pettingzoo/common.py`

 * *Files 12% similar despite different names*

```diff
@@ -118,35 +118,37 @@
                     del group_obs_spec[key]
             if group_obs_spec.is_empty():
                 del observation_spec[group]
         if "state" in observation_spec.keys():
             del observation_spec["state"]
         if observation_spec.is_empty():
             return None
-
         return observation_spec
 
     def observation_spec(self, env: EnvBase) -> CompositeSpec:
         observation_spec = env.observation_spec.clone()
         for group in self.group_map(env):
             group_obs_spec = observation_spec[group]
             for key in list(group_obs_spec.keys()):
                 if key != "observation":
                     del group_obs_spec[key]
-
+        if "state" in observation_spec.keys():
+            del observation_spec["state"]
         return observation_spec
 
     def info_spec(self, env: EnvBase) -> Optional[CompositeSpec]:
         observation_spec = env.observation_spec.clone()
         for group in self.group_map(env):
             group_obs_spec = observation_spec[group]
             for key in list(group_obs_spec.keys()):
                 if key != "info":
                     del group_obs_spec[key]
+        if "state" in observation_spec.keys():
+            del observation_spec["state"]
         return observation_spec
 
     def action_spec(self, env: EnvBase) -> CompositeSpec:
-        return env.input_spec["full_action_spec"]
+        return env.full_action_spec
 
     @staticmethod
     def env_name() -> str:
         return "pettingzoo"
```

### Comparing `benchmarl-1.1.1/benchmarl/environments/pettingzoo/multiwalker.py` & `benchmarl-1.2.0/benchmarl/environments/pettingzoo/multiwalker.py`

 * *Files identical despite different names*

### Comparing `benchmarl-1.1.1/benchmarl/environments/pettingzoo/waterworld.py` & `benchmarl-1.2.0/benchmarl/environments/pettingzoo/waterworld.py`

 * *Files identical despite different names*

### Comparing `benchmarl-1.1.1/benchmarl/environments/smacv2/common.py` & `benchmarl-1.2.0/benchmarl/environments/smacv2/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
     def info_spec(self, env: EnvBase) -> Optional[CompositeSpec]:
         observation_spec = env.observation_spec.clone()
         del observation_spec["state"]
         del observation_spec["agents"]
         return observation_spec
 
     def action_spec(self, env: EnvBase) -> CompositeSpec:
-        return env.input_spec["full_action_spec"]
+        return env.full_action_spec
 
     @staticmethod
     def log_info(batch: TensorDictBase) -> Dict[str, float]:
         done = batch.get(("next", "done")).squeeze(-1)
         return {
             "collection/info/win_rate": batch.get(("next", "info", "battle_won"))[done]
             .to(torch.float)
```

### Comparing `benchmarl-1.1.1/benchmarl/environments/vmas/common.py` & `benchmarl-1.2.0/benchmarl/environments/vmas/common.py`

 * *Files identical despite different names*

### Comparing `benchmarl-1.1.1/benchmarl/environments/vmas/navigation.py` & `benchmarl-1.2.0/benchmarl/environments/vmas/navigation.py`

 * *Files identical despite different names*

### Comparing `benchmarl-1.1.1/benchmarl/environments/vmas/simple_tag.py` & `benchmarl-1.2.0/benchmarl/environments/vmas/simple_tag.py`

 * *Files identical despite different names*

### Comparing `benchmarl-1.1.1/benchmarl/environments/vmas/wind_flocking.py` & `benchmarl-1.2.0/benchmarl/environments/vmas/wind_flocking.py`

 * *Files identical despite different names*

### Comparing `benchmarl-1.1.1/benchmarl/eval_results.py` & `benchmarl-1.2.0/benchmarl/eval_results.py`

 * *Files identical despite different names*

### Comparing `benchmarl-1.1.1/benchmarl/experiment/callback.py` & `benchmarl-1.2.0/benchmarl/experiment/callback.py`

 * *Files identical despite different names*

### Comparing `benchmarl-1.1.1/benchmarl/experiment/experiment.py` & `benchmarl-1.2.0/benchmarl/experiment/experiment.py`

 * *Files 1% similar despite different names*

```diff
@@ -383,42 +383,51 @@
             self.task.get_env_fun(
                 num_envs=self.config.n_envs_per_worker(self.on_policy),
                 continuous_actions=self.continuous_actions,
                 seed=self.seed,
                 device=self.config.sampling_device,
             )
         )
-
         self.observation_spec = self.task.observation_spec(test_env)
         self.info_spec = self.task.info_spec(test_env)
         self.state_spec = self.task.state_spec(test_env)
         self.action_mask_spec = self.task.action_mask_spec(test_env)
         self.action_spec = self.task.action_spec(test_env)
         self.group_map = self.task.group_map(test_env)
         self.train_group_map = copy.deepcopy(self.group_map)
         self.max_steps = self.task.max_steps(test_env)
 
-        transforms = [self.task.get_reward_sum_transform(test_env)]
-        transform = Compose(*transforms)
+        transforms_env = self.task.get_env_transforms(test_env)
+        transforms_training = transforms_env + [
+            self.task.get_reward_sum_transform(test_env)
+        ]
+
+        transforms_env = Compose(*transforms_env)
+        transforms_training = Compose(*transforms_training)
 
         if test_env.batch_size == ():
             self.env_func = lambda: TransformedEnv(
                 SerialEnv(self.config.n_envs_per_worker(self.on_policy), env_func),
-                transform.clone(),
+                transforms_training.clone(),
             )
         else:
-            self.env_func = lambda: TransformedEnv(env_func(), transform.clone())
+            self.env_func = lambda: TransformedEnv(
+                env_func(), transforms_training.clone()
+            )
 
-        self.test_env = test_env.to(self.config.sampling_device)
+        self.test_env = TransformedEnv(test_env, transforms_env.clone()).to(
+            self.config.sampling_device
+        )
 
     def _setup_algorithm(self):
         self.algorithm = self.algorithm_config.get_algorithm(experiment=self)
         self.replay_buffers = {
             group: self.algorithm.get_replay_buffer(
                 group=group,
+                transforms=self.task.get_replay_buffer_transforms(self.test_env),
             )
             for group in self.group_map.keys()
         }
         self.losses = {
             group: self.algorithm.get_loss_and_updater(group)[0]
             for group in self.group_map.keys()
         }
```

### Comparing `benchmarl-1.1.1/benchmarl/experiment/logger.py` & `benchmarl-1.2.0/benchmarl/experiment/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -220,18 +220,19 @@
                 if isinstance(logger, WandbLogger):
                     logger.experiment.save(
                         json_file, base_path=os.path.dirname(json_file)
                     )
 
         self.log(to_log, step=step)
         if video_frames is not None and rollouts[0].batch_size[0] > 1:
+            video_frames = np.stack(
+                video_frames[: rollouts[0].batch_size[0] - 1], axis=0
+            )
             vid = torch.tensor(
-                np.transpose(
-                    video_frames[: rollouts[0].batch_size[0] - 1], (0, 3, 1, 2)
-                ),
+                np.transpose(video_frames, (0, 3, 1, 2)),
                 dtype=torch.uint8,
             ).unsqueeze(0)
             for logger in self.loggers:
                 if isinstance(logger, WandbLogger):
                     logger.log_video("eval/video", vid, fps=20, commit=False)
                 else:
                     logger.log_video("eval_video", vid, step=step)
```

### Comparing `benchmarl-1.1.1/benchmarl/hydra_config.py` & `benchmarl-1.2.0/benchmarl/hydra_config.py`

 * *Files identical despite different names*

### Comparing `benchmarl-1.1.1/benchmarl/models/common.py` & `benchmarl-1.2.0/benchmarl/models/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 
 from abc import ABC, abstractmethod
 from dataclasses import asdict, dataclass
 from typing import Any, Callable, Dict, List, Optional, Sequence
 
 from tensordict import TensorDictBase
 from tensordict.nn import TensorDictModuleBase, TensorDictSequential
-from torchrl.data import CompositeSpec, UnboundedContinuousTensorSpec
+from tensordict.utils import NestedKey
+from torchrl.data import CompositeSpec, TensorSpec, UnboundedContinuousTensorSpec
 from torchrl.envs import EnvBase
 
 from benchmarl.utils import _class_from_name, _read_yaml_config, DEVICE_TYPING
 
 
 def _check_spec(tensordict, spec):
     if not spec.is_in(tensordict):
@@ -99,39 +100,45 @@
         self.device = device
         self.n_agents = n_agents
         self.action_spec = action_spec
 
         self.in_keys = list(self.input_spec.keys(True, True))
         self.out_keys = list(self.output_spec.keys(True, True))
 
-        self.in_key = self.in_keys[0]
         self.out_key = self.out_keys[0]
-        self.input_leaf_spec = self.input_spec[self.in_key]
         self.output_leaf_spec = self.output_spec[self.out_key]
 
         self._perform_checks()
 
     @property
     def output_has_agent_dim(self) -> bool:
         """
         This is a dynamically computed attribute that indicates if the output will have the agent dimension.
         This will be false when ``share_params==True and centralised==True``, and true in all other cases.
         When output_has_agent_dim is true, your model's output should contain the multi-agent dimension,
         and the dimension should be absent otherwise
         """
         return output_has_agent_dim(self.share_params, self.centralised)
 
+    @property
+    def in_key(self) -> NestedKey:
+        if len(self.in_keys) > 1:
+            raise ValueError("Model has more than one input key")
+        return self.in_keys[0]
+
+    @property
+    def input_leaf_spec(self) -> TensorSpec:
+        return self.input_spec[self.in_key]
+
     def _perform_checks(self):
         if not self.input_has_agent_dim and not self.centralised:
             raise ValueError(
                 "If input does not have an agent dimension the model should be marked as centralised"
             )
 
-        if len(self.in_keys) > 1:
-            raise ValueError("Currently models support just one input key")
         if len(self.out_keys) > 1:
             raise ValueError("Currently models support just one output key")
 
         if self.agent_group in self.input_spec.keys() and self.input_spec[
             self.agent_group
         ].shape != (self.n_agents,):
             raise ValueError(
@@ -154,15 +161,15 @@
     # Abstract methods to implement
     ###############################
 
     @abstractmethod
     def _forward(self, tensordict: TensorDictBase) -> TensorDictBase:
         """
         Method to implement for the forward pass of the model.
-        It should read self.in_key, process it and write self.out_key.
+        It should read self.in_keys, process it and write self.out_key.
 
         Args:
             tensordict (TensorDictBase): the input td
 
         Returns: the input td with the written self.out_key
 
         """
```

### Comparing `benchmarl-1.1.1/benchmarl/models/gnn.py` & `benchmarl-1.2.0/benchmarl/models/gnn.py`

 * *Files 11% similar despite different names*

```diff
@@ -100,15 +100,17 @@
         **kwargs,
     ):
         self.topology = topology
         self.self_loops = self_loops
 
         super().__init__(**kwargs)
 
-        self.input_features = self.input_leaf_spec.shape[-1]
+        self.input_features = sum(
+            [spec.shape[-1] for spec in self.input_spec.values(True, True)]
+        )
         self.output_features = self.output_leaf_spec.shape[-1]
 
         if gnn_kwargs is None:
             gnn_kwargs = {}
         gnn_kwargs.update(
             {"in_channels": self.input_features, "out_channels": self.output_features}
         )
@@ -138,43 +140,60 @@
         if not self.input_has_agent_dim:
             raise ValueError(
                 "The GNN module is not compatible with input that does not have the agent dimension,"
                 "such as the global state in centralised critics. Please choose another critic model"
                 "if your algorithm has a centralized critic and the task has a global state."
             )
 
-        if self.input_leaf_spec.shape[-2] != self.n_agents:
+        input_shape = None
+        for input_key, input_spec in self.input_spec.items(True, True):
+            if (self.input_has_agent_dim and len(input_spec.shape) == 2) or (
+                not self.input_has_agent_dim and len(input_spec.shape) == 1
+            ):
+                if input_shape is None:
+                    input_shape = input_spec.shape[:-1]
+                else:
+                    if input_spec.shape[:-1] != input_shape:
+                        raise ValueError(
+                            f"GNN inputs should all have the same shape up to the last dimension, got {self.input_spec}"
+                        )
+            else:
+                raise ValueError(
+                    f"GNN input value {input_key} from {self.input_spec} has an invalid shape"
+                )
+
+        if input_shape[-1] != self.n_agents:
             raise ValueError(
-                "The second to last input spec dimension should be the number of agents"
+                f"The second to last input spec dimension should be the number of agents, got {self.input_spec}"
             )
         if (
             self.output_has_agent_dim
             and self.output_leaf_spec.shape[-2] != self.n_agents
         ):
             raise ValueError(
                 "If the GNN output has the agent dimension,"
                 " the second to last spec dimension should be the number of agents"
             )
 
     def _forward(self, tensordict: TensorDictBase) -> TensorDictBase:
         # Gather in_key
-        input = tensordict.get(self.in_key)
+        input = torch.cat([tensordict.get(in_key) for in_key in self.in_keys], dim=-1)
 
         batch_size = input.shape[:-2]
 
         graph = batch_from_dense_to_ptg(x=input, edge_index=self.edge_index)
 
         if not self.share_params:
             res = torch.stack(
                 [
                     gnn(graph.x, graph.edge_index).view(
                         *batch_size,
                         self.n_agents,
                         self.output_features,
-                    )[:, i]
+                    )[..., i, :]
                     for i, gnn in enumerate(self.gnns)
                 ],
                 dim=-2,
             )
 
         else:
             res = self.gnns[0](
```

### Comparing `benchmarl-1.1.1/benchmarl/models/mlp.py` & `benchmarl-1.2.0/benchmarl/models/mlp.py`

 * *Files 26% similar despite different names*

```diff
@@ -44,15 +44,17 @@
             n_agents=kwargs.pop("n_agents"),
             centralised=kwargs.pop("centralised"),
             share_params=kwargs.pop("share_params"),
             device=kwargs.pop("device"),
             action_spec=kwargs.pop("action_spec"),
         )
 
-        self.input_features = self.input_leaf_spec.shape[-1]
+        self.input_features = sum(
+            [spec.shape[-1] for spec in self.input_spec.values(True, True)]
+        )
         self.output_features = self.output_leaf_spec.shape[-1]
 
         if self.input_has_agent_dim:
             self.mlp = MultiAgentMLP(
                 n_agent_inputs=self.input_features,
                 n_agent_outputs=self.output_features,
                 n_agents=self.n_agents,
@@ -73,31 +75,48 @@
                     for _ in range(self.n_agents if not self.share_params else 1)
                 ]
             )
 
     def _perform_checks(self):
         super()._perform_checks()
 
-        if self.input_has_agent_dim and self.input_leaf_spec.shape[-2] != self.n_agents:
-            raise ValueError(
-                "If the MLP input has the agent dimension,"
-                " the second to last spec dimension should be the number of agents"
-            )
+        input_shape = None
+        for input_key, input_spec in self.input_spec.items(True, True):
+            if (self.input_has_agent_dim and len(input_spec.shape) == 2) or (
+                not self.input_has_agent_dim and len(input_spec.shape) == 1
+            ):
+                if input_shape is None:
+                    input_shape = input_spec.shape[:-1]
+                else:
+                    if input_spec.shape[:-1] != input_shape:
+                        raise ValueError(
+                            f"MLP inputs should all have the same shape up to the last dimension, got {self.input_spec}"
+                        )
+            else:
+                raise ValueError(
+                    f"MLP input value {input_key} from {self.input_spec} has an invalid shape, maybe you need a CNN?"
+                )
+        if self.input_has_agent_dim:
+            if input_shape[-1] != self.n_agents:
+                raise ValueError(
+                    "If the MLP input has the agent dimension,"
+                    " the second to last spec dimension should be the number of agents, got {self.input_spec}"
+                )
         if (
             self.output_has_agent_dim
             and self.output_leaf_spec.shape[-2] != self.n_agents
         ):
             raise ValueError(
                 "If the MLP output has the agent dimension,"
                 " the second to last spec dimension should be the number of agents"
             )
 
     def _forward(self, tensordict: TensorDictBase) -> TensorDictBase:
         # Gather in_key
-        input = tensordict.get(self.in_key)
+        input = torch.cat([tensordict.get(in_key) for in_key in self.in_keys], dim=-1)
 
         # Has multi-agent input dimension
         if self.input_has_agent_dim:
             res = self.mlp.forward(input)
             if not self.output_has_agent_dim:
                 # If we are here the module is centralised and parameter shared.
                 # Thus the multi-agent dimension has been expanded,
```

### Comparing `benchmarl-1.1.1/benchmarl/run.py` & `benchmarl-1.2.0/benchmarl/run.py`

 * *Files identical despite different names*

### Comparing `benchmarl-1.1.1/benchmarl/utils.py` & `benchmarl-1.2.0/benchmarl/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 DEVICE_TYPING = Union[torch.device, str, int]
 
 
 def _read_yaml_config(config_file: str) -> Dict[str, Any]:
     with open(config_file) as config:
         yaml_string = config.read()
     config_dict = yaml.safe_load(yaml_string)
+    if config_dict is None:
+        config_dict = {}
     if "defaults" in config_dict.keys():
         del config_dict["defaults"]
     return config_dict
 
 
 def _class_from_name(name: str):
     name_split = name.split(".")
```

### Comparing `benchmarl-1.1.1/setup.py` & `benchmarl-1.2.0/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,44 +1,60 @@
 #  Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 #  This source code is licensed under the license found in the
 #  LICENSE file in the root directory of this source tree.
 #
 import os
+import pathlib
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 
 def package_files(directory):
     paths = []
     for path, _, filenames in os.walk(directory):
         for filename in filenames:
             paths.append(os.path.join("..", path, filename))
     return paths
 
 
+def get_version():
+    """Gets the benchmarl version."""
+    path = CWD / "benchmarl" / "__init__.py"
+    content = path.read_text()
+
+    for line in content.splitlines():
+        if line.startswith("__version__"):
+            return line.strip().split()[-1].strip().strip('"')
+    raise RuntimeError("bad version data in __init__.py")
+
+
+CWD = pathlib.Path(__file__).absolute().parent
+
 extra_files = package_files(
     str(
         Path(os.path.dirname(os.path.realpath(__file__)))
         / Path("benchmarl")
         / Path("conf")
     )
 )
 
 setup(
     name="benchmarl",
-    version="1.1.1",
+    version=get_version(),
     description="BenchMARL",
     url="https://github.com/facebookresearch/BenchMARL",
     author="Matteo Bettini",
     author_email="mb2389@cl.cam.ac.uk",
-    install_requires=["torchrl==0.3.1", "tqdm", "hydra-core"],
+    install_requires=["torchrl==0.4.0", "tqdm", "hydra-core"],
     extras_require={
         "vmas": ["vmas>=1.3.4"],
         "pettingzoo": ["pettingzoo[all]>=1.24.3"],
+        "meltingpot": ["dm-meltingpot"],
         "gnn": ["torch_geometric"],
+        "logging": ["moviepy", "wandb", "torchvision"],
     },
     packages=find_packages(),
     include_package_data=True,
     package_data={"": extra_files},
 )
```

### Comparing `benchmarl-1.1.1/test/test_algorithm.py` & `benchmarl-1.2.0/test/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `benchmarl-1.1.1/test/test_pettingzoo.py` & `benchmarl-1.2.0/test/test_pettingzoo.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from benchmarl.algorithms import (
     algorithm_config_registry,
     IppoConfig,
     IsacConfig,
     MaddpgConfig,
     MasacConfig,
     QmixConfig,
-    VdnConfig,
 )
 from benchmarl.algorithms.common import AlgorithmConfig
 from benchmarl.environments import PettingZooTask, Task
 from benchmarl.experiment import Experiment
 
 from utils import _has_pettingzoo
 from utils_experiment import ExperimentUtils
@@ -114,17 +113,15 @@
         task: Task,
         experiment_config,
         mlp_sequence_config,
         prefer_continuous,
     ):
         experiment_config.prefer_continuous_actions = prefer_continuous
         algo_config = algo_config.get_from_yaml()
-        if isinstance(algo_config, VdnConfig):
-            # There are some bugs currently in TorchRL https://github.com/pytorch/rl/issues/1593
-            pytest.skip()
+
         ExperimentUtils.check_experiment_loading(
             algo_config=algo_config,
             model_config=mlp_sequence_config,
             experiment_config=experiment_config,
             task=task.get_from_yaml(),
         )
```

### Comparing `benchmarl-1.1.1/test/test_smacv2.py` & `benchmarl-1.2.0/test/test_smacv2.py`

 * *Files identical despite different names*

### Comparing `benchmarl-1.1.1/test/test_task.py` & `benchmarl-1.2.0/test/test_task.py`

 * *Files identical despite different names*

### Comparing `benchmarl-1.1.1/test/test_vmas.py` & `benchmarl-1.2.0/test/test_vmas.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,14 @@
     algorithm_config_registry,
     IddpgConfig,
     IppoConfig,
     IsacConfig,
     MaddpgConfig,
     MasacConfig,
     QmixConfig,
-    VdnConfig,
 )
 from benchmarl.algorithms.common import AlgorithmConfig
 from benchmarl.environments import Task, VmasTask
 from benchmarl.experiment import Experiment
 from benchmarl.models import MlpConfig
 from torch import nn
 from utils import _has_vmas
@@ -103,17 +102,15 @@
         self,
         algo_config,
         task: Task,
         experiment_config,
         mlp_sequence_config,
     ):
         algo_config = algo_config.get_from_yaml()
-        if isinstance(algo_config, VdnConfig):
-            # There are some bugs currently in TorchRL https://github.com/pytorch/rl/issues/1593
-            pytest.skip()
+
         ExperimentUtils.check_experiment_loading(
             algo_config=algo_config,
             model_config=mlp_sequence_config,
             experiment_config=experiment_config,
             task=task.get_from_yaml(),
         )
```

