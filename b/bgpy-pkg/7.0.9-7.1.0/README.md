# Comparing `tmp/bgpy_pkg-7.0.9.tar.gz` & `tmp/bgpy_pkg-7.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bgpy_pkg-7.0.9.tar", last modified: Thu Apr 18 09:10:30 2024, max compression
+gzip compressed data, was "bgpy_pkg-7.1.0.tar", last modified: Fri Apr 26 07:22:33 2024, max compression
```

## Comparing `bgpy_pkg-7.0.9.tar` & `bgpy_pkg-7.1.0.tar`

### file list

```diff
@@ -1,199 +1,203 @@
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.414698 bgpy_pkg-7.0.9/
--rwxrwxr-x   0 anon      (1000) anon      (1000)     1460 2024-01-30 07:34:53.000000 bgpy_pkg-7.0.9/LICENSE.txt
--rw-rw-r--   0 anon      (1000) anon      (1000)       76 2024-01-30 07:34:53.000000 bgpy_pkg-7.0.9/MANIFEST.in
--rw-r--r--   0 anon      (1000) anon      (1000)     4622 2024-04-18 09:10:30.414698 bgpy_pkg-7.0.9/PKG-INFO
--rw-rw-r--   0 anon      (1000) anon      (1000)     1342 2024-01-31 07:10:08.000000 bgpy_pkg-7.0.9/README.md
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.394698 bgpy_pkg-7.0.9/bgpy/
--rw-rw-r--   0 anon      (1000) anon      (1000)      275 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/__init__.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      874 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/__main__.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.394698 bgpy_pkg-7.0.9/bgpy/as_graphs/
--rw-rw-r--   0 anon      (1000) anon      (1000)      513 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/as_graphs/__init__.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.394698 bgpy_pkg-7.0.9/bgpy/as_graphs/base/
--rw-rw-r--   0 anon      (1000) anon      (1000)      396 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/as_graphs/base/__init__.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.398698 bgpy_pkg-7.0.9/bgpy/as_graphs/base/as_graph/
--rw-rw-r--   0 anon      (1000) anon      (1000)       83 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/as_graphs/base/as_graph/__init__.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     9806 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/as_graphs/base/as_graph/as_graph.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     6062 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/as_graphs/base/as_graph/base_as.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     2444 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/as_graphs/base/as_graph/customer_cone_funcs.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     3185 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/as_graphs/base/as_graph/graph_building_funcs.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1228 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/as_graphs/base/as_graph/propagation_rank_funcs.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1821 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/as_graphs/base/as_graph_collector.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     3769 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/as_graphs/base/as_graph_constructor.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1562 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/as_graphs/base/as_graph_info.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.398698 bgpy_pkg-7.0.9/bgpy/as_graphs/base/links/
--rw-rw-r--   0 anon      (1000) anon      (1000)      168 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/as_graphs/base/links/__init__.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1149 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/as_graphs/base/links/customer_provider_link.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      911 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/as_graphs/base/links/link.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      687 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/as_graphs/base/links/peer_link.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.398698 bgpy_pkg-7.0.9/bgpy/as_graphs/caida_as_graph/
--rw-rw-r--   0 anon      (1000) anon      (1000)      260 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/as_graphs/caida_as_graph/__init__.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      239 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/as_graphs/caida_as_graph/caida_as_graph.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     3848 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/as_graphs/caida_as_graph/caida_as_graph_collector.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     4649 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/as_graphs/caida_as_graph/caida_as_graph_constructor.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     2811 2024-04-15 22:21:08.000000 bgpy_pkg-7.0.9/bgpy/enums.py
--rw-rw-r--   0 anon      (1000) anon      (1000)        0 2024-01-30 07:34:53.000000 bgpy_pkg-7.0.9/bgpy/py.typed
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.398698 bgpy_pkg-7.0.9/bgpy/simulation_engine/
--rw-rw-r--   0 anon      (1000) anon      (1000)     2311 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/__init__.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.398698 bgpy_pkg-7.0.9/bgpy/simulation_engine/ann_containers/
--rw-rw-r--   0 anon      (1000) anon      (1000)      302 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/ann_containers/__init__.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1717 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/ann_containers/ann_container.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      370 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/ann_containers/local_rib.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      975 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/ann_containers/recv_queue.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     2421 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/ann_containers/ribs_in.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1047 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/ann_containers/ribs_out.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     2894 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/ann_containers/send_queue.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     5311 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/announcement.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.398698 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/
--rw-rw-r--   0 anon      (1000) anon      (1000)      590 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/__init__.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.398698 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/aspa/
--rw-rw-r--   0 anon      (1000) anon      (1000)       98 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/aspa/__init__.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     5142 2024-04-18 08:26:10.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/aspa/aspa.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      226 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/aspa/aspa_full.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.398698 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/bgp/
--rw-rw-r--   0 anon      (1000) anon      (1000)       81 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/bgp/__init__.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.398698 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/bgp/bgp/
--rw-rw-r--   0 anon      (1000) anon      (1000)       40 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/bgp/bgp/__init__.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     3417 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/bgp/bgp/bgp.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     2768 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/bgp/bgp/gao_rexford.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     3348 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/bgp/bgp/process_incoming_funcs.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     3446 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/bgp/bgp/propagate_funcs.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.398698 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/bgp/bgp_full/
--rw-rw-r--   0 anon      (1000) anon      (1000)       53 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/bgp/bgp_full/__init__.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     2918 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/bgp/bgp_full/bgp_full.py
--rw-rw-r--   0 anon      (1000) anon      (1000)    10946 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/bgp/bgp_full/process_incoming_funcs.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1796 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/bgp/bgp_full/propagate_funcs.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.402698 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/bgpsec/
--rw-rw-r--   0 anon      (1000) anon      (1000)      110 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/bgpsec/__init__.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     4350 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/bgpsec/bgpsec.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      224 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/bgpsec/bgpsec_full.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.402698 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/only_to_customers/
--rw-rw-r--   0 anon      (1000) anon      (1000)      168 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/only_to_customers/__init__.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1532 2024-03-28 08:04:49.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/only_to_customers/only_to_customers.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      294 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/only_to_customers/only_to_customers_full.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.402698 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/pathend/
--rw-rw-r--   0 anon      (1000) anon      (1000)      116 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/pathend/__init__.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1129 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/pathend/pathend.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      244 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/pathend/pathend_full.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     2926 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/policy.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.402698 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/rov/
--rw-rw-r--   0 anon      (1000) anon      (1000)      195 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/rov/__init__.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1110 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/rov/peer_rov.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      219 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/rov/peer_rov_full.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      885 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/rov/rov.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      220 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/rov/rov_full.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.402698 bgpy_pkg-7.0.9/bgpy/simulation_engine/simulation_engines/
--rw-rw-r--   0 anon      (1000) anon      (1000)      161 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/simulation_engines/__init__.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     3582 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/simulation_engines/base_simulation_engine.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     7142 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/simulation_engines/simulation_engine.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.402698 bgpy_pkg-7.0.9/bgpy/simulation_framework/
--rw-rw-r--   0 anon      (1000) anon      (1000)     1115 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_framework/__init__.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.402698 bgpy_pkg-7.0.9/bgpy/simulation_framework/as_graph_analyzers/
--rw-rw-r--   0 anon      (1000) anon      (1000)      157 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/simulation_framework/as_graph_analyzers/__init__.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     6521 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/simulation_framework/as_graph_analyzers/as_graph_analyzer.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      748 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/simulation_framework/as_graph_analyzers/base_as_graph_analyzer.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     9418 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/simulation_framework/graph_factory.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.402698 bgpy_pkg-7.0.9/bgpy/simulation_framework/metric_tracker/
--rw-rw-r--   0 anon      (1000) anon      (1000)      149 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/simulation_framework/metric_tracker/__init__.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      461 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/simulation_framework/metric_tracker/data_key.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     4556 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/simulation_framework/metric_tracker/metric.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      367 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/simulation_framework/metric_tracker/metric_key.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     9936 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/simulation_framework/metric_tracker/metric_tracker.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.402698 bgpy_pkg-7.0.9/bgpy/simulation_framework/scenarios/
--rw-rw-r--   0 anon      (1000) anon      (1000)      899 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_framework/scenarios/__init__.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.406698 bgpy_pkg-7.0.9/bgpy/simulation_framework/scenarios/custom_scenarios/
--rw-rw-r--   0 anon      (1000) anon      (1000)      693 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/simulation_framework/scenarios/custom_scenarios/__init__.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     6968 2024-03-28 08:32:38.000000 bgpy_pkg-7.0.9/bgpy/simulation_framework/scenarios/custom_scenarios/accidental_route_leak.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1418 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_framework/scenarios/custom_scenarios/non_routed_prefix_hijack.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1636 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_framework/scenarios/custom_scenarios/non_routed_superprefix_hijack.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1945 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_framework/scenarios/custom_scenarios/non_routed_superprefix_prefix_hijack.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     2044 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_framework/scenarios/custom_scenarios/prefix_hijack.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     2058 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_framework/scenarios/custom_scenarios/subprefix_hijack.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     2381 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_framework/scenarios/custom_scenarios/superprefix_prefix_hijack.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1766 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_framework/scenarios/custom_scenarios/valid_prefix.py
--rw-rw-r--   0 anon      (1000) anon      (1000)    16728 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_framework/scenarios/preprocess_anns_funcs.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      462 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_framework/scenarios/roa_info.py
--rw-rw-r--   0 anon      (1000) anon      (1000)    23095 2024-04-04 07:57:43.000000 bgpy_pkg-7.0.9/bgpy/simulation_framework/scenarios/scenario.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     6663 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_framework/scenarios/scenario_config.py
--rw-rw-r--   0 anon      (1000) anon      (1000)    15693 2024-04-08 14:47:25.000000 bgpy_pkg-7.0.9/bgpy/simulation_framework/simulation.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1576 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/simulation_framework/utils.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.406698 bgpy_pkg-7.0.9/bgpy/tests/
--rw-rw-r--   0 anon      (1000) anon      (1000)      228 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/tests/__init__.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     2412 2024-03-13 03:26:50.000000 bgpy_pkg-7.0.9/bgpy/tests/conftest.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.406698 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/
--rw-rw-r--   0 anon      (1000) anon      (1000)      175 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/__init__.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.406698 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/
--rw-rw-r--   0 anon      (1000) anon      (1000)      180 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/__init__.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.406698 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/
--rw-rw-r--   0 anon      (1000) anon      (1000)     1855 2024-04-18 08:52:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/__init__.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1529 2024-04-18 08:48:15.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/as_graph_info_000.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      734 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_000.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      759 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_001.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1338 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_002.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      765 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_003.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      788 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_004.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      790 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_005.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      806 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_006.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      808 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_007.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      813 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_008.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      834 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_009.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      862 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_010.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      824 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_011.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      935 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_012.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      960 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_013.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1126 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_014.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1114 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_015.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1112 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_016.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1147 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_017.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1110 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_018.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1137 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_019.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1144 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_020.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      972 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_021.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      979 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_022.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1136 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_023.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1154 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_024.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1167 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_025.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1305 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_026.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1338 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_027.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1349 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_028.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1514 2024-04-18 08:54:44.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_029.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.410698 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/internals/
--rw-rw-r--   0 anon      (1000) anon      (1000)      368 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/internals/__init__.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     2206 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/internals/internal_config_000.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     2338 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/internals/internal_config_001.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     2792 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/internals/internal_config_002.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1211 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/internals/internal_config_003.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1950 2024-04-18 06:19:14.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/internals/internal_config_004.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      780 2024-04-18 07:44:17.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/test_engine.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.410698 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/utils/
--rw-rw-r--   0 anon      (1000) anon      (1000)      285 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/utils/__init__.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1757 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/utils/diagram_aggregator.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      566 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/utils/engine_test_config.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     9473 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/utils/engine_tester.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.410698 bgpy_pkg-7.0.9/bgpy/tests/framework_tests/
--rw-rw-r--   0 anon      (1000) anon      (1000)        0 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/tests/framework_tests/__init__.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.410698 bgpy_pkg-7.0.9/bgpy/tests/framework_tests/system_tests/
--rw-rw-r--   0 anon      (1000) anon      (1000)       76 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/tests/framework_tests/system_tests/__init__.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      896 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/framework_tests/system_tests/test_sim_inputs.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.410698 bgpy_pkg-7.0.9/bgpy/tests/framework_tests/unit_tests/
--rw-rw-r--   0 anon      (1000) anon      (1000)        0 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/tests/framework_tests/unit_tests/__init__.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      478 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/tests/framework_tests/unit_tests/conftest.py
--rw-rw-r--   0 anon      (1000) anon      (1000)    15144 2024-03-13 03:26:50.000000 bgpy_pkg-7.0.9/bgpy/tests/framework_tests/unit_tests/test_scenario.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.410698 bgpy_pkg-7.0.9/bgpy/utils/
--rw-rw-r--   0 anon      (1000) anon      (1000)      279 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/utils/__init__.py
--rw-rw-r--   0 anon      (1000) anon      (1000)    11631 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/utils/diagram.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1038 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/utils/engine_run_config.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     8230 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/utils/engine_runner.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.410698 bgpy_pkg-7.0.9/bgpy/utils/simulator_codec/
--rw-rw-r--   0 anon      (1000) anon      (1000)       74 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/utils/simulator_codec/__init__.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     2834 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/utils/simulator_codec/simulator_codec.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      322 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/utils/simulator_codec/simulator_loader.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.410698 bgpy_pkg-7.0.9/bgpy_pkg.egg-info/
--rw-r--r--   0 anon      (1000) anon      (1000)     4622 2024-04-18 09:10:30.000000 bgpy_pkg-7.0.9/bgpy_pkg.egg-info/PKG-INFO
--rw-rw-r--   0 anon      (1000) anon      (1000)     8523 2024-04-18 09:10:30.000000 bgpy_pkg-7.0.9/bgpy_pkg.egg-info/SOURCES.txt
--rw-rw-r--   0 anon      (1000) anon      (1000)        1 2024-04-18 09:10:30.000000 bgpy_pkg-7.0.9/bgpy_pkg.egg-info/dependency_links.txt
--rw-rw-r--   0 anon      (1000) anon      (1000)       44 2024-04-18 09:10:30.000000 bgpy_pkg-7.0.9/bgpy_pkg.egg-info/entry_points.txt
--rw-rw-r--   0 anon      (1000) anon      (1000)      370 2024-04-18 09:10:30.000000 bgpy_pkg-7.0.9/bgpy_pkg.egg-info/requires.txt
--rw-rw-r--   0 anon      (1000) anon      (1000)        5 2024-04-18 09:10:30.000000 bgpy_pkg-7.0.9/bgpy_pkg.egg-info/top_level.txt
--rw-rw-r--   0 anon      (1000) anon      (1000)     3465 2024-04-18 09:10:06.000000 bgpy_pkg-7.0.9/pyproject.toml
--rwxrwxr-x   0 anon      (1000) anon      (1000)       69 2024-04-18 09:10:30.414698 bgpy_pkg-7.0.9/setup.cfg
--rw-rw-r--   0 anon      (1000) anon      (1000)     1157 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/tox.ini
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-26 07:22:33.515713 bgpy_pkg-7.1.0/
+-rwxrwxr-x   0 anon      (1000) anon      (1000)     1460 2024-01-30 07:34:53.000000 bgpy_pkg-7.1.0/LICENSE.txt
+-rw-rw-r--   0 anon      (1000) anon      (1000)       76 2024-01-30 07:34:53.000000 bgpy_pkg-7.1.0/MANIFEST.in
+-rw-r--r--   0 anon      (1000) anon      (1000)     4622 2024-04-26 07:22:33.515713 bgpy_pkg-7.1.0/PKG-INFO
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1342 2024-01-31 07:10:08.000000 bgpy_pkg-7.1.0/README.md
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-26 07:22:33.499713 bgpy_pkg-7.1.0/bgpy/
+-rw-rw-r--   0 anon      (1000) anon      (1000)      275 2024-02-23 22:41:12.000000 bgpy_pkg-7.1.0/bgpy/__init__.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      874 2024-04-26 04:42:33.000000 bgpy_pkg-7.1.0/bgpy/__main__.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-26 07:22:33.499713 bgpy_pkg-7.1.0/bgpy/as_graphs/
+-rw-rw-r--   0 anon      (1000) anon      (1000)      513 2024-02-23 22:41:12.000000 bgpy_pkg-7.1.0/bgpy/as_graphs/__init__.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-26 07:22:33.499713 bgpy_pkg-7.1.0/bgpy/as_graphs/base/
+-rw-rw-r--   0 anon      (1000) anon      (1000)      396 2024-02-23 22:41:12.000000 bgpy_pkg-7.1.0/bgpy/as_graphs/base/__init__.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-26 07:22:33.499713 bgpy_pkg-7.1.0/bgpy/as_graphs/base/as_graph/
+-rw-rw-r--   0 anon      (1000) anon      (1000)       83 2024-02-23 22:41:12.000000 bgpy_pkg-7.1.0/bgpy/as_graphs/base/as_graph/__init__.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     9806 2024-04-26 04:42:33.000000 bgpy_pkg-7.1.0/bgpy/as_graphs/base/as_graph/as_graph.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     6062 2024-04-26 04:42:33.000000 bgpy_pkg-7.1.0/bgpy/as_graphs/base/as_graph/base_as.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     2444 2024-04-26 04:42:33.000000 bgpy_pkg-7.1.0/bgpy/as_graphs/base/as_graph/customer_cone_funcs.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     3185 2024-02-23 22:41:12.000000 bgpy_pkg-7.1.0/bgpy/as_graphs/base/as_graph/graph_building_funcs.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1228 2024-02-23 22:41:12.000000 bgpy_pkg-7.1.0/bgpy/as_graphs/base/as_graph/propagation_rank_funcs.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1821 2024-02-23 22:41:12.000000 bgpy_pkg-7.1.0/bgpy/as_graphs/base/as_graph_collector.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     3769 2024-02-23 22:41:12.000000 bgpy_pkg-7.1.0/bgpy/as_graphs/base/as_graph_constructor.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1562 2024-02-23 22:41:12.000000 bgpy_pkg-7.1.0/bgpy/as_graphs/base/as_graph_info.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-26 07:22:33.499713 bgpy_pkg-7.1.0/bgpy/as_graphs/base/links/
+-rw-rw-r--   0 anon      (1000) anon      (1000)      168 2024-02-23 22:41:12.000000 bgpy_pkg-7.1.0/bgpy/as_graphs/base/links/__init__.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1149 2024-02-23 22:41:12.000000 bgpy_pkg-7.1.0/bgpy/as_graphs/base/links/customer_provider_link.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      911 2024-02-23 22:41:12.000000 bgpy_pkg-7.1.0/bgpy/as_graphs/base/links/link.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      687 2024-02-23 22:41:12.000000 bgpy_pkg-7.1.0/bgpy/as_graphs/base/links/peer_link.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-26 07:22:33.499713 bgpy_pkg-7.1.0/bgpy/as_graphs/caida_as_graph/
+-rw-rw-r--   0 anon      (1000) anon      (1000)      260 2024-02-23 22:41:12.000000 bgpy_pkg-7.1.0/bgpy/as_graphs/caida_as_graph/__init__.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      239 2024-02-23 22:41:12.000000 bgpy_pkg-7.1.0/bgpy/as_graphs/caida_as_graph/caida_as_graph.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     3848 2024-02-23 22:41:12.000000 bgpy_pkg-7.1.0/bgpy/as_graphs/caida_as_graph/caida_as_graph_collector.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     4649 2024-02-23 22:41:12.000000 bgpy_pkg-7.1.0/bgpy/as_graphs/caida_as_graph/caida_as_graph_constructor.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     2811 2024-04-15 22:21:08.000000 bgpy_pkg-7.1.0/bgpy/enums.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)        0 2024-01-30 07:34:53.000000 bgpy_pkg-7.1.0/bgpy/py.typed
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-26 07:22:33.499713 bgpy_pkg-7.1.0/bgpy/simulation_engine/
+-rw-rw-r--   0 anon      (1000) anon      (1000)     2409 2024-04-26 07:06:11.000000 bgpy_pkg-7.1.0/bgpy/simulation_engine/__init__.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-26 07:22:33.503713 bgpy_pkg-7.1.0/bgpy/simulation_engine/ann_containers/
+-rw-rw-r--   0 anon      (1000) anon      (1000)      302 2024-02-23 22:41:12.000000 bgpy_pkg-7.1.0/bgpy/simulation_engine/ann_containers/__init__.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1717 2024-02-23 22:41:12.000000 bgpy_pkg-7.1.0/bgpy/simulation_engine/ann_containers/ann_container.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      370 2024-02-23 22:41:12.000000 bgpy_pkg-7.1.0/bgpy/simulation_engine/ann_containers/local_rib.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      975 2024-02-23 22:41:12.000000 bgpy_pkg-7.1.0/bgpy/simulation_engine/ann_containers/recv_queue.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     2421 2024-02-23 22:41:12.000000 bgpy_pkg-7.1.0/bgpy/simulation_engine/ann_containers/ribs_in.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1047 2024-02-23 22:41:12.000000 bgpy_pkg-7.1.0/bgpy/simulation_engine/ann_containers/ribs_out.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     2894 2024-02-23 22:41:12.000000 bgpy_pkg-7.1.0/bgpy/simulation_engine/ann_containers/send_queue.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     5311 2024-02-24 05:53:40.000000 bgpy_pkg-7.1.0/bgpy/simulation_engine/announcement.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-26 07:22:33.503713 bgpy_pkg-7.1.0/bgpy/simulation_engine/policies/
+-rw-rw-r--   0 anon      (1000) anon      (1000)      667 2024-04-26 07:06:11.000000 bgpy_pkg-7.1.0/bgpy/simulation_engine/policies/__init__.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-26 07:22:33.503713 bgpy_pkg-7.1.0/bgpy/simulation_engine/policies/aspa/
+-rw-rw-r--   0 anon      (1000) anon      (1000)       98 2024-02-24 05:53:40.000000 bgpy_pkg-7.1.0/bgpy/simulation_engine/policies/aspa/__init__.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     5142 2024-04-18 08:26:10.000000 bgpy_pkg-7.1.0/bgpy/simulation_engine/policies/aspa/aspa.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      226 2024-02-24 05:53:40.000000 bgpy_pkg-7.1.0/bgpy/simulation_engine/policies/aspa/aspa_full.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-26 07:22:33.503713 bgpy_pkg-7.1.0/bgpy/simulation_engine/policies/bgp/
+-rw-rw-r--   0 anon      (1000) anon      (1000)       81 2024-02-24 05:53:40.000000 bgpy_pkg-7.1.0/bgpy/simulation_engine/policies/bgp/__init__.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-26 07:22:33.503713 bgpy_pkg-7.1.0/bgpy/simulation_engine/policies/bgp/bgp/
+-rw-rw-r--   0 anon      (1000) anon      (1000)       40 2024-02-24 05:53:40.000000 bgpy_pkg-7.1.0/bgpy/simulation_engine/policies/bgp/bgp/__init__.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     3417 2024-02-24 05:53:40.000000 bgpy_pkg-7.1.0/bgpy/simulation_engine/policies/bgp/bgp/bgp.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     2768 2024-02-24 05:53:40.000000 bgpy_pkg-7.1.0/bgpy/simulation_engine/policies/bgp/bgp/gao_rexford.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     3348 2024-02-24 05:53:40.000000 bgpy_pkg-7.1.0/bgpy/simulation_engine/policies/bgp/bgp/process_incoming_funcs.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     3446 2024-04-26 06:41:47.000000 bgpy_pkg-7.1.0/bgpy/simulation_engine/policies/bgp/bgp/propagate_funcs.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-26 07:22:33.503713 bgpy_pkg-7.1.0/bgpy/simulation_engine/policies/bgp/bgp_full/
+-rw-rw-r--   0 anon      (1000) anon      (1000)       53 2024-02-24 05:53:40.000000 bgpy_pkg-7.1.0/bgpy/simulation_engine/policies/bgp/bgp_full/__init__.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     2918 2024-02-24 05:53:40.000000 bgpy_pkg-7.1.0/bgpy/simulation_engine/policies/bgp/bgp_full/bgp_full.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)    10946 2024-02-24 05:53:40.000000 bgpy_pkg-7.1.0/bgpy/simulation_engine/policies/bgp/bgp_full/process_incoming_funcs.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1796 2024-02-24 05:53:40.000000 bgpy_pkg-7.1.0/bgpy/simulation_engine/policies/bgp/bgp_full/propagate_funcs.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-26 07:22:33.503713 bgpy_pkg-7.1.0/bgpy/simulation_engine/policies/bgpsec/
+-rw-rw-r--   0 anon      (1000) anon      (1000)      110 2024-02-24 05:53:40.000000 bgpy_pkg-7.1.0/bgpy/simulation_engine/policies/bgpsec/__init__.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     4350 2024-02-24 05:53:40.000000 bgpy_pkg-7.1.0/bgpy/simulation_engine/policies/bgpsec/bgpsec.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      224 2024-02-24 05:53:40.000000 bgpy_pkg-7.1.0/bgpy/simulation_engine/policies/bgpsec/bgpsec_full.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-26 07:22:33.503713 bgpy_pkg-7.1.0/bgpy/simulation_engine/policies/only_to_customers/
+-rw-rw-r--   0 anon      (1000) anon      (1000)      168 2024-02-24 05:53:40.000000 bgpy_pkg-7.1.0/bgpy/simulation_engine/policies/only_to_customers/__init__.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1532 2024-03-28 08:04:49.000000 bgpy_pkg-7.1.0/bgpy/simulation_engine/policies/only_to_customers/only_to_customers.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      294 2024-02-24 05:53:40.000000 bgpy_pkg-7.1.0/bgpy/simulation_engine/policies/only_to_customers/only_to_customers_full.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-26 07:22:33.503713 bgpy_pkg-7.1.0/bgpy/simulation_engine/policies/path_end/
+-rw-rw-r--   0 anon      (1000) anon      (1000)      118 2024-04-26 07:06:11.000000 bgpy_pkg-7.1.0/bgpy/simulation_engine/policies/path_end/__init__.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1131 2024-04-26 07:06:11.000000 bgpy_pkg-7.1.0/bgpy/simulation_engine/policies/path_end/path_end.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      246 2024-04-26 07:06:11.000000 bgpy_pkg-7.1.0/bgpy/simulation_engine/policies/path_end/path_end_full.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-26 07:22:33.503713 bgpy_pkg-7.1.0/bgpy/simulation_engine/policies/pathend/
+-rw-rw-r--   0 anon      (1000) anon      (1000)      116 2024-02-24 05:53:40.000000 bgpy_pkg-7.1.0/bgpy/simulation_engine/policies/pathend/__init__.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1655 2024-04-26 07:06:11.000000 bgpy_pkg-7.1.0/bgpy/simulation_engine/policies/pathend/pathend.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      244 2024-02-24 05:53:40.000000 bgpy_pkg-7.1.0/bgpy/simulation_engine/policies/pathend/pathend_full.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     2926 2024-02-23 22:41:12.000000 bgpy_pkg-7.1.0/bgpy/simulation_engine/policies/policy.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-26 07:22:33.503713 bgpy_pkg-7.1.0/bgpy/simulation_engine/policies/rov/
+-rw-rw-r--   0 anon      (1000) anon      (1000)      195 2024-02-24 05:53:40.000000 bgpy_pkg-7.1.0/bgpy/simulation_engine/policies/rov/__init__.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1110 2024-02-24 05:53:40.000000 bgpy_pkg-7.1.0/bgpy/simulation_engine/policies/rov/peer_rov.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      219 2024-02-24 05:53:40.000000 bgpy_pkg-7.1.0/bgpy/simulation_engine/policies/rov/peer_rov_full.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      885 2024-02-24 05:53:40.000000 bgpy_pkg-7.1.0/bgpy/simulation_engine/policies/rov/rov.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      220 2024-02-24 05:53:40.000000 bgpy_pkg-7.1.0/bgpy/simulation_engine/policies/rov/rov_full.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-26 07:22:33.503713 bgpy_pkg-7.1.0/bgpy/simulation_engine/simulation_engines/
+-rw-rw-r--   0 anon      (1000) anon      (1000)      161 2024-02-23 22:41:12.000000 bgpy_pkg-7.1.0/bgpy/simulation_engine/simulation_engines/__init__.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     3697 2024-04-26 07:06:11.000000 bgpy_pkg-7.1.0/bgpy/simulation_engine/simulation_engines/base_simulation_engine.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     8253 2024-04-26 07:06:11.000000 bgpy_pkg-7.1.0/bgpy/simulation_engine/simulation_engines/simulation_engine.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-26 07:22:33.507713 bgpy_pkg-7.1.0/bgpy/simulation_framework/
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1115 2024-02-24 05:53:40.000000 bgpy_pkg-7.1.0/bgpy/simulation_framework/__init__.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-26 07:22:33.507713 bgpy_pkg-7.1.0/bgpy/simulation_framework/as_graph_analyzers/
+-rw-rw-r--   0 anon      (1000) anon      (1000)      157 2024-02-23 22:41:12.000000 bgpy_pkg-7.1.0/bgpy/simulation_framework/as_graph_analyzers/__init__.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     6521 2024-02-23 22:41:12.000000 bgpy_pkg-7.1.0/bgpy/simulation_framework/as_graph_analyzers/as_graph_analyzer.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      748 2024-02-23 22:41:12.000000 bgpy_pkg-7.1.0/bgpy/simulation_framework/as_graph_analyzers/base_as_graph_analyzer.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     9418 2024-02-23 22:41:12.000000 bgpy_pkg-7.1.0/bgpy/simulation_framework/graph_factory.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-26 07:22:33.507713 bgpy_pkg-7.1.0/bgpy/simulation_framework/metric_tracker/
+-rw-rw-r--   0 anon      (1000) anon      (1000)      149 2024-02-23 22:41:12.000000 bgpy_pkg-7.1.0/bgpy/simulation_framework/metric_tracker/__init__.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      461 2024-02-23 22:41:12.000000 bgpy_pkg-7.1.0/bgpy/simulation_framework/metric_tracker/data_key.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     4556 2024-02-23 22:41:12.000000 bgpy_pkg-7.1.0/bgpy/simulation_framework/metric_tracker/metric.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      367 2024-02-23 22:41:12.000000 bgpy_pkg-7.1.0/bgpy/simulation_framework/metric_tracker/metric_key.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     9936 2024-02-23 22:41:12.000000 bgpy_pkg-7.1.0/bgpy/simulation_framework/metric_tracker/metric_tracker.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-26 07:22:33.507713 bgpy_pkg-7.1.0/bgpy/simulation_framework/scenarios/
+-rw-rw-r--   0 anon      (1000) anon      (1000)      899 2024-04-26 05:17:27.000000 bgpy_pkg-7.1.0/bgpy/simulation_framework/scenarios/__init__.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-26 07:22:33.507713 bgpy_pkg-7.1.0/bgpy/simulation_framework/scenarios/custom_scenarios/
+-rw-rw-r--   0 anon      (1000) anon      (1000)      693 2024-02-23 22:41:12.000000 bgpy_pkg-7.1.0/bgpy/simulation_framework/scenarios/custom_scenarios/__init__.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     8080 2024-04-26 07:06:11.000000 bgpy_pkg-7.1.0/bgpy/simulation_framework/scenarios/custom_scenarios/accidental_route_leak.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1418 2024-02-24 05:53:40.000000 bgpy_pkg-7.1.0/bgpy/simulation_framework/scenarios/custom_scenarios/non_routed_prefix_hijack.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1636 2024-02-24 05:53:40.000000 bgpy_pkg-7.1.0/bgpy/simulation_framework/scenarios/custom_scenarios/non_routed_superprefix_hijack.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1945 2024-02-24 05:53:40.000000 bgpy_pkg-7.1.0/bgpy/simulation_framework/scenarios/custom_scenarios/non_routed_superprefix_prefix_hijack.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     2044 2024-02-24 05:53:40.000000 bgpy_pkg-7.1.0/bgpy/simulation_framework/scenarios/custom_scenarios/prefix_hijack.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     2058 2024-02-24 05:53:40.000000 bgpy_pkg-7.1.0/bgpy/simulation_framework/scenarios/custom_scenarios/subprefix_hijack.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     2381 2024-02-24 05:53:40.000000 bgpy_pkg-7.1.0/bgpy/simulation_framework/scenarios/custom_scenarios/superprefix_prefix_hijack.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1766 2024-02-24 05:53:40.000000 bgpy_pkg-7.1.0/bgpy/simulation_framework/scenarios/custom_scenarios/valid_prefix.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)    17506 2024-04-26 07:06:11.000000 bgpy_pkg-7.1.0/bgpy/simulation_framework/scenarios/preprocess_anns_funcs.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      462 2024-02-24 05:53:40.000000 bgpy_pkg-7.1.0/bgpy/simulation_framework/scenarios/roa_info.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)    23183 2024-04-26 07:06:11.000000 bgpy_pkg-7.1.0/bgpy/simulation_framework/scenarios/scenario.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     6772 2024-04-26 07:06:11.000000 bgpy_pkg-7.1.0/bgpy/simulation_framework/scenarios/scenario_config.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)    15693 2024-04-08 14:47:25.000000 bgpy_pkg-7.1.0/bgpy/simulation_framework/simulation.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1576 2024-02-23 22:41:12.000000 bgpy_pkg-7.1.0/bgpy/simulation_framework/utils.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-26 07:22:33.507713 bgpy_pkg-7.1.0/bgpy/tests/
+-rw-rw-r--   0 anon      (1000) anon      (1000)      228 2024-02-23 22:41:12.000000 bgpy_pkg-7.1.0/bgpy/tests/__init__.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     2412 2024-03-13 03:26:50.000000 bgpy_pkg-7.1.0/bgpy/tests/conftest.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-26 07:22:33.507713 bgpy_pkg-7.1.0/bgpy/tests/engine_tests/
+-rw-rw-r--   0 anon      (1000) anon      (1000)      175 2024-02-23 22:41:12.000000 bgpy_pkg-7.1.0/bgpy/tests/engine_tests/__init__.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-26 07:22:33.507713 bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/
+-rw-rw-r--   0 anon      (1000) anon      (1000)      180 2024-04-26 05:18:48.000000 bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/__init__.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-26 07:22:33.511713 bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/examples/
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1855 2024-04-26 05:18:48.000000 bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/examples/__init__.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1529 2024-04-26 05:18:48.000000 bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/examples/as_graph_info_000.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      734 2024-04-26 05:18:48.000000 bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_000.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      759 2024-04-26 05:18:48.000000 bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_001.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1338 2024-04-26 05:18:48.000000 bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_002.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      765 2024-04-26 05:18:48.000000 bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_003.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      788 2024-04-26 05:18:48.000000 bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_004.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      790 2024-04-26 05:18:48.000000 bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_005.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      806 2024-04-26 05:18:48.000000 bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_006.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      808 2024-04-26 05:18:48.000000 bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_007.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      813 2024-04-26 05:18:48.000000 bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_008.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      834 2024-04-26 05:18:48.000000 bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_009.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      862 2024-04-26 05:18:48.000000 bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_010.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      824 2024-04-26 05:18:48.000000 bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_011.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      971 2024-04-26 07:06:11.000000 bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_012.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      966 2024-04-26 05:18:48.000000 bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_013.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1132 2024-04-26 05:18:48.000000 bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_014.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1132 2024-04-26 07:06:11.000000 bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_015.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1130 2024-04-26 07:06:11.000000 bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_016.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1147 2024-04-26 07:06:11.000000 bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_017.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1110 2024-04-26 07:06:11.000000 bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_018.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1137 2024-04-26 05:18:48.000000 bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_019.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1144 2024-04-26 05:18:48.000000 bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_020.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      972 2024-04-26 05:18:48.000000 bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_021.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      979 2024-04-26 05:18:48.000000 bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_022.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1154 2024-04-26 07:06:11.000000 bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_023.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1190 2024-04-26 07:06:11.000000 bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_024.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1167 2024-04-26 05:18:48.000000 bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_025.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1305 2024-04-26 05:18:48.000000 bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_026.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1338 2024-04-26 05:18:48.000000 bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_027.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1349 2024-04-26 05:18:48.000000 bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_028.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1532 2024-04-26 07:06:11.000000 bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_029.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-26 07:22:33.511713 bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/internals/
+-rw-rw-r--   0 anon      (1000) anon      (1000)      368 2024-04-26 05:18:48.000000 bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/internals/__init__.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     2206 2024-04-26 05:18:48.000000 bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/internals/internal_config_000.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     2338 2024-04-26 05:18:48.000000 bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/internals/internal_config_001.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     2792 2024-04-26 05:18:48.000000 bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/internals/internal_config_002.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1211 2024-04-26 05:18:48.000000 bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/internals/internal_config_003.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1968 2024-04-26 07:06:11.000000 bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/internals/internal_config_004.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      780 2024-04-18 07:44:17.000000 bgpy_pkg-7.1.0/bgpy/tests/engine_tests/test_engine.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-26 07:22:33.511713 bgpy_pkg-7.1.0/bgpy/tests/engine_tests/utils/
+-rw-rw-r--   0 anon      (1000) anon      (1000)      285 2024-02-23 22:41:12.000000 bgpy_pkg-7.1.0/bgpy/tests/engine_tests/utils/__init__.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1757 2024-02-23 22:41:12.000000 bgpy_pkg-7.1.0/bgpy/tests/engine_tests/utils/diagram_aggregator.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      566 2024-02-23 22:41:12.000000 bgpy_pkg-7.1.0/bgpy/tests/engine_tests/utils/engine_test_config.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     9473 2024-02-23 22:41:12.000000 bgpy_pkg-7.1.0/bgpy/tests/engine_tests/utils/engine_tester.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-26 07:22:33.511713 bgpy_pkg-7.1.0/bgpy/tests/framework_tests/
+-rw-rw-r--   0 anon      (1000) anon      (1000)        0 2024-02-23 22:41:12.000000 bgpy_pkg-7.1.0/bgpy/tests/framework_tests/__init__.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-26 07:22:33.511713 bgpy_pkg-7.1.0/bgpy/tests/framework_tests/system_tests/
+-rw-rw-r--   0 anon      (1000) anon      (1000)       76 2024-02-23 22:41:12.000000 bgpy_pkg-7.1.0/bgpy/tests/framework_tests/system_tests/__init__.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      896 2024-02-24 05:53:40.000000 bgpy_pkg-7.1.0/bgpy/tests/framework_tests/system_tests/test_sim_inputs.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-26 07:22:33.511713 bgpy_pkg-7.1.0/bgpy/tests/framework_tests/unit_tests/
+-rw-rw-r--   0 anon      (1000) anon      (1000)        0 2024-02-23 22:41:12.000000 bgpy_pkg-7.1.0/bgpy/tests/framework_tests/unit_tests/__init__.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      478 2024-02-23 22:41:12.000000 bgpy_pkg-7.1.0/bgpy/tests/framework_tests/unit_tests/conftest.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)    15144 2024-03-13 03:26:50.000000 bgpy_pkg-7.1.0/bgpy/tests/framework_tests/unit_tests/test_scenario.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-26 07:22:33.511713 bgpy_pkg-7.1.0/bgpy/utils/
+-rw-rw-r--   0 anon      (1000) anon      (1000)      279 2024-02-23 22:41:12.000000 bgpy_pkg-7.1.0/bgpy/utils/__init__.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)    11631 2024-02-24 05:53:40.000000 bgpy_pkg-7.1.0/bgpy/utils/diagram.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1038 2024-02-23 22:41:12.000000 bgpy_pkg-7.1.0/bgpy/utils/engine_run_config.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     8230 2024-02-23 22:41:12.000000 bgpy_pkg-7.1.0/bgpy/utils/engine_runner.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-26 07:22:33.515713 bgpy_pkg-7.1.0/bgpy/utils/simulator_codec/
+-rw-rw-r--   0 anon      (1000) anon      (1000)       74 2024-02-23 22:41:12.000000 bgpy_pkg-7.1.0/bgpy/utils/simulator_codec/__init__.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     2834 2024-02-23 22:41:12.000000 bgpy_pkg-7.1.0/bgpy/utils/simulator_codec/simulator_codec.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      322 2024-02-23 22:41:12.000000 bgpy_pkg-7.1.0/bgpy/utils/simulator_codec/simulator_loader.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-26 07:22:33.515713 bgpy_pkg-7.1.0/bgpy_pkg.egg-info/
+-rw-r--r--   0 anon      (1000) anon      (1000)     4622 2024-04-26 07:22:33.000000 bgpy_pkg-7.1.0/bgpy_pkg.egg-info/PKG-INFO
+-rw-rw-r--   0 anon      (1000) anon      (1000)     8687 2024-04-26 07:22:33.000000 bgpy_pkg-7.1.0/bgpy_pkg.egg-info/SOURCES.txt
+-rw-rw-r--   0 anon      (1000) anon      (1000)        1 2024-04-26 07:22:33.000000 bgpy_pkg-7.1.0/bgpy_pkg.egg-info/dependency_links.txt
+-rw-rw-r--   0 anon      (1000) anon      (1000)       44 2024-04-26 07:22:33.000000 bgpy_pkg-7.1.0/bgpy_pkg.egg-info/entry_points.txt
+-rw-rw-r--   0 anon      (1000) anon      (1000)      370 2024-04-26 07:22:33.000000 bgpy_pkg-7.1.0/bgpy_pkg.egg-info/requires.txt
+-rw-rw-r--   0 anon      (1000) anon      (1000)        5 2024-04-26 07:22:33.000000 bgpy_pkg-7.1.0/bgpy_pkg.egg-info/top_level.txt
+-rw-rw-r--   0 anon      (1000) anon      (1000)     3465 2024-04-26 07:06:11.000000 bgpy_pkg-7.1.0/pyproject.toml
+-rwxrwxr-x   0 anon      (1000) anon      (1000)       69 2024-04-26 07:22:33.515713 bgpy_pkg-7.1.0/setup.cfg
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1157 2024-02-24 05:53:40.000000 bgpy_pkg-7.1.0/tox.ini
```

### Comparing `bgpy_pkg-7.0.9/LICENSE.txt` & `bgpy_pkg-7.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/PKG-INFO` & `bgpy_pkg-7.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bgpy_pkg
-Version: 7.0.9
+Version: 7.1.0
 Summary: Simulates BGP and ROV in an extensible manner
 Author-email: Justin Furuness <jfuruness@gmail.com>, Cameron Morris <cameron.morris@uconn.edu>, Reynaldo Morillo <reynaldo.morillo@uconn.edu>, Arvind Kasiliya <arvind.kasiliya@uconn.edu>
 Maintainer-email: Justin Furuness <jfuruness@gmail.com>
 License: Copyright 2020 Justin Furuness
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
```

### Comparing `bgpy_pkg-7.0.9/README.md` & `bgpy_pkg-7.1.0/README.md`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/__main__.py` & `bgpy_pkg-7.1.0/bgpy/__main__.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/as_graphs/__init__.py` & `bgpy_pkg-7.1.0/bgpy/as_graphs/__init__.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/as_graphs/base/as_graph/as_graph.py` & `bgpy_pkg-7.1.0/bgpy/as_graphs/base/as_graph/as_graph.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/as_graphs/base/as_graph/base_as.py` & `bgpy_pkg-7.1.0/bgpy/as_graphs/base/as_graph/base_as.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/as_graphs/base/as_graph/customer_cone_funcs.py` & `bgpy_pkg-7.1.0/bgpy/as_graphs/base/as_graph/customer_cone_funcs.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/as_graphs/base/as_graph/graph_building_funcs.py` & `bgpy_pkg-7.1.0/bgpy/as_graphs/base/as_graph/graph_building_funcs.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/as_graphs/base/as_graph/propagation_rank_funcs.py` & `bgpy_pkg-7.1.0/bgpy/as_graphs/base/as_graph/propagation_rank_funcs.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/as_graphs/base/as_graph_collector.py` & `bgpy_pkg-7.1.0/bgpy/as_graphs/base/as_graph_collector.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/as_graphs/base/as_graph_constructor.py` & `bgpy_pkg-7.1.0/bgpy/as_graphs/base/as_graph_constructor.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/as_graphs/base/as_graph_info.py` & `bgpy_pkg-7.1.0/bgpy/as_graphs/base/as_graph_info.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/as_graphs/base/links/customer_provider_link.py` & `bgpy_pkg-7.1.0/bgpy/as_graphs/base/links/customer_provider_link.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/as_graphs/base/links/link.py` & `bgpy_pkg-7.1.0/bgpy/as_graphs/base/links/link.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/as_graphs/base/links/peer_link.py` & `bgpy_pkg-7.1.0/bgpy/as_graphs/base/links/peer_link.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/as_graphs/caida_as_graph/caida_as_graph_collector.py` & `bgpy_pkg-7.1.0/bgpy/as_graphs/caida_as_graph/caida_as_graph_collector.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/as_graphs/caida_as_graph/caida_as_graph_constructor.py` & `bgpy_pkg-7.1.0/bgpy/as_graphs/caida_as_graph/caida_as_graph_constructor.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/enums.py` & `bgpy_pkg-7.1.0/bgpy/enums.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/simulation_engine/__init__.py` & `bgpy_pkg-7.1.0/bgpy/simulation_engine/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 from .policies import ROVFull
 from .policies import BGPSecFull
 from .policies import BGPSec
 from .policies import OnlyToCustomers
 from .policies import OnlyToCustomersFull
 from .policies import Pathend
 from .policies import PathendFull
+from .policies import PathEnd
+from .policies import PathEndFull
 from .policies import ASPA
 from .policies import ASPAFull
 
 # Old - just keeping these around for backwards compatability
 from .policies import BGP as BGPSimplePolicy
 from .policies import BGPFull as BGPPolicy
 from .policies import PeerROV as PeerROVSimplePolicy
@@ -58,14 +60,16 @@
     "Policy",
     "BGPSecFull",
     "BGPSec",
     "OnlyToCustomersFull",
     "OnlyToCustomers",
     "Pathend",
     "PathendFull",
+    "PathEnd",
+    "PathEndFull",
     "ASPA",
     "ASPAFull",
     "BGPSimplePolicy",
     "BGPPolicy",
     "PeerROVSimplePolicy",
     "PeerROVPolicy",
     "ROVSimplePolicy",
```

### Comparing `bgpy_pkg-7.0.9/bgpy/simulation_engine/ann_containers/ann_container.py` & `bgpy_pkg-7.1.0/bgpy/simulation_engine/ann_containers/ann_container.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/simulation_engine/ann_containers/recv_queue.py` & `bgpy_pkg-7.1.0/bgpy/simulation_engine/ann_containers/recv_queue.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/simulation_engine/ann_containers/ribs_in.py` & `bgpy_pkg-7.1.0/bgpy/simulation_engine/ann_containers/ribs_in.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/simulation_engine/ann_containers/ribs_out.py` & `bgpy_pkg-7.1.0/bgpy/simulation_engine/ann_containers/ribs_out.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/simulation_engine/ann_containers/send_queue.py` & `bgpy_pkg-7.1.0/bgpy/simulation_engine/ann_containers/send_queue.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/simulation_engine/announcement.py` & `bgpy_pkg-7.1.0/bgpy/simulation_engine/announcement.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/__init__.py` & `bgpy_pkg-7.1.0/bgpy/simulation_engine/policies/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     ROV,
     ROVFull,
 )
 from .bgpsec import BGPSecFull
 from .bgpsec import BGPSec
 from .only_to_customers import OnlyToCustomers, OnlyToCustomersFull
 from .pathend import Pathend, PathendFull
+from .path_end import PathEnd, PathEndFull
 from .aspa import ASPA, ASPAFull
 
 __all__ = [
     "BGP",
     "BGPFull",
     "Policy",
     "PeerROV",
@@ -22,10 +23,12 @@
     "ROVFull",
     "BGPSecFull",
     "BGPSec",
     "OnlyToCustomers",
     "OnlyToCustomersFull",
     "Pathend",
     "PathendFull",
+    "PathEnd",
+    "PathEndFull",
     "ASPA",
     "ASPAFull",
 ]
```

### Comparing `bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/aspa/aspa.py` & `bgpy_pkg-7.1.0/bgpy/simulation_engine/policies/aspa/aspa.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/bgp/bgp/bgp.py` & `bgpy_pkg-7.1.0/bgpy/simulation_engine/policies/bgp/bgp/bgp.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/bgp/bgp/gao_rexford.py` & `bgpy_pkg-7.1.0/bgpy/simulation_engine/policies/bgp/bgp/gao_rexford.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/bgp/bgp/process_incoming_funcs.py` & `bgpy_pkg-7.1.0/bgpy/simulation_engine/policies/bgp/bgp/process_incoming_funcs.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/bgp/bgp/propagate_funcs.py` & `bgpy_pkg-7.1.0/bgpy/simulation_engine/policies/bgp/bgp/propagate_funcs.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/bgp/bgp_full/bgp_full.py` & `bgpy_pkg-7.1.0/bgpy/simulation_engine/policies/bgp/bgp_full/bgp_full.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/bgp/bgp_full/process_incoming_funcs.py` & `bgpy_pkg-7.1.0/bgpy/simulation_engine/policies/bgp/bgp_full/process_incoming_funcs.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/bgp/bgp_full/propagate_funcs.py` & `bgpy_pkg-7.1.0/bgpy/simulation_engine/policies/bgp/bgp_full/propagate_funcs.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/bgpsec/bgpsec.py` & `bgpy_pkg-7.1.0/bgpy/simulation_engine/policies/bgpsec/bgpsec.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/only_to_customers/only_to_customers.py` & `bgpy_pkg-7.1.0/bgpy/simulation_engine/policies/only_to_customers/only_to_customers.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/pathend/pathend.py` & `bgpy_pkg-7.1.0/bgpy/simulation_engine/policies/path_end/path_end.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 
 from bgpy.simulation_engine.policies.rov import ROV
 
 if TYPE_CHECKING:
     from bgpy.simulation_engine import Announcement as Ann
 
 
-class Pathend(ROV):
-    """An Policy that deploys Pathend"""
+class PathEnd(ROV):
+    """An Policy that deploys Path-End"""
 
-    name: str = "Pathend"
+    name: str = "Path-End"
 
     def _valid_ann(self, ann: "Ann", *args, **kwargs) -> bool:  # type: ignore
         """Returns announcement validity by checking pathend records"""
 
         origin_asn = ann.origin
         origin_as_obj = self.as_.as_graph.as_dict[origin_asn]
         # If the origin is deploying pathend and the path is longer than 1
-        if isinstance(origin_as_obj.policy, Pathend) and len(ann.as_path) > 1:
+        if isinstance(origin_as_obj.policy, PathEnd) and len(ann.as_path) > 1:
             # If the provider is real, do the loop check
             # Mypy thinks this is unreachable for some reason, even tho tests pass
             for neighbor in origin_as_obj.neighbors:  # type: ignore
                 if neighbor.asn == ann.as_path[-2]:
                     return super()._valid_ann(ann, *args, **kwargs)
             # Provider is fake, return False
             return False
```

### Comparing `bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/policy.py` & `bgpy_pkg-7.1.0/bgpy/simulation_engine/policies/policy.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/rov/peer_rov.py` & `bgpy_pkg-7.1.0/bgpy/simulation_engine/policies/rov/peer_rov.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/rov/rov.py` & `bgpy_pkg-7.1.0/bgpy/simulation_engine/policies/rov/rov.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/simulation_engine/simulation_engines/base_simulation_engine.py` & `bgpy_pkg-7.1.0/bgpy/simulation_engine/simulation_engines/base_simulation_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,16 @@
         self,
         announcements: tuple["Ann", ...] = (),
         BasePolicyCls: type[Policy] = Policy,
         non_default_asn_cls_dict: frozendict[int, type[Policy]] = (
             frozendict()  # type: ignore
         ),
         prev_scenario: Optional["Scenario"] = None,
+        attacker_asns: frozenset[int] = frozenset(),
+        AttackerBasePolicyCls: Optional[type[Policy]] = None,
     ) -> frozenset[type[Policy]]:
         """Sets AS classes and seeds announcements"""
 
         raise NotImplementedError
 
     #####################
     # Propagation funcs #
```

### Comparing `bgpy_pkg-7.0.9/bgpy/simulation_engine/simulation_engines/simulation_engine.py` & `bgpy_pkg-7.1.0/bgpy/simulation_framework/scenarios/scenario_config.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,189 +1,173 @@
+import abc
+from dataclasses import asdict, dataclass, field
 from typing import Any, Optional, TYPE_CHECKING
 
 from frozendict import frozendict
 
-from bgpy.enums import Relationships
-from bgpy.simulation_engine import Policy
-from bgpy.simulation_engine.policies import BGP
-
-from .base_simulation_engine import BaseSimulationEngine
-
-# https://stackoverflow.com/a/57005931/8903959
-if TYPE_CHECKING:
-    from bgpy.simulation_engine import Announcement as Ann
-    from bgpy.simulation_framework import Scenario
+from bgpy.enums import ASGroups
 
+from bgpy.simulation_engine import Announcement as Ann
+from bgpy.simulation_engine import Policy
+from bgpy.simulation_engine import BGP
 
-class SimulationEngine(BaseSimulationEngine):
-    """Python simulation engine representation"""
+from .preprocess_anns_funcs import noop, PREPROCESS_ANNS_FUNC_TYPE
+from .roa_info import ROAInfo
 
-    ###############
-    # Setup funcs #
-    ###############
-
-    def setup(
-        self,
-        announcements: tuple["Ann", ...] = (),
-        BasePolicyCls: type[Policy] = BGP,
-        non_default_asn_cls_dict: frozendict[int, type[Policy]] = (
-            frozendict()  # type: ignore
-        ),
-        prev_scenario: Optional["Scenario"] = None,
-    ) -> frozenset[type[Policy]]:
-        """Sets AS classes and seeds announcements"""
 
-        policies_used: frozenset[type[Policy]] = self._set_as_classes(
-            BasePolicyCls, non_default_asn_cls_dict, prev_scenario
-        )
-        self._seed_announcements(announcements, prev_scenario)
-        self.ready_to_run_round = 0
-        return policies_used
-
-    def _set_as_classes(
-        self,
-        BasePolicyCls: type[Policy],
-        non_default_asn_cls_dict: frozendict[int, type[Policy]],
-        prev_scenario: Optional["Scenario"] = None,
-    ) -> frozenset[type[Policy]]:
-        """Resets Engine ASes and changes their AS class
-
-        We do this here because we already seed from the scenario
-        to allow for easy overriding. If scenario controls seeding,
-        it doesn't make sense for engine to control resetting either
-        and have each do half and half
-        """
+if TYPE_CHECKING:
+    from .scenario import Scenario
 
-        policy_classes_used = set()
-        # Done here to save as much time  as possible
-        for as_obj in self.as_graph:
-            # Delete the old policy and remove references so that RAM can be reclaimed
-            del as_obj.policy.as_
-            # set the AS class to be the proper type of AS
-            Cls = non_default_asn_cls_dict.get(as_obj.asn, BasePolicyCls)
-            as_obj.policy = Cls(as_=as_obj)
-            policy_classes_used.add(Cls)
-        return frozenset(policy_classes_used)
-
-    def _seed_announcements(
-        self,
-        announcements: tuple["Ann", ...] = (),
-        prev_scenario: Optional["Scenario"] = None,
-    ) -> None:
-        """Seeds announcement at the proper AS
+pseudo_base_cls_dict: dict[type[Policy], type[Policy]] = dict()
 
-        Since this is the simulator engine, we should
-        never have to worry about overlapping announcements
-        """
 
-        for ann in announcements:
-            assert ann.seed_asn is not None
-            # Get the AS object to seed at
-            # Must ignore type because it doesn't see assert above
-            obj_to_seed = self.as_graph.as_dict[ann.seed_asn]  # type: ignore
-            obj_to_seed.policy.seed_ann(ann)
-
-    #####################
-    # Propagation funcs #
-    #####################
-
-    def run(self, propagation_round: int = 0, scenario: Optional["Scenario"] = None):
-        """Propogates announcements and ensures proper setup"""
-
-        # Ensure that the simulator is ready to run this round
-        if self.ready_to_run_round != propagation_round:
-            raise Exception(f"Engine not set up to run for {propagation_round} round")
-        assert scenario, "This can't be empty"
-
-        # import time
-        # start = time.perf_counter()
-        # Propogate anns
-        self._propagate(propagation_round, scenario)
-        # print(f"prop time {time.perf_counter() - start}")
-        # Increment the ready to run round
-        self.ready_to_run_round += 1
-
-    def _propagate(self, propagation_round: int, scenario: "Scenario"):
-        """Propogates announcements
-
-        to stick with Gao Rexford, we propagate to
-        0. providers
-        2. peers
-        3. customers
+class MISSINGPolicy(Policy):
+    name: str = "missing"
+    pass
+
+
+@dataclass(frozen=True)
+class ScenarioConfig:
+    """Contains information required to set up a scenario/attack
+
+    Is reused for multiple trials (thus, frozen)
+    """
+
+    ScenarioCls: type["Scenario"]
+    # Set in post_init
+    propagation_rounds: int = None  # type: ignore
+    preprocess_anns_func: PREPROCESS_ANNS_FUNC_TYPE = noop
+    # This is the base type of announcement for this class
+    # You can specify a different base ann
+    AnnCls: type[Ann] = Ann
+    BasePolicyCls: type[Policy] = BGP
+    # Fixed in post init, but can't show mypy for some reason
+    AdoptPolicyCls: type[Policy] = MISSINGPolicy  # type: ignore
+    # Used to override attacker's base policy class
+    AttackerBasePolicyCls: Optional[type[Policy]] = None
+    num_attackers: int = 1
+    num_victims: int = 1
+    # Adoption is equal across these atributes of the engine
+    adoption_subcategory_attrs: tuple[str, ...] = (
+        ASGroups.STUBS_OR_MH.value,
+        ASGroups.ETC.value,
+        ASGroups.INPUT_CLIQUE.value,
+    )
+    # Attackers can be chosen from this attribute of the engine
+    attacker_subcategory_attr: str = ASGroups.STUBS_OR_MH.value
+    # Victims can be chosen from this attribute of the engine
+    victim_subcategory_attr: str = ASGroups.STUBS_OR_MH.value
+    # ASes that are hardcoded to specific values
+    hardcoded_asn_cls_dict: frozendict[int, type[Policy]] = field(
+        # Mypy doesn't understand frozendict typing, just ignore it
+        default_factory=frozendict  # type: ignore
+    )
+    # Only necessary if coming from YAML or the test suite
+    override_attacker_asns: Optional[frozenset[int]] = None
+    override_victim_asns: Optional[frozenset[int]] = None
+    # For some reason mypy has trouble with empty frozendicts
+    # So I've included that as a second option for typing purposes
+    # (specifically with the tests)
+    override_non_default_asn_cls_dict: Any = None
+    # Unfortunately this causes lots of errors in mypy, even though
+    # it's correct. No idea why it's failing here, possibly something
+    # internal to frozendict. Either way, it doesn't matter, this is
+    # pretty much only used within the tests, which would fail if this
+    # was wrong anyways
+    # override_non_default_asn_cls_dict: Union[
+    #    Optional[frozendict[int, type[Policy]]],
+    #    frozendict[str, None]
+    # ] = None
+    override_announcements: tuple["Ann", ...] = ()
+    override_roa_infos: tuple[ROAInfo, ...] = ()
+    # If you'd like to add an extra CSV label you do so here
+    csv_label: str = ""
+    # Deprecated param, don't use
+    scenario_label: str = ""
+
+    def __post_init__(self):
+        """sets AdoptPolicyCls if it is None
+
+        This is done to fix the following:
+        Scenario 1 has 3 BGP Policyes and 1 AdoptCls
+        Scenario 2 has no adopt classes, so 4 BGP
+        Scenario 3 we want to run ROV++, but what were the adopting Policyes from
+        scenario 1? We don't know anymore.
+        Instead for scenario 2, we have 3 BGP Policyes and 1 Psuedo BGP Policy
+        Then scenario 3 will still work as expected
         """
 
-        self._propagate_to_providers(propagation_round, scenario)
-        self._propagate_to_peers(propagation_round, scenario)
-        self._propagate_to_customers(propagation_round, scenario)
-
-    def _propagate_to_providers(self, propagation_round: int, scenario: "Scenario"):
-        """Propogate to providers"""
-
-        # Propogation ranks go from stubs to input_clique in ascending order
-        # By customer provider pairs (peers are ignored for the ranks)
-        for i, rank in enumerate(self.as_graph.propagation_ranks):
-            # Nothing to process at the start
-            if i > 0:
-                # Process first because maybe it recv from lower ranks
-                for as_obj in rank:
-                    as_obj.policy.process_incoming_anns(
-                        from_rel=Relationships.CUSTOMERS,
-                        propagation_round=propagation_round,
-                        scenario=scenario,
-                    )
-            # Send to the higher ranks
-            for as_obj in rank:
-                as_obj.policy.propagate_to_providers()
-
-    def _propagate_to_peers(
-        self, propagation_round: int, scenario: Optional["Scenario"]
-    ):
-        """Propagate to peers"""
-
-        # The reason you must separate this for loop here
-        # is because propagation ranks do not take into account peering
-        # It'd be impossible to take into account peering
-        # since different customers peer to different ranks
-        # So first do customer to provider propagation, then peer propagation
-        for as_obj in self.as_graph:
-            as_obj.policy.propagate_to_peers()
-        for as_obj in self.as_graph:
-            as_obj.policy.process_incoming_anns(
-                from_rel=Relationships.PEERS,
-                propagation_round=propagation_round,
-                scenario=scenario,
+        if self.propagation_rounds is None:
+            object.__setattr__(  # type: ignore
+                self, "propagation_rounds", self.ScenarioCls.min_propagation_rounds
             )
 
-    def _propagate_to_customers(self, propagation_round: int, scenario: "Scenario"):
-        """Propagate to customers"""
+        if self.ScenarioCls.min_propagation_rounds > self.propagation_rounds:
+            raise ValueError(
+                f"{self.ScenarioCls.__name__} requires a minimum of "
+                f"{self.ScenarioCls.min_propagation_rounds} propagation rounds "
+                f"but this scenario_config has only {self.propagation_rounds} "
+                "propagation rounds"
+            )
 
-        # Propogation ranks go from stubs to input_clique in ascending order
-        # By customer provider pairs (peers are ignored for the ranks)
-        # So here we start at the highest rank(input_clique) and propagate down
-        for i, rank in enumerate(reversed(self.as_graph.propagation_ranks)):
-            # There are no incomming Anns at the top
-            if i > 0:
-                for as_obj in rank:
-                    as_obj.policy.process_incoming_anns(
-                        from_rel=Relationships.PROVIDERS,
-                        propagation_round=propagation_round,
-                        scenario=scenario,
-                    )
-            for as_obj in rank:
-                as_obj.policy.propagate_to_customers()
+        if self.AdoptPolicyCls == MISSINGPolicy:
+            # mypy says this is unreachable, which is wrong
+            global pseudo_base_cls_dict  # type: ignore
+            AdoptPolicyCls = pseudo_base_cls_dict.get(self.BasePolicyCls)
+            if not AdoptPolicyCls:
+                name: str = f"Pseudo {self.BasePolicyCls.name}".replace(" ", "")
+                PseudoBaseCls = type(name, (self.BasePolicyCls,), {"name": name})
+                pseudo_base_cls_dict[self.BasePolicyCls] = PseudoBaseCls
+                # Must set for pickling purposes
+                setattr(abc, name, PseudoBaseCls)
+                AdoptPolicyCls = PseudoBaseCls
+            object.__setattr__(self, "AdoptPolicyCls", AdoptPolicyCls)
+        # Better error messages when setting this var
+        if not isinstance(self.hardcoded_asn_cls_dict, frozendict):  # type: ignore
+            raise TypeError(
+                "hardcoded_asn_cls_dict of ScenarioConfig is not frozendict "
+                f"and is instead {type(self.hardcoded_asn_cls_dict)}. Please "
+                "change the type to frozendict so that it is hashable"
+            )
 
     ##############
-    # Yaml funcs #
+    # Yaml Funcs #
     ##############
 
-    def __to_yaml_dict__(self) -> dict[str, Any]:
+    @property
+    def _yamlable_hardcoded_asn_cls_dict(self) -> dict[int, str]:
+        """Converts non default as cls dict to a yamlable dict of asn: name"""
+
+        return {
+            asn: Policy.subclass_to_name_dict[PolicyCls]
+            for asn, PolicyCls in self.hardcoded_asn_cls_dict.items()
+        }
+
+    @staticmethod
+    def _get_hardcoded_asn_cls_dict_from_yaml(
+        yaml_dict,
+    ) -> dict[int, type[Policy]]:
+        """Converts yamlified non_default_as_cls_dict back to normal asn: class"""
+
+        return {
+            asn: Policy.name_to_subclass_dict[name] for asn, name in yaml_dict.items()
+        }
+
+    def __to_yaml_dict__(self) -> dict[Any, Any]:
         """This optional method is called when you call yaml.dump()"""
 
-        return dict(vars(self))
+        yaml_dict = dict()
+        for k, v in asdict(self).items():
+            if k == "hardcoded_asn_cls_dict":
+                yaml_dict[k] = self._yamlable_hardcoded_asn_cls_dict
+            else:
+                yaml_dict[k] = v
+        return yaml_dict
 
     @classmethod
-    def __from_yaml_dict__(
-        cls: type["SimulationEngine"], dct: dict[str, Any], yaml_tag: Any
-    ) -> "SimulationEngine":
+    def __from_yaml_dict__(cls, dct, yaml_tag):
         """This optional method is called when you call yaml.load()"""
 
+        dct["hardcoded_asn_cls_dict"] = cls._get_hardcoded_asn_cls_dict_from_yaml(
+            dct["hardcoded_asn_cls_dict"]
+        )
         return cls(**dct)
```

### Comparing `bgpy_pkg-7.0.9/bgpy/simulation_framework/__init__.py` & `bgpy_pkg-7.1.0/bgpy/simulation_framework/__init__.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/simulation_framework/as_graph_analyzers/as_graph_analyzer.py` & `bgpy_pkg-7.1.0/bgpy/simulation_framework/as_graph_analyzers/as_graph_analyzer.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/simulation_framework/as_graph_analyzers/base_as_graph_analyzer.py` & `bgpy_pkg-7.1.0/bgpy/simulation_framework/as_graph_analyzers/base_as_graph_analyzer.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/simulation_framework/graph_factory.py` & `bgpy_pkg-7.1.0/bgpy/simulation_framework/graph_factory.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/simulation_framework/metric_tracker/metric.py` & `bgpy_pkg-7.1.0/bgpy/simulation_framework/metric_tracker/metric.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/simulation_framework/metric_tracker/metric_tracker.py` & `bgpy_pkg-7.1.0/bgpy/simulation_framework/metric_tracker/metric_tracker.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/simulation_framework/scenarios/__init__.py` & `bgpy_pkg-7.1.0/bgpy/simulation_framework/scenarios/__init__.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/simulation_framework/scenarios/custom_scenarios/__init__.py` & `bgpy_pkg-7.1.0/bgpy/simulation_framework/scenarios/custom_scenarios/__init__.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/simulation_framework/scenarios/custom_scenarios/accidental_route_leak.py` & `bgpy_pkg-7.1.0/bgpy/simulation_framework/scenarios/custom_scenarios/accidental_route_leak.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, TYPE_CHECKING
+from typing import Optional, Union, TYPE_CHECKING
 import warnings
 
 from bgpy.enums import ASGroups, Relationships, SpecialPercentAdoptions, Timestamps
 from bgpy.as_graphs.base.as_graph.customer_cone_funcs import _get_cone_size_helper
 
 from .valid_prefix import ValidPrefix
 from ..scenario import Scenario
@@ -26,14 +26,16 @@
         scenario_config: ScenarioConfig,
         percent_adoption: float | SpecialPercentAdoptions = 0,
         engine: Optional["BaseSimulationEngine"] = None,
         prev_scenario: Optional["Scenario"] = None,
         preprocess_anns_func: PREPROCESS_ANNS_FUNC_TYPE = noop,
     ):
 
+        assert engine, "Need engine for customer cones"
+        self._attackers_customer_cones_asns: set[int] = set()
         super().__init__(
             scenario_config=scenario_config,
             percent_adoption=percent_adoption,
             engine=engine,
             prev_scenario=prev_scenario,
             preprocess_anns_func=preprocess_anns_func,
         )
@@ -46,25 +48,14 @@
                 f"{self.scenario_config.attacker_subcategory_attr} "
                 f"for your scenario {self.__class__.__name__}, "
                 f"but {self.__class__.__name__} can't leak from stubs. "
                 "To suppress this warning, override warning_as_groups"
             )
             warnings.warn(msg, RuntimeWarning)
 
-        # Stores customer cones of attacker ASNs, used in untrackable func
-        self._attackers_customer_cones_asns: set[int] = set()
-        assert engine, "Need engine for customer cones"
-        for attacker_asn in self.attacker_asns:
-            self._attackers_customer_cones_asns.update(
-                self._get_cone_size_helper(
-                    engine.as_graph.as_dict[attacker_asn],
-                    dict(),
-                ),
-            )
-
     # Just returns customer cone
     _get_cone_size_helper = _get_cone_size_helper
 
     def post_propagation_hook(
         self,
         engine: "BaseSimulationEngine",
         percent_adopt: float | SpecialPercentAdoptions,
@@ -122,27 +113,65 @@
                     )
             self.announcements = tuple(announcements)
             self.setup_engine(engine)
             engine.ready_to_run_round = 1
         elif propagation_round > 1:
             raise NotImplementedError
 
-    def _get_attacker_asns(self, *args, **kwargs):
+    def _get_attacker_asns(
+        self,
+        override_attacker_asns: Optional[frozenset[int]],
+        engine: Optional["BaseSimulationEngine"],
+        prev_scenario: Optional["Scenario"],
+    ) -> frozenset[int]:
         """Gets attacker ASNs, overriding the valid prefix which has no attackers
 
         There is a very rare case where the attacker can not perform the route leak
         due to a disconnection, which happens around .1% in the CAIDA topology.
         In theory - you could just look at the provider cone of the victim,
         and then the peers of that provider cone (and of the victim itself), and
         then the customer cones of all of those ASes to get the list of possible
         valid attackers. However, we consider the attacker being unable to attack
         in extremely rare cases a valid result, and thus do not change the random
         selection. Doing so would also be a lot slower for a very extreme edge case
         """
-        return Scenario._get_attacker_asns(self, *args, **kwargs)
+
+        assert engine, "Need engine for attacker customer cones"
+        attacker_asns = Scenario._get_attacker_asns(
+            self, override_attacker_asns, engine, prev_scenario
+        )
+        # Stores customer cones of attacker ASNs
+        # used in untrackable func and when selecting victims
+        for attacker_asn in attacker_asns:
+            self._attackers_customer_cones_asns.update(
+                self._get_cone_size_helper(
+                    engine.as_graph.as_dict[attacker_asn],
+                    dict(),
+                ),
+            )
+        return attacker_asns
+
+    def _get_possible_victim_asns(
+        self,
+        engine: "BaseSimulationEngine",
+        percent_adoption: Union[float, SpecialPercentAdoptions],
+        prev_scenario: Optional["Scenario"],
+    ) -> frozenset[int]:
+        """Returns possible victim ASNs, defaulted from config
+
+        Modified to not allow victims to be in attackers customer cone,
+        since if a victim is the customer of leaker, it's not really a leak
+        """
+
+        possible_asns = super()._get_possible_victim_asns(
+            engine, percent_adoption, prev_scenario
+        )
+        # Remove attacker's customer conesfrom possible victims
+        possible_asns = possible_asns.difference(self._attackers_customer_cones_asns)
+        return possible_asns
 
     @property
     def warning_as_groups(self) -> frozenset[str]:
         """Returns a frozenset of ASGroups that should raise a warning"""
 
         return frozenset(
             [
```

### Comparing `bgpy_pkg-7.0.9/bgpy/simulation_framework/scenarios/custom_scenarios/non_routed_prefix_hijack.py` & `bgpy_pkg-7.1.0/bgpy/simulation_framework/scenarios/custom_scenarios/non_routed_prefix_hijack.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/simulation_framework/scenarios/custom_scenarios/non_routed_superprefix_hijack.py` & `bgpy_pkg-7.1.0/bgpy/simulation_framework/scenarios/custom_scenarios/non_routed_superprefix_hijack.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/simulation_framework/scenarios/custom_scenarios/non_routed_superprefix_prefix_hijack.py` & `bgpy_pkg-7.1.0/bgpy/simulation_framework/scenarios/custom_scenarios/non_routed_superprefix_prefix_hijack.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/simulation_framework/scenarios/custom_scenarios/prefix_hijack.py` & `bgpy_pkg-7.1.0/bgpy/simulation_framework/scenarios/custom_scenarios/prefix_hijack.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/simulation_framework/scenarios/custom_scenarios/subprefix_hijack.py` & `bgpy_pkg-7.1.0/bgpy/simulation_framework/scenarios/custom_scenarios/subprefix_hijack.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/simulation_framework/scenarios/custom_scenarios/superprefix_prefix_hijack.py` & `bgpy_pkg-7.1.0/bgpy/simulation_framework/scenarios/custom_scenarios/superprefix_prefix_hijack.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/simulation_framework/scenarios/custom_scenarios/valid_prefix.py` & `bgpy_pkg-7.1.0/bgpy/simulation_framework/scenarios/custom_scenarios/valid_prefix.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/simulation_framework/scenarios/preprocess_anns_funcs.py` & `bgpy_pkg-7.1.0/bgpy/simulation_framework/scenarios/preprocess_anns_funcs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from collections import deque
 from typing import Callable, Optional, TYPE_CHECKING
+import warnings
 
 from bgpy.simulation_engine import BGPFull, ASPA, Pathend
 
 if TYPE_CHECKING:
     from bgpy.as_graphs import AS
     from bgpy.simulation_framework.scenario import Scenario
     from bgpy.simulation_engine import Announcement as Ann, BaseSimulationEngine
@@ -28,15 +29,15 @@
     prev_scenario: Optional["Scenario"],
 ) -> tuple["Ann", ...]:
     """No op, the default preprocessing step"""
 
     return unprocessed_anns
 
 
-def origin_hijack(
+def forged_origin_export_all_hijack(
     self_scenario: "Scenario",
     unprocessed_anns: tuple["Ann", ...],
     engine: Optional["BaseSimulationEngine"],
     prev_scenario: Optional["Scenario"],
 ) -> tuple["Ann", ...]:
     """Makes the attack use an origin hijack to be valid by ROA"""
 
@@ -63,14 +64,24 @@
 
         else:
             processed_anns.append(ann)
 
     return tuple(processed_anns)
 
 
+def origin_hijack(*args, **kwargs):  # type: ignore
+    warnings.warn(
+        "origin_hijack is deprecated and will be removed in a future version."
+        " Please use forged_origin_export_all_hijack instead.",
+        DeprecationWarning,
+        stacklevel=2,
+    )
+    return forged_origin_export_all_hijack(*args, **kwargs)  # type: ignore
+
+
 def shortest_path_export_all_hijack(
     self_scenario: "Scenario",
     unprocessed_anns: tuple["Ann", ...],
     engine: Optional["BaseSimulationEngine"],
     prev_scenario: Optional["Scenario"],
 ) -> tuple["Ann", ...]:
     """Makes the attack use shortest path export all to bypass pathsec protections
@@ -95,15 +106,17 @@
         elif any(
             issubclass(x, ASPA) for x in self_scenario.non_default_asn_cls_dict.values()
         ):
             shortest_as_path = _find_shortest_non_adopting_path_general(
                 valid_ann.origin, self_scenario, engine
             )
         else:
-            return origin_hijack(self_scenario, unprocessed_anns, engine, prev_scenario)
+            return forged_origin_export_all_hijack(
+                self_scenario, unprocessed_anns, engine, prev_scenario
+            )
 
         if shortest_as_path:
             # This can happen if the attacker is the shortest path
             # See shortest_path_export_all_aspa_simple_provider test (27)
             if shortest_as_path[0] == ann.as_path[0] and len(shortest_as_path) > 1:
                 shortest_as_path = shortest_as_path[1:]
             processed_anns.append(
@@ -119,36 +132,37 @@
             )
 
         else:
             processed_anns.append(ann)
     return tuple(processed_anns)
 
 
-def origin_spoofing_hijack(
+def neighbor_spoofing_hijack(
     self_scenario: "Scenario",
     unprocessed_anns: tuple["Ann", ...],
     engine: Optional["BaseSimulationEngine"],
     prev_scenario: Optional["Scenario"],
 ) -> tuple["Ann", ...]:
     """Makes the attack use origin spoofing to be valid by ROA"""
 
+    unprocessed_anns = shortest_path_export_all_hijack(
+        self_scenario, unprocessed_anns, engine, prev_scenario
+    )
     processed_anns = list()
 
-    valid_ann = _get_valid_by_roa_ann(self_scenario.victim_asns, unprocessed_anns)
-
     for ann in unprocessed_anns:
         # If the announcement is from the attacker
-        if ann.invalid_by_roa:
-            if ann.prefix != valid_ann.prefix:
-                raise NotImplementedError("TODO: get the valid origin per prefix")
+        if any(x in ann.as_path for x in self_scenario.attacker_asns):
+            neighbor_asn = ann.as_path[0]
+            assert neighbor_asn in self_scenario.attacker_asns
             # Make the AS path be just the victim
             processed_ann = ann.copy(
                 {
-                    "as_path": (valid_ann.origin,),
-                    "next_hop_asn": ann.origin,
+                    "as_path": tuple(ann.as_path[1:]),
+                    "next_hop_asn": neighbor_asn,
                     # Ann.copy overwrites seed_asn and traceback by default
                     # so include these here to make sure that doesn't happen
                     "seed_asn": ann.seed_asn,
                     "traceback_end": ann.traceback_end,
                 }
             )
             processed_anns.append(processed_ann)
@@ -215,14 +229,20 @@
     assert engine, "mypy"
     root_as_obj = engine.as_graph.as_dict[root_asn]
     for first_provider in root_as_obj.providers:
         # You only need legit origin and their provider, you don't need three
         # for secondary_provider in first_provider.providers:
         #     return (secondary_provider.asn, first_provider.asn, root_asn)
         return (first_provider.asn, root_asn)
+    # Some ASes don't have providers, and are stubs that are peered
+    for first_peer in root_as_obj.peers:
+        return (first_peer.asn, root_asn)
+    # Strange case but it could happen
+    for first_customer in root_as_obj.customers:
+        return (first_customer.asn, root_asn)
     return None
 
 
 def _find_shortest_non_adopting_path_general(
     root_asn: int,
     self_scenario: "Scenario",
     engine: Optional["BaseSimulationEngine"],
```

### Comparing `bgpy_pkg-7.0.9/bgpy/simulation_framework/scenarios/scenario.py` & `bgpy_pkg-7.1.0/bgpy/simulation_framework/scenarios/scenario.py`

 * *Files 1% similar despite different names*

```diff
@@ -390,14 +390,16 @@
         """Sets up engine"""
 
         self.policy_classes_used = engine.setup(
             self.announcements,
             self.scenario_config.BasePolicyCls,
             self.non_default_asn_cls_dict,
             prev_scenario,
+            self.attacker_asns,
+            self.scenario_config.AttackerBasePolicyCls,
         )
 
     ##################
     # Subclass Funcs #
     ##################
 
     @abstractmethod
```

### Comparing `bgpy_pkg-7.0.9/bgpy/simulation_framework/simulation.py` & `bgpy_pkg-7.1.0/bgpy/simulation_framework/simulation.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/simulation_framework/utils.py` & `bgpy_pkg-7.1.0/bgpy/simulation_framework/utils.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/tests/conftest.py` & `bgpy_pkg-7.1.0/bgpy/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/__init__.py` & `bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/as_graph_info_000.py` & `bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/examples/as_graph_info_000.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_000.py` & `bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_000.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_001.py` & `bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_001.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_002.py` & `bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_002.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_003.py` & `bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_003.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_004.py` & `bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_004.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_005.py` & `bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_005.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_006.py` & `bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_006.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_007.py` & `bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_007.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_008.py` & `bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_008.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_009.py` & `bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_009.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_010.py` & `bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_010.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_011.py` & `bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_011.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_012.py` & `bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_012.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,19 +15,19 @@
 
 desc = (
     "Origin prefix hijack thwarting ROV\n"
     "This also demonstrates the loop prevention mechanism at 777"
 )
 
 ex_config_012 = EngineTestConfig(
-    name="ex_012_origin_hijack_rov_simple",
+    name="ex_012_forged_origin_export_all_hijack_rov_simple",
     desc=desc,
     scenario_config=ScenarioConfig(
         ScenarioCls=PrefixHijack,
-        preprocess_anns_func=preprocess_anns_funcs.origin_hijack,
+        preprocess_anns_func=preprocess_anns_funcs.forged_origin_export_all_hijack,
         BasePolicyCls=ROV,
         override_attacker_asns=frozenset({ASNs.ATTACKER.value}),
         override_victim_asns=frozenset({ASNs.VICTIM.value}),
         override_non_default_asn_cls_dict=frozendict({}),
     ),
     as_graph_info=as_graph_info_000,
 )
```

### Comparing `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_013.py` & `bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_015.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 from frozendict import frozendict
 from bgpy.enums import ASNs
 from .as_graph_info_000 import as_graph_info_000
 from bgpy.tests.engine_tests.utils import EngineTestConfig
 
-from bgpy.simulation_engine import (
-    ROV,
-)
+from bgpy.simulation_engine import BGP, PathEnd
 from bgpy.simulation_framework import (
     ScenarioConfig,
     PrefixHijack,
     preprocess_anns_funcs,
 )
 
 
 desc = (
-    "Origin spoofing prefix hijack thwarting ROV\n"
-    "This attack reaches more ASes than just the origin hijack"
+    "Origin prefix hijack with pathend simple\n"
+    "PathEnd checks the end of the path for valid providers\n"
+    "and is thus protected against simple origin hijacks"
 )
 
-ex_config_013 = EngineTestConfig(
-    name="ex_013_origin_spoofing_hijack_rov_simple",
+ex_config_015 = EngineTestConfig(
+    name="ex_015_origin_prefix_hijack_pathend_simple",
     desc=desc,
     scenario_config=ScenarioConfig(
         ScenarioCls=PrefixHijack,
-        preprocess_anns_func=preprocess_anns_funcs.origin_spoofing_hijack,
-        BasePolicyCls=ROV,
+        preprocess_anns_func=preprocess_anns_funcs.forged_origin_export_all_hijack,
+        BasePolicyCls=BGP,
         override_attacker_asns=frozenset({ASNs.ATTACKER.value}),
         override_victim_asns=frozenset({ASNs.VICTIM.value}),
-        override_non_default_asn_cls_dict=frozendict({}),
+        override_non_default_asn_cls_dict=frozendict(
+            {
+                1: PathEnd,
+                ASNs.VICTIM.value: PathEnd,
+            }
+        ),
     ),
     as_graph_info=as_graph_info_000,
 )
```

### Comparing `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_014.py` & `bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_025.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 from frozendict import frozendict
 from bgpy.enums import ASNs
 from .as_graph_info_000 import as_graph_info_000
 from bgpy.tests.engine_tests.utils import EngineTestConfig
 
-from bgpy.simulation_engine import BGP, BGPSec
+from bgpy.simulation_engine import BGP, ASPA
 from bgpy.simulation_framework import (
     ScenarioConfig,
     PrefixHijack,
     preprocess_anns_funcs,
 )
 
 
 desc = (
-    "Origin spoofing prefix hijack with bgpsec simple\n"
-    "BGPSec is security third, which doesn't amount to much\n"
-    "AS 2 is saved, but as long as the chain is broken, AS 5"
-    " is still hijacked"
+    "shortest path export all against ASPASimple from a customer\n"
+    "AS 5 fails to detect the shortest path export all"
 )
 
-ex_config_014 = EngineTestConfig(
-    name="ex_014_origin_spoofing_hijack_bgpsec",
+ex_config_025 = EngineTestConfig(
+    name="ex_025_shortest_path_export_all_aspa_simple_customer",
     desc=desc,
     scenario_config=ScenarioConfig(
         ScenarioCls=PrefixHijack,
-        preprocess_anns_func=preprocess_anns_funcs.origin_spoofing_hijack,
-        BasePolicyCls=BGPSec,
+        preprocess_anns_func=preprocess_anns_funcs.shortest_path_export_all_hijack,
+        BasePolicyCls=BGP,
+        AdoptPolicyCls=ASPA,
         override_attacker_asns=frozenset({ASNs.ATTACKER.value}),
         override_victim_asns=frozenset({ASNs.VICTIM.value}),
         override_non_default_asn_cls_dict=frozendict(
             {
-                ASNs.ATTACKER.value: BGP,
+                2: ASPA,
+                5: ASPA,
+                10: ASPA,
+                ASNs.VICTIM.value: ASPA,
             }
         ),
     ),
     as_graph_info=as_graph_info_000,
 )
```

### Comparing `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_015.py` & `bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_016.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 from frozendict import frozendict
 from bgpy.enums import ASNs
 from .as_graph_info_000 import as_graph_info_000
 from bgpy.tests.engine_tests.utils import EngineTestConfig
 
-from bgpy.simulation_engine import BGP, Pathend
+from bgpy.simulation_engine import BGP, PathEndFull
 from bgpy.simulation_framework import (
     ScenarioConfig,
     PrefixHijack,
     preprocess_anns_funcs,
 )
 
 
 desc = (
-    "Origin prefix hijack with pathend simple\n"
-    "Pathend checks the end of the path for valid providers\n"
+    "Origin prefix hijack with pathend\n"
+    "PathEnd checks the end of the path for valid providers\n"
     "and is thus protected against simple origin hijacks"
 )
 
-ex_config_015 = EngineTestConfig(
-    name="ex_015_origin_prefix_hijack_pathend_simple",
+ex_config_016 = EngineTestConfig(
+    name="ex_016_origin_prefix_hijack_pathend",
     desc=desc,
     scenario_config=ScenarioConfig(
         ScenarioCls=PrefixHijack,
-        preprocess_anns_func=preprocess_anns_funcs.origin_hijack,
+        preprocess_anns_func=preprocess_anns_funcs.forged_origin_export_all_hijack,
         BasePolicyCls=BGP,
         override_attacker_asns=frozenset({ASNs.ATTACKER.value}),
         override_victim_asns=frozenset({ASNs.VICTIM.value}),
         override_non_default_asn_cls_dict=frozendict(
             {
-                1: Pathend,
-                ASNs.VICTIM.value: Pathend,
+                1: PathEndFull,
+                ASNs.VICTIM.value: PathEndFull,
             }
         ),
     ),
     as_graph_info=as_graph_info_000,
 )
```

### Comparing `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_016.py` & `bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_024.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 from frozendict import frozendict
 from bgpy.enums import ASNs
 from .as_graph_info_000 import as_graph_info_000
 from bgpy.tests.engine_tests.utils import EngineTestConfig
 
-from bgpy.simulation_engine import BGP, PathendFull
+from bgpy.simulation_engine import BGPFull, ASPAFull
 from bgpy.simulation_framework import (
     ScenarioConfig,
-    PrefixHijack,
+    SubprefixHijack,
     preprocess_anns_funcs,
 )
 
 
 desc = (
-    "Origin prefix hijack with pathend\n"
-    "Pathend checks the end of the path for valid providers\n"
-    "and is thus protected against simple origin hijacks"
+    "subprefix origin hijack against ASPA\n"
+    "This isn't realistic, just for testing to test the downstream"
+    "Use the subprefix to check"
 )
 
-ex_config_016 = EngineTestConfig(
-    name="ex_016_origin_prefix_hijack_pathend",
+ex_config_024 = EngineTestConfig(
+    name="ex_024_subprefix_forged_origin_export_all_hijack_aspa_downstream_verification",
     desc=desc,
     scenario_config=ScenarioConfig(
-        ScenarioCls=PrefixHijack,
-        preprocess_anns_func=preprocess_anns_funcs.origin_hijack,
-        BasePolicyCls=BGP,
+        ScenarioCls=SubprefixHijack,
+        preprocess_anns_func=preprocess_anns_funcs.forged_origin_export_all_hijack,
+        BasePolicyCls=BGPFull,
         override_attacker_asns=frozenset({ASNs.ATTACKER.value}),
         override_victim_asns=frozenset({ASNs.VICTIM.value}),
         override_non_default_asn_cls_dict=frozendict(
             {
-                1: PathendFull,
-                ASNs.VICTIM.value: PathendFull,
+                2: ASPAFull,
+                10: ASPAFull,
+                ASNs.VICTIM.value: ASPAFull,
             }
         ),
     ),
     as_graph_info=as_graph_info_000,
 )
```

### Comparing `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_017.py` & `bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_017.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 from frozendict import frozendict
 from bgpy.enums import ASNs
 from .as_graph_info_000 import as_graph_info_000
 from bgpy.tests.engine_tests.utils import EngineTestConfig
 
-from bgpy.simulation_engine import BGP, Pathend
+from bgpy.simulation_engine import BGP, PathEnd
 from bgpy.simulation_framework import (
     ScenarioConfig,
     PrefixHijack,
     preprocess_anns_funcs,
 )
 
 
 desc = (
     "shortest path export all attack against pathend simple\n"
-    "Pathend checks the end of the path for valid providers\n"
+    "PathEnd checks the end of the path for valid providers\n"
     "so anything beyond the third AS is not protected"
 )
 
 ex_config_017 = EngineTestConfig(
     name="ex_017_shortest_path_export_all_pathend_simple",
     desc=desc,
     scenario_config=ScenarioConfig(
         ScenarioCls=PrefixHijack,
         preprocess_anns_func=preprocess_anns_funcs.shortest_path_export_all_hijack,
         BasePolicyCls=BGP,
         override_attacker_asns=frozenset({ASNs.ATTACKER.value}),
         override_victim_asns=frozenset({ASNs.VICTIM.value}),
         override_non_default_asn_cls_dict=frozendict(
             {
-                1: Pathend,
-                ASNs.VICTIM.value: Pathend,
+                1: PathEnd,
+                ASNs.VICTIM.value: PathEnd,
             }
         ),
     ),
     as_graph_info=as_graph_info_000,
 )
```

### Comparing `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_018.py` & `bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_018.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 from frozendict import frozendict
 from bgpy.enums import ASNs
 from .as_graph_info_000 import as_graph_info_000
 from bgpy.tests.engine_tests.utils import EngineTestConfig
 
-from bgpy.simulation_engine import BGP, Pathend
+from bgpy.simulation_engine import BGP, PathEnd
 from bgpy.simulation_framework import (
     ScenarioConfig,
     AccidentalRouteLeak,
     preprocess_anns_funcs,
 )
 
 
 desc = (
     "accidental route leak against pathend simple\n"
-    "Pathend checks the end of the path for valid providers\n"
+    "PathEnd checks the end of the path for valid providers\n"
     "so anything beyond the third AS is not protected"
 )
 
 ex_config_018 = EngineTestConfig(
     name="ex_018_route_leak_pathend_simple",
     desc=desc,
     scenario_config=ScenarioConfig(
         ScenarioCls=AccidentalRouteLeak,
         preprocess_anns_func=preprocess_anns_funcs.noop,
         BasePolicyCls=BGP,
         override_attacker_asns=frozenset({ASNs.ATTACKER.value}),
         override_victim_asns=frozenset({ASNs.VICTIM.value}),
         override_non_default_asn_cls_dict=frozendict(
             {
-                1: Pathend,
-                ASNs.VICTIM.value: Pathend,
+                1: PathEnd,
+                ASNs.VICTIM.value: PathEnd,
             }
         ),
     ),
     as_graph_info=as_graph_info_000,
 )
```

### Comparing `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_019.py` & `bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_019.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_020.py` & `bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_020.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_021.py` & `bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_021.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_022.py` & `bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_022.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_023.py` & `bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_023.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 )
 
 ex_config_023 = EngineTestConfig(
     name="ex_023_subprefix_origin_aspa_simple_downstream_verification",
     desc=desc,
     scenario_config=ScenarioConfig(
         ScenarioCls=SubprefixHijack,
-        preprocess_anns_func=preprocess_anns_funcs.origin_hijack,
+        preprocess_anns_func=preprocess_anns_funcs.forged_origin_export_all_hijack,
         BasePolicyCls=BGP,
         override_attacker_asns=frozenset({ASNs.ATTACKER.value}),
         override_victim_asns=frozenset({ASNs.VICTIM.value}),
         override_non_default_asn_cls_dict=frozendict(
             {
                 2: ASPA,
                 10: ASPA,
```

### Comparing `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_024.py` & `bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_027.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,45 @@
 from frozendict import frozendict
 from bgpy.enums import ASNs
 from .as_graph_info_000 import as_graph_info_000
 from bgpy.tests.engine_tests.utils import EngineTestConfig
 
-from bgpy.simulation_engine import BGPFull, ASPAFull
+from bgpy.simulation_engine import BGP, ASPA
 from bgpy.simulation_framework import (
     ScenarioConfig,
-    SubprefixHijack,
+    PrefixHijack,
     preprocess_anns_funcs,
 )
 
 
 desc = (
-    "subprefix origin hijack against ASPA\n"
-    "This isn't realistic, just for testing to test the downstream"
-    "Use the subprefix to check"
+    "shortest path export all against ASPASimple from a provider\n"
+    "AS prevents the attack, this is merely to check attack functionality"
 )
 
-ex_config_024 = EngineTestConfig(
-    name="ex_024_subprefix_origin_hijack_aspa_downstream_verification",
+ex_config_027 = EngineTestConfig(
+    name="ex_027_shortest_path_export_all_aspa_simple_provider",
     desc=desc,
     scenario_config=ScenarioConfig(
-        ScenarioCls=SubprefixHijack,
-        preprocess_anns_func=preprocess_anns_funcs.origin_hijack,
-        BasePolicyCls=BGPFull,
+        ScenarioCls=PrefixHijack,
+        preprocess_anns_func=preprocess_anns_funcs.shortest_path_export_all_hijack,
+        BasePolicyCls=BGP,
+        AdoptPolicyCls=ASPA,
         override_attacker_asns=frozenset({ASNs.ATTACKER.value}),
         override_victim_asns=frozenset({ASNs.VICTIM.value}),
         override_non_default_asn_cls_dict=frozendict(
             {
-                2: ASPAFull,
-                10: ASPAFull,
-                ASNs.VICTIM.value: ASPAFull,
+                2: ASPA,
+                3: ASPA,
+                4: ASPA,
+                5: ASPA,
+                8: ASPA,
+                9: ASPA,
+                10: ASPA,
+                11: ASPA,
+                12: ASPA,
+                ASNs.VICTIM.value: ASPA,
             }
         ),
     ),
     as_graph_info=as_graph_info_000,
 )
```

### Comparing `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_025.py` & `bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_028.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,38 +2,46 @@
 from bgpy.enums import ASNs
 from .as_graph_info_000 import as_graph_info_000
 from bgpy.tests.engine_tests.utils import EngineTestConfig
 
 from bgpy.simulation_engine import BGP, ASPA
 from bgpy.simulation_framework import (
     ScenarioConfig,
-    PrefixHijack,
+    AccidentalRouteLeak,
     preprocess_anns_funcs,
 )
 
 
 desc = (
-    "shortest path export all against ASPASimple from a customer\n"
-    "AS 5 fails to detect the shortest path export all"
+    "Route leak to check when v_max_complement==u_min\n"
+    " (this is merely to check functionality)"
 )
 
-ex_config_025 = EngineTestConfig(
-    name="ex_025_shortest_path_export_all_aspa_simple_customer",
+ex_config_028 = EngineTestConfig(
+    name="ex_028_route_leak_aspa_simple_u_min_v_max_check",
     desc=desc,
     scenario_config=ScenarioConfig(
-        ScenarioCls=PrefixHijack,
-        preprocess_anns_func=preprocess_anns_funcs.shortest_path_export_all_hijack,
+        ScenarioCls=AccidentalRouteLeak,
+        preprocess_anns_func=preprocess_anns_funcs.noop,
         BasePolicyCls=BGP,
         AdoptPolicyCls=ASPA,
         override_attacker_asns=frozenset({ASNs.ATTACKER.value}),
         override_victim_asns=frozenset({ASNs.VICTIM.value}),
         override_non_default_asn_cls_dict=frozendict(
             {
+                1: ASPA,
                 2: ASPA,
+                3: ASPA,
+                4: ASPA,
                 5: ASPA,
+                8: ASPA,
+                9: ASPA,
                 10: ASPA,
+                11: ASPA,
+                12: ASPA,
                 ASNs.VICTIM.value: ASPA,
+                ASNs.ATTACKER.value: ASPA,
             }
         ),
     ),
     as_graph_info=as_graph_info_000,
 )
```

### Comparing `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_026.py` & `bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_026.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_027.py` & `bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/internals/internal_config_003.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,45 +1,48 @@
 from frozendict import frozendict
-from bgpy.enums import ASNs
-from .as_graph_info_000 import as_graph_info_000
 from bgpy.tests.engine_tests.utils import EngineTestConfig
 
-from bgpy.simulation_engine import BGP, ASPA
+
+from bgpy.simulation_engine import BGP, OnlyToCustomers
 from bgpy.simulation_framework import (
+    AccidentalRouteLeak,
     ScenarioConfig,
-    PrefixHijack,
-    preprocess_anns_funcs,
 )
+from bgpy.enums import ASNs
+
+from bgpy.as_graphs import PeerLink
+from bgpy.as_graphs import ASGraphInfo
+
 
+r"""Graph to test OTC from a peer
 
-desc = (
-    "shortest path export all against ASPASimple from a provider\n"
-    "AS prevents the attack, this is merely to check attack functionality"
+777 - 666 - 1
+"""
+
+as_graph_info = ASGraphInfo(
+    peer_links=frozenset(
+        [
+            PeerLink(ASNs.VICTIM.value, ASNs.ATTACKER.value),
+            PeerLink(ASNs.ATTACKER.value, 1),
+        ]
+    ),
+    customer_provider_links=frozenset(),
 )
 
-ex_config_027 = EngineTestConfig(
-    name="ex_027_shortest_path_export_all_aspa_simple_provider",
-    desc=desc,
+
+internal_config_003 = EngineTestConfig(
+    name="internal_003",
+    desc="Accidental route leak to a peer with OTC Simple",
     scenario_config=ScenarioConfig(
-        ScenarioCls=PrefixHijack,
-        preprocess_anns_func=preprocess_anns_funcs.shortest_path_export_all_hijack,
+        ScenarioCls=AccidentalRouteLeak,
         BasePolicyCls=BGP,
-        AdoptPolicyCls=ASPA,
-        override_attacker_asns=frozenset({ASNs.ATTACKER.value}),
         override_victim_asns=frozenset({ASNs.VICTIM.value}),
+        override_attacker_asns=frozenset({ASNs.ATTACKER.value}),
         override_non_default_asn_cls_dict=frozendict(
             {
-                2: ASPA,
-                3: ASPA,
-                4: ASPA,
-                5: ASPA,
-                8: ASPA,
-                9: ASPA,
-                10: ASPA,
-                11: ASPA,
-                12: ASPA,
-                ASNs.VICTIM.value: ASPA,
+                1: OnlyToCustomers,
+                ASNs.VICTIM.value: OnlyToCustomers,
             }
         ),
     ),
-    as_graph_info=as_graph_info_000,
+    as_graph_info=as_graph_info,
 )
```

### Comparing `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_029.py` & `bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_029.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 desc = "ASPA weirdness. rejects upstream, accepts downstream"
 
 ex_config_029 = EngineTestConfig(
     name="ex_029_aspa_weirdness",
     desc=desc,
     scenario_config=ScenarioConfig(
         ScenarioCls=PrefixHijack,
-        preprocess_anns_func=preprocess_anns_funcs.origin_hijack,
+        preprocess_anns_func=preprocess_anns_funcs.forged_origin_export_all_hijack,
         BasePolicyCls=BGP,
         AdoptPolicyCls=ASPA,
         override_attacker_asns=frozenset({ASNs.ATTACKER.value}),
         override_victim_asns=frozenset({ASNs.VICTIM.value}),
         override_non_default_asn_cls_dict=frozendict(
             {
                 4: ASPA,
```

### Comparing `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/internals/internal_config_000.py` & `bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/internals/internal_config_000.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/internals/internal_config_001.py` & `bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/internals/internal_config_001.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/internals/internal_config_002.py` & `bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/internals/internal_config_002.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/internals/internal_config_004.py` & `bgpy_pkg-7.1.0/bgpy/tests/engine_tests/engine_test_configs/internals/internal_config_004.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     desc=(
         "ASPA RFC Section 12. "
         " Previously this diagram used to show an off by 1 bug for ASPA, so we"
         " prevent it from popping up again"
     ),
     scenario_config=ScenarioConfig(
         ScenarioCls=PrefixHijack,
-        preprocess_anns_func=preprocess_anns_funcs.origin_hijack,
+        preprocess_anns_func=preprocess_anns_funcs.forged_origin_export_all_hijack,
         BasePolicyCls=BGP,
         override_victim_asns=frozenset({ASNs.VICTIM.value}),
         override_attacker_asns=frozenset({ASNs.ATTACKER.value}),
         override_non_default_asn_cls_dict=frozendict(
             {
                 1: ASPA,
                 2: ASPA,
```

### Comparing `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/test_engine.py` & `bgpy_pkg-7.1.0/bgpy/tests/engine_tests/test_engine.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/utils/diagram_aggregator.py` & `bgpy_pkg-7.1.0/bgpy/tests/engine_tests/utils/diagram_aggregator.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/utils/engine_test_config.py` & `bgpy_pkg-7.1.0/bgpy/tests/engine_tests/utils/engine_test_config.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/utils/engine_tester.py` & `bgpy_pkg-7.1.0/bgpy/tests/engine_tests/utils/engine_tester.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/tests/framework_tests/system_tests/test_sim_inputs.py` & `bgpy_pkg-7.1.0/bgpy/tests/framework_tests/system_tests/test_sim_inputs.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/tests/framework_tests/unit_tests/test_scenario.py` & `bgpy_pkg-7.1.0/bgpy/tests/framework_tests/unit_tests/test_scenario.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/utils/diagram.py` & `bgpy_pkg-7.1.0/bgpy/utils/diagram.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/utils/engine_run_config.py` & `bgpy_pkg-7.1.0/bgpy/utils/engine_run_config.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/utils/engine_runner.py` & `bgpy_pkg-7.1.0/bgpy/utils/engine_runner.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy/utils/simulator_codec/simulator_codec.py` & `bgpy_pkg-7.1.0/bgpy/utils/simulator_codec/simulator_codec.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.9/bgpy_pkg.egg-info/PKG-INFO` & `bgpy_pkg-7.1.0/bgpy_pkg.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bgpy_pkg
-Version: 7.0.9
+Version: 7.1.0
 Summary: Simulates BGP and ROV in an extensible manner
 Author-email: Justin Furuness <jfuruness@gmail.com>, Cameron Morris <cameron.morris@uconn.edu>, Reynaldo Morillo <reynaldo.morillo@uconn.edu>, Arvind Kasiliya <arvind.kasiliya@uconn.edu>
 Maintainer-email: Justin Furuness <jfuruness@gmail.com>
 License: Copyright 2020 Justin Furuness
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
```

### Comparing `bgpy_pkg-7.0.9/bgpy_pkg.egg-info/SOURCES.txt` & `bgpy_pkg-7.1.0/bgpy_pkg.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,17 @@
 bgpy/simulation_engine/policies/bgp/bgp_full/propagate_funcs.py
 bgpy/simulation_engine/policies/bgpsec/__init__.py
 bgpy/simulation_engine/policies/bgpsec/bgpsec.py
 bgpy/simulation_engine/policies/bgpsec/bgpsec_full.py
 bgpy/simulation_engine/policies/only_to_customers/__init__.py
 bgpy/simulation_engine/policies/only_to_customers/only_to_customers.py
 bgpy/simulation_engine/policies/only_to_customers/only_to_customers_full.py
+bgpy/simulation_engine/policies/path_end/__init__.py
+bgpy/simulation_engine/policies/path_end/path_end.py
+bgpy/simulation_engine/policies/path_end/path_end_full.py
 bgpy/simulation_engine/policies/pathend/__init__.py
 bgpy/simulation_engine/policies/pathend/pathend.py
 bgpy/simulation_engine/policies/pathend/pathend_full.py
 bgpy/simulation_engine/policies/rov/__init__.py
 bgpy/simulation_engine/policies/rov/peer_rov.py
 bgpy/simulation_engine/policies/rov/peer_rov_full.py
 bgpy/simulation_engine/policies/rov/rov.py
```

### Comparing `bgpy_pkg-7.0.9/pyproject.toml` & `bgpy_pkg-7.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=69.0.3", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bgpy_pkg"
-version = "7.0.9"
+version = "7.1.0"
 requires-python = ">=3.10"
 description = "Simulates BGP and ROV in an extensible manner"
 readme = "README.md"
 authors = [
     {name = "Justin Furuness", email = "jfuruness@gmail.com"},
     {name = "Cameron Morris", email = "cameron.morris@uconn.edu"},
     {name = "Reynaldo Morillo", email = "reynaldo.morillo@uconn.edu"},
```

### Comparing `bgpy_pkg-7.0.9/tox.ini` & `bgpy_pkg-7.1.0/tox.ini`

 * *Files identical despite different names*

