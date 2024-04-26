# Comparing `tmp/byteblower_test_cases_low_latency-1.2.0.tar.gz` & `tmp/byteblower_test_cases_low_latency-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "byteblower_test_cases_low_latency-1.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "byteblower_test_cases_low_latency-1.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `byteblower_test_cases_low_latency-1.2.0.tar` & `byteblower_test_cases_low_latency-1.2.1.tar`

### file list

```diff
@@ -1,96 +1,96 @@
--rw-r--r--   0        0        0     8285 2024-02-14 16:30:13.265648 byteblower_test_cases_low_latency-1.2.0/README.rst
--rw-r--r--   0        0        0       45 2024-01-19 09:10:52.489868 byteblower_test_cases_low_latency-1.2.0/byteblower/test_cases/low_latency/.gitignore
--rw-r--r--   0        0        0      209 2024-01-19 09:10:52.489868 byteblower_test_cases_low_latency-1.2.0/byteblower/test_cases/low_latency/__init__.py
--rw-r--r--   0        0        0      349 2024-01-19 09:10:52.489868 byteblower_test_cases_low_latency-1.2.0/byteblower/test_cases/low_latency/__main__.py
--rw-r--r--   0        0        0     3547 2024-01-26 10:35:09.820403 byteblower_test_cases_low_latency-1.2.0/byteblower/test_cases/low_latency/_arguments.py
--rw-r--r--   0        0        0      694 2024-01-26 07:43:21.626476 byteblower_test_cases_low_latency-1.2.0/byteblower/test_cases/low_latency/_config_file.py
--rw-r--r--   0        0        0      951 2024-01-26 07:43:21.626476 byteblower_test_cases_low_latency-1.2.0/byteblower/test_cases/low_latency/_definitions.py
--rw-r--r--   0        0        0     2892 2024-01-26 10:35:09.820403 byteblower_test_cases_low_latency-1.2.0/byteblower/test_cases/low_latency/_endpoint_factory.py
--rw-r--r--   0        0        0    23052 2024-02-14 14:42:04.508950 byteblower_test_cases_low_latency-1.2.0/byteblower/test_cases/low_latency/_flow_factory.py
--rw-r--r--   0        0        0    17577 2024-01-26 10:35:09.820403 byteblower_test_cases_low_latency-1.2.0/byteblower/test_cases/low_latency/_lld.py
--rw-r--r--   0        0        0     2466 2024-01-26 10:35:09.820403 byteblower_test_cases_low_latency-1.2.0/byteblower/test_cases/low_latency/_port_factory.py
--rw-r--r--   0        0        0     1607 2024-01-26 10:35:09.820403 byteblower_test_cases_low_latency-1.2.0/byteblower/test_cases/low_latency/_scouting_flow.py
--rw-r--r--   0        0        0     5532 2024-01-26 10:35:09.820403 byteblower_test_cases_low_latency-1.2.0/byteblower/test_cases/low_latency/_stream_data_gatherer.py
--rw-r--r--   0        0        0      160 2024-02-14 17:33:31.336191 byteblower_test_cases_low_latency-1.2.0/byteblower/test_cases/low_latency/_version.py
--rw-r--r--   0        0        0     1348 2024-01-19 09:10:52.637868 byteblower_test_cases_low_latency-1.2.0/byteblower/test_cases/low_latency/cli.py
--rw-r--r--   0        0        0     3863 2024-01-26 10:35:09.820403 byteblower_test_cases_low_latency-1.2.0/byteblower/test_cases/low_latency/csvaggregator.py
--rw-r--r--   0        0        0     9835 2024-01-26 10:35:09.820403 byteblower_test_cases_low_latency-1.2.0/byteblower/test_cases/low_latency/dynamic_frameblastingflow.py
--rw-r--r--   0        0        0      737 2024-01-26 07:43:21.626476 byteblower_test_cases_low_latency-1.2.0/byteblower/test_cases/low_latency/exceptions.py
--rw-r--r--   0        0        0     9710 2024-01-26 10:35:09.820403 byteblower_test_cases_low_latency-1.2.0/byteblower/test_cases/low_latency/l4s_analysers.py
--rw-r--r--   0        0        0     7768 2024-01-26 10:35:09.820403 byteblower_test_cases_low_latency-1.2.0/byteblower/test_cases/low_latency/l4s_frameblastingflow.py
--rw-r--r--   0        0        0    16781 2024-01-26 10:35:09.820403 byteblower_test_cases_low_latency-1.2.0/byteblower/test_cases/low_latency/outlier_latency_cdf_analyser.py
--rw-r--r--   0        0        0        7 2024-01-19 09:10:52.637868 byteblower_test_cases_low_latency-1.2.0/docs/.gitignore
--rw-r--r--   0        0        0      638 2024-01-19 09:10:52.637868 byteblower_test_cases_low_latency-1.2.0/docs/Makefile
--rw-r--r--   0        0        0      804 2024-01-26 07:43:21.626476 byteblower_test_cases_low_latency-1.2.0/docs/make.bat
--rw-r--r--   0        0        0       51 2024-02-13 21:45:37.219869 byteblower_test_cases_low_latency-1.2.0/docs/source/.gitignore
--rw-r--r--   0        0        0      919 2024-01-26 07:43:21.626476 byteblower_test_cases_low_latency-1.2.0/docs/source/_include/_example_test_scenario.rst
--rw-r--r--   0        0        0        0 2024-02-14 17:33:00.480240 byteblower_test_cases_low_latency-1.2.0/docs/source/_static/.gitkeep
--rw-r--r--   0        0        0      301 2024-02-07 15:37:24.763645 byteblower_test_cases_low_latency-1.2.0/docs/source/_static/excentis.css
--rw-r--r--   0        0        0     4044 2024-01-30 13:14:51.999661 byteblower_test_cases_low_latency-1.2.0/docs/source/cli/index.rst
--rw-r--r--   0        0        0    10127 2024-02-14 17:28:53.316720 byteblower_test_cases_low_latency-1.2.0/docs/source/conf.py
--rw-r--r--   0        0        0     3606 2024-02-01 14:08:19.067705 byteblower_test_cases_low_latency-1.2.0/docs/source/config/conference.rst
--rw-r--r--   0        0        0     1752 2024-01-26 07:43:21.874477 byteblower_test_cases_low_latency-1.2.0/docs/source/config/dynamic_frame_blasting.rst
--rw-r--r--   0        0        0     2071 2024-01-26 07:43:21.874477 byteblower_test_cases_low_latency-1.2.0/docs/source/config/frame_blasting.rst
--rw-r--r--   0        0        0     1347 2024-01-26 07:43:21.874477 byteblower_test_cases_low_latency-1.2.0/docs/source/config/gaming.rst
--rw-r--r--   0        0        0     1146 2024-02-01 14:08:19.067705 byteblower_test_cases_low_latency-1.2.0/docs/source/config/http.rst
--rw-r--r--   0        0        0     5909 2024-01-30 13:14:51.999661 byteblower_test_cases_low_latency-1.2.0/docs/source/config/index.rst
--rw-r--r--   0        0        0     1537 2024-01-26 07:43:21.874477 byteblower_test_cases_low_latency-1.2.0/docs/source/config/l4s_frame_blasting.rst
--rw-r--r--   0        0        0      823 2024-01-26 07:43:21.874477 byteblower_test_cases_low_latency-1.2.0/docs/source/config/video.rst
--rw-r--r--   0        0        0     1352 2024-01-26 07:43:21.874477 byteblower_test_cases_low_latency-1.2.0/docs/source/config/voice.rst
--rw-r--r--   0        0        0    10940 2024-02-14 16:55:34.658653 byteblower_test_cases_low_latency-1.2.0/docs/source/examples/basic.rst
--rw-r--r--   0        0        0     3019 2024-02-14 16:55:34.658653 byteblower_test_cases_low_latency-1.2.0/docs/source/examples/index.rst
--rw-r--r--   0        0        0    15425 2024-02-14 16:55:34.658653 byteblower_test_cases_low_latency-1.2.0/docs/source/examples/l4s.rst
--rw-r--r--   0        0        0    69694 2024-02-01 14:08:19.067705 byteblower_test_cases_low_latency-1.2.0/docs/source/extra/test-cases/low-latency/json/config-schema.json
--rw-r--r--   0        0        0     2543 2024-02-13 13:42:29.704225 byteblower_test_cases_low_latency-1.2.0/docs/source/extra/test-cases/low-latency/json/endpoint/low_latency.json
--rw-r--r--   0        0        0     3279 2024-02-14 16:45:23.959753 byteblower_test_cases_low_latency-1.2.0/docs/source/extra/test-cases/low-latency/json/l4s/endpoint/low_latency.json
--rw-r--r--   0        0        0     3244 2024-02-14 15:59:45.889410 byteblower_test_cases_low_latency-1.2.0/docs/source/extra/test-cases/low-latency/json/l4s/port/low_latency.json
--rw-r--r--   0        0        0     2508 2024-02-13 13:42:29.704225 byteblower_test_cases_low_latency-1.2.0/docs/source/extra/test-cases/low-latency/json/port/low_latency.json
--rw-r--r--   0        0        0    13413 2024-02-14 14:51:11.716298 byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/intermediate/html_report_config.png
--rw-r--r--   0        0        0   130059 2024-02-14 14:51:11.716298 byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/intermediate/html_report_correlated.png
--rw-r--r--   0        0        0    31733 2024-02-14 14:51:11.716298 byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/intermediate/html_report_gaming_config.png
--rw-r--r--   0        0        0    35064 2024-02-14 14:51:11.716298 byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/intermediate/html_report_gaming_graph.png
--rw-r--r--   0        0        0    30909 2024-02-14 14:51:11.716298 byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/intermediate/html_report_gaming_stats.png
--rw-r--r--   0        0        0     6520 2024-02-14 14:51:11.716298 byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/intermediate/html_report_http_analysis.png
--rw-r--r--   0        0        0   119366 2024-02-14 14:51:11.720298 byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/intermediate/html_report_http_graph.png
--rw-r--r--   0        0        0    15992 2024-02-14 14:51:11.720298 byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/intermediate/html_report_status_and_env.png
--rw-r--r--   0        0        0    37591 2024-02-14 14:51:11.720298 byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/intermediate/html_report_udp_graph.png
--rw-r--r--   0        0        0    31901 2024-02-14 14:51:11.720298 byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/intermediate/html_report_udp_stats.png
--rw-r--r--   0        0        0     4985 2024-02-14 14:51:11.720298 byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/intermediate/html_report_udp_status.png
--rw-r--r--   0        0        0   103787 2024-02-14 14:51:11.720298 byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/intermediate/html_report_voice_graph.png
--rw-r--r--   0        0        0    49844 2024-02-14 14:51:11.720298 byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/intermediate/html_report_voice_stats.png
--rw-r--r--   0        0        0     4813 2024-02-14 14:51:11.720298 byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/intermediate/html_report_voice_status.png
--rw-r--r--   0        0        0    14102 2024-02-14 14:51:11.720298 byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/l4s_intermediate/html_report_config.png
--rw-r--r--   0        0        0    41474 2024-02-14 15:35:43.243404 byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/l4s_intermediate/html_report_correlated_ccdf.png
--rw-r--r--   0        0        0   176999 2024-02-14 15:35:43.243404 byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/l4s_intermediate/html_report_correlated_thr.png
--rw-r--r--   0        0        0    38345 2024-02-14 14:51:11.724298 byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/l4s_intermediate/html_report_flow_run.png
--rw-r--r--   0        0        0   127248 2024-02-14 15:35:43.247404 byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/l4s_intermediate/html_report_gaming_ccdf.png
--rw-r--r--   0        0        0   193678 2024-02-14 15:35:43.247404 byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/l4s_intermediate/html_report_gaming_loss.png
--rw-r--r--   0        0        0    12703 2024-02-14 15:35:43.247404 byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/l4s_intermediate/html_report_http_analysis.png
--rw-r--r--   0        0        0    19459 2024-02-14 15:35:43.247404 byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/l4s_intermediate/html_report_http_config.png
--rw-r--r--   0        0        0   128409 2024-02-14 15:35:43.251404 byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/l4s_intermediate/html_report_http_graph.png
--rw-r--r--   0        0        0    13367 2024-02-14 15:35:43.251404 byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/l4s_intermediate/html_report_l4s_http_analysis.png
--rw-r--r--   0        0        0   121304 2024-02-14 15:35:43.251404 byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/l4s_intermediate/html_report_l4s_http_graph.png
--rw-r--r--   0        0        0    14841 2024-02-14 14:51:11.732298 byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/l4s_intermediate/html_report_status_and_env.png
--rw-r--r--   0        0        0    40577 2024-02-14 15:35:43.251404 byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/l4s_intermediate/html_report_udp_cdf_graph.png
--rw-r--r--   0        0        0    42790 2024-02-14 15:35:43.251404 byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/l4s_intermediate/html_report_udp_cdf_status_and_stats.png
--rw-r--r--   0        0        0    41786 2024-02-14 15:35:43.251404 byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/l4s_intermediate/html_report_udp_loss_analyser.png
--rw-r--r--   0        0        0    96583 2024-02-14 15:35:43.255404 byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/l4s_intermediate/html_report_udp_loss_graph.png
--rw-r--r--   0        0        0    39276 2024-02-14 15:35:43.255404 byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/l4s_intermediate/html_report_udp_loss_stats.png
--rw-r--r--   0        0        0   101406 2024-02-14 15:35:43.255404 byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/l4s_intermediate/html_report_voice_graph.png
--rw-r--r--   0        0        0    64833 2024-02-14 15:35:43.255404 byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/l4s_intermediate/html_report_voice_stats.png
--rw-r--r--   0        0        0    13457 2024-02-14 15:35:43.255404 byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/l4s_intermediate/html_report_voice_status.png
--rw-r--r--   0        0        0   136289 2024-01-26 07:43:21.878477 byteblower_test_cases_low_latency-1.2.0/docs/source/images/html_report_Loss_latency_analyser.png
--rw-r--r--   0        0        0   124331 2024-01-26 07:43:21.878477 byteblower_test_cases_low_latency-1.2.0/docs/source/images/html_report_aggregated_results.png
--rw-r--r--   0        0        0    24588 2024-01-26 07:43:21.878477 byteblower_test_cases_low_latency-1.2.0/docs/source/images/html_report_config.png
--rw-r--r--   0        0        0    33492 2024-01-26 07:43:21.878477 byteblower_test_cases_low_latency-1.2.0/docs/source/images/html_report_config_table.png
--rw-r--r--   0        0        0    56307 2024-01-26 07:43:21.878477 byteblower_test_cases_low_latency-1.2.0/docs/source/images/html_report_http_analyser.png
--rw-r--r--   0        0        0    75988 2024-01-26 07:43:21.878477 byteblower_test_cases_low_latency-1.2.0/docs/source/images/html_report_latency.png
--rw-r--r--   0        0        0    90900 2024-01-26 07:43:21.882477 byteblower_test_cases_low_latency-1.2.0/docs/source/images/html_report_latency_sum.png
--rw-r--r--   0        0        0   120807 2024-01-26 07:43:21.882477 byteblower_test_cases_low_latency-1.2.0/docs/source/images/html_report_loss_analyser.png
--rw-r--r--   0        0        0   156060 2024-02-14 16:08:22.548877 byteblower_test_cases_low_latency-1.2.0/docs/source/images/l4s_graph_over_time.png
--rw-r--r--   0        0        0      446 2024-02-14 15:54:22.285418 byteblower_test_cases_low_latency-1.2.0/docs/source/index.rst
--rw-r--r--   0        0        0      570 2024-02-14 16:55:34.658653 byteblower_test_cases_low_latency-1.2.0/docs/source/master_index.rst
--rw-r--r--   0        0        0     4909 2024-02-14 17:28:53.316720 byteblower_test_cases_low_latency-1.2.0/docs/source/overview.rst
--rw-r--r--   0        0        0     6223 2024-01-26 07:43:21.882477 byteblower_test_cases_low_latency-1.2.0/docs/source/quick_start.rst
--rw-r--r--   0        0        0     8263 2024-02-14 17:28:53.316720 byteblower_test_cases_low_latency-1.2.0/pyproject.toml
--rw-r--r--   0        0        0    11153 1970-01-01 00:00:00.000000 byteblower_test_cases_low_latency-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     8287 2024-04-25 18:56:34.570069 byteblower_test_cases_low_latency-1.2.1/README.rst
+-rw-r--r--   0        0        0       45 2024-01-19 09:10:44.545897 byteblower_test_cases_low_latency-1.2.1/byteblower/test_cases/low_latency/.gitignore
+-rw-r--r--   0        0        0      209 2024-01-19 09:10:44.545897 byteblower_test_cases_low_latency-1.2.1/byteblower/test_cases/low_latency/__init__.py
+-rw-r--r--   0        0        0      349 2024-01-19 09:10:44.545897 byteblower_test_cases_low_latency-1.2.1/byteblower/test_cases/low_latency/__main__.py
+-rw-r--r--   0        0        0     3547 2024-01-26 10:35:12.328401 byteblower_test_cases_low_latency-1.2.1/byteblower/test_cases/low_latency/_arguments.py
+-rw-r--r--   0        0        0      694 2024-01-26 07:43:21.978477 byteblower_test_cases_low_latency-1.2.1/byteblower/test_cases/low_latency/_config_file.py
+-rw-r--r--   0        0        0      951 2024-01-26 07:43:22.030477 byteblower_test_cases_low_latency-1.2.1/byteblower/test_cases/low_latency/_definitions.py
+-rw-r--r--   0        0        0     2892 2024-01-26 10:35:12.328401 byteblower_test_cases_low_latency-1.2.1/byteblower/test_cases/low_latency/_endpoint_factory.py
+-rw-r--r--   0        0        0    23052 2024-02-14 14:42:04.344950 byteblower_test_cases_low_latency-1.2.1/byteblower/test_cases/low_latency/_flow_factory.py
+-rw-r--r--   0        0        0    17797 2024-04-25 11:33:44.324106 byteblower_test_cases_low_latency-1.2.1/byteblower/test_cases/low_latency/_lld.py
+-rw-r--r--   0        0        0     2466 2024-01-26 10:35:12.328401 byteblower_test_cases_low_latency-1.2.1/byteblower/test_cases/low_latency/_port_factory.py
+-rw-r--r--   0        0        0     1607 2024-01-26 10:35:12.328401 byteblower_test_cases_low_latency-1.2.1/byteblower/test_cases/low_latency/_scouting_flow.py
+-rw-r--r--   0        0        0     5532 2024-01-26 10:35:12.328401 byteblower_test_cases_low_latency-1.2.1/byteblower/test_cases/low_latency/_stream_data_gatherer.py
+-rw-r--r--   0        0        0      160 2024-04-26 12:28:15.868704 byteblower_test_cases_low_latency-1.2.1/byteblower/test_cases/low_latency/_version.py
+-rw-r--r--   0        0        0     1348 2024-01-19 09:10:44.545897 byteblower_test_cases_low_latency-1.2.1/byteblower/test_cases/low_latency/cli.py
+-rw-r--r--   0        0        0     3863 2024-01-26 10:35:12.328401 byteblower_test_cases_low_latency-1.2.1/byteblower/test_cases/low_latency/csvaggregator.py
+-rw-r--r--   0        0        0     9835 2024-01-26 10:35:12.328401 byteblower_test_cases_low_latency-1.2.1/byteblower/test_cases/low_latency/dynamic_frameblastingflow.py
+-rw-r--r--   0        0        0      737 2024-01-26 07:43:22.034477 byteblower_test_cases_low_latency-1.2.1/byteblower/test_cases/low_latency/exceptions.py
+-rw-r--r--   0        0        0     9710 2024-01-26 10:35:12.328401 byteblower_test_cases_low_latency-1.2.1/byteblower/test_cases/low_latency/l4s_analysers.py
+-rw-r--r--   0        0        0     7768 2024-01-26 10:35:12.328401 byteblower_test_cases_low_latency-1.2.1/byteblower/test_cases/low_latency/l4s_frameblastingflow.py
+-rw-r--r--   0        0        0    16781 2024-01-26 10:35:12.332401 byteblower_test_cases_low_latency-1.2.1/byteblower/test_cases/low_latency/outlier_latency_cdf_analyser.py
+-rw-r--r--   0        0        0        7 2024-01-19 09:10:44.545897 byteblower_test_cases_low_latency-1.2.1/docs/.gitignore
+-rw-r--r--   0        0        0      638 2024-01-19 09:10:44.545897 byteblower_test_cases_low_latency-1.2.1/docs/Makefile
+-rw-r--r--   0        0        0      804 2024-01-26 07:43:22.034477 byteblower_test_cases_low_latency-1.2.1/docs/make.bat
+-rw-r--r--   0        0        0       51 2024-02-13 21:45:24.379875 byteblower_test_cases_low_latency-1.2.1/docs/source/.gitignore
+-rw-r--r--   0        0        0      919 2024-01-26 07:43:22.034477 byteblower_test_cases_low_latency-1.2.1/docs/source/_include/_example_test_scenario.rst
+-rw-r--r--   0        0        0        0 2024-04-26 12:27:40.816769 byteblower_test_cases_low_latency-1.2.1/docs/source/_static/.gitkeep
+-rw-r--r--   0        0        0      301 2024-02-07 15:37:25.279645 byteblower_test_cases_low_latency-1.2.1/docs/source/_static/excentis.css
+-rw-r--r--   0        0        0     4044 2024-01-30 13:14:52.251661 byteblower_test_cases_low_latency-1.2.1/docs/source/cli/index.rst
+-rw-r--r--   0        0        0    10127 2024-04-25 18:56:34.722069 byteblower_test_cases_low_latency-1.2.1/docs/source/conf.py
+-rw-r--r--   0        0        0     3606 2024-02-01 14:08:18.411708 byteblower_test_cases_low_latency-1.2.1/docs/source/config/conference.rst
+-rw-r--r--   0        0        0     1757 2024-04-25 11:55:48.047286 byteblower_test_cases_low_latency-1.2.1/docs/source/config/dynamic_frame_blasting.rst
+-rw-r--r--   0        0        0     2085 2024-04-25 11:55:48.047286 byteblower_test_cases_low_latency-1.2.1/docs/source/config/frame_blasting.rst
+-rw-r--r--   0        0        0     1347 2024-01-26 07:43:22.034477 byteblower_test_cases_low_latency-1.2.1/docs/source/config/gaming.rst
+-rw-r--r--   0        0        0     1146 2024-02-01 14:08:18.411708 byteblower_test_cases_low_latency-1.2.1/docs/source/config/http.rst
+-rw-r--r--   0        0        0     5908 2024-04-25 11:55:48.047286 byteblower_test_cases_low_latency-1.2.1/docs/source/config/index.rst
+-rw-r--r--   0        0        0     1542 2024-04-25 11:55:48.047286 byteblower_test_cases_low_latency-1.2.1/docs/source/config/l4s_frame_blasting.rst
+-rw-r--r--   0        0        0      823 2024-01-26 07:43:22.034477 byteblower_test_cases_low_latency-1.2.1/docs/source/config/video.rst
+-rw-r--r--   0        0        0     1361 2024-04-25 11:55:48.047286 byteblower_test_cases_low_latency-1.2.1/docs/source/config/voice.rst
+-rw-r--r--   0        0        0    10940 2024-04-25 11:33:44.432106 byteblower_test_cases_low_latency-1.2.1/docs/source/examples/basic.rst
+-rw-r--r--   0        0        0     3019 2024-02-14 16:55:34.014652 byteblower_test_cases_low_latency-1.2.1/docs/source/examples/index.rst
+-rw-r--r--   0        0        0    15425 2024-04-25 11:33:44.620106 byteblower_test_cases_low_latency-1.2.1/docs/source/examples/l4s.rst
+-rw-r--r--   0        0        0    97606 2024-04-25 13:08:30.930486 byteblower_test_cases_low_latency-1.2.1/docs/source/extra/test-cases/low-latency/json/config-schema.json
+-rw-r--r--   0        0        0     2650 2024-04-25 11:55:48.047286 byteblower_test_cases_low_latency-1.2.1/docs/source/extra/test-cases/low-latency/json/endpoint/low_latency.json
+-rw-r--r--   0        0        0     3386 2024-04-25 11:55:48.047286 byteblower_test_cases_low_latency-1.2.1/docs/source/extra/test-cases/low-latency/json/l4s/endpoint/low_latency.json
+-rw-r--r--   0        0        0     3351 2024-04-25 11:55:48.047286 byteblower_test_cases_low_latency-1.2.1/docs/source/extra/test-cases/low-latency/json/l4s/port/low_latency.json
+-rw-r--r--   0        0        0     2615 2024-04-25 11:55:48.047286 byteblower_test_cases_low_latency-1.2.1/docs/source/extra/test-cases/low-latency/json/port/low_latency.json
+-rw-r--r--   0        0        0    13413 2024-02-14 14:51:10.168299 byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/intermediate/html_report_config.png
+-rw-r--r--   0        0        0   130059 2024-02-14 14:51:10.172299 byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/intermediate/html_report_correlated.png
+-rw-r--r--   0        0        0    31733 2024-02-14 14:51:10.172299 byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/intermediate/html_report_gaming_config.png
+-rw-r--r--   0        0        0    35064 2024-02-14 14:51:10.172299 byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/intermediate/html_report_gaming_graph.png
+-rw-r--r--   0        0        0    30909 2024-02-14 14:51:10.172299 byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/intermediate/html_report_gaming_stats.png
+-rw-r--r--   0        0        0     6520 2024-02-14 14:51:10.172299 byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/intermediate/html_report_http_analysis.png
+-rw-r--r--   0        0        0   119366 2024-02-14 14:51:10.172299 byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/intermediate/html_report_http_graph.png
+-rw-r--r--   0        0        0    15992 2024-02-14 14:51:10.172299 byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/intermediate/html_report_status_and_env.png
+-rw-r--r--   0        0        0    37591 2024-02-14 14:51:10.172299 byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/intermediate/html_report_udp_graph.png
+-rw-r--r--   0        0        0    31901 2024-02-14 14:51:10.172299 byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/intermediate/html_report_udp_stats.png
+-rw-r--r--   0        0        0     4985 2024-02-14 14:51:10.172299 byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/intermediate/html_report_udp_status.png
+-rw-r--r--   0        0        0   103787 2024-02-14 14:51:10.176299 byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/intermediate/html_report_voice_graph.png
+-rw-r--r--   0        0        0    49844 2024-02-14 14:51:10.176299 byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/intermediate/html_report_voice_stats.png
+-rw-r--r--   0        0        0     4813 2024-02-14 14:51:10.176299 byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/intermediate/html_report_voice_status.png
+-rw-r--r--   0        0        0    14102 2024-02-14 14:51:10.176299 byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/l4s_intermediate/html_report_config.png
+-rw-r--r--   0        0        0    41474 2024-02-14 15:35:43.387404 byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/l4s_intermediate/html_report_correlated_ccdf.png
+-rw-r--r--   0        0        0   176999 2024-02-14 15:35:43.391404 byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/l4s_intermediate/html_report_correlated_thr.png
+-rw-r--r--   0        0        0    38345 2024-04-25 11:33:44.768106 byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/l4s_intermediate/html_report_flow_run.png
+-rw-r--r--   0        0        0   127248 2024-02-14 15:35:43.391404 byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/l4s_intermediate/html_report_gaming_ccdf.png
+-rw-r--r--   0        0        0   193678 2024-02-14 15:35:43.391404 byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/l4s_intermediate/html_report_gaming_loss.png
+-rw-r--r--   0        0        0    12703 2024-02-14 15:35:43.391404 byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/l4s_intermediate/html_report_http_analysis.png
+-rw-r--r--   0        0        0    19459 2024-02-14 15:35:43.395404 byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/l4s_intermediate/html_report_http_config.png
+-rw-r--r--   0        0        0   128409 2024-02-14 15:35:43.395404 byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/l4s_intermediate/html_report_http_graph.png
+-rw-r--r--   0        0        0    13367 2024-02-14 15:35:43.395404 byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/l4s_intermediate/html_report_l4s_http_analysis.png
+-rw-r--r--   0        0        0   121304 2024-02-14 15:35:43.395404 byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/l4s_intermediate/html_report_l4s_http_graph.png
+-rw-r--r--   0        0        0    14841 2024-02-14 14:51:10.180299 byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/l4s_intermediate/html_report_status_and_env.png
+-rw-r--r--   0        0        0    40577 2024-02-14 15:35:43.395404 byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/l4s_intermediate/html_report_udp_cdf_graph.png
+-rw-r--r--   0        0        0    42790 2024-02-14 15:35:43.395404 byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/l4s_intermediate/html_report_udp_cdf_status_and_stats.png
+-rw-r--r--   0        0        0    41786 2024-02-14 15:35:43.399404 byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/l4s_intermediate/html_report_udp_loss_analyser.png
+-rw-r--r--   0        0        0    96583 2024-02-14 15:35:43.399404 byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/l4s_intermediate/html_report_udp_loss_graph.png
+-rw-r--r--   0        0        0    39276 2024-02-14 15:35:43.399404 byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/l4s_intermediate/html_report_udp_loss_stats.png
+-rw-r--r--   0        0        0   101406 2024-02-14 15:35:43.439403 byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/l4s_intermediate/html_report_voice_graph.png
+-rw-r--r--   0        0        0    64833 2024-02-14 15:35:43.443403 byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/l4s_intermediate/html_report_voice_stats.png
+-rw-r--r--   0        0        0    13457 2024-02-14 15:35:43.443403 byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/l4s_intermediate/html_report_voice_status.png
+-rw-r--r--   0        0        0   136289 2024-01-26 07:43:22.054478 byteblower_test_cases_low_latency-1.2.1/docs/source/images/html_report_Loss_latency_analyser.png
+-rw-r--r--   0        0        0   124331 2024-01-26 07:43:22.054478 byteblower_test_cases_low_latency-1.2.1/docs/source/images/html_report_aggregated_results.png
+-rw-r--r--   0        0        0    24588 2024-01-26 07:43:22.054478 byteblower_test_cases_low_latency-1.2.1/docs/source/images/html_report_config.png
+-rw-r--r--   0        0        0    33492 2024-01-26 07:43:22.054478 byteblower_test_cases_low_latency-1.2.1/docs/source/images/html_report_config_table.png
+-rw-r--r--   0        0        0    56307 2024-01-26 07:43:22.058477 byteblower_test_cases_low_latency-1.2.1/docs/source/images/html_report_http_analyser.png
+-rw-r--r--   0        0        0    75988 2024-01-26 07:43:22.058477 byteblower_test_cases_low_latency-1.2.1/docs/source/images/html_report_latency.png
+-rw-r--r--   0        0        0    90900 2024-01-26 07:43:22.058477 byteblower_test_cases_low_latency-1.2.1/docs/source/images/html_report_latency_sum.png
+-rw-r--r--   0        0        0   120807 2024-01-26 07:43:22.058477 byteblower_test_cases_low_latency-1.2.1/docs/source/images/html_report_loss_analyser.png
+-rw-r--r--   0        0        0   156060 2024-02-14 16:08:16.516914 byteblower_test_cases_low_latency-1.2.1/docs/source/images/l4s_graph_over_time.png
+-rw-r--r--   0        0        0      446 2024-02-14 15:54:20.097418 byteblower_test_cases_low_latency-1.2.1/docs/source/index.rst
+-rw-r--r--   0        0        0      570 2024-02-14 16:55:34.014652 byteblower_test_cases_low_latency-1.2.1/docs/source/master_index.rst
+-rw-r--r--   0        0        0     4909 2024-04-25 11:33:44.880107 byteblower_test_cases_low_latency-1.2.1/docs/source/overview.rst
+-rw-r--r--   0        0        0     6223 2024-04-25 11:33:44.924106 byteblower_test_cases_low_latency-1.2.1/docs/source/quick_start.rst
+-rw-r--r--   0        0        0     8263 2024-04-25 18:56:34.798069 byteblower_test_cases_low_latency-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0    11155 1970-01-01 00:00:00.000000 byteblower_test_cases_low_latency-1.2.1/PKG-INFO
```

### Comparing `byteblower_test_cases_low_latency-1.2.0/README.rst` & `byteblower_test_cases_low_latency-1.2.1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -195,15 +195,15 @@
 For example (*to get help for the command-line arguments*):
 
 #. As a python module:
 
    .. code-block:: shell
 
       # To get help for the command-line arguments:
-      python -m byteblower.test_case.low_latency --help
+      python -m byteblower.test_cases.low_latency --help
 
 #. As a command-line script:
 
    .. code-block:: shell
 
       # To get help for the command-line arguments:
       byteblower-test-cases-low-latency --help
@@ -251,15 +251,15 @@
       byteblower-test-case-low-latency --report-path reports
 
 Integrated
 ----------
 
 .. code-block:: python
 
-   from byteblower.test_case.low_latency import run
+   from byteblower.test_cases.low_latency import run
 
    # Defining test configuration, report path and report file name prefix:
    test_config = {} # Here you should provide your test setup + frame(s') configuration(s)
    report_path = 'my-output-folder' # Optional: provide the path to the output folder, defaults to the current working directory
    report_prefix = 'my-dut-feature-test' # Optional: provide prefix of the output files, defaults to 'report'
 
    # Run the low latency validation test:
```

### Comparing `byteblower_test_cases_low_latency-1.2.0/byteblower/test_cases/low_latency/_arguments.py` & `byteblower_test_cases_low_latency-1.2.1/byteblower/test_cases/low_latency/_arguments.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/byteblower/test_cases/low_latency/_config_file.py` & `byteblower_test_cases_low_latency-1.2.1/byteblower/test_cases/low_latency/_config_file.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/byteblower/test_cases/low_latency/_definitions.py` & `byteblower_test_cases_low_latency-1.2.1/byteblower/test_cases/low_latency/_definitions.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/byteblower/test_cases/low_latency/_endpoint_factory.py` & `byteblower_test_cases_low_latency-1.2.1/byteblower/test_cases/low_latency/_endpoint_factory.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/byteblower/test_cases/low_latency/_flow_factory.py` & `byteblower_test_cases_low_latency-1.2.1/byteblower/test_cases/low_latency/_flow_factory.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/byteblower/test_cases/low_latency/_lld.py` & `byteblower_test_cases_low_latency-1.2.1/byteblower/test_cases/low_latency/_lld.py`

 * *Files 2% similar despite different names*

```diff
@@ -343,29 +343,30 @@
 ) -> None:
 
     for flow_configuration in flow_configurations:
         flow_name = flow_configuration.get("name", "<unnamed flow>")
         flow_type = flow_configuration["type"]
 
         # Sanity checks
-        if flow_type.lower() != "frame_blasting" and (
+        # TODO: NAT keepalive support for Video Conference Flow
+        if flow_type.lower() not in _FRAME_BLASTING_BASED_FLOWS and (
                 "nat_keep_alive" in flow_configuration
                 or "napt_keep_alive" in flow_configuration):
             raise InvalidInput(
                 f"{flow_name}: NAT/NAPT keep-alive (nat_keep_alive) is only"
                 " supported for frame blasting flows"
             )
 
         add_reverse_direction = flow_configuration.pop(
             "add_reverse_direction", False
         )
         reverse_flow_group = flow_configuration.pop("reverse_flow_group", [])
 
-        # NOTE: Deprecated ``nat_keep_alive`` in v1.2.0,
-        # TODO: Remove ``napt_keep_alive`` in v1.4.0
+        # NOTE: Deprecated ``nat_keep_alive`` in v1.1.0,
+        # TODO: Remove ``napt_keep_alive`` in v1.3.0
         nat_keep_alive = flow_configuration.pop("nat_keep_alive", None)
         napt_keep_alive = flow_configuration.pop("napt_keep_alive", None)
         if napt_keep_alive is not None:
             if nat_keep_alive is not None:
                 raise InvalidInput(
                     f"{flow_name}: Prefer nat_keep_alive over napt_keep_alive."
                     " Do not specify both."
@@ -385,14 +386,23 @@
             port_group_map,
             add_reverse_direction=add_reverse_direction,
             reverse_flow_group=reverse_flow_group,
             nat_keep_alive=nat_keep_alive
         )
 
 
+_FRAME_BLASTING_BASED_FLOWS = (
+    'frame_blasting',
+    'l4s_frame_blasting',
+    'dynamic_frame_blasting',
+    'voice',
+    'gaming',
+)
+
+
 def _initialize_port_flows(
     scenario: Scenario,
     flow_configuration: _FlowConfiguration,
     layer2_speed: Layer2Speed,
     port_group_map: _PortGroupMap,
     add_reverse_direction: bool = False,
     reverse_flow_group: List = None,
```

### Comparing `byteblower_test_cases_low_latency-1.2.0/byteblower/test_cases/low_latency/_port_factory.py` & `byteblower_test_cases_low_latency-1.2.1/byteblower/test_cases/low_latency/_port_factory.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/byteblower/test_cases/low_latency/_scouting_flow.py` & `byteblower_test_cases_low_latency-1.2.1/byteblower/test_cases/low_latency/_scouting_flow.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/byteblower/test_cases/low_latency/_stream_data_gatherer.py` & `byteblower_test_cases_low_latency-1.2.1/byteblower/test_cases/low_latency/_stream_data_gatherer.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/byteblower/test_cases/low_latency/cli.py` & `byteblower_test_cases_low_latency-1.2.1/byteblower/test_cases/low_latency/cli.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/byteblower/test_cases/low_latency/csvaggregator.py` & `byteblower_test_cases_low_latency-1.2.1/byteblower/test_cases/low_latency/csvaggregator.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/byteblower/test_cases/low_latency/dynamic_frameblastingflow.py` & `byteblower_test_cases_low_latency-1.2.1/byteblower/test_cases/low_latency/dynamic_frameblastingflow.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/byteblower/test_cases/low_latency/exceptions.py` & `byteblower_test_cases_low_latency-1.2.1/byteblower/test_cases/low_latency/exceptions.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/byteblower/test_cases/low_latency/l4s_analysers.py` & `byteblower_test_cases_low_latency-1.2.1/byteblower/test_cases/low_latency/l4s_analysers.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/byteblower/test_cases/low_latency/l4s_frameblastingflow.py` & `byteblower_test_cases_low_latency-1.2.1/byteblower/test_cases/low_latency/l4s_frameblastingflow.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/byteblower/test_cases/low_latency/outlier_latency_cdf_analyser.py` & `byteblower_test_cases_low_latency-1.2.1/byteblower/test_cases/low_latency/outlier_latency_cdf_analyser.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/docs/Makefile` & `byteblower_test_cases_low_latency-1.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/docs/make.bat` & `byteblower_test_cases_low_latency-1.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/docs/source/_include/_example_test_scenario.rst` & `byteblower_test_cases_low_latency-1.2.1/docs/source/_include/_example_test_scenario.rst`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/docs/source/cli/index.rst` & `byteblower_test_cases_low_latency-1.2.1/docs/source/cli/index.rst`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/docs/source/conf.py` & `byteblower_test_cases_low_latency-1.2.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/docs/source/config/conference.rst` & `byteblower_test_cases_low_latency-1.2.1/docs/source/config/conference.rst`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/docs/source/config/dynamic_frame_blasting.rst` & `byteblower_test_cases_low_latency-1.2.1/docs/source/config/dynamic_frame_blasting.rst`

 * *Files 0% similar despite different names*

```diff
@@ -39,11 +39,11 @@
          "max_loss_percentage": "<max_loss_percentage:float>",
          "quantile": "<quantile:float>",
          "min_percentile": "<min_percentile:float>",
          "max_percentile": "<max_percentile:float>"
       }
    }
 
-.. jsonschema:: ../extra/test-cases/low-latency/json/config-schema.json#/$defs/dynamic_frame_blasting
+.. jsonschema:: ../extra/test-cases/low-latency/json/config-schema.json#/$defs/dynamic_frame_blasting_flow
    :auto_reference:
    :auto_target:
    :lift_title: False
```

### Comparing `byteblower_test_cases_low_latency-1.2.0/docs/source/config/frame_blasting.rst` & `byteblower_test_cases_low_latency-1.2.1/docs/source/config/frame_blasting.rst`

 * *Files 4% similar despite different names*

```diff
@@ -37,26 +37,26 @@
          "max_loss_percentage": "<max_loss_percentage:float>",
          "quantile": "<quantile:float>",
          "min_percentile": "<min_percentile:float>",
          "max_percentile": "<max_percentile:float>"
       }
    }
 
-.. jsonschema:: ../extra/test-cases/low-latency/json/config-schema.json#/$defs/frame_blasting
+.. jsonschema:: ../extra/test-cases/low-latency/json/config-schema.json#/$defs/frame_blasting_flow
    :auto_reference:
    :auto_target:
    :lift_title: False
 
 .. jsonschema:: ../extra/test-cases/low-latency/json/config-schema.json#/$defs/frame_loss_analysis
    :auto_target:
    :auto_reference:
    :lift_title: False
 
 .. jsonschema:: ../extra/test-cases/low-latency/json/config-schema.json#/$defs/latency_loss_analysis
    :auto_target:
    :auto_reference:
    :lift_title: False
 
-.. jsonschema:: ../extra/test-cases/low-latency/json/config-schema.json#/$defs/l4s
+.. jsonschema:: ../extra/test-cases/low-latency/json/config-schema.json#/$defs/l4s_analysis
    :auto_reference:
    :auto_target:
    :lift_title: False
```

### Comparing `byteblower_test_cases_low_latency-1.2.0/docs/source/config/gaming.rst` & `byteblower_test_cases_low_latency-1.2.1/docs/source/config/gaming.rst`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/docs/source/config/http.rst` & `byteblower_test_cases_low_latency-1.2.1/docs/source/config/http.rst`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/docs/source/config/index.rst` & `byteblower_test_cases_low_latency-1.2.1/docs/source/config/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,15 @@
    :auto_target:
    :lift_title: False
 
 .. jsonschema:: ../extra/test-cases/low-latency/json/config-schema.json#/$defs/port
    :auto_reference:
    :auto_target:
 
-.. jsonschema:: ../extra/test-cases/low-latency/json/config-schema.json#/$defs/vlans
+.. jsonschema:: ../extra/test-cases/low-latency/json/config-schema.json#/$defs/vlan
    :auto_reference:
    :auto_target:
 
 .. jsonschema:: ../extra/test-cases/low-latency/json/config-schema.json#/$defs/port_group
    :auto_reference:
    :auto_target:
```

### Comparing `byteblower_test_cases_low_latency-1.2.0/docs/source/config/l4s_frame_blasting.rst` & `byteblower_test_cases_low_latency-1.2.1/docs/source/config/l4s_frame_blasting.rst`

 * *Files 0% similar despite different names*

```diff
@@ -36,11 +36,11 @@
          "quantile": "<quantile:float>",
          "min_percentile": "<min_percentile:float>",
          "max_percentile": "<max_percentile:float>"
       }
    }
 
 
-.. jsonschema:: ../extra/test-cases/low-latency/json/config-schema.json#/$defs/l4s_frame_blasting
+.. jsonschema:: ../extra/test-cases/low-latency/json/config-schema.json#/$defs/l4s_frame_blasting_flow
    :auto_reference:
    :auto_target:
    :lift_title: False
```

### Comparing `byteblower_test_cases_low_latency-1.2.0/docs/source/config/video.rst` & `byteblower_test_cases_low_latency-1.2.1/docs/source/config/video.rst`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/docs/source/config/voice.rst` & `byteblower_test_cases_low_latency-1.2.1/docs/source/config/voice.rst`

 * *Files 2% similar despite different names*

```diff
@@ -37,11 +37,11 @@
    }
 
 .. jsonschema:: ../extra/test-cases/low-latency/json/config-schema.json#/$defs/voice_flow
    :auto_reference:
    :auto_target:
    :lift_title: False
 
-.. jsonschema:: ../extra/test-cases/low-latency/json/config-schema.json#/$defs/mos
+.. jsonschema:: ../extra/test-cases/low-latency/json/config-schema.json#/$defs/mos_analysis
    :auto_target:
    :auto_reference:
    :lift_title: False
```

### Comparing `byteblower_test_cases_low_latency-1.2.0/docs/source/examples/basic.rst` & `byteblower_test_cases_low_latency-1.2.1/docs/source/examples/basic.rst`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/docs/source/examples/index.rst` & `byteblower_test_cases_low_latency-1.2.1/docs/source/examples/index.rst`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/docs/source/examples/l4s.rst` & `byteblower_test_cases_low_latency-1.2.1/docs/source/examples/l4s.rst`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/docs/source/extra/test-cases/low-latency/json/endpoint/low_latency.json` & `byteblower_test_cases_low_latency-1.2.1/docs/source/extra/test-cases/low-latency/json/endpoint/low_latency.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.875%*

 * *Differences: {"'$schema'": "'https://api.byteblower.com/test-framework/json/test-cases/low-latency/config-schema.json'"}*

```diff
@@ -1,8 +1,9 @@
 {
+    "$schema": "https://api.byteblower.com/test-framework/json/test-cases/low-latency/config-schema.json",
     "enable_scouting_flows": true,
     "flows": [
         {
             "bitrate": 150000000.0,
             "destination": {
                 "port_group": [
                     "classic_cpe"
```

### Comparing `byteblower_test_cases_low_latency-1.2.0/docs/source/extra/test-cases/low-latency/json/l4s/endpoint/low_latency.json` & `byteblower_test_cases_low_latency-1.2.1/docs/source/extra/test-cases/low-latency/json/l4s/endpoint/low_latency.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.875%*

 * *Differences: {"'$schema'": "'https://api.byteblower.com/test-framework/json/test-cases/low-latency/config-schema.json'"}*

```diff
@@ -1,8 +1,9 @@
 {
+    "$schema": "https://api.byteblower.com/test-framework/json/test-cases/low-latency/config-schema.json",
     "enable_scouting_flows": true,
     "flows": [
         {
             "analysis": {
                 "latency": true
             },
             "bitrate": 90000000.0,
```

### Comparing `byteblower_test_cases_low_latency-1.2.0/docs/source/extra/test-cases/low-latency/json/l4s/port/low_latency.json` & `byteblower_test_cases_low_latency-1.2.1/docs/source/extra/test-cases/low-latency/json/l4s/port/low_latency.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8571428571428571%*

 * *Differences: {"'$schema'": "'https://api.byteblower.com/test-framework/json/test-cases/low-latency/config-schema.json'"}*

```diff
@@ -1,8 +1,9 @@
 {
+    "$schema": "https://api.byteblower.com/test-framework/json/test-cases/low-latency/config-schema.json",
     "enable_scouting_flows": true,
     "flows": [
         {
             "analysis": {
                 "latency": true
             },
             "bitrate": 90000000.0,
```

### Comparing `byteblower_test_cases_low_latency-1.2.0/docs/source/extra/test-cases/low-latency/json/port/low_latency.json` & `byteblower_test_cases_low_latency-1.2.1/docs/source/extra/test-cases/low-latency/json/port/low_latency.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8571428571428571%*

 * *Differences: {"'$schema'": "'https://api.byteblower.com/test-framework/json/test-cases/low-latency/config-schema.json'"}*

```diff
@@ -1,8 +1,9 @@
 {
+    "$schema": "https://api.byteblower.com/test-framework/json/test-cases/low-latency/config-schema.json",
     "enable_scouting_flows": true,
     "flows": [
         {
             "bitrate": 150000000.0,
             "destination": {
                 "port_group": [
                     "classic_cpe"
```

### Comparing `byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/intermediate/html_report_config.png` & `byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/intermediate/html_report_config.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/intermediate/html_report_correlated.png` & `byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/intermediate/html_report_correlated.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/intermediate/html_report_gaming_config.png` & `byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/intermediate/html_report_gaming_config.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/intermediate/html_report_gaming_graph.png` & `byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/intermediate/html_report_gaming_graph.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/intermediate/html_report_gaming_stats.png` & `byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/intermediate/html_report_gaming_stats.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/intermediate/html_report_http_analysis.png` & `byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/intermediate/html_report_http_analysis.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/intermediate/html_report_http_graph.png` & `byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/intermediate/html_report_http_graph.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/intermediate/html_report_status_and_env.png` & `byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/intermediate/html_report_status_and_env.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/intermediate/html_report_udp_graph.png` & `byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/intermediate/html_report_udp_graph.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/intermediate/html_report_udp_stats.png` & `byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/intermediate/html_report_udp_stats.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/intermediate/html_report_udp_status.png` & `byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/intermediate/html_report_udp_status.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/intermediate/html_report_voice_graph.png` & `byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/intermediate/html_report_voice_graph.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/intermediate/html_report_voice_stats.png` & `byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/intermediate/html_report_voice_stats.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/intermediate/html_report_voice_status.png` & `byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/intermediate/html_report_voice_status.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/l4s_intermediate/html_report_config.png` & `byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/l4s_intermediate/html_report_config.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/l4s_intermediate/html_report_correlated_ccdf.png` & `byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/l4s_intermediate/html_report_correlated_ccdf.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/l4s_intermediate/html_report_correlated_thr.png` & `byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/l4s_intermediate/html_report_correlated_thr.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/l4s_intermediate/html_report_flow_run.png` & `byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/l4s_intermediate/html_report_flow_run.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/l4s_intermediate/html_report_gaming_ccdf.png` & `byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/l4s_intermediate/html_report_gaming_ccdf.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/l4s_intermediate/html_report_gaming_loss.png` & `byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/l4s_intermediate/html_report_gaming_loss.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/l4s_intermediate/html_report_http_analysis.png` & `byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/l4s_intermediate/html_report_http_analysis.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/l4s_intermediate/html_report_http_config.png` & `byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/l4s_intermediate/html_report_http_config.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/l4s_intermediate/html_report_http_graph.png` & `byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/l4s_intermediate/html_report_http_graph.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/l4s_intermediate/html_report_l4s_http_analysis.png` & `byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/l4s_intermediate/html_report_l4s_http_analysis.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/l4s_intermediate/html_report_l4s_http_graph.png` & `byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/l4s_intermediate/html_report_l4s_http_graph.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/l4s_intermediate/html_report_status_and_env.png` & `byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/l4s_intermediate/html_report_status_and_env.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/l4s_intermediate/html_report_udp_cdf_graph.png` & `byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/l4s_intermediate/html_report_udp_cdf_graph.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/l4s_intermediate/html_report_udp_cdf_status_and_stats.png` & `byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/l4s_intermediate/html_report_udp_cdf_status_and_stats.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/l4s_intermediate/html_report_udp_loss_analyser.png` & `byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/l4s_intermediate/html_report_udp_loss_analyser.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/l4s_intermediate/html_report_udp_loss_graph.png` & `byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/l4s_intermediate/html_report_udp_loss_graph.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/l4s_intermediate/html_report_udp_loss_stats.png` & `byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/l4s_intermediate/html_report_udp_loss_stats.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/l4s_intermediate/html_report_voice_graph.png` & `byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/l4s_intermediate/html_report_voice_graph.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/l4s_intermediate/html_report_voice_stats.png` & `byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/l4s_intermediate/html_report_voice_stats.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/docs/source/images/examples/l4s_intermediate/html_report_voice_status.png` & `byteblower_test_cases_low_latency-1.2.1/docs/source/images/examples/l4s_intermediate/html_report_voice_status.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/docs/source/images/html_report_Loss_latency_analyser.png` & `byteblower_test_cases_low_latency-1.2.1/docs/source/images/html_report_Loss_latency_analyser.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/docs/source/images/html_report_aggregated_results.png` & `byteblower_test_cases_low_latency-1.2.1/docs/source/images/html_report_aggregated_results.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/docs/source/images/html_report_config.png` & `byteblower_test_cases_low_latency-1.2.1/docs/source/images/html_report_config.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/docs/source/images/html_report_config_table.png` & `byteblower_test_cases_low_latency-1.2.1/docs/source/images/html_report_config_table.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/docs/source/images/html_report_http_analyser.png` & `byteblower_test_cases_low_latency-1.2.1/docs/source/images/html_report_http_analyser.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/docs/source/images/html_report_latency.png` & `byteblower_test_cases_low_latency-1.2.1/docs/source/images/html_report_latency.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/docs/source/images/html_report_latency_sum.png` & `byteblower_test_cases_low_latency-1.2.1/docs/source/images/html_report_latency_sum.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/docs/source/images/html_report_loss_analyser.png` & `byteblower_test_cases_low_latency-1.2.1/docs/source/images/html_report_loss_analyser.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/docs/source/images/l4s_graph_over_time.png` & `byteblower_test_cases_low_latency-1.2.1/docs/source/images/l4s_graph_over_time.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/docs/source/master_index.rst` & `byteblower_test_cases_low_latency-1.2.1/docs/source/master_index.rst`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/docs/source/overview.rst` & `byteblower_test_cases_low_latency-1.2.1/docs/source/overview.rst`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/docs/source/quick_start.rst` & `byteblower_test_cases_low_latency-1.2.1/docs/source/quick_start.rst`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/pyproject.toml` & `byteblower_test_cases_low_latency-1.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `byteblower_test_cases_low_latency-1.2.0/PKG-INFO` & `byteblower_test_cases_low_latency-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: byteblower-test-cases-low-latency
-Version: 1.2.0
+Version: 1.2.1
 Summary: Low Latency test case using ByteBlower.
 Keywords: ByteBlower,network test,traffic test,test case,LLD,Low-Latency DOCSIS,L4S
 Author-email: ByteBlower Development Team <support.byteblower@excentis.com>
 Maintainer-email: Tom Ghyselinck <tom.ghyselinck@excentis.com>, Abdennour Rachedi <abdennour.rachedi@excentis.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
@@ -252,15 +252,15 @@
 For example (*to get help for the command-line arguments*):
 
 #. As a python module:
 
    .. code-block:: shell
 
       # To get help for the command-line arguments:
-      python -m byteblower.test_case.low_latency --help
+      python -m byteblower.test_cases.low_latency --help
 
 #. As a command-line script:
 
    .. code-block:: shell
 
       # To get help for the command-line arguments:
       byteblower-test-cases-low-latency --help
@@ -308,15 +308,15 @@
       byteblower-test-case-low-latency --report-path reports
 
 Integrated
 ----------
 
 .. code-block:: python
 
-   from byteblower.test_case.low_latency import run
+   from byteblower.test_cases.low_latency import run
 
    # Defining test configuration, report path and report file name prefix:
    test_config = {} # Here you should provide your test setup + frame(s') configuration(s)
    report_path = 'my-output-folder' # Optional: provide the path to the output folder, defaults to the current working directory
    report_prefix = 'my-dut-feature-test' # Optional: provide prefix of the output files, defaults to 'report'
 
    # Run the low latency validation test:
```

