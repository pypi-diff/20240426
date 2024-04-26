# Comparing `tmp/byteblower_test_framework-1.3.0.tar.gz` & `tmp/byteblower_test_framework-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "byteblower_test_framework-1.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "byteblower_test_framework-1.3.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `byteblower_test_framework-1.3.0.tar` & `byteblower_test_framework-1.3.1.tar`

### file list

```diff
@@ -1,198 +1,198 @@
--rw-r--r--   0        0        0     7652 2024-01-22 08:40:15.750003 byteblower_test_framework-1.3.0/LICENSE
--rw-r--r--   0        0        0    17271 2024-02-14 16:03:06.160761 byteblower_test_framework-1.3.0/README.pypi.rst
--rw-r--r--   0        0        0      132 2024-01-22 08:40:15.754003 byteblower_test_framework-1.3.0/byteblower_test_framework/__init__.py
--rw-r--r--   0        0        0      341 2024-01-22 08:40:15.754003 byteblower_test_framework-1.3.0/byteblower_test_framework/__main__.py
--rw-r--r--   0        0        0        0 2024-02-14 17:31:39.070157 byteblower_test_framework-1.3.0/byteblower_test_framework/_analysis/__init__.py
--rw-r--r--   0        0        0    23827 2024-01-22 08:40:15.754003 byteblower_test_framework-1.3.0/byteblower_test_framework/_analysis/analyseraggregator.py
--rw-r--r--   0        0        0    12528 2024-02-01 16:04:24.996924 byteblower_test_framework-1.3.0/byteblower_test_framework/_analysis/bufferanalyser.py
--rw-r--r--   0        0        0       40 2024-01-22 08:40:15.754003 byteblower_test_framework-1.3.0/byteblower_test_framework/_analysis/data_analysis/__init__.py
--rw-r--r--   0        0        0     2001 2024-01-24 12:31:29.999390 byteblower_test_framework-1.3.0/byteblower_test_framework/_analysis/data_analysis/data_analyser.py
--rw-r--r--   0        0        0    37635 2024-01-24 12:31:30.003390 byteblower_test_framework-1.3.0/byteblower_test_framework/_analysis/data_analysis/frameblasting.py
--rw-r--r--   0        0        0     4481 2024-02-07 13:06:58.833138 byteblower_test_framework-1.3.0/byteblower_test_framework/_analysis/data_analysis/tcp.py
--rw-r--r--   0        0        0       40 2024-01-22 08:40:15.758003 byteblower_test_framework-1.3.0/byteblower_test_framework/_analysis/data_gathering/__init__.py
--rw-r--r--   0        0        0     5623 2024-01-24 12:31:30.003390 byteblower_test_framework-1.3.0/byteblower_test_framework/_analysis/data_gathering/_filter.py
--rw-r--r--   0        0        0     8941 2024-01-25 10:18:45.290074 byteblower_test_framework-1.3.0/byteblower_test_framework/_analysis/data_gathering/_rx_trigger_controller.py
--rw-r--r--   0        0        0     1953 2024-01-25 10:18:45.290074 byteblower_test_framework-1.3.0/byteblower_test_framework/_analysis/data_gathering/data_gatherer.py
--rw-r--r--   0        0        0     7103 2024-01-24 12:31:30.003390 byteblower_test_framework-1.3.0/byteblower_test_framework/_analysis/data_gathering/stream.py
--rw-r--r--   0        0        0    29267 2024-02-13 13:47:02.941738 byteblower_test_framework-1.3.0/byteblower_test_framework/_analysis/data_gathering/tcp.py
--rw-r--r--   0        0        0    27881 2024-01-25 09:05:41.159877 byteblower_test_framework-1.3.0/byteblower_test_framework/_analysis/data_gathering/trigger.py
--rw-r--r--   0        0        0     6140 2024-02-01 16:04:25.004924 byteblower_test_framework-1.3.0/byteblower_test_framework/_analysis/flow_analyser.py
--rw-r--r--   0        0        0     9006 2024-02-01 16:04:25.004924 byteblower_test_framework-1.3.0/byteblower_test_framework/_analysis/framelossanalyser.py
--rw-r--r--   0        0        0     8368 2024-01-24 12:31:30.007390 byteblower_test_framework-1.3.0/byteblower_test_framework/_analysis/helpers.py
--rw-r--r--   0        0        0     8184 2024-02-05 08:51:01.922009 byteblower_test_framework-1.3.0/byteblower_test_framework/_analysis/httpanalyser.py
--rw-r--r--   0        0        0     3891 2024-01-22 08:40:15.762004 byteblower_test_framework-1.3.0/byteblower_test_framework/_analysis/latencyaggregator.py
--rw-r--r--   0        0        0    25190 2024-02-01 16:04:25.004924 byteblower_test_framework-1.3.0/byteblower_test_framework/_analysis/latencyanalyser.py
--rw-r--r--   0        0        0       40 2024-01-22 08:40:15.762004 byteblower_test_framework-1.3.0/byteblower_test_framework/_analysis/plotting/__init__.py
--rw-r--r--   0        0        0     4826 2024-01-22 08:40:15.762004 byteblower_test_framework-1.3.0/byteblower_test_framework/_analysis/plotting/generic_chart.py
--rw-r--r--   0        0        0       31 2024-01-22 08:40:15.762004 byteblower_test_framework-1.3.0/byteblower_test_framework/_analysis/render/__init__.py
--rw-r--r--   0        0        0    20121 2024-01-22 08:40:15.762004 byteblower_test_framework-1.3.0/byteblower_test_framework/_analysis/render/frameblasting.py
--rw-r--r--   0        0        0      889 2024-01-22 08:40:15.762004 byteblower_test_framework-1.3.0/byteblower_test_framework/_analysis/render/renderer.py
--rw-r--r--   0        0        0    15852 2024-02-07 13:52:14.374651 byteblower_test_framework-1.3.0/byteblower_test_framework/_analysis/render/tcp.py
--rw-r--r--   0        0        0       34 2024-01-22 08:40:15.762004 byteblower_test_framework-1.3.0/byteblower_test_framework/_analysis/storage/__init__.py
--rw-r--r--   0        0        0       44 2024-01-22 08:40:15.762004 byteblower_test_framework-1.3.0/byteblower_test_framework/_analysis/storage/data_store.py
--rw-r--r--   0        0        0     2406 2024-01-22 08:40:15.766003 byteblower_test_framework-1.3.0/byteblower_test_framework/_analysis/storage/frame_count.py
--rw-r--r--   0        0        0     1363 2024-01-22 08:40:15.766003 byteblower_test_framework-1.3.0/byteblower_test_framework/_analysis/storage/stream.py
--rw-r--r--   0        0        0     8577 2024-02-05 15:33:06.974035 byteblower_test_framework-1.3.0/byteblower_test_framework/_analysis/storage/tcp.py
--rw-r--r--   0        0        0     5425 2024-01-22 08:40:15.766003 byteblower_test_framework-1.3.0/byteblower_test_framework/_analysis/storage/trigger.py
--rw-r--r--   0        0        0     4403 2024-02-01 16:04:25.008924 byteblower_test_framework-1.3.0/byteblower_test_framework/_analysis/voiceanalyser.py
--rw-r--r--   0        0        0       46 2024-01-22 08:40:15.766003 byteblower_test_framework-1.3.0/byteblower_test_framework/_cli/__init__.py
--rw-r--r--   0        0        0     3495 2024-01-22 08:40:15.766003 byteblower_test_framework-1.3.0/byteblower_test_framework/_cli/_arguments.py
--rw-r--r--   0        0        0      694 2024-01-22 08:40:15.766003 byteblower_test_framework-1.3.0/byteblower_test_framework/_cli/_config_file.py
--rw-r--r--   0        0        0      482 2024-01-24 12:31:30.011391 byteblower_test_framework-1.3.0/byteblower_test_framework/_cli/_definitions.py
--rw-r--r--   0        0        0     2853 2024-01-24 12:31:30.011391 byteblower_test_framework-1.3.0/byteblower_test_framework/_cli/_endpoint_factory.py
--rw-r--r--   0        0        0     7425 2024-02-02 17:21:22.221678 byteblower_test_framework-1.3.0/byteblower_test_framework/_cli/_flow_factory.py
--rw-r--r--   0        0        0     2426 2024-01-24 12:31:30.011391 byteblower_test_framework-1.3.0/byteblower_test_framework/_cli/_port_factory.py
--rw-r--r--   0        0        0    13360 2024-01-24 12:31:30.015390 byteblower_test_framework-1.3.0/byteblower_test_framework/_cli/_with_json_configfile.py
--rw-r--r--   0        0        0      234 2024-01-22 08:40:15.770003 byteblower_test_framework-1.3.0/byteblower_test_framework/_cli/exceptions.py
--rw-r--r--   0        0        0        0 2024-02-14 17:31:39.078158 byteblower_test_framework-1.3.0/byteblower_test_framework/_endpoint/__init__.py
--rw-r--r--   0        0        0     8225 2024-01-24 12:31:30.015390 byteblower_test_framework-1.3.0/byteblower_test_framework/_endpoint/endpoint.py
--rw-r--r--   0        0        0     1047 2024-01-24 12:31:30.015390 byteblower_test_framework-1.3.0/byteblower_test_framework/_endpoint/helpers.py
--rw-r--r--   0        0        0        0 2024-02-14 17:31:39.078158 byteblower_test_framework-1.3.0/byteblower_test_framework/_endpoint/ipv4/__init__.py
--rw-r--r--   0        0        0     3038 2024-01-24 12:31:30.015390 byteblower_test_framework-1.3.0/byteblower_test_framework/_endpoint/ipv4/endpoint.py
--rw-r--r--   0        0        0     4202 2024-01-24 12:31:30.015390 byteblower_test_framework-1.3.0/byteblower_test_framework/_endpoint/ipv4/nat.py
--rw-r--r--   0        0        0     4507 2024-01-24 12:31:30.015390 byteblower_test_framework-1.3.0/byteblower_test_framework/_endpoint/ipv4/port.py
--rw-r--r--   0        0        0        0 2024-02-14 17:31:39.078158 byteblower_test_framework-1.3.0/byteblower_test_framework/_endpoint/ipv6/__init__.py
--rw-r--r--   0        0        0     5298 2024-01-24 12:31:30.015390 byteblower_test_framework-1.3.0/byteblower_test_framework/_endpoint/ipv6/endpoint.py
--rw-r--r--   0        0        0     4807 2024-01-22 08:40:15.770003 byteblower_test_framework-1.3.0/byteblower_test_framework/_endpoint/ipv6/port.py
--rw-r--r--   0        0        0    12478 2024-01-24 12:31:30.015390 byteblower_test_framework-1.3.0/byteblower_test_framework/_endpoint/nat_discovery.py
--rw-r--r--   0        0        0     4617 2024-01-24 12:31:30.015390 byteblower_test_framework-1.3.0/byteblower_test_framework/_endpoint/nat_endpoint.py
--rw-r--r--   0        0        0    15498 2024-01-24 12:31:30.019390 byteblower_test_framework-1.3.0/byteblower_test_framework/_endpoint/port.py
--rw-r--r--   0        0        0        0 2024-02-14 17:31:39.082157 byteblower_test_framework-1.3.0/byteblower_test_framework/_factory/__init__.py
--rw-r--r--   0        0        0     4274 2024-01-24 12:31:30.019390 byteblower_test_framework-1.3.0/byteblower_test_framework/_factory/frame.py
--rw-r--r--   0        0        0       55 2024-01-22 08:40:15.770003 byteblower_test_framework-1.3.0/byteblower_test_framework/_helpers/__init__.py
--rw-r--r--   0        0        0     2087 2024-02-08 16:09:16.881606 byteblower_test_framework-1.3.0/byteblower_test_framework/_helpers/capabilities.py
--rw-r--r--   0        0        0      282 2024-02-08 16:09:16.881606 byteblower_test_framework-1.3.0/byteblower_test_framework/_helpers/compat.py
--rw-r--r--   0        0        0     7338 2024-01-24 12:31:30.019390 byteblower_test_framework-1.3.0/byteblower_test_framework/_helpers/syncexec.py
--rw-r--r--   0        0        0     1098 2024-01-24 12:31:30.019390 byteblower_test_framework-1.3.0/byteblower_test_framework/_helpers/taggable.py
--rw-r--r--   0        0        0        0 2024-02-14 17:31:39.082157 byteblower_test_framework-1.3.0/byteblower_test_framework/_host/__init__.py
--rw-r--r--   0        0        0     6743 2024-01-24 12:31:30.019390 byteblower_test_framework-1.3.0/byteblower_test_framework/_host/meetingpoint.py
--rw-r--r--   0        0        0     3408 2024-01-22 08:40:15.770003 byteblower_test_framework-1.3.0/byteblower_test_framework/_host/server.py
--rw-r--r--   0        0        0        0 2024-02-14 17:31:39.082157 byteblower_test_framework-1.3.0/byteblower_test_framework/_report/__init__.py
--rw-r--r--   0        0        0    10512 2024-01-22 08:40:15.774003 byteblower_test_framework-1.3.0/byteblower_test_framework/_report/byteblowerhtmlreport.py
--rw-r--r--   0        0        0     8222 2024-01-22 08:40:15.774003 byteblower_test_framework-1.3.0/byteblower_test_framework/_report/byteblowerjsonreport.py
--rw-r--r--   0        0        0     4109 2024-01-22 08:40:15.774003 byteblower_test_framework-1.3.0/byteblower_test_framework/_report/byteblowerreport.py
--rw-r--r--   0        0        0     3732 2024-01-22 08:40:15.774003 byteblower_test_framework-1.3.0/byteblower_test_framework/_report/byteblowerunittestreport.py
--rw-r--r--   0        0        0      327 2024-01-22 08:40:15.774003 byteblower_test_framework-1.3.0/byteblower_test_framework/_report/helper.py
--rw-r--r--   0        0        0     1947 2024-01-22 08:40:15.774003 byteblower_test_framework-1.3.0/byteblower_test_framework/_report/options.py
--rw-r--r--   0        0        0  3089944 2024-01-22 08:40:15.826004 byteblower_test_framework-1.3.0/byteblower_test_framework/_report/templates/embedded-fonts.css
--rw-r--r--   0        0        0      901 2024-01-22 08:40:15.826004 byteblower_test_framework-1.3.0/byteblower_test_framework/_report/templates/flow_section.html
--rw-r--r--   0        0        0      367 2024-01-22 08:40:15.826004 byteblower_test_framework-1.3.0/byteblower_test_framework/_report/templates/report.html
--rw-r--r--   0        0        0    59284 2024-01-22 08:40:15.830004 byteblower_test_framework-1.3.0/byteblower_test_framework/_report/templates/report_footer.html
--rw-r--r--   0        0        0       97 2024-01-22 08:40:15.830004 byteblower_test_framework-1.3.0/byteblower_test_framework/_report/templates/report_head_style.html
--rw-r--r--   0        0        0    11242 2024-01-22 08:40:15.830004 byteblower_test_framework-1.3.0/byteblower_test_framework/_report/templates/report_header.html
--rw-r--r--   0        0        0      451 2024-01-22 08:40:15.830004 byteblower_test_framework-1.3.0/byteblower_test_framework/_report/templates/report_main.html
--rw-r--r--   0        0        0     1631 2024-01-22 08:40:15.830004 byteblower_test_framework-1.3.0/byteblower_test_framework/_report/templates/report_pass_fail.html
--rw-r--r--   0        0        0      391 2024-01-22 08:40:15.830004 byteblower_test_framework-1.3.0/byteblower_test_framework/_report/templates/test_section.html
--rw-r--r--   0        0        0     7389 2024-01-22 08:40:15.830004 byteblower_test_framework-1.3.0/byteblower_test_framework/_report/templates/testframework.css
--rw-r--r--   0        0        0     4155 2024-01-22 08:40:15.830004 byteblower_test_framework-1.3.0/byteblower_test_framework/_report/unittestreport.py
--rw-r--r--   0        0        0    18629 2024-01-25 09:05:41.163878 byteblower_test_framework-1.3.0/byteblower_test_framework/_scenario.py
--rw-r--r--   0        0        0        0 2024-02-14 17:31:39.086158 byteblower_test_framework-1.3.0/byteblower_test_framework/_traffic/__init__.py
--rw-r--r--   0        0        0    15879 2024-02-13 15:33:45.416359 byteblower_test_framework-1.3.0/byteblower_test_framework/_traffic/_http_client_controller.py
--rw-r--r--   0        0        0     6421 2024-01-24 12:31:30.019390 byteblower_test_framework-1.3.0/byteblower_test_framework/_traffic/_tx_stream_controller.py
--rw-r--r--   0        0        0     1707 2024-01-24 12:31:30.019390 byteblower_test_framework-1.3.0/byteblower_test_framework/_traffic/constants.py
--rw-r--r--   0        0        0    11192 2024-01-24 12:31:30.023390 byteblower_test_framework-1.3.0/byteblower_test_framework/_traffic/flow.py
--rw-r--r--   0        0        0     8655 2024-01-31 12:44:51.233568 byteblower_test_framework-1.3.0/byteblower_test_framework/_traffic/frame.py
--rw-r--r--   0        0        0    16972 2024-01-25 10:18:45.290074 byteblower_test_framework-1.3.0/byteblower_test_framework/_traffic/frameblastingflow.py
--rw-r--r--   0        0        0     7242 2024-01-31 12:44:51.233568 byteblower_test_framework-1.3.0/byteblower_test_framework/_traffic/gamingflow.py
--rw-r--r--   0        0        0     4595 2024-01-24 12:31:30.023390 byteblower_test_framework-1.3.0/byteblower_test_framework/_traffic/helpers.py
--rw-r--r--   0        0        0    16371 2024-02-05 15:33:06.978035 byteblower_test_framework-1.3.0/byteblower_test_framework/_traffic/httpflow.py
--rw-r--r--   0        0        0     5348 2024-01-30 13:42:49.367240 byteblower_test_framework-1.3.0/byteblower_test_framework/_traffic/imix.py
--rw-r--r--   0        0        0        0 2024-02-14 17:31:39.086158 byteblower_test_framework-1.3.0/byteblower_test_framework/_traffic/ipv4/__init__.py
--rw-r--r--   0        0        0     4836 2024-01-31 12:44:51.233568 byteblower_test_framework-1.3.0/byteblower_test_framework/_traffic/ipv4/frame.py
--rw-r--r--   0        0        0        0 2024-02-14 17:31:39.086158 byteblower_test_framework-1.3.0/byteblower_test_framework/_traffic/ipv6/__init__.py
--rw-r--r--   0        0        0     4569 2024-01-31 12:44:51.237568 byteblower_test_framework-1.3.0/byteblower_test_framework/_traffic/ipv6/frame.py
--rw-r--r--   0        0        0     6621 2024-01-31 12:44:51.237568 byteblower_test_framework-1.3.0/byteblower_test_framework/_traffic/mobile_frame.py
--rw-r--r--   0        0        0     1167 2024-01-22 08:40:15.834004 byteblower_test_framework-1.3.0/byteblower_test_framework/_traffic/stream.py
--rw-r--r--   0        0        0    25738 2024-02-08 16:09:16.881606 byteblower_test_framework-1.3.0/byteblower_test_framework/_traffic/tcpflow.py
--rw-r--r--   0        0        0    10951 2024-01-24 12:31:30.027391 byteblower_test_framework-1.3.0/byteblower_test_framework/_traffic/videoflow.py
--rw-r--r--   0        0        0     5977 2024-01-31 12:44:51.237568 byteblower_test_framework-1.3.0/byteblower_test_framework/_traffic/voiceflow.py
--rw-r--r--   0        0        0      160 2024-02-14 17:31:56.202227 byteblower_test_framework-1.3.0/byteblower_test_framework/_version.py
--rw-r--r--   0        0        0      615 2024-01-22 08:40:15.838004 byteblower_test_framework-1.3.0/byteblower_test_framework/all.py
--rw-r--r--   0        0        0     1587 2024-02-01 16:04:25.012924 byteblower_test_framework-1.3.0/byteblower_test_framework/analysis.py
--rw-r--r--   0        0        0     2029 2024-01-22 08:40:15.838004 byteblower_test_framework-1.3.0/byteblower_test_framework/cli.py
--rw-r--r--   0        0        0     3071 2024-01-24 12:31:30.031391 byteblower_test_framework-1.3.0/byteblower_test_framework/constants.py
--rw-r--r--   0        0        0     1496 2024-01-24 12:31:30.031391 byteblower_test_framework-1.3.0/byteblower_test_framework/endpoint.py
--rw-r--r--   0        0        0     2518 2024-02-01 16:04:25.012924 byteblower_test_framework-1.3.0/byteblower_test_framework/exceptions.py
--rw-r--r--   0        0        0      320 2024-01-22 08:40:15.838004 byteblower_test_framework-1.3.0/byteblower_test_framework/factory.py
--rw-r--r--   0        0        0      432 2024-01-24 12:31:30.031391 byteblower_test_framework-1.3.0/byteblower_test_framework/host.py
--rw-r--r--   0        0        0      356 2024-01-22 08:40:15.838004 byteblower_test_framework-1.3.0/byteblower_test_framework/logging.py
--rw-r--r--   0        0        0     1125 2024-01-22 08:40:15.838004 byteblower_test_framework-1.3.0/byteblower_test_framework/report.py
--rw-r--r--   0        0        0      127 2024-01-22 08:40:15.842004 byteblower_test_framework-1.3.0/byteblower_test_framework/run.py
--rw-r--r--   0        0        0     3457 2024-02-01 08:31:17.044440 byteblower_test_framework-1.3.0/byteblower_test_framework/traffic.py
--rw-r--r--   0        0        0        7 2024-01-22 08:40:15.842004 byteblower_test_framework-1.3.0/docs/.gitignore
--rw-r--r--   0        0        0      638 2024-01-22 08:40:15.842004 byteblower_test_framework-1.3.0/docs/Makefile
--rw-r--r--   0        0        0       63 2024-02-13 11:59:18.018812 byteblower_test_framework-1.3.0/docs/source/.gitignore
--rw-r--r--   0        0        0      961 2024-01-25 08:30:59.770528 byteblower_test_framework-1.3.0/docs/source/_include/_example_test_scenario.rst
--rw-r--r--   0        0        0        0 2024-02-14 17:31:39.094158 byteblower_test_framework-1.3.0/docs/source/_static/.gitkeep
--rw-r--r--   0        0        0      301 2024-02-07 11:13:37.243129 byteblower_test_framework-1.3.0/docs/source/_static/excentis.css
--rw-r--r--   0        0        0    18577 2024-02-14 16:03:06.164761 byteblower_test_framework-1.3.0/docs/source/changelog.rst
--rw-r--r--   0        0        0      386 2024-01-25 08:30:59.770528 byteblower_test_framework-1.3.0/docs/source/cli/config_file.rst
--rw-r--r--   0        0        0     4269 2024-02-07 14:08:47.543473 byteblower_test_framework-1.3.0/docs/source/cli/index.rst
--rw-r--r--   0        0        0    10108 2024-02-14 17:27:07.553050 byteblower_test_framework-1.3.0/docs/source/conf.py
--rw-r--r--   0        0        0     4414 2024-02-02 17:21:22.225678 byteblower_test_framework-1.3.0/docs/source/config/index.rst
--rw-r--r--   0        0        0     9536 2024-02-14 16:03:06.164761 byteblower_test_framework-1.3.0/docs/source/examples/basic.rst
--rw-r--r--   0        0        0     2549 2024-02-14 16:03:06.164761 byteblower_test_framework-1.3.0/docs/source/examples/index.rst
--rw-r--r--   0        0        0    11425 2024-02-14 16:03:06.164761 byteblower_test_framework-1.3.0/docs/source/examples/l4s.rst
--rw-r--r--   0        0        0    28655 2024-02-07 11:13:37.247129 byteblower_test_framework-1.3.0/docs/source/extra/byteblower-test-framework/json/cli-config-schema.json
--rw-r--r--   0        0        0     1827 2024-02-12 10:55:08.385946 byteblower_test_framework-1.3.0/docs/source/extra/byteblower-test-framework/json/endpoint/byteblower_test_framework.json
--rw-r--r--   0        0        0     2422 2024-02-14 16:03:06.168761 byteblower_test_framework-1.3.0/docs/source/extra/byteblower-test-framework/json/l4s/endpoint/byteblower_test_framework.json
--rw-r--r--   0        0        0     2395 2024-02-14 16:03:06.172761 byteblower_test_framework-1.3.0/docs/source/extra/byteblower-test-framework/json/l4s/port/byteblower_test_framework.json
--rw-r--r--   0        0        0     1832 2024-02-12 10:55:08.385946 byteblower_test_framework-1.3.0/docs/source/extra/byteblower-test-framework/json/port/byteblower_test_framework.json
--rw-r--r--   0        0        0    10037 2024-02-14 14:34:29.767432 byteblower_test_framework-1.3.0/docs/source/images/examples/basic/html_report_config.png
--rw-r--r--   0        0        0    33764 2024-02-14 14:34:29.767432 byteblower_test_framework-1.3.0/docs/source/images/examples/basic/html_report_correlated.png
--rw-r--r--   0        0        0    11147 2024-02-14 14:34:29.767432 byteblower_test_framework-1.3.0/docs/source/images/examples/basic/html_report_http_analysis.png
--rw-r--r--   0        0        0    35739 2024-02-12 10:55:08.389946 byteblower_test_framework-1.3.0/docs/source/images/examples/basic/html_report_http_config.png
--rw-r--r--   0        0        0    56274 2024-02-07 12:07:39.596659 byteblower_test_framework-1.3.0/docs/source/images/examples/basic/html_report_http_graph.png
--rw-r--r--   0        0        0   177513 2024-02-14 14:34:29.771432 byteblower_test_framework-1.3.0/docs/source/images/examples/basic/html_report_http_reverse_flow.png
--rw-r--r--   0        0        0    18205 2024-02-14 14:34:29.775432 byteblower_test_framework-1.3.0/docs/source/images/examples/basic/html_report_status_and_env.png
--rw-r--r--   0        0        0    48702 2024-02-14 14:34:29.775432 byteblower_test_framework-1.3.0/docs/source/images/examples/basic/html_report_udp_cdf_graph.png
--rw-r--r--   0        0        0    43215 2024-02-14 14:34:29.775432 byteblower_test_framework-1.3.0/docs/source/images/examples/basic/html_report_udp_cdf_status_and_stats.png
--rw-r--r--   0        0        0    16339 2024-02-14 14:34:29.779432 byteblower_test_framework-1.3.0/docs/source/images/examples/basic/html_report_udp_config.png
--rw-r--r--   0        0        0    41786 2024-02-07 12:07:39.600659 byteblower_test_framework-1.3.0/docs/source/images/examples/basic/html_report_udp_loss_analyser.png
--rw-r--r--   0        0        0   137274 2024-02-14 14:34:29.779432 byteblower_test_framework-1.3.0/docs/source/images/examples/basic/html_report_udp_loss_graph.png
--rw-r--r--   0        0        0    40664 2024-02-14 14:34:29.779432 byteblower_test_framework-1.3.0/docs/source/images/examples/basic/html_report_udp_loss_stats.png
--rw-r--r--   0        0        0    18348 2024-02-12 10:55:08.393946 byteblower_test_framework-1.3.0/docs/source/images/examples/l4s_basic/html_report_config.png
--rw-r--r--   0        0        0    11366 2024-02-14 14:34:29.783432 byteblower_test_framework-1.3.0/docs/source/images/examples/l4s_basic/html_report_http_analysis.png
--rw-r--r--   0        0        0    37382 2024-02-12 10:55:08.393946 byteblower_test_framework-1.3.0/docs/source/images/examples/l4s_basic/html_report_http_config.png
--rw-r--r--   0        0        0   122058 2024-02-12 10:55:08.397946 byteblower_test_framework-1.3.0/docs/source/images/examples/l4s_basic/html_report_http_graph.png
--rw-r--r--   0        0        0    11136 2024-02-14 14:34:29.783432 byteblower_test_framework-1.3.0/docs/source/images/examples/l4s_basic/html_report_l4s_http_analysis.png
--rw-r--r--   0        0        0    37547 2024-02-12 10:55:08.401946 byteblower_test_framework-1.3.0/docs/source/images/examples/l4s_basic/html_report_l4s_http_config.png
--rw-r--r--   0        0        0   118393 2024-02-12 10:55:08.401946 byteblower_test_framework-1.3.0/docs/source/images/examples/l4s_basic/html_report_l4s_http_graph.png
--rw-r--r--   0        0        0    19400 2024-02-14 14:34:29.783432 byteblower_test_framework-1.3.0/docs/source/images/examples/l4s_basic/html_report_status_and_env.png
--rw-r--r--   0        0        0    30636 2024-02-12 10:55:08.405946 byteblower_test_framework-1.3.0/docs/source/images/examples/l4s_basic/html_report_udp_config.png
--rw-r--r--   0        0        0    50195 2024-02-12 10:55:08.405946 byteblower_test_framework-1.3.0/docs/source/images/examples/l4s_basic/html_report_udp_graph.png
--rw-r--r--   0        0        0    39415 2024-02-12 10:55:08.405946 byteblower_test_framework-1.3.0/docs/source/images/examples/l4s_basic/html_report_udp_stats.png
--rw-r--r--   0        0        0     5586 2024-02-12 10:55:08.405946 byteblower_test_framework-1.3.0/docs/source/images/examples/l4s_basic/html_report_udp_status.png
--rw-r--r--   0        0        0    96873 2024-02-13 21:24:39.668922 byteblower_test_framework-1.3.0/docs/source/images/overview/compare_latency_ccdf.png
--rw-r--r--   0        0        0     9201 2024-02-13 21:24:39.672922 byteblower_test_framework-1.3.0/docs/source/images/overview/kpi_analysis.png
--rw-r--r--   0        0        0     4401 2024-02-13 21:24:39.672922 byteblower_test_framework-1.3.0/docs/source/images/overview/kpi_summary.png
--rw-r--r--   0        0        0    53638 2024-02-13 21:24:39.672922 byteblower_test_framework-1.3.0/docs/source/images/overview/latency_ccdf.png
--rw-r--r--   0        0        0    71169 2024-02-13 21:24:39.676922 byteblower_test_framework-1.3.0/docs/source/images/overview/latency_cdf.png
--rw-r--r--   0        0        0     6575 2024-02-13 21:24:39.676922 byteblower_test_framework-1.3.0/docs/source/images/overview/streaming_video_buffer_summary.png
--rw-r--r--   0        0        0   123877 2024-02-13 21:24:39.680922 byteblower_test_framework-1.3.0/docs/source/images/overview/streaming_video_graph_over_time.png
--rw-r--r--   0        0        0   173390 2024-02-13 21:24:39.680922 byteblower_test_framework-1.3.0/docs/source/images/overview/tcp_graph_over_time.png
--rw-r--r--   0        0        0   160349 2024-02-13 21:24:39.684922 byteblower_test_framework-1.3.0/docs/source/images/overview/voice_graph_over_time.png
--rw-r--r--   0        0        0     9450 2024-02-13 21:24:39.684922 byteblower_test_framework-1.3.0/docs/source/images/overview/voice_summary.png
--rw-r--r--   0        0        0      525 2024-02-13 10:24:07.249939 byteblower_test_framework-1.3.0/docs/source/index.rst
--rw-r--r--   0        0        0     4283 2024-02-14 14:25:24.869471 byteblower_test_framework-1.3.0/docs/source/master_index.rst
--rw-r--r--   0        0        0     6423 2024-02-14 14:25:24.869471 byteblower_test_framework-1.3.0/docs/source/overview.rst
--rw-r--r--   0        0        0     5311 2024-02-13 09:20:02.891694 byteblower_test_framework-1.3.0/docs/source/quick_start.rst
--rw-r--r--   0        0        0      117 2024-01-22 08:40:15.846004 byteblower_test_framework-1.3.0/docs/source/reference.rst
--rw-r--r--   0        0        0      192 2024-02-14 17:31:27.000000 byteblower_test_framework-1.3.0/docs/source/reference/byteblower_test_framework.all.rst
--rw-r--r--   0        0        0      194 2024-02-14 17:31:26.000000 byteblower_test_framework-1.3.0/docs/source/reference/byteblower_test_framework.analysis.rst
--rw-r--r--   0        0        0      179 2024-02-14 17:31:26.000000 byteblower_test_framework-1.3.0/docs/source/reference/byteblower_test_framework.cli.rst
--rw-r--r--   0        0        0      197 2024-02-14 17:31:26.000000 byteblower_test_framework-1.3.0/docs/source/reference/byteblower_test_framework.constants.rst
--rw-r--r--   0        0        0      194 2024-02-14 17:31:26.000000 byteblower_test_framework-1.3.0/docs/source/reference/byteblower_test_framework.endpoint.rst
--rw-r--r--   0        0        0      200 2024-02-14 17:31:26.000000 byteblower_test_framework-1.3.0/docs/source/reference/byteblower_test_framework.exceptions.rst
--rw-r--r--   0        0        0      191 2024-02-14 17:31:26.000000 byteblower_test_framework-1.3.0/docs/source/reference/byteblower_test_framework.factory.rst
--rw-r--r--   0        0        0      182 2024-02-14 17:31:26.000000 byteblower_test_framework-1.3.0/docs/source/reference/byteblower_test_framework.host.rst
--rw-r--r--   0        0        0      191 2024-02-14 17:31:26.000000 byteblower_test_framework-1.3.0/docs/source/reference/byteblower_test_framework.logging.rst
--rw-r--r--   0        0        0      188 2024-02-14 17:31:26.000000 byteblower_test_framework-1.3.0/docs/source/reference/byteblower_test_framework.report.rst
--rw-r--r--   0        0        0      691 2024-02-14 17:31:26.000000 byteblower_test_framework-1.3.0/docs/source/reference/byteblower_test_framework.rst
--rw-r--r--   0        0        0      179 2024-02-14 17:31:26.000000 byteblower_test_framework-1.3.0/docs/source/reference/byteblower_test_framework.run.rst
--rw-r--r--   0        0        0      191 2024-02-14 17:31:26.000000 byteblower_test_framework-1.3.0/docs/source/reference/byteblower_test_framework.traffic.rst
--rw-r--r--   0        0        0      112 2024-02-14 17:31:26.000000 byteblower_test_framework-1.3.0/docs/source/reference/modules.rst
--rw-r--r--   0        0        0      608 2024-01-22 08:40:15.846004 byteblower_test_framework-1.3.0/docs/source/todo.rst
--rw-r--r--   0        0        0     1590 2024-01-31 15:03:32.589755 byteblower_test_framework-1.3.0/docs/source/versioning.rst
--rw-r--r--   0        0        0     9315 2024-02-14 17:27:07.553050 byteblower_test_framework-1.3.0/pyproject.toml
--rw-r--r--   0        0        0    20431 1970-01-01 00:00:00.000000 byteblower_test_framework-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     7652 2024-01-22 08:45:34.265233 byteblower_test_framework-1.3.1/LICENSE
+-rw-r--r--   0        0        0    17271 2024-04-26 09:58:57.437603 byteblower_test_framework-1.3.1/README.pypi.rst
+-rw-r--r--   0        0        0      132 2024-01-22 08:45:34.269234 byteblower_test_framework-1.3.1/byteblower_test_framework/__init__.py
+-rw-r--r--   0        0        0      341 2024-01-22 08:45:34.269234 byteblower_test_framework-1.3.1/byteblower_test_framework/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-26 12:27:30.381713 byteblower_test_framework-1.3.1/byteblower_test_framework/_analysis/__init__.py
+-rw-r--r--   0        0        0    23827 2024-01-22 08:45:34.269234 byteblower_test_framework-1.3.1/byteblower_test_framework/_analysis/analyseraggregator.py
+-rw-r--r--   0        0        0    12528 2024-02-02 09:31:41.951480 byteblower_test_framework-1.3.1/byteblower_test_framework/_analysis/bufferanalyser.py
+-rw-r--r--   0        0        0       40 2024-01-22 08:45:34.273234 byteblower_test_framework-1.3.1/byteblower_test_framework/_analysis/data_analysis/__init__.py
+-rw-r--r--   0        0        0     2001 2024-01-24 12:31:04.669292 byteblower_test_framework-1.3.1/byteblower_test_framework/_analysis/data_analysis/data_analyser.py
+-rw-r--r--   0        0        0    37770 2024-04-26 09:58:57.437603 byteblower_test_framework-1.3.1/byteblower_test_framework/_analysis/data_analysis/frameblasting.py
+-rw-r--r--   0        0        0     4481 2024-02-07 13:06:29.807022 byteblower_test_framework-1.3.1/byteblower_test_framework/_analysis/data_analysis/tcp.py
+-rw-r--r--   0        0        0       40 2024-01-22 08:45:34.273234 byteblower_test_framework-1.3.1/byteblower_test_framework/_analysis/data_gathering/__init__.py
+-rw-r--r--   0        0        0     5623 2024-01-24 12:31:04.669292 byteblower_test_framework-1.3.1/byteblower_test_framework/_analysis/data_gathering/_filter.py
+-rw-r--r--   0        0        0     8941 2024-01-25 10:20:07.471131 byteblower_test_framework-1.3.1/byteblower_test_framework/_analysis/data_gathering/_rx_trigger_controller.py
+-rw-r--r--   0        0        0     1953 2024-01-25 10:20:07.471131 byteblower_test_framework-1.3.1/byteblower_test_framework/_analysis/data_gathering/data_gatherer.py
+-rw-r--r--   0        0        0     7103 2024-01-24 12:31:04.673292 byteblower_test_framework-1.3.1/byteblower_test_framework/_analysis/data_gathering/stream.py
+-rw-r--r--   0        0        0    29267 2024-02-13 13:47:26.435633 byteblower_test_framework-1.3.1/byteblower_test_framework/_analysis/data_gathering/tcp.py
+-rw-r--r--   0        0        0    27881 2024-01-25 09:05:39.204815 byteblower_test_framework-1.3.1/byteblower_test_framework/_analysis/data_gathering/trigger.py
+-rw-r--r--   0        0        0     6140 2024-02-02 09:31:41.955480 byteblower_test_framework-1.3.1/byteblower_test_framework/_analysis/flow_analyser.py
+-rw-r--r--   0        0        0     9006 2024-02-02 09:31:41.955480 byteblower_test_framework-1.3.1/byteblower_test_framework/_analysis/framelossanalyser.py
+-rw-r--r--   0        0        0     8368 2024-01-24 12:31:04.673292 byteblower_test_framework-1.3.1/byteblower_test_framework/_analysis/helpers.py
+-rw-r--r--   0        0        0     8184 2024-02-05 08:49:42.266897 byteblower_test_framework-1.3.1/byteblower_test_framework/_analysis/httpanalyser.py
+-rw-r--r--   0        0        0     3891 2024-01-22 08:45:34.277233 byteblower_test_framework-1.3.1/byteblower_test_framework/_analysis/latencyaggregator.py
+-rw-r--r--   0        0        0    25190 2024-02-02 09:31:41.955480 byteblower_test_framework-1.3.1/byteblower_test_framework/_analysis/latencyanalyser.py
+-rw-r--r--   0        0        0       40 2024-01-22 08:45:34.281233 byteblower_test_framework-1.3.1/byteblower_test_framework/_analysis/plotting/__init__.py
+-rw-r--r--   0        0        0     4826 2024-01-22 08:45:34.281233 byteblower_test_framework-1.3.1/byteblower_test_framework/_analysis/plotting/generic_chart.py
+-rw-r--r--   0        0        0       31 2024-01-22 08:45:34.281233 byteblower_test_framework-1.3.1/byteblower_test_framework/_analysis/render/__init__.py
+-rw-r--r--   0        0        0    20121 2024-01-22 08:45:34.281233 byteblower_test_framework-1.3.1/byteblower_test_framework/_analysis/render/frameblasting.py
+-rw-r--r--   0        0        0      889 2024-01-22 08:45:34.281233 byteblower_test_framework-1.3.1/byteblower_test_framework/_analysis/render/renderer.py
+-rw-r--r--   0        0        0    15852 2024-02-07 14:07:55.452548 byteblower_test_framework-1.3.1/byteblower_test_framework/_analysis/render/tcp.py
+-rw-r--r--   0        0        0       34 2024-01-22 08:45:34.281233 byteblower_test_framework-1.3.1/byteblower_test_framework/_analysis/storage/__init__.py
+-rw-r--r--   0        0        0       44 2024-01-22 08:45:34.281233 byteblower_test_framework-1.3.1/byteblower_test_framework/_analysis/storage/data_store.py
+-rw-r--r--   0        0        0     2406 2024-01-22 08:45:34.281233 byteblower_test_framework-1.3.1/byteblower_test_framework/_analysis/storage/frame_count.py
+-rw-r--r--   0        0        0     1363 2024-01-22 08:45:34.281233 byteblower_test_framework-1.3.1/byteblower_test_framework/_analysis/storage/stream.py
+-rw-r--r--   0        0        0     8577 2024-02-05 15:32:38.602771 byteblower_test_framework-1.3.1/byteblower_test_framework/_analysis/storage/tcp.py
+-rw-r--r--   0        0        0     5425 2024-01-22 08:45:34.285234 byteblower_test_framework-1.3.1/byteblower_test_framework/_analysis/storage/trigger.py
+-rw-r--r--   0        0        0     4403 2024-02-02 09:31:41.959480 byteblower_test_framework-1.3.1/byteblower_test_framework/_analysis/voiceanalyser.py
+-rw-r--r--   0        0        0       46 2024-01-22 08:45:34.285234 byteblower_test_framework-1.3.1/byteblower_test_framework/_cli/__init__.py
+-rw-r--r--   0        0        0     3495 2024-01-22 08:45:34.285234 byteblower_test_framework-1.3.1/byteblower_test_framework/_cli/_arguments.py
+-rw-r--r--   0        0        0      694 2024-01-22 08:45:34.285234 byteblower_test_framework-1.3.1/byteblower_test_framework/_cli/_config_file.py
+-rw-r--r--   0        0        0      482 2024-01-24 12:31:04.677292 byteblower_test_framework-1.3.1/byteblower_test_framework/_cli/_definitions.py
+-rw-r--r--   0        0        0     2853 2024-01-24 12:31:04.677292 byteblower_test_framework-1.3.1/byteblower_test_framework/_cli/_endpoint_factory.py
+-rw-r--r--   0        0        0     7425 2024-02-02 17:21:20.756347 byteblower_test_framework-1.3.1/byteblower_test_framework/_cli/_flow_factory.py
+-rw-r--r--   0        0        0     2426 2024-01-24 12:31:04.681292 byteblower_test_framework-1.3.1/byteblower_test_framework/_cli/_port_factory.py
+-rw-r--r--   0        0        0    13360 2024-01-24 12:31:04.681292 byteblower_test_framework-1.3.1/byteblower_test_framework/_cli/_with_json_configfile.py
+-rw-r--r--   0        0        0      234 2024-01-22 08:45:34.285234 byteblower_test_framework-1.3.1/byteblower_test_framework/_cli/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-26 12:27:30.389713 byteblower_test_framework-1.3.1/byteblower_test_framework/_endpoint/__init__.py
+-rw-r--r--   0        0        0     8225 2024-01-24 12:31:04.681292 byteblower_test_framework-1.3.1/byteblower_test_framework/_endpoint/endpoint.py
+-rw-r--r--   0        0        0     4563 2024-04-26 09:32:06.419621 byteblower_test_framework-1.3.1/byteblower_test_framework/_endpoint/helpers.py
+-rw-r--r--   0        0        0        0 2024-04-26 12:27:30.389713 byteblower_test_framework-1.3.1/byteblower_test_framework/_endpoint/ipv4/__init__.py
+-rw-r--r--   0        0        0     3038 2024-01-24 12:31:04.681292 byteblower_test_framework-1.3.1/byteblower_test_framework/_endpoint/ipv4/endpoint.py
+-rw-r--r--   0        0        0     4202 2024-01-24 12:31:04.681292 byteblower_test_framework-1.3.1/byteblower_test_framework/_endpoint/ipv4/nat.py
+-rw-r--r--   0        0        0     4507 2024-01-24 12:31:04.681292 byteblower_test_framework-1.3.1/byteblower_test_framework/_endpoint/ipv4/port.py
+-rw-r--r--   0        0        0        0 2024-04-26 12:27:30.389713 byteblower_test_framework-1.3.1/byteblower_test_framework/_endpoint/ipv6/__init__.py
+-rw-r--r--   0        0        0     5298 2024-01-24 12:31:04.681292 byteblower_test_framework-1.3.1/byteblower_test_framework/_endpoint/ipv6/endpoint.py
+-rw-r--r--   0        0        0     4807 2024-01-22 08:45:34.289234 byteblower_test_framework-1.3.1/byteblower_test_framework/_endpoint/ipv6/port.py
+-rw-r--r--   0        0        0    12759 2024-04-26 09:32:06.419621 byteblower_test_framework-1.3.1/byteblower_test_framework/_endpoint/nat_discovery.py
+-rw-r--r--   0        0        0     4617 2024-01-24 12:31:04.685292 byteblower_test_framework-1.3.1/byteblower_test_framework/_endpoint/nat_endpoint.py
+-rw-r--r--   0        0        0    15498 2024-01-24 12:31:04.685292 byteblower_test_framework-1.3.1/byteblower_test_framework/_endpoint/port.py
+-rw-r--r--   0        0        0        0 2024-04-26 12:27:30.389713 byteblower_test_framework-1.3.1/byteblower_test_framework/_factory/__init__.py
+-rw-r--r--   0        0        0     4274 2024-01-24 12:31:04.685292 byteblower_test_framework-1.3.1/byteblower_test_framework/_factory/frame.py
+-rw-r--r--   0        0        0       55 2024-01-22 08:45:34.289234 byteblower_test_framework-1.3.1/byteblower_test_framework/_helpers/__init__.py
+-rw-r--r--   0        0        0     2087 2024-02-12 10:56:56.045472 byteblower_test_framework-1.3.1/byteblower_test_framework/_helpers/capabilities.py
+-rw-r--r--   0        0        0      282 2024-02-12 10:56:56.045472 byteblower_test_framework-1.3.1/byteblower_test_framework/_helpers/compat.py
+-rw-r--r--   0        0        0     7338 2024-01-24 12:31:04.685292 byteblower_test_framework-1.3.1/byteblower_test_framework/_helpers/syncexec.py
+-rw-r--r--   0        0        0     1098 2024-01-24 12:31:04.685292 byteblower_test_framework-1.3.1/byteblower_test_framework/_helpers/taggable.py
+-rw-r--r--   0        0        0        0 2024-04-26 12:27:30.389713 byteblower_test_framework-1.3.1/byteblower_test_framework/_host/__init__.py
+-rw-r--r--   0        0        0     6743 2024-01-24 12:31:04.685292 byteblower_test_framework-1.3.1/byteblower_test_framework/_host/meetingpoint.py
+-rw-r--r--   0        0        0     3408 2024-01-22 08:45:34.293233 byteblower_test_framework-1.3.1/byteblower_test_framework/_host/server.py
+-rw-r--r--   0        0        0        0 2024-04-26 12:27:30.389713 byteblower_test_framework-1.3.1/byteblower_test_framework/_report/__init__.py
+-rw-r--r--   0        0        0    10512 2024-01-22 08:45:34.293233 byteblower_test_framework-1.3.1/byteblower_test_framework/_report/byteblowerhtmlreport.py
+-rw-r--r--   0        0        0     8222 2024-01-22 08:45:34.293233 byteblower_test_framework-1.3.1/byteblower_test_framework/_report/byteblowerjsonreport.py
+-rw-r--r--   0        0        0     4109 2024-01-22 08:45:34.293233 byteblower_test_framework-1.3.1/byteblower_test_framework/_report/byteblowerreport.py
+-rw-r--r--   0        0        0     3732 2024-01-22 08:45:34.293233 byteblower_test_framework-1.3.1/byteblower_test_framework/_report/byteblowerunittestreport.py
+-rw-r--r--   0        0        0      327 2024-01-22 08:45:34.293233 byteblower_test_framework-1.3.1/byteblower_test_framework/_report/helper.py
+-rw-r--r--   0        0        0     1947 2024-01-22 08:45:34.293233 byteblower_test_framework-1.3.1/byteblower_test_framework/_report/options.py
+-rw-r--r--   0        0        0  3089944 2024-01-22 08:45:34.349234 byteblower_test_framework-1.3.1/byteblower_test_framework/_report/templates/embedded-fonts.css
+-rw-r--r--   0        0        0      901 2024-01-22 08:45:34.353234 byteblower_test_framework-1.3.1/byteblower_test_framework/_report/templates/flow_section.html
+-rw-r--r--   0        0        0      673 2024-04-26 09:58:57.437603 byteblower_test_framework-1.3.1/byteblower_test_framework/_report/templates/report.html
+-rw-r--r--   0        0        0    59284 2024-01-22 08:45:34.353234 byteblower_test_framework-1.3.1/byteblower_test_framework/_report/templates/report_footer.html
+-rw-r--r--   0        0        0       97 2024-01-22 08:45:34.353234 byteblower_test_framework-1.3.1/byteblower_test_framework/_report/templates/report_head_style.html
+-rw-r--r--   0        0        0    11242 2024-01-22 08:45:34.353234 byteblower_test_framework-1.3.1/byteblower_test_framework/_report/templates/report_header.html
+-rw-r--r--   0        0        0      451 2024-01-22 08:45:34.353234 byteblower_test_framework-1.3.1/byteblower_test_framework/_report/templates/report_main.html
+-rw-r--r--   0        0        0     1631 2024-01-22 08:45:34.353234 byteblower_test_framework-1.3.1/byteblower_test_framework/_report/templates/report_pass_fail.html
+-rw-r--r--   0        0        0      391 2024-01-22 08:45:34.353234 byteblower_test_framework-1.3.1/byteblower_test_framework/_report/templates/test_section.html
+-rw-r--r--   0        0        0     7389 2024-01-22 08:45:34.353234 byteblower_test_framework-1.3.1/byteblower_test_framework/_report/templates/testframework.css
+-rw-r--r--   0        0        0     4155 2024-01-22 08:45:34.353234 byteblower_test_framework-1.3.1/byteblower_test_framework/_report/unittestreport.py
+-rw-r--r--   0        0        0    18629 2024-01-25 09:05:39.208815 byteblower_test_framework-1.3.1/byteblower_test_framework/_scenario.py
+-rw-r--r--   0        0        0        0 2024-04-26 12:27:30.389713 byteblower_test_framework-1.3.1/byteblower_test_framework/_traffic/__init__.py
+-rw-r--r--   0        0        0    15879 2024-02-13 15:33:26.362349 byteblower_test_framework-1.3.1/byteblower_test_framework/_traffic/_http_client_controller.py
+-rw-r--r--   0        0        0     6421 2024-01-24 12:31:04.685292 byteblower_test_framework-1.3.1/byteblower_test_framework/_traffic/_tx_stream_controller.py
+-rw-r--r--   0        0        0     1707 2024-01-24 12:31:04.685292 byteblower_test_framework-1.3.1/byteblower_test_framework/_traffic/constants.py
+-rw-r--r--   0        0        0    11192 2024-01-24 12:31:04.689292 byteblower_test_framework-1.3.1/byteblower_test_framework/_traffic/flow.py
+-rw-r--r--   0        0        0     6016 2024-04-26 09:32:06.423621 byteblower_test_framework-1.3.1/byteblower_test_framework/_traffic/frame.py
+-rw-r--r--   0        0        0    16972 2024-01-25 10:20:07.475131 byteblower_test_framework-1.3.1/byteblower_test_framework/_traffic/frameblastingflow.py
+-rw-r--r--   0        0        0     7242 2024-01-31 12:44:55.099177 byteblower_test_framework-1.3.1/byteblower_test_framework/_traffic/gamingflow.py
+-rw-r--r--   0        0        0     4595 2024-01-24 12:31:04.689292 byteblower_test_framework-1.3.1/byteblower_test_framework/_traffic/helpers.py
+-rw-r--r--   0        0        0    16371 2024-02-05 15:32:38.602771 byteblower_test_framework-1.3.1/byteblower_test_framework/_traffic/httpflow.py
+-rw-r--r--   0        0        0     5348 2024-01-24 12:31:04.689292 byteblower_test_framework-1.3.1/byteblower_test_framework/_traffic/imix.py
+-rw-r--r--   0        0        0        0 2024-04-26 12:27:30.389713 byteblower_test_framework-1.3.1/byteblower_test_framework/_traffic/ipv4/__init__.py
+-rw-r--r--   0        0        0     4836 2024-01-31 12:44:55.103177 byteblower_test_framework-1.3.1/byteblower_test_framework/_traffic/ipv4/frame.py
+-rw-r--r--   0        0        0        0 2024-04-26 12:27:30.389713 byteblower_test_framework-1.3.1/byteblower_test_framework/_traffic/ipv6/__init__.py
+-rw-r--r--   0        0        0     4569 2024-01-31 12:44:55.103177 byteblower_test_framework-1.3.1/byteblower_test_framework/_traffic/ipv6/frame.py
+-rw-r--r--   0        0        0     6621 2024-01-31 12:44:55.103177 byteblower_test_framework-1.3.1/byteblower_test_framework/_traffic/mobile_frame.py
+-rw-r--r--   0        0        0     1167 2024-01-22 08:45:34.361234 byteblower_test_framework-1.3.1/byteblower_test_framework/_traffic/stream.py
+-rw-r--r--   0        0        0    25738 2024-02-12 10:56:56.045472 byteblower_test_framework-1.3.1/byteblower_test_framework/_traffic/tcpflow.py
+-rw-r--r--   0        0        0    10951 2024-01-24 12:31:04.693292 byteblower_test_framework-1.3.1/byteblower_test_framework/_traffic/videoflow.py
+-rw-r--r--   0        0        0     5977 2024-01-31 12:44:55.103177 byteblower_test_framework-1.3.1/byteblower_test_framework/_traffic/voiceflow.py
+-rw-r--r--   0        0        0      160 2024-04-26 12:27:43.185733 byteblower_test_framework-1.3.1/byteblower_test_framework/_version.py
+-rw-r--r--   0        0        0      615 2024-01-22 08:45:34.365234 byteblower_test_framework-1.3.1/byteblower_test_framework/all.py
+-rw-r--r--   0        0        0     1587 2024-02-02 09:31:41.967480 byteblower_test_framework-1.3.1/byteblower_test_framework/analysis.py
+-rw-r--r--   0        0        0     2029 2024-01-22 08:45:34.365234 byteblower_test_framework-1.3.1/byteblower_test_framework/cli.py
+-rw-r--r--   0        0        0     3071 2024-01-24 12:31:04.693292 byteblower_test_framework-1.3.1/byteblower_test_framework/constants.py
+-rw-r--r--   0        0        0     1496 2024-01-24 12:31:04.697292 byteblower_test_framework-1.3.1/byteblower_test_framework/endpoint.py
+-rw-r--r--   0        0        0     2518 2024-02-02 09:31:41.967480 byteblower_test_framework-1.3.1/byteblower_test_framework/exceptions.py
+-rw-r--r--   0        0        0      320 2024-01-22 08:45:34.365234 byteblower_test_framework-1.3.1/byteblower_test_framework/factory.py
+-rw-r--r--   0        0        0      432 2024-01-24 12:31:04.697292 byteblower_test_framework-1.3.1/byteblower_test_framework/host.py
+-rw-r--r--   0        0        0      356 2024-01-22 08:45:34.365234 byteblower_test_framework-1.3.1/byteblower_test_framework/logging.py
+-rw-r--r--   0        0        0     1125 2024-01-22 08:45:34.365234 byteblower_test_framework-1.3.1/byteblower_test_framework/report.py
+-rw-r--r--   0        0        0      127 2024-01-22 08:45:34.365234 byteblower_test_framework-1.3.1/byteblower_test_framework/run.py
+-rw-r--r--   0        0        0     3457 2024-02-01 08:33:05.557816 byteblower_test_framework-1.3.1/byteblower_test_framework/traffic.py
+-rw-r--r--   0        0        0        7 2024-01-22 08:45:34.365234 byteblower_test_framework-1.3.1/docs/.gitignore
+-rw-r--r--   0        0        0      638 2024-01-22 08:45:34.365234 byteblower_test_framework-1.3.1/docs/Makefile
+-rw-r--r--   0        0        0       63 2024-02-13 12:00:09.461043 byteblower_test_framework-1.3.1/docs/source/.gitignore
+-rw-r--r--   0        0        0      961 2024-01-25 08:31:25.274831 byteblower_test_framework-1.3.1/docs/source/_include/_example_test_scenario.rst
+-rw-r--r--   0        0        0        0 2024-04-26 12:27:30.393713 byteblower_test_framework-1.3.1/docs/source/_static/.gitkeep
+-rw-r--r--   0        0        0      301 2024-02-07 11:19:00.562750 byteblower_test_framework-1.3.1/docs/source/_static/excentis.css
+-rw-r--r--   0        0        0    18940 2024-04-26 09:58:57.437603 byteblower_test_framework-1.3.1/docs/source/changelog.rst
+-rw-r--r--   0        0        0      386 2024-01-25 08:31:25.278831 byteblower_test_framework-1.3.1/docs/source/cli/config_file.rst
+-rw-r--r--   0        0        0     4269 2024-02-07 14:07:55.452548 byteblower_test_framework-1.3.1/docs/source/cli/index.rst
+-rw-r--r--   0        0        0    10108 2024-04-26 09:58:57.441603 byteblower_test_framework-1.3.1/docs/source/conf.py
+-rw-r--r--   0        0        0     4414 2024-02-02 09:31:41.971480 byteblower_test_framework-1.3.1/docs/source/config/index.rst
+-rw-r--r--   0        0        0     9536 2024-04-22 14:59:45.328545 byteblower_test_framework-1.3.1/docs/source/examples/basic.rst
+-rw-r--r--   0        0        0     2549 2024-02-14 16:23:53.871927 byteblower_test_framework-1.3.1/docs/source/examples/index.rst
+-rw-r--r--   0        0        0    11425 2024-04-22 14:59:45.336545 byteblower_test_framework-1.3.1/docs/source/examples/l4s.rst
+-rw-r--r--   0        0        0    31715 2024-04-26 09:58:57.441603 byteblower_test_framework-1.3.1/docs/source/extra/byteblower-test-framework/json/cli-config-schema.json
+-rw-r--r--   0        0        0     1894 2024-04-26 09:58:57.441603 byteblower_test_framework-1.3.1/docs/source/extra/byteblower-test-framework/json/endpoint/byteblower_test_framework.json
+-rw-r--r--   0        0        0     2510 2024-04-26 09:58:57.441603 byteblower_test_framework-1.3.1/docs/source/extra/byteblower-test-framework/json/l4s/endpoint/byteblower_test_framework.json
+-rw-r--r--   0        0        0     2483 2024-04-26 09:58:57.441603 byteblower_test_framework-1.3.1/docs/source/extra/byteblower-test-framework/json/l4s/port/byteblower_test_framework.json
+-rw-r--r--   0        0        0     1924 2024-04-26 09:58:57.441603 byteblower_test_framework-1.3.1/docs/source/extra/byteblower-test-framework/json/port/byteblower_test_framework.json
+-rw-r--r--   0        0        0    10037 2024-02-14 15:18:28.843744 byteblower_test_framework-1.3.1/docs/source/images/examples/basic/html_report_config.png
+-rw-r--r--   0        0        0    33764 2024-02-14 15:18:28.843744 byteblower_test_framework-1.3.1/docs/source/images/examples/basic/html_report_correlated.png
+-rw-r--r--   0        0        0    11147 2024-02-14 15:18:28.843744 byteblower_test_framework-1.3.1/docs/source/images/examples/basic/html_report_http_analysis.png
+-rw-r--r--   0        0        0    35739 2024-02-12 10:56:56.057472 byteblower_test_framework-1.3.1/docs/source/images/examples/basic/html_report_http_config.png
+-rw-r--r--   0        0        0    56274 2024-02-07 12:07:39.982682 byteblower_test_framework-1.3.1/docs/source/images/examples/basic/html_report_http_graph.png
+-rw-r--r--   0        0        0   177513 2024-02-14 15:18:28.847744 byteblower_test_framework-1.3.1/docs/source/images/examples/basic/html_report_http_reverse_flow.png
+-rw-r--r--   0        0        0    18205 2024-02-14 15:18:28.851744 byteblower_test_framework-1.3.1/docs/source/images/examples/basic/html_report_status_and_env.png
+-rw-r--r--   0        0        0    48702 2024-02-14 15:18:28.851744 byteblower_test_framework-1.3.1/docs/source/images/examples/basic/html_report_udp_cdf_graph.png
+-rw-r--r--   0        0        0    43215 2024-02-14 15:18:28.851744 byteblower_test_framework-1.3.1/docs/source/images/examples/basic/html_report_udp_cdf_status_and_stats.png
+-rw-r--r--   0        0        0    16339 2024-02-14 15:18:28.851744 byteblower_test_framework-1.3.1/docs/source/images/examples/basic/html_report_udp_config.png
+-rw-r--r--   0        0        0    41786 2024-02-07 12:07:39.986682 byteblower_test_framework-1.3.1/docs/source/images/examples/basic/html_report_udp_loss_analyser.png
+-rw-r--r--   0        0        0   137274 2024-02-14 15:18:28.855744 byteblower_test_framework-1.3.1/docs/source/images/examples/basic/html_report_udp_loss_graph.png
+-rw-r--r--   0        0        0    40664 2024-02-14 15:18:28.855744 byteblower_test_framework-1.3.1/docs/source/images/examples/basic/html_report_udp_loss_stats.png
+-rw-r--r--   0        0        0    18348 2024-02-12 10:56:56.057472 byteblower_test_framework-1.3.1/docs/source/images/examples/l4s_basic/html_report_config.png
+-rw-r--r--   0        0        0    11366 2024-02-14 15:18:28.855744 byteblower_test_framework-1.3.1/docs/source/images/examples/l4s_basic/html_report_http_analysis.png
+-rw-r--r--   0        0        0    37382 2024-02-12 10:56:56.061472 byteblower_test_framework-1.3.1/docs/source/images/examples/l4s_basic/html_report_http_config.png
+-rw-r--r--   0        0        0   122058 2024-02-12 10:56:56.061472 byteblower_test_framework-1.3.1/docs/source/images/examples/l4s_basic/html_report_http_graph.png
+-rw-r--r--   0        0        0    11136 2024-02-14 15:18:28.855744 byteblower_test_framework-1.3.1/docs/source/images/examples/l4s_basic/html_report_l4s_http_analysis.png
+-rw-r--r--   0        0        0    37547 2024-02-12 10:56:56.069472 byteblower_test_framework-1.3.1/docs/source/images/examples/l4s_basic/html_report_l4s_http_config.png
+-rw-r--r--   0        0        0   118393 2024-02-12 10:56:56.069472 byteblower_test_framework-1.3.1/docs/source/images/examples/l4s_basic/html_report_l4s_http_graph.png
+-rw-r--r--   0        0        0    19400 2024-02-14 15:18:28.859744 byteblower_test_framework-1.3.1/docs/source/images/examples/l4s_basic/html_report_status_and_env.png
+-rw-r--r--   0        0        0    30636 2024-02-12 10:56:56.073472 byteblower_test_framework-1.3.1/docs/source/images/examples/l4s_basic/html_report_udp_config.png
+-rw-r--r--   0        0        0    50195 2024-02-12 10:56:56.073472 byteblower_test_framework-1.3.1/docs/source/images/examples/l4s_basic/html_report_udp_graph.png
+-rw-r--r--   0        0        0    39415 2024-02-12 10:56:56.073472 byteblower_test_framework-1.3.1/docs/source/images/examples/l4s_basic/html_report_udp_stats.png
+-rw-r--r--   0        0        0     5586 2024-02-12 10:56:56.073472 byteblower_test_framework-1.3.1/docs/source/images/examples/l4s_basic/html_report_udp_status.png
+-rw-r--r--   0        0        0    96873 2024-02-13 21:24:39.798178 byteblower_test_framework-1.3.1/docs/source/images/overview/compare_latency_ccdf.png
+-rw-r--r--   0        0        0     9201 2024-02-13 21:24:39.798178 byteblower_test_framework-1.3.1/docs/source/images/overview/kpi_analysis.png
+-rw-r--r--   0        0        0     4401 2024-02-13 21:24:39.802178 byteblower_test_framework-1.3.1/docs/source/images/overview/kpi_summary.png
+-rw-r--r--   0        0        0    53638 2024-02-13 21:24:39.802178 byteblower_test_framework-1.3.1/docs/source/images/overview/latency_ccdf.png
+-rw-r--r--   0        0        0    71169 2024-02-13 21:24:39.802178 byteblower_test_framework-1.3.1/docs/source/images/overview/latency_cdf.png
+-rw-r--r--   0        0        0     6575 2024-02-13 21:24:39.806177 byteblower_test_framework-1.3.1/docs/source/images/overview/streaming_video_buffer_summary.png
+-rw-r--r--   0        0        0   123877 2024-02-13 21:24:39.806177 byteblower_test_framework-1.3.1/docs/source/images/overview/streaming_video_graph_over_time.png
+-rw-r--r--   0        0        0   173390 2024-02-13 21:24:39.810177 byteblower_test_framework-1.3.1/docs/source/images/overview/tcp_graph_over_time.png
+-rw-r--r--   0        0        0   160349 2024-02-13 21:24:39.814178 byteblower_test_framework-1.3.1/docs/source/images/overview/voice_graph_over_time.png
+-rw-r--r--   0        0        0     9450 2024-02-13 21:24:39.814178 byteblower_test_framework-1.3.1/docs/source/images/overview/voice_summary.png
+-rw-r--r--   0        0        0      525 2024-02-13 10:23:49.942891 byteblower_test_framework-1.3.1/docs/source/index.rst
+-rw-r--r--   0        0        0     4283 2024-02-14 14:25:48.599653 byteblower_test_framework-1.3.1/docs/source/master_index.rst
+-rw-r--r--   0        0        0     6423 2024-02-14 14:25:48.599653 byteblower_test_framework-1.3.1/docs/source/overview.rst
+-rw-r--r--   0        0        0     5311 2024-04-22 14:59:45.704546 byteblower_test_framework-1.3.1/docs/source/quick_start.rst
+-rw-r--r--   0        0        0      117 2024-01-22 08:45:34.373234 byteblower_test_framework-1.3.1/docs/source/reference.rst
+-rw-r--r--   0        0        0      192 2024-04-26 12:27:17.000000 byteblower_test_framework-1.3.1/docs/source/reference/byteblower_test_framework.all.rst
+-rw-r--r--   0        0        0      194 2024-04-26 12:27:17.000000 byteblower_test_framework-1.3.1/docs/source/reference/byteblower_test_framework.analysis.rst
+-rw-r--r--   0        0        0      179 2024-04-26 12:27:17.000000 byteblower_test_framework-1.3.1/docs/source/reference/byteblower_test_framework.cli.rst
+-rw-r--r--   0        0        0      197 2024-04-26 12:27:17.000000 byteblower_test_framework-1.3.1/docs/source/reference/byteblower_test_framework.constants.rst
+-rw-r--r--   0        0        0      194 2024-04-26 12:27:17.000000 byteblower_test_framework-1.3.1/docs/source/reference/byteblower_test_framework.endpoint.rst
+-rw-r--r--   0        0        0      200 2024-04-26 12:27:17.000000 byteblower_test_framework-1.3.1/docs/source/reference/byteblower_test_framework.exceptions.rst
+-rw-r--r--   0        0        0      191 2024-04-26 12:27:17.000000 byteblower_test_framework-1.3.1/docs/source/reference/byteblower_test_framework.factory.rst
+-rw-r--r--   0        0        0      182 2024-04-26 12:27:17.000000 byteblower_test_framework-1.3.1/docs/source/reference/byteblower_test_framework.host.rst
+-rw-r--r--   0        0        0      191 2024-04-26 12:27:17.000000 byteblower_test_framework-1.3.1/docs/source/reference/byteblower_test_framework.logging.rst
+-rw-r--r--   0        0        0      188 2024-04-26 12:27:17.000000 byteblower_test_framework-1.3.1/docs/source/reference/byteblower_test_framework.report.rst
+-rw-r--r--   0        0        0      691 2024-04-26 12:27:17.000000 byteblower_test_framework-1.3.1/docs/source/reference/byteblower_test_framework.rst
+-rw-r--r--   0        0        0      179 2024-04-26 12:27:17.000000 byteblower_test_framework-1.3.1/docs/source/reference/byteblower_test_framework.run.rst
+-rw-r--r--   0        0        0      191 2024-04-26 12:27:17.000000 byteblower_test_framework-1.3.1/docs/source/reference/byteblower_test_framework.traffic.rst
+-rw-r--r--   0        0        0      112 2024-04-26 12:27:17.000000 byteblower_test_framework-1.3.1/docs/source/reference/modules.rst
+-rw-r--r--   0        0        0      608 2024-01-22 08:45:34.373234 byteblower_test_framework-1.3.1/docs/source/todo.rst
+-rw-r--r--   0        0        0     1590 2024-01-31 15:03:24.624043 byteblower_test_framework-1.3.1/docs/source/versioning.rst
+-rw-r--r--   0        0        0     9315 2024-04-26 09:58:57.445603 byteblower_test_framework-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0    20431 1970-01-01 00:00:00.000000 byteblower_test_framework-1.3.1/PKG-INFO
```

### Comparing `byteblower_test_framework-1.3.0/LICENSE` & `byteblower_test_framework-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/README.pypi.rst` & `byteblower_test_framework-1.3.1/README.pypi.rst`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_analysis/analyseraggregator.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_analysis/analyseraggregator.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_analysis/bufferanalyser.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_analysis/bufferanalyser.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_analysis/data_analysis/data_analyser.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_analysis/data_analysis/data_analyser.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_analysis/data_analysis/frameblasting.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_analysis/data_analysis/frameblasting.py`

 * *Files 0% similar despite different names*

```diff
@@ -774,15 +774,22 @@
             {
                 'start': latency_range_min + bucket_index * bucket_width,
                 'end': latency_range_min + (bucket_index + 1) * bucket_width,
                 'packets': packet_count,
             } for bucket_index, packet_count in
             enumerate(self._data.packet_count_buckets)
         )
-        histogram = DataFrame(data=histogram_data)
+        histogram = DataFrame(
+            columns=[
+                'start',
+                'end',
+                'packets',
+            ],
+            data=histogram_data,
+        )
 
         return histogram
 
 
 class MosAnalyser(DataAnalyser):
 
     __slots__ = (
```

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_analysis/data_analysis/tcp.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_analysis/data_analysis/tcp.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_analysis/data_gathering/_filter.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_analysis/data_gathering/_filter.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_analysis/data_gathering/_rx_trigger_controller.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_analysis/data_gathering/_rx_trigger_controller.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_analysis/data_gathering/data_gatherer.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_analysis/data_gathering/data_gatherer.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_analysis/data_gathering/stream.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_analysis/data_gathering/stream.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_analysis/data_gathering/tcp.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_analysis/data_gathering/tcp.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_analysis/data_gathering/trigger.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_analysis/data_gathering/trigger.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_analysis/flow_analyser.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_analysis/flow_analyser.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_analysis/framelossanalyser.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_analysis/framelossanalyser.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_analysis/helpers.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_analysis/helpers.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_analysis/httpanalyser.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_analysis/httpanalyser.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_analysis/latencyaggregator.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_analysis/latencyaggregator.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_analysis/latencyanalyser.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_analysis/latencyanalyser.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_analysis/plotting/generic_chart.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_analysis/plotting/generic_chart.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_analysis/render/frameblasting.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_analysis/render/frameblasting.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_analysis/render/renderer.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_analysis/render/renderer.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_analysis/render/tcp.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_analysis/render/tcp.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_analysis/storage/frame_count.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_analysis/storage/frame_count.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_analysis/storage/stream.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_analysis/storage/stream.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_analysis/storage/tcp.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_analysis/storage/tcp.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_analysis/storage/trigger.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_analysis/storage/trigger.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_analysis/voiceanalyser.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_analysis/voiceanalyser.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_cli/_arguments.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_cli/_arguments.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_cli/_config_file.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_cli/_config_file.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_cli/_endpoint_factory.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_cli/_endpoint_factory.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_cli/_flow_factory.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_cli/_flow_factory.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_cli/_port_factory.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_cli/_port_factory.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_cli/_with_json_configfile.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_cli/_with_json_configfile.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_endpoint/endpoint.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_endpoint/endpoint.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_endpoint/ipv4/endpoint.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_endpoint/ipv4/endpoint.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_endpoint/ipv4/nat.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_endpoint/ipv4/nat.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_endpoint/ipv4/port.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_endpoint/ipv4/port.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_endpoint/ipv6/endpoint.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_endpoint/ipv6/endpoint.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_endpoint/ipv6/port.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_endpoint/ipv6/port.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_endpoint/nat_discovery.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_endpoint/nat_discovery.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from scapy.layers.inet import IP, UDP, Ether
 from scapy.layers.inet6 import IPv6
 from scapy.packet import Raw
 
 from ..constants import UDP_DYNAMIC_PORT_START
 from ..exceptions import NatDiscoveryFailed
 from .endpoint import Endpoint
+from .helpers import build_layer2_5_headers
 from .port import Port
 
 _CACHE_KEY_FORMAT = '{}/{}'
 
 
 # See also:
 #
@@ -164,19 +165,25 @@
             )
 
             # Build frame content
             # NOTE: Done in
             # byteblower_test_framework.logging.configure_logging():
             # logging.getLogger("scapy.runtime").setLevel(logging.ERROR)
 
+            scapy_layer2_5_headers = build_layer2_5_headers(
+                self._local_port
+            )
+
             payload = 'a' * (200)
             scapy_udp_payload = Raw(payload.encode('ascii', 'strict'))
             scapy_udp_header = UDP(dport=remote_udp_port, sport=local_udp_port)
             scapy_ip_header = IP(src=local_ip_address, dst=remote_ip_address)
             scapy_ethernet_header = Ether(src=self._local_port.mac, dst=mac)
+            for scapy_layer2_5_header in scapy_layer2_5_headers:
+                scapy_ethernet_header /= scapy_layer2_5_header
             scapy_frame = (
                 scapy_ethernet_header / scapy_ip_header / scapy_udp_header /
                 scapy_udp_payload
             )
             logging.debug(
                 'NaptResolver for %r: Transmit Content: %s',
                 self._local_port.name, scapy_frame.summary()
```

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_endpoint/nat_endpoint.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_endpoint/nat_endpoint.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_endpoint/port.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_endpoint/port.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_factory/frame.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_factory/frame.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_helpers/capabilities.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_helpers/capabilities.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_helpers/syncexec.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_helpers/syncexec.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_helpers/taggable.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_helpers/taggable.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_host/meetingpoint.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_host/meetingpoint.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_host/server.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_host/server.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_report/byteblowerhtmlreport.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_report/byteblowerhtmlreport.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_report/byteblowerjsonreport.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_report/byteblowerjsonreport.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_report/byteblowerreport.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_report/byteblowerreport.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_report/byteblowerunittestreport.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_report/byteblowerunittestreport.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_report/options.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_report/options.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_report/templates/embedded-fonts.css` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_report/templates/embedded-fonts.css`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_report/templates/flow_section.html` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_report/templates/flow_section.html`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_report/templates/report_footer.html` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_report/templates/report_footer.html`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_report/templates/report_header.html` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_report/templates/report_header.html`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_report/templates/report_pass_fail.html` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_report/templates/report_pass_fail.html`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_report/templates/testframework.css` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_report/templates/testframework.css`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_report/unittestreport.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_report/unittestreport.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_scenario.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_scenario.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_traffic/_http_client_controller.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_traffic/_http_client_controller.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_traffic/_tx_stream_controller.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_traffic/_tx_stream_controller.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_traffic/constants.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_traffic/constants.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_traffic/flow.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_traffic/flow.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_traffic/frame.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_traffic/mobile_frame.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,82 +1,89 @@
-"""Frame interface module."""
+"""Mobile frame module."""
 import logging
-from abc import ABC, abstractmethod
-from typing import (  # for type hinting
-    TYPE_CHECKING,
-    Iterator,
-    Optional,
-    Sequence,
-    Union,
-)
+from abc import ABC
+from typing import TYPE_CHECKING, Optional, Union  # for type hinting
 
-from byteblowerll.byteblower import Frame as TxFrame  # for type hinting
+from byteblowerll.byteblower import FrameMobile as TxFrame
 from byteblowerll.byteblower import FrameTagTx  # for type hinting
-from byteblowerll.byteblower import VLANTag  # for type hinting
-from byteblowerll.byteblower import Stream as TxStream  # for type hinting
-# XXX - Avoid circular import with scapy 2.4.5 on macOS Monterey:
-# Similar to https://github.com/secdev/scapy/issues/3246
-# from scapy.layers.l2 import Ether  # for type hinting
-# from scapy.layers.l2 import Dot1AD, Dot1Q
-from scapy.all import \
-    Ether  # for type hinting; pylint: disable=no-name-in-module
-from scapy.all import Dot1AD, Dot1Q  # pylint: disable=no-name-in-module
+from byteblowerll.byteblower import StreamMobile as TxStream
 
+from .._endpoint.endpoint import Endpoint
+from .._endpoint.ipv4.endpoint import IPv4Endpoint
+from .._endpoint.ipv6.endpoint import IPv6Endpoint
+from .._endpoint.port import Port
 from ..constants import DEFAULT_FRAME_LENGTH, UDP_DYNAMIC_PORT_START
-from ..exceptions import ByteBlowerTestFrameworkException, InvalidInput
-from .constants import VLAN_HEADER_LENGTH  # for sanity check
-from .constants import VLAN_C_TAG, VLAN_S_TAG
+from ..exceptions import FeatureNotSupported
+from .constants import IPV4_FULL_HEADER_LENGTH, IPV6_FULL_HEADER_LENGTH
+from .helpers import get_ip_traffic_class
 
 if TYPE_CHECKING:
-    # NOTE: Import does not work at runtime: cyclic import dependencies
-    # See also: https://mypy.readthedocs.io/en/stable/runtime_troubles.html#import-cycles, pylint: disable=line-too-long
-    from .._endpoint.endpoint import Endpoint  # for type hinting
-    from .._endpoint.port import Port, VlanFlatConfig  # for type hinting
+    # NOTE: Import because referenced in docstrings:
+    from ..constants import DEFAULT_IP_DSCP, DEFAULT_IP_ECN
+    from ..exceptions import ConflictingInput, InvalidInput
 
-assert VLAN_HEADER_LENGTH == len(Dot1Q()), "Unexpected VLAN header length"
 
+class MobileFrame(ABC):
+    """Mobile Frame Interface.
 
-class Frame(ABC):
-    """Frame interface."""
+    .. versionadded:: 1.2.0
+       Added for ByteBlower Endpoint support.
+    """
 
-    __slots__ = (
+    _slots__ = (
         '_length',
         '_udp_src',
         '_udp_dest',
+        '_ip_traffic_class',
         '_latency_tag',
         '_frame',
     )
 
     def __init__(
         self,
-        _minimum_length: int,
         length: Optional[int] = None,
         udp_src: Optional[int] = None,
         udp_dest: Optional[int] = None,
+        ip_dscp: Optional[int] = None,
+        ip_ecn: Optional[int] = None,
+        ip_traffic_class: Optional[int] = None,
         latency_tag: bool = False
     ) -> None:
-        """Create the base frame.
+        """Create the mobile frame for the wireless endpoint.
 
-        :param _minimum_length: Required minimum length of the frame,
-           used for sanity check
-        :type _minimum_length: int
-        :param length: Frame length. This is the layer 2 (Ethernet) frame length
-           *excluding* Ethernet FCS and *excluding* VLAN tags,
+        :param length: Frame length. This is the layer 2 (Ethernet)
+           frame length *excluding* Ethernet FCS and *excluding* VLAN tags,
            defaults to :const:`DEFAULT_FRAME_LENGTH`
-        :type length: Optional[int], optional
+        :type length: int, optional
         :param udp_src: UDP source port, defaults to
            :const:`UDP_DYNAMIC_PORT_START`
-        :type udp_src: Optional[int], optional
+        :type udp_src: int, optional
         :param udp_dest: UDP destination port, defaults to
            :const:`UDP_DYNAMIC_PORT_START`
-        :type udp_dest: Optional[int], optional
+        :type udp_dest: int, optional
+        :param ip_dscp: IP Differentiated Services Code Point (DSCP),
+            mutual exclusive with ``ip_traffic_class``,
+            defaults to :const:`DEFAULT_IP_DSCP`
+        :type ip_dscp: Optional[int], optional
+        :param ip_ecn: IP Explicit Congestion Notification (ECN),
+            mutual exclusive with ``ip_traffic_class``,
+            defaults to :const:`DEFAULT_IP_ECN`
+        :type ip_ecn: Optional[int], optional
+        :param ip_traffic_class: The IP traffic class value is used to
+           specify the exact value of either the *IPv4 ToS field* or the
+           *IPv6 Traffic Class field*,
+           mutual exclusive with ``ip_dscp`` and ``ip_ecn``,
+           defaults to field value composed from ``ip_dscp`` and ``ip_ecn``.
+        :type ip_traffic_class: Optional[int], optional
         :param latency_tag: Enable latency tag generation in the Frame,
            defaults to ``False``
         :type latency_tag: bool, optional
         :raises InvalidInput: When invalid configuration values are given.
+        :raises ConflictingInput: When invalid combination of configuration
+           parameters is given
         """
         if length is None:
             length = DEFAULT_FRAME_LENGTH
 
         if udp_src is None:
             udp_src = UDP_DYNAMIC_PORT_START
 
@@ -85,151 +92,87 @@
 
         self._length = length
         self._udp_src = udp_src
         self._udp_dest = udp_dest
         self._latency_tag = latency_tag
         self._frame: TxFrame = None
 
-        # Sanity checks
-        if self._length < _minimum_length:
-            raise InvalidInput(
-                'Frame length too small.'
-                f' Must be at least {_minimum_length}B.'
-            )
-
-    @staticmethod
-    def _vlan_config(
-        source_port: 'Port'
-    ) -> Iterator[Sequence['VlanFlatConfig']]:
-        """Return list of VLAN (stack) configuration (generator).
-
-        Similar to :meth:`Port.vlan_config`, but raises an exception
-        when we have Layer 2.5 configurations other than :class:`VLANTag`
-        or we have unsupported VLAN configurations.
-
-        :param source_port: Port to get the VLAN configuration from
-        :type source_port: Port
-        :raises ByteBlowerTestFrameworkException: In case of Layer 2.5
-           other than VLAN
-        :return:
-           Ordered collection (Outer -> Inner) of VLAN configuration tuples
-        :yield: VLAN configuration for current layer 2.5
-        :rtype: Iterator[Sequence[VlanFlatConfig]]
-        """
-        layer2_5 = source_port.layer2_5
-        for l2_5 in layer2_5:
-            if not isinstance(l2_5, VLANTag):
-                raise ByteBlowerTestFrameworkException(
-                    f'Unsupported Layer 2.5 configuration: {type(l2_5)!r}'
-                )
-            yield (
-                l2_5.ProtocolIDGet(), l2_5.IDGet(), l2_5.DropEligibleGet(),
-                l2_5.PriorityGet()
-            )
-
-    def _build_layer2_5_headers(
-        self, source_port: 'Port'
-    ) -> Sequence[Union[Dot1Q, Dot1AD]]:
-        return [
-            Frame._build_layer2_5_header(*vlan_config)
-            for vlan_config in Frame._vlan_config(source_port)
-        ]
-
-    @staticmethod
-    def _build_layer2_5_header(
-        vlan_tpid: int, vlan_id: int, vlan_dei: bool, vlan_pcp: int
-    ) -> Union[Dot1Q, Dot1AD]:
-        """Build a layer 2.5 header for the given VLAN configuration.
-
-        :param vlan_tpid: VLAN Protocol ID (TPID)
-        :type vlan_tpid: int
-        :param vlan_id: VLAN ID (VID)
-        :type vlan_id: int
-        :param vlan_dei: Drop Eligible flag (DEI)
-        :type vlan_dei: bool
-        :param vlan_pcp: Priority Code Point (PCP)
-        :type vlan_pcp: int
-        :raises InvalidInput: When VLAN is configured with an unsupported TPID
-        :return: scapy header for Layer2.5
-        :rtype: Union[Dot1Q, Dot1AD]
-        """
-        if vlan_tpid == VLAN_S_TAG:
-            return Dot1AD(prio=vlan_pcp, id=vlan_dei, vlan=vlan_id)
-        if vlan_tpid == VLAN_C_TAG:
-            return Dot1Q(prio=vlan_pcp, id=vlan_dei, vlan=vlan_id)
-        raise InvalidInput(
-            f'VLAN TPID {vlan_tpid} is not supported.'
-            f' Please use S-Tag {VLAN_S_TAG} or C-tag {VLAN_C_TAG}'
+        self._ip_traffic_class = get_ip_traffic_class(
+            "IP Traffic Class",
+            ip_traffic_class=ip_traffic_class,
+            ip_dscp=ip_dscp,
+            ip_ecn=ip_ecn,
         )
 
-    def _build_payload(self, header_length: int) -> str:
-        return 'a' * (self._length - header_length)
-
-    @abstractmethod
     def build_frame_content(
-        self, source_port: Union['Port', 'Endpoint'],
-        destination_port: ['Port', 'Endpoint']
-    ) -> Ether:
-        """Obtain needed information to build the frame.
+        self, source_port: Port, destination_port: Union[Port, Endpoint]
+    ):
+        """Obtain needed information to build the mobile frame.
 
         .. warning::
            Internal use only. Use with care.
 
-        .. versionadded:: 1.2.0
-           Added for ByteBlower Endpoint support.
-
         :meta private:
         """
+        if isinstance(source_port, IPv4Endpoint):
+            payload = self._build_payload(IPV4_FULL_HEADER_LENGTH)
+        elif isinstance(source_port, IPv6Endpoint):
+            payload = self._build_payload(IPV6_FULL_HEADER_LENGTH)
+        else:
+            raise FeatureNotSupported(
+                'Unsupported source endpoint'
+                f' type: {type(source_port).__name__!r}'
+            )
 
-    def add(self, frame_content: Ether, stream: TxStream) -> None:
-        """Add created frame to the stream.
+        return payload, destination_port.ip.compressed
+
+    def _build_payload(self, header_length: int) -> str:
+        return 'a' * (self._length - header_length)
+
+    def add(self, frame_content: str, stream: TxStream):
+        """Add the created frame to the stream.
 
         .. warning::
            Internal use only. Use with care.
 
-        .. versionadded:: 1.2.0
-           Added for ByteBlower Endpoint support.
-
         :meta private:
         """
+        payload, destination_ip = frame_content
+
+        payload_bytes = payload.encode('ascii', 'strict')
 
-        # Add this frame to the stream
-        frame_content = bytearray(bytes(frame_content))
+        hexbytes = ''.join((format(b, "02x") for b in payload_bytes))
 
-        # The ByteBlower API expects an 'str' as input
-        # for the Frame::BytesSet(), we need to convert the bytearray.
-        hexbytes = ''.join((format(b, '02x') for b in frame_content))
         self._frame: TxFrame = stream.FrameAdd()
-        self._frame.BytesSet(hexbytes)
+        self._frame.PayloadSet(hexbytes)
 
         if self._latency_tag:
             # Enable latency for this frame.
             # The frame frame contents will be altered
             # so it contains a timestamp.
             frame_tag: FrameTagTx = self._frame.FrameTagTimeGet()
             frame_tag.Enable(True)
 
-        # Enable auto checksum, ....
-        self._frame.L3AutoChecksumEnable(True)
-        self._frame.L3AutoLengthEnable(True)
-        self._frame.L4AutoChecksumEnable(True)
-        self._frame.L4AutoLengthEnable(True)
+        stream.DestinationAddressSet(destination_ip)
+        stream.DestinationPortSet(self._udp_dest)
+        stream.SourcePortSet(self._udp_src)
+        stream.TypeOfServiceSet(self._ip_traffic_class)
 
     def release(self, stream: TxStream) -> None:
         """
         Release this frame resources used on the ByteBlower system.
 
         .. note::
            The resources related to the stream itself is not released.
         """
         try:
             bb_frame = self._frame
             del self._frame
         except AttributeError:
-            logging.warning('Frame: Already destroyed?', exc_info=True)
+            logging.warning('MobileFrame: Already destroyed?', exc_info=True)
         else:
             if bb_frame is not None:
                 # NOTE: Not really required when we destroy the stream
                 #       afterwards
                 stream.FrameDestroy(bb_frame)
 
     @property
```

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_traffic/frameblastingflow.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_traffic/frameblastingflow.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_traffic/gamingflow.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_traffic/gamingflow.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_traffic/helpers.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_traffic/helpers.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_traffic/httpflow.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_traffic/httpflow.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_traffic/imix.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_traffic/imix.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_traffic/ipv4/frame.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_traffic/ipv4/frame.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_traffic/ipv6/frame.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_traffic/ipv6/frame.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_traffic/mobile_frame.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_traffic/frame.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,178 +1,167 @@
-"""Mobile frame module."""
+"""Frame interface module."""
 import logging
-from abc import ABC
-from typing import TYPE_CHECKING, Optional, Union  # for type hinting
+from abc import ABC, abstractmethod
+from typing import TYPE_CHECKING, Optional, Sequence, Union  # for type hinting
 
-from byteblowerll.byteblower import FrameMobile as TxFrame
-from byteblowerll.byteblower import FrameTagTx  # for type hinting
-from byteblowerll.byteblower import StreamMobile as TxStream
-
-from .._endpoint.endpoint import Endpoint
-from .._endpoint.ipv4.endpoint import IPv4Endpoint
-from .._endpoint.ipv6.endpoint import IPv6Endpoint
-from .._endpoint.port import Port
+from .._endpoint.helpers import build_layer2_5_headers
 from ..constants import DEFAULT_FRAME_LENGTH, UDP_DYNAMIC_PORT_START
-from ..exceptions import FeatureNotSupported
-from .constants import IPV4_FULL_HEADER_LENGTH, IPV6_FULL_HEADER_LENGTH
-from .helpers import get_ip_traffic_class
+from ..exceptions import InvalidInput
 
 if TYPE_CHECKING:
-    # NOTE: Import because referenced in docstrings:
-    from ..constants import DEFAULT_IP_DSCP, DEFAULT_IP_ECN
-    from ..exceptions import ConflictingInput, InvalidInput
+    # For type hinting and avoiding cyclic imports
 
+    from byteblowerll.byteblower import Frame as TxFrame
+    from byteblowerll.byteblower import FrameTagTx
+    from byteblowerll.byteblower import Stream as TxStream
+    # XXX - Avoid circular import with scapy 2.4.5 on macOS Monterey:
+    # Similar to https://github.com/secdev/scapy/issues/3246
+    # from scapy.layers.l2 import Ether
+    # from scapy.layers.l2 import Dot1AD, Dot1Q
+    from scapy.all import \
+        Ether  # for type hinting; pylint: disable=no-name-in-module
+    from scapy.all import Dot1AD, Dot1Q  # pylint: disable=no-name-in-module
+
+    # NOTE: Import does not work at runtime: cyclic import dependencies
+    # See also: https://mypy.readthedocs.io/en/stable/runtime_troubles.html#import-cycles, pylint: disable=line-too-long
+    from .._endpoint.endpoint import Endpoint
+    from .._endpoint.port import Port
 
-class MobileFrame(ABC):
-    """Mobile Frame Interface.
 
-    .. versionadded:: 1.2.0
-       Added for ByteBlower Endpoint support.
-    """
+class Frame(ABC):
+    """Frame interface."""
 
-    _slots__ = (
+    __slots__ = (
         '_length',
         '_udp_src',
         '_udp_dest',
-        '_ip_traffic_class',
         '_latency_tag',
         '_frame',
     )
 
     def __init__(
         self,
+        _minimum_length: int,
         length: Optional[int] = None,
         udp_src: Optional[int] = None,
         udp_dest: Optional[int] = None,
-        ip_dscp: Optional[int] = None,
-        ip_ecn: Optional[int] = None,
-        ip_traffic_class: Optional[int] = None,
         latency_tag: bool = False
     ) -> None:
-        """Create the mobile frame for the wireless endpoint.
+        """Create the base frame.
 
-        :param length: Frame length. This is the layer 2 (Ethernet)
-           frame length *excluding* Ethernet FCS and *excluding* VLAN tags,
+        :param _minimum_length: Required minimum length of the frame,
+           used for sanity check
+        :type _minimum_length: int
+        :param length: Frame length. This is the layer 2 (Ethernet) frame length
+           *excluding* Ethernet FCS and *excluding* VLAN tags,
            defaults to :const:`DEFAULT_FRAME_LENGTH`
-        :type length: int, optional
+        :type length: Optional[int], optional
         :param udp_src: UDP source port, defaults to
            :const:`UDP_DYNAMIC_PORT_START`
-        :type udp_src: int, optional
+        :type udp_src: Optional[int], optional
         :param udp_dest: UDP destination port, defaults to
            :const:`UDP_DYNAMIC_PORT_START`
-        :type udp_dest: int, optional
-        :param ip_dscp: IP Differentiated Services Code Point (DSCP),
-            mutual exclusive with ``ip_traffic_class``,
-            defaults to :const:`DEFAULT_IP_DSCP`
-        :type ip_dscp: Optional[int], optional
-        :param ip_ecn: IP Explicit Congestion Notification (ECN),
-            mutual exclusive with ``ip_traffic_class``,
-            defaults to :const:`DEFAULT_IP_ECN`
-        :type ip_ecn: Optional[int], optional
-        :param ip_traffic_class: The IP traffic class value is used to
-           specify the exact value of either the *IPv4 ToS field* or the
-           *IPv6 Traffic Class field*,
-           mutual exclusive with ``ip_dscp`` and ``ip_ecn``,
-           defaults to field value composed from ``ip_dscp`` and ``ip_ecn``.
-        :type ip_traffic_class: Optional[int], optional
+        :type udp_dest: Optional[int], optional
         :param latency_tag: Enable latency tag generation in the Frame,
            defaults to ``False``
         :type latency_tag: bool, optional
         :raises InvalidInput: When invalid configuration values are given.
-        :raises ConflictingInput: When invalid combination of configuration
-           parameters is given
         """
         if length is None:
             length = DEFAULT_FRAME_LENGTH
 
         if udp_src is None:
             udp_src = UDP_DYNAMIC_PORT_START
 
         if udp_dest is None:
             udp_dest = UDP_DYNAMIC_PORT_START
 
         self._length = length
         self._udp_src = udp_src
         self._udp_dest = udp_dest
         self._latency_tag = latency_tag
-        self._frame: TxFrame = None
+        self._frame: 'TxFrame' = None
 
-        self._ip_traffic_class = get_ip_traffic_class(
-            "IP Traffic Class",
-            ip_traffic_class=ip_traffic_class,
-            ip_dscp=ip_dscp,
-            ip_ecn=ip_ecn,
-        )
+        # Sanity checks
+        if self._length < _minimum_length:
+            raise InvalidInput(
+                'Frame length too small.'
+                f' Must be at least {_minimum_length}B.'
+            )
+
+    def _build_layer2_5_headers(
+        self, source_port: 'Port'
+    ) -> Sequence[Union['Dot1Q', 'Dot1AD']]:
+        return build_layer2_5_headers(source_port)
 
+    def _build_payload(self, header_length: int) -> str:
+        return 'a' * (self._length - header_length)
+
+    @abstractmethod
     def build_frame_content(
-        self, source_port: Port, destination_port: Union[Port, Endpoint]
-    ):
-        """Obtain needed information to build the mobile frame.
+        self, source_port: Union['Port', 'Endpoint'],
+        destination_port: Union['Port', 'Endpoint']
+    ) -> 'Ether':
+        """Obtain needed information to build the frame.
 
         .. warning::
            Internal use only. Use with care.
 
+        .. versionadded:: 1.2.0
+           Added for ByteBlower Endpoint support.
+
         :meta private:
         """
-        if isinstance(source_port, IPv4Endpoint):
-            payload = self._build_payload(IPV4_FULL_HEADER_LENGTH)
-        elif isinstance(source_port, IPv6Endpoint):
-            payload = self._build_payload(IPV6_FULL_HEADER_LENGTH)
-        else:
-            raise FeatureNotSupported(
-                'Unsupported source endpoint'
-                f' type: {type(source_port).__name__!r}'
-            )
-
-        return payload, destination_port.ip.compressed
 
-    def _build_payload(self, header_length: int) -> str:
-        return 'a' * (self._length - header_length)
-
-    def add(self, frame_content: str, stream: TxStream):
-        """Add the created frame to the stream.
+    def add(self, frame_content: 'Ether', stream: 'TxStream') -> None:
+        """Add created frame to the stream.
 
         .. warning::
            Internal use only. Use with care.
 
+        .. versionadded:: 1.2.0
+           Added for ByteBlower Endpoint support.
+
         :meta private:
         """
-        payload, destination_ip = frame_content
-
-        payload_bytes = payload.encode('ascii', 'strict')
 
-        hexbytes = ''.join((format(b, "02x") for b in payload_bytes))
+        # Add this frame to the stream
+        frame_content = bytearray(bytes(frame_content))
 
-        self._frame: TxFrame = stream.FrameAdd()
-        self._frame.PayloadSet(hexbytes)
+        # The ByteBlower API expects an 'str' as input
+        # for the Frame::BytesSet(), we need to convert the bytearray.
+        hexbytes = ''.join((format(b, '02x') for b in frame_content))
+        self._frame: 'TxFrame' = stream.FrameAdd()
+        self._frame.BytesSet(hexbytes)
 
         if self._latency_tag:
             # Enable latency for this frame.
             # The frame frame contents will be altered
             # so it contains a timestamp.
-            frame_tag: FrameTagTx = self._frame.FrameTagTimeGet()
+            frame_tag: 'FrameTagTx' = self._frame.FrameTagTimeGet()
             frame_tag.Enable(True)
 
-        stream.DestinationAddressSet(destination_ip)
-        stream.DestinationPortSet(self._udp_dest)
-        stream.SourcePortSet(self._udp_src)
-        stream.TypeOfServiceSet(self._ip_traffic_class)
+        # Enable auto checksum, ....
+        self._frame.L3AutoChecksumEnable(True)
+        self._frame.L3AutoLengthEnable(True)
+        self._frame.L4AutoChecksumEnable(True)
+        self._frame.L4AutoLengthEnable(True)
 
-    def release(self, stream: TxStream) -> None:
+    def release(self, stream: 'TxStream') -> None:
         """
         Release this frame resources used on the ByteBlower system.
 
         .. note::
            The resources related to the stream itself is not released.
         """
         try:
             bb_frame = self._frame
             del self._frame
         except AttributeError:
-            logging.warning('MobileFrame: Already destroyed?', exc_info=True)
+            logging.warning('Frame: Already destroyed?', exc_info=True)
         else:
             if bb_frame is not None:
                 # NOTE: Not really required when we destroy the stream
                 #       afterwards
                 stream.FrameDestroy(bb_frame)
 
     @property
```

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_traffic/stream.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_traffic/stream.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_traffic/tcpflow.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_traffic/tcpflow.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_traffic/videoflow.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_traffic/videoflow.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/_traffic/voiceflow.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/_traffic/voiceflow.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/all.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/all.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/analysis.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/analysis.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/cli.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/cli.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/constants.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/constants.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/endpoint.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/endpoint.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/exceptions.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/exceptions.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/report.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/report.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/byteblower_test_framework/traffic.py` & `byteblower_test_framework-1.3.1/byteblower_test_framework/traffic.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/docs/Makefile` & `byteblower_test_framework-1.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/docs/source/_include/_example_test_scenario.rst` & `byteblower_test_framework-1.3.1/docs/source/_include/_example_test_scenario.rst`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/docs/source/changelog.rst` & `byteblower_test_framework-1.3.1/docs/source/changelog.rst`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,30 @@
 .. _Versioning: https://api.byteblower.com/test-framework/latest/byteblower-test-framework/versioning.html
 .. _byteblowerll: https://pypi.org/project/byteblowerll/
 .. _ByteBlower Endpoint: https://www.excentis.com/products/byteblower-endpoint/
 
 **Note**: *Have a look at our* Versioning_ *for more information about
 how releases are handled for the ByteBlower Test Framework*.
 
+v1.3.1
+======
+
+Improvements
+------------
+
+- Support NAT discovery for ports on VLAN tags.
+- Added Excentis icon to HTML report.
+- Better default port configuration for example JSON scenario definitions.
+
+Fixes
+-----
+
+- Fixed exception when no data was received in the latency histogram.
+- Fixed issues in command-line scenario definition JSON schema definition.
+
 v1.3.0
 ======
 
 Improvements
 ------------
 
 - Support for `Low Latency, Low Loss, and Scalable Throughput (L4S)`_ on TCP
```

### Comparing `byteblower_test_framework-1.3.0/docs/source/cli/index.rst` & `byteblower_test_framework-1.3.1/docs/source/cli/index.rst`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/docs/source/conf.py` & `byteblower_test_framework-1.3.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/docs/source/config/index.rst` & `byteblower_test_framework-1.3.1/docs/source/config/index.rst`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/docs/source/examples/basic.rst` & `byteblower_test_framework-1.3.1/docs/source/examples/basic.rst`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/docs/source/examples/index.rst` & `byteblower_test_framework-1.3.1/docs/source/examples/index.rst`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/docs/source/examples/l4s.rst` & `byteblower_test_framework-1.3.1/docs/source/examples/l4s.rst`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/docs/source/extra/byteblower-test-framework/json/cli-config-schema.json` & `byteblower_test_framework-1.3.1/docs/source/extra/byteblower-test-framework/json/cli-config-schema.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9911940402028867%*

 * *Differences: {"'$defs'": "{'flow_list': {'title': 'Flow definition list'}, 'maximum_run_time': {'minimum': 0, "*

 * *            "delete: ['format']}, 'port': {'properties': {'interface': {'pattern': "*

 * *            "'^(nontrunk[-][0-9]+|trunk[-][0-9]+[-][0-9]+)$'}, 'uuid': {'oneOf': "*

 * *            "[OrderedDict([('format', 'uuid')]), OrderedDict([('format', None)])]}, 'vlans': "*

 * *            "{'items': {'$ref': '#/$defs/vlan'}}, 'ipv4': {'oneOf': {0: {'oneOf': "*

 * *            "[OrderedDict([('enum', ['dhcp'])]), OrderedDict([('fo […]*

```diff
@@ -5,15 +5,15 @@
             "properties": {
                 "add_reverse_direction": {
                     "$$description": [
                         "The reverse flow uses the same configuration as the original.",
                         "Defaults to ``false``"
                     ],
                     "description": "Enables adding a flow in the reverse direction of the original flow.",
-                    "type": "string"
+                    "type": "boolean"
                 },
                 "destination": {
                     "additionalProperties": false,
                     "description": "Specifying the destination for receiving data for this flow",
                     "properties": {
                         "port_group": {
                             "description": "List of port groups specifying the receiving ports",
@@ -25,39 +25,44 @@
                     },
                     "type": "object"
                 },
                 "dscp": {
                     "description": "Differentiated Services Code Point. Defaults to :const:`DEFAULT_IP_DSCP` (``0x00``)",
                     "oneOf": [
                         {
-                            "type": "number"
+                            "maximum": 63,
+                            "minimum": 0,
+                            "type": "integer"
                         },
                         {
                             "type": "string"
                         }
                     ],
                     "title": "IP DSCP"
                 },
                 "ecn": {
                     "description": "Explicit Congestion Notification code point. Defaults to :const:`DEFAULT_IP_ECN` (``0x00``)",
                     "oneOf": [
                         {
-                            "type": "number"
+                            "maximum": 3,
+                            "minimum": 0,
+                            "type": "integer"
                         },
                         {
                             "type": "string"
                         }
                     ],
                     "title": "IP ECN"
                 },
                 "initial_time_to_wait": {
                     "$$description": [
                         "Defaults to 0 (start immediately)"
                     ],
                     "description": "Initial time to wait to start the flow in seconds.",
+                    "minimum": 0,
                     "type": "number"
                 },
                 "name": {
                     "description": "Name of this Flow, defaults to auto-generated name when set to ``none``",
                     "type": "string"
                 },
                 "source": {
@@ -72,14 +77,18 @@
                             "type": "array"
                         }
                     },
                     "type": "object"
                 },
                 "type": {
                     "description": "Type of the flow. Defines which specific flow parameters will be possible.",
+                    "enum": [
+                        "frame_blasting",
+                        "http"
+                    ],
                     "type": "string"
                 }
             },
             "title": "Flow definition",
             "type": "object"
         },
         "flow_list": {
@@ -91,15 +100,15 @@
                         "$ref": "#/$defs/frame_blasting_flow"
                     },
                     {
                         "$ref": "#/$defs/http_flow"
                     }
                 ]
             },
-            "title": "Flow definitions",
+            "title": "Flow definition list",
             "type": "array"
         },
         "frame_blasting_flow": {
             "$$target": "#/$defs/frame_blasting_flow",
             "allOf": [
                 {
                     "$ref": "#/$defs/flow"
@@ -119,40 +128,45 @@
                         },
                         "bitrate": {
                             "$$description": [
                                 "Excludes the VLAN tag bytes (*when applicable*), mutual exclusive ",
                                 "with ``frame_rate``, defaults to ``none``"
                             ],
                             "description": "Rate at which the bits are transmitted (in bits per second).",
-                            "type": "string"
+                            "exclusiveMinimum": 0,
+                            "type": "number"
                         },
                         "duration": {
                             "$$description": [
                                 "Defaults to ``none`` (use ``number_of_frames`` instead)"
                             ],
                             "description": "Duration of the flow in seconds.",
-                            "type": "string"
+                            "exclusiveMinimum": 0,
+                            "type": "number"
                         },
                         "frame_rate": {
                             "$$description": [
                                 "Mutual exclusive with ``bitrate``. Defaults to :const:`DEFAULT_FRAME_RATE`",
                                 "(``100``) when ``bitrate`` is not provided."
                             ],
                             "description": "Rate at which the frames are transmitted (in frames per second).",
+                            "exclusiveMinimum": 0,
                             "type": "number"
                         },
                         "frame_size": {
                             "description": "Frame size in Bytes without CRC, defaults to ``none``",
-                            "type": "number"
+                            "minimum": 42,
+                            "type": "integer"
                         },
                         "napt_keep_alive": {
                             "$$description": [
                                 ".. deprecated:: v1.2.0",
                                 "   Use ``nat_keep_alive`` instead. Will be removed in v1.4.0."
                             ],
+                            "deprecated": true,
                             "type": "boolean"
                         },
                         "nat_keep_alive": {
                             "$$description": [
                                 "The direction will be from the endpoint behind a NAT/NAPT",
                                 "gateway to the port at the public side of the NAT/NAPT gateway.",
                                 "Defaults to ``false``.",
@@ -173,29 +187,32 @@
                         },
                         "number_of_frames": {
                             "$$description": [
                                 "Defaults to :const:`DEFAULT_NUMBER_OF_FRAMES`",
                                 "(``none`` == *defined by scenario maximum run time*)."
                             ],
                             "description": "Number of frames to transmit.",
-                            "type": "string"
+                            "exclusiveMinimum": 0,
+                            "type": "integer"
                         }
                     }
                 }
             ],
             "description": "Specific parameters for frame blasting flow. The ``type`` MUST be defined as ``frame_blasting``.",
             "title": "Frame blasting flow",
             "type": "object"
         },
         "frame_loss_analysis": {
             "$$target": "#/$defs/frame_loss_analysis",
             "description": "Specific frame loss analysis related parameters",
             "properties": {
                 "max_loss_percentage": {
                     "description": "Maximum allowed frame/byte loss in %, defaults to :const:`DEFAULT_LOSS_PERCENTAGE` (``1.0``)",
+                    "maximum": 100,
+                    "minimum": 0,
                     "type": "number"
                 }
             },
             "title": "Frame loss analysis parameters",
             "type": "object"
         },
         "http_flow": {
@@ -207,21 +224,22 @@
                 {
                     "properties": {
                         "duration": {
                             "$$description": [
                                 "Mutual exclusive with ``request_size``. Defaults to ``none``"
                             ],
                             "description": "The time it takes for a TCP request to be completed.",
+                            "exclusiveMinimum": 0,
                             "type": "number"
                         },
                         "enable_l4s": {
                             "$$description": [
-                                "Defaults to ``false`` (no L4S analysis, server default TCP Prague,",
-                                "disabled for ByteBlower Port, host operating system default for",
-                                "ByteBlower Endpoint).",
+                                "Defaults to ``false`` (no L4S analysis, default TCP Prague",
+                                "for ByteBlower Server,disabled for ByteBlower Port, host",
+                                "operating system default for ByteBlower Endpoint).",
                                 "",
                                 ".. note::",
                                 "   - L4S support requires at least ByteBlower API v2.22.0,",
                                 "     Server and Meeting Point v2.22.0, and ByteBlower",
                                 "     Endpoint v2.22.0.",
                                 "   - When using Endpoints, L4S must be supported and",
                                 "     enabled in the hosting OS",
@@ -236,105 +254,122 @@
                             "$$description": [
                                 "Mutual exclusive with ``rate_limit``. Defaults to ``none`` (== *no limit*).",
                                 "",
                                 ".. versionadded:: 1.2.0",
                                 "   Added ``maximum_bitrate`` deprecating ``rate_limit``."
                             ],
                             "description": "Limit the data traffic rate (in bits per second).",
+                            "exclusiveMinimum": 0,
                             "type": "number"
                         },
                         "rate_limit": {
                             "$$description": [
                                 "Mutual exclusive with ``maximum_bitrate``. Defaults to ``none`` (== *no limit*).",
                                 "",
                                 ".. deprecated:: 1.2.0",
                                 "   Deprecated ``rate_limit`` in favor of ``maximum_bitrate``.",
                                 "   Will be removed in the next release."
                             ],
+                            "deprecated": true,
                             "description": "Limit the data traffic rate (in Bytes per second).",
+                            "exclusiveMinimum": 0,
                             "type": "number"
                         },
                         "receive_window_scaling": {
                             "$$description": [
                                 "Defaults to ``none``.",
                                 "",
                                 "When ByteBlower Endpoints are involved, this setting will",
                                 "not be applied on them, but only on the HTTP Server on the",
                                 "ByteBlower Port. The ByteBlower Endpoint has no control over",
                                 "the TCP parameters of the host operating system's. It is then",
                                 "up to the Endpoint's host configuration whether this setting",
                                 "will be applicable or not."
                             ],
                             "description": "When given, enable receive window scaling with the given scale factor.",
-                            "type": "number"
+                            "maximum": 12,
+                            "minimum": 0,
+                            "type": "integer"
                         },
                         "request_size": {
                             "$$description": [
                                 "Mutual exclusive with ``duration``. Defaults to ``none``"
                             ],
                             "description": "The size of the TCP request packet in bytes.",
-                            "type": "number"
+                            "exclusiveMinimum": 0,
+                            "type": "integer"
                         },
                         "slow_start_threshold": {
                             "$$description": [
                                 "Defaults to ``none``.",
                                 "",
                                 "When ByteBlower Endpoints are involved, this setting will",
                                 "not be applied on them, but only on the HTTP Server on the",
                                 "ByteBlower Port. The ByteBlower Endpoint has no control over",
                                 "the TCP parameters of the host operating system's. It is then",
                                 "up to the Endpoint's host configuration whether this setting",
                                 "will be applicable or not."
                             ],
                             "description": "TCP Slow start threshold value.",
-                            "type": "number"
+                            "maximum": 2147483647,
+                            "minimum": 0,
+                            "type": "integer"
                         },
                         "tcp_client_port": {
                             "description": "Port number of the TCP client, defaults to ``none``",
-                            "type": "number"
+                            "maximum": 65535,
+                            "minimum": 0,
+                            "type": "integer"
                         },
                         "tcp_server_port": {
                             "description": "Port number of the TCP server, defaults to ``none``",
-                            "type": "number"
+                            "maximum": 65535,
+                            "minimum": 0,
+                            "type": "integer"
                         }
                     }
                 }
             ],
             "description": "Specific parameters for HTTP flow. The ``type`` MUST be defined as ``http``.",
             "title": "HTTP flow parameters",
             "type": "object"
         },
         "latency_loss_analysis": {
             "$$target": "#/$defs/latency_loss_analysis",
             "description": "Specific latency & frame loss analysis related parameters",
             "properties": {
                 "latency": {
-                    "description": "Set to ``true`` to enable latency analysis (latency statistics over time, distribution, CDF,CCDF, ..), defaults to ``false``",
-                    "type": "bool"
+                    "description": "Set to ``true`` to enable latency analysis (latency statistics over time, distribution, CDF, CCDF, ...), defaults to ``false``",
+                    "type": "boolean"
                 },
                 "max_loss_percentage": {
                     "description": "Maximum allowed frame/byte loss in %, defaults to :const:`DEFAULT_LOSS_PERCENTAGE` (``1.0``)",
+                    "maximum": 100,
+                    "minimum": 0,
                     "type": "number"
                 },
                 "max_threshold_latency": {
                     "description": "Maximum allowed latency in milliseconds, defaults to :const:`DEFAULT_MAX_LATENCY_THRESHOLD` (``5.0``)",
+                    "title": "Maximum latency threshold",
                     "type": "number"
                 },
                 "quantile": {
-                    "description": "Quantile for which the latency must be less than the given maximum latency, defaults to:const:`DEFAULT_QUANTILE` (``99.9``)",
+                    "description": "Quantile for which the latency must be less than the given maximum latency, defaults to :const:`DEFAULT_QUANTILE` (``99.9``)",
+                    "maximum": 100,
+                    "minimum": 0,
                     "type": "number"
                 }
             },
             "title": "Latency & frame loss analysis parameters",
             "type": "object"
         },
         "maximum_run_time": {
             "$$target": "#/$defs/maximum_run_time",
             "description": "Maximum run time of the scenario in seconds",
-            "format": "float",
+            "minimum": 0,
             "title": "Maximum run time",
             "type": "number"
         },
         "meeting_point_address": {
             "$$description": [
                 ".. versionadded:: 1.2.0",
                 "   Support for ByteBlower Endpoint."
@@ -364,21 +399,23 @@
                         "Default: *Assigned by DHCP* or *none* for static IPv4 address configuration.",
                         "",
                         ".. note::",
                         "   - Will be supported for IPv6 once manual address configuration is supported.",
                         "   - Not supported by ByteBlower Endpoint."
                     ],
                     "description": "(Default) Gateway of the IPv4 network.",
+                    "format": "ipv4",
                     "type": "string"
                 },
                 "interface": {
                     "$$description": [
                         "*ByteBlower Port only*. Mutually exclusive with ``\"uuid\"``."
                     ],
                     "description": "Name of the physical ByteBlower interface where this ByteBlower port is created.",
+                    "pattern": "^(nontrunk[-][0-9]+|trunk[-][0-9]+[-][0-9]+)$",
                     "type": "string"
                 },
                 "ipv4": {
                     "$$description": [
                         "Supports the following values:",
                         "",
                         "- *IPv4 address* for static IPv4 IP address (*ByteBlower Port only*).",
@@ -392,46 +429,66 @@
                         "",
                         ".. versionchanged:: 1.2.0",
                         "   Support for ByteBlower Endpoint."
                     ],
                     "description": "Enable IPv4 on this traffic endpoint.",
                     "oneOf": [
                         {
+                            "oneOf": [
+                                {
+                                    "enum": [
+                                        "dhcp"
+                                    ]
+                                },
+                                {
+                                    "format": "ipv4"
+                                }
+                            ],
                             "type": "string"
                         },
                         {
-                            "type": "bool"
+                            "type": "boolean"
                         }
                     ],
                     "title": "IPv4 addressing method"
                 },
                 "ipv6": {
                     "$$description": [
                         "Supports the following values:",
                         "",
                         "- ``\"dhcp\"``: to let the port perform DHCPv6 (*ByteBlower Port only*)",
-                        "- ``\"slaac\"``: to let the port perform stateless address auto-configuration (",
-                        "  *ByteBlower Port only*).",
-                        "- ``\"true\"``: To use the IPv6 address(es) of the system (*ByteBlower Endpoint only*).",
+                        "- ``\"slaac\"``: to let the port perform stateless address auto-configuration (*ByteBlower Port only*).",
+                        "- ``true``: To use the IPv6 address(es) of the system (*ByteBlower Endpoint only*).",
                         "",
-                        "  Default: *undefined*.",
+                        "Default: *undefined*.",
                         "",
                         ".. note::",
                         "   For ByteBlower Endpoint, you must specify either ``\"ipv4\": true`` or ``\"ipv6\": true``.",
                         "",
                         ".. versionchanged:: 1.2.0",
                         "   Support for ByteBlower Endpoint."
                     ],
                     "description": "Enable IPv6 on this traffic endpoint.",
                     "oneOf": [
                         {
+                            "oneOf": [
+                                {
+                                    "enum": [
+                                        "dhcp",
+                                        "slaac"
+                                    ]
+                                },
+                                {
+                                    "format": "ipv6"
+                                }
+                            ],
                             "type": "string"
                         },
                         {
-                            "type": "bool"
+                            "type": "boolean"
                         }
                     ],
                     "title": "IPv6 addressing method"
                 },
                 "name": {
                     "$$description": [
                         "(a friendly name to identify this endpoint)."
@@ -443,25 +500,26 @@
                     "$$description": [
                         "Defaults to ``false``.",
                         "",
                         ".. note::",
                         "   Enabled by default for ByteBlower Endpoint."
                     ],
                     "description": "Define whether this port is located behind a NAT gateway.",
-                    "type": "bool"
+                    "type": "boolean"
                 },
                 "netmask": {
                     "$$description": [
                         "Default: *Assigned by DHCP* or ``255.255.255.0`` for static IPv4 address configuration.",
                         "",
                         ".. note::",
                         "   - Will be supported for IPv6 once manual address configuration is supported.",
                         "   - Not supported by ByteBlower Endpoint."
                     ],
                     "description": "Netmask of the IPv4 network.",
+                    "format": "ipv4",
                     "type": "string"
                 },
                 "port_group": {
                     "$$description": [
                         "Used to identify to which flows this port will be part of",
                         "(either as source or destination)."
                     ],
@@ -479,32 +537,41 @@
                         "   Using an Endpoint also requires the ``\"meeting_point\"`` to be provided",
                         "   *and* ``\"ipv4\"`` or ``\"ipv6\"`` set to ``true`` for this port configuration.",
                         "",
                         ".. versionadded:: 1.2.0",
                         "   Support for ByteBlower Endpoint."
                     ],
                     "description": "Device identifier of the ByteBlower Endpoint.",
+                    "oneOf": [
+                        {
+                            "format": "uuid"
+                        },
+                        {
+                            "format": null
+                        }
+                    ],
                     "type": "string"
                 },
                 "vlans": {
                     "$$description": [
                         ".. note::",
                         "   Not supported by ByteBlower Endpoint."
                     ],
                     "description": "List of VLAN (stack) configurations.",
                     "items": {
-                        "$ref": "#/$defs/vlans"
+                        "$ref": "#/$defs/vlan"
                     },
                     "type": "array"
                 }
             },
             "title": "Configuration parameters for a ByteBlower Port or Endpoint",
             "type": "object"
         },
         "port_group": {
+            "$$target": "#/$defs/port_group",
             "description": "Definition of a port group",
             "title": "Port group",
             "type": "string"
         },
         "port_list": {
             "$$target": "#/$defs/port_list",
             "description": "Flat list of ports.",
@@ -549,43 +616,49 @@
                 {
                     "format": "ipv6"
                 }
             ],
             "title": "ByteBlower server address",
             "type": "string"
         },
-        "vlans": {
-            "$$target": "#/$defs/vlans",
+        "vlan": {
+            "$$target": "#/$defs/vlan",
             "properties": {
                 "drop_eligible": {
                     "description": "1-bit flag. Default: 0",
+                    "maximum": 1,
+                    "minimum": 0,
                     "type": "integer"
                 },
                 "id": {
                     "description": "VLAN ID (12-bit; 0-4095)",
+                    "maximum": 4095,
+                    "minimum": 0,
                     "type": "integer"
                 },
                 "priority": {
                     "description": "3 bits defining the VLAN PCP bits. Default: 0",
+                    "maximum": 3,
+                    "minimum": 0,
                     "type": "integer"
                 },
                 "protocol_id": {
                     "$$description": [
                         "Default value is:",
                         "",
                         "- ``\"0x8100\"`` for a single VLAN configuration",
                         "- ``\"0x88a8\"`` for the outer VLAN(s) in a VLAN stack configuration",
                         "- ``\"0x8100\"`` for the most inner VLAN in a VLAN stack configuration.",
                         "",
                         ".. note::",
-                        "   Configuration of the VLAN protocol ID (TPID) requires ByteBlower Server",
-                        "",
-                        "   version >= 2.20.0."
+                        "   Configuration of the VLAN protocol ID (TPID) requires ByteBlower Server version >= 2.20.0."
                     ],
                     "description": "VLAN protocol ID (TPID).",
+                    "maximum": 65535,
+                    "minimum": 0,
                     "type": "integer"
                 }
             },
             "title": "VLAN (stack) configuration",
             "type": "object"
         }
     },
```

### Comparing `byteblower_test_framework-1.3.0/docs/source/extra/byteblower-test-framework/json/endpoint/byteblower_test_framework.json` & `byteblower_test_framework-1.3.1/docs/source/extra/byteblower-test-framework/json/port/byteblower_test_framework.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.65625%*

 * *Differences: {"'$schema'": "'https://api.byteblower.com/test-framework/json/cli-config-schema.json'",*

 * * "'ports'": "{0: {'ipv4': '192.168.1.2', 'netmask': '255.255.255.0', 'gateway': '192.168.1.254'}, "*

 * *            "1: {'ipv4': 'dhcp', 'interface': 'trunk-1-4', 'nat': True, delete: ['uuid']}}",*

 * * "'report'": "{replace: OrderedDict([('html', True), ('json', True), ('junit_xml', False)])}",*

 * * 'delete': "['meeting_point']"}*

```diff
@@ -1,8 +1,9 @@
 {
+    "$schema": "https://api.byteblower.com/test-framework/json/cli-config-schema.json",
     "enable_scouting_flows": true,
     "flows": [
         {
             "analysis": {
                 "latency": true,
                 "max_loss_percentage": 1,
                 "max_threshold_latency": 20
@@ -39,33 +40,35 @@
                     "classic_nsi"
                 ]
             },
             "type": "http"
         }
     ],
     "maximum_run_time": 30.0,
-    "meeting_point": "byteblower-meeting-point.example.com.",
     "ports": [
         {
+            "gateway": "192.168.1.254",
             "interface": "trunk-1-3",
-            "ipv4": "dhcp",
+            "ipv4": "192.168.1.2",
             "name": "NSI",
+            "netmask": "255.255.255.0",
             "port_group": [
                 "classic_nsi"
             ]
         },
         {
-            "ipv4": true,
+            "interface": "trunk-1-4",
+            "ipv4": "dhcp",
             "name": "CPE",
+            "nat": true,
             "port_group": [
                 "classic_cpe"
-            ],
-            "uuid": "4d9a5fdb-32b4-4523-ace9-5972518de13b"
+            ]
         }
     ],
     "report": {
-        "html_report": true,
-        "json_report": true,
-        "junit_xml_report": false
+        "html": true,
+        "json": true,
+        "junit_xml": false
     },
     "server": "byteblower-server.example.com."
 }
```

### Comparing `byteblower_test_framework-1.3.0/docs/source/extra/byteblower-test-framework/json/l4s/endpoint/byteblower_test_framework.json` & `byteblower_test_framework-1.3.1/docs/source/extra/byteblower-test-framework/json/l4s/port/byteblower_test_framework.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8449404761904762%*

 * *Differences: {"'$schema'": "'https://api.byteblower.com/test-framework/json/cli-config-schema.json'",*

 * * "'ports'": "{0: {'interface': 'trunk-1-3', 'ipv4': 'dhcp', delete: ['netmask']}, 1: {'interface': "*

 * *            "'trunk-1-3', 'ipv4': 'dhcp', delete: ['netmask']}, 2: {'ipv4': '192.168.1.2', "*

 * *            "'interface': 'trunk-1-4', 'netmask': '255.255.255.0', 'gateway': '192.168.1.254', "*

 * *            "delete: ['uuid']}}"}*

```diff
@@ -1,8 +1,9 @@
 {
+    "$schema": "https://api.byteblower.com/test-framework/json/cli-config-schema.json",
     "enable_scouting_flows": true,
     "flows": [
         {
             "destination": {
                 "port_group": [
                     "classic_cpe"
                 ]
@@ -54,39 +55,39 @@
             "type": "frame_blasting"
         }
     ],
     "maximum_run_time": 60.0,
     "meeting_point": "byteblower-meeting-point.example.com.",
     "ports": [
         {
-            "interface": "trunk-1-8",
-            "ipv4": "192.168.1.1",
+            "interface": "trunk-1-3",
+            "ipv4": "dhcp",
             "name": "classic NSI",
-            "netmask": "255.255.255.0",
             "port_group": [
                 "classic_nsi"
             ]
         },
         {
-            "interface": "trunk-1-8",
-            "ipv4": "192.168.1.2",
+            "interface": "trunk-1-3",
+            "ipv4": "dhcp",
             "name": "L4S NSI",
-            "netmask": "255.255.255.0",
             "port_group": [
                 "l4s_nsi"
             ]
         },
         {
-            "ipv4": true,
+            "gateway": "192.168.1.254",
+            "interface": "trunk-1-4",
+            "ipv4": "192.168.1.2",
             "name": "CPE",
+            "netmask": "255.255.255.0",
             "port_group": [
                 "classic_cpe",
                 "l4s_cpe"
-            ],
-            "uuid": "4d9a5fdb-32b4-4523-ace9-5972518de13b"
+            ]
         }
     ],
     "report": {
         "html": true,
         "json": true,
         "junit_xml": false
     },
```

### Comparing `byteblower_test_framework-1.3.0/docs/source/extra/byteblower-test-framework/json/l4s/port/byteblower_test_framework.json` & `byteblower_test_framework-1.3.1/docs/source/extra/byteblower-test-framework/json/l4s/endpoint/byteblower_test_framework.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8449404761904762%*

 * *Differences: {"'$schema'": "'https://api.byteblower.com/test-framework/json/cli-config-schema.json'",*

 * * "'ports'": "{0: {'interface': 'trunk-1-8', 'ipv4': '192.168.1.1', 'netmask': '255.255.255.0'}, 1: "*

 * *            "{'interface': 'trunk-1-8', 'ipv4': '192.168.1.2', 'netmask': '255.255.255.0'}, 2: "*

 * *            "{'ipv4': True, 'uuid': '4d9a5fdb-32b4-4523-ace9-5972518de13b', delete: ['interface', "*

 * *            "'netmask', 'gateway']}}"}*

```diff
@@ -1,8 +1,9 @@
 {
+    "$schema": "https://api.byteblower.com/test-framework/json/cli-config-schema.json",
     "enable_scouting_flows": true,
     "flows": [
         {
             "destination": {
                 "port_group": [
                     "classic_cpe"
                 ]
@@ -54,39 +55,39 @@
             "type": "frame_blasting"
         }
     ],
     "maximum_run_time": 60.0,
     "meeting_point": "byteblower-meeting-point.example.com.",
     "ports": [
         {
-            "interface": "trunk-1-3",
-            "ipv4": "dhcp",
+            "interface": "trunk-1-8",
+            "ipv4": "192.168.1.1",
             "name": "classic NSI",
+            "netmask": "255.255.255.0",
             "port_group": [
                 "classic_nsi"
             ]
         },
         {
-            "interface": "trunk-1-3",
-            "ipv4": "dhcp",
+            "interface": "trunk-1-8",
+            "ipv4": "192.168.1.2",
             "name": "L4S NSI",
+            "netmask": "255.255.255.0",
             "port_group": [
                 "l4s_nsi"
             ]
         },
         {
-            "gateway": "192.168.1.254",
-            "interface": "trunk-1-4",
-            "ipv4": "192.168.1.2",
+            "ipv4": true,
             "name": "CPE",
-            "netmask": "255.255.255.0",
             "port_group": [
                 "classic_cpe",
                 "l4s_cpe"
-            ]
+            ],
+            "uuid": "4d9a5fdb-32b4-4523-ace9-5972518de13b"
         }
     ],
     "report": {
         "html": true,
         "json": true,
         "junit_xml": false
     },
```

### Comparing `byteblower_test_framework-1.3.0/docs/source/extra/byteblower-test-framework/json/port/byteblower_test_framework.json` & `byteblower_test_framework-1.3.1/docs/source/extra/byteblower-test-framework/json/endpoint/byteblower_test_framework.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6674107142857143%*

 * *Differences: {"'$schema'": "'https://api.byteblower.com/test-framework/json/cli-config-schema.json'",*

 * * "'meeting_point'": "'byteblower-meeting-point.example.com.'",*

 * * "'ports'": "{1: {'ipv4': True, 'uuid': '4d9a5fdb-32b4-4523-ace9-5972518de13b', delete: "*

 * *            "['interface', 'netmask', 'gateway']}}",*

 * * "'report'": "{replace: OrderedDict([('html', True), ('json', True), ('junit_xml', False)])}"}*

```diff
@@ -1,8 +1,9 @@
 {
+    "$schema": "https://api.byteblower.com/test-framework/json/cli-config-schema.json",
     "enable_scouting_flows": true,
     "flows": [
         {
             "analysis": {
                 "latency": true,
                 "max_loss_percentage": 1,
                 "max_threshold_latency": 20
@@ -39,34 +40,33 @@
                     "classic_nsi"
                 ]
             },
             "type": "http"
         }
     ],
     "maximum_run_time": 30.0,
+    "meeting_point": "byteblower-meeting-point.example.com.",
     "ports": [
         {
             "interface": "trunk-1-3",
             "ipv4": "dhcp",
             "name": "NSI",
             "port_group": [
                 "classic_nsi"
             ]
         },
         {
-            "gateway": "192.168.1.254",
-            "interface": "trunk-1-4",
-            "ipv4": "192.168.1.2",
+            "ipv4": true,
             "name": "CPE",
-            "netmask": "255.255.255.0",
             "port_group": [
                 "classic_cpe"
-            ]
+            ],
+            "uuid": "4d9a5fdb-32b4-4523-ace9-5972518de13b"
         }
     ],
     "report": {
-        "html_report": true,
-        "json_report": true,
-        "junit_xml_report": false
+        "html": true,
+        "json": true,
+        "junit_xml": false
     },
     "server": "byteblower-server.example.com."
 }
```

### Comparing `byteblower_test_framework-1.3.0/docs/source/images/examples/basic/html_report_config.png` & `byteblower_test_framework-1.3.1/docs/source/images/examples/basic/html_report_config.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/docs/source/images/examples/basic/html_report_correlated.png` & `byteblower_test_framework-1.3.1/docs/source/images/examples/basic/html_report_correlated.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/docs/source/images/examples/basic/html_report_http_analysis.png` & `byteblower_test_framework-1.3.1/docs/source/images/examples/basic/html_report_http_analysis.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/docs/source/images/examples/basic/html_report_http_config.png` & `byteblower_test_framework-1.3.1/docs/source/images/examples/basic/html_report_http_config.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/docs/source/images/examples/basic/html_report_http_graph.png` & `byteblower_test_framework-1.3.1/docs/source/images/examples/basic/html_report_http_graph.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/docs/source/images/examples/basic/html_report_http_reverse_flow.png` & `byteblower_test_framework-1.3.1/docs/source/images/examples/basic/html_report_http_reverse_flow.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/docs/source/images/examples/basic/html_report_status_and_env.png` & `byteblower_test_framework-1.3.1/docs/source/images/examples/basic/html_report_status_and_env.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/docs/source/images/examples/basic/html_report_udp_cdf_graph.png` & `byteblower_test_framework-1.3.1/docs/source/images/examples/basic/html_report_udp_cdf_graph.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/docs/source/images/examples/basic/html_report_udp_cdf_status_and_stats.png` & `byteblower_test_framework-1.3.1/docs/source/images/examples/basic/html_report_udp_cdf_status_and_stats.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/docs/source/images/examples/basic/html_report_udp_config.png` & `byteblower_test_framework-1.3.1/docs/source/images/examples/basic/html_report_udp_config.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/docs/source/images/examples/basic/html_report_udp_loss_analyser.png` & `byteblower_test_framework-1.3.1/docs/source/images/examples/basic/html_report_udp_loss_analyser.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/docs/source/images/examples/basic/html_report_udp_loss_graph.png` & `byteblower_test_framework-1.3.1/docs/source/images/examples/basic/html_report_udp_loss_graph.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/docs/source/images/examples/basic/html_report_udp_loss_stats.png` & `byteblower_test_framework-1.3.1/docs/source/images/examples/basic/html_report_udp_loss_stats.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/docs/source/images/examples/l4s_basic/html_report_config.png` & `byteblower_test_framework-1.3.1/docs/source/images/examples/l4s_basic/html_report_config.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/docs/source/images/examples/l4s_basic/html_report_http_analysis.png` & `byteblower_test_framework-1.3.1/docs/source/images/examples/l4s_basic/html_report_http_analysis.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/docs/source/images/examples/l4s_basic/html_report_http_config.png` & `byteblower_test_framework-1.3.1/docs/source/images/examples/l4s_basic/html_report_http_config.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/docs/source/images/examples/l4s_basic/html_report_http_graph.png` & `byteblower_test_framework-1.3.1/docs/source/images/examples/l4s_basic/html_report_http_graph.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/docs/source/images/examples/l4s_basic/html_report_l4s_http_analysis.png` & `byteblower_test_framework-1.3.1/docs/source/images/examples/l4s_basic/html_report_l4s_http_analysis.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/docs/source/images/examples/l4s_basic/html_report_l4s_http_config.png` & `byteblower_test_framework-1.3.1/docs/source/images/examples/l4s_basic/html_report_l4s_http_config.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/docs/source/images/examples/l4s_basic/html_report_l4s_http_graph.png` & `byteblower_test_framework-1.3.1/docs/source/images/examples/l4s_basic/html_report_l4s_http_graph.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/docs/source/images/examples/l4s_basic/html_report_status_and_env.png` & `byteblower_test_framework-1.3.1/docs/source/images/examples/l4s_basic/html_report_status_and_env.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/docs/source/images/examples/l4s_basic/html_report_udp_config.png` & `byteblower_test_framework-1.3.1/docs/source/images/examples/l4s_basic/html_report_udp_config.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/docs/source/images/examples/l4s_basic/html_report_udp_graph.png` & `byteblower_test_framework-1.3.1/docs/source/images/examples/l4s_basic/html_report_udp_graph.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/docs/source/images/examples/l4s_basic/html_report_udp_stats.png` & `byteblower_test_framework-1.3.1/docs/source/images/examples/l4s_basic/html_report_udp_stats.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/docs/source/images/examples/l4s_basic/html_report_udp_status.png` & `byteblower_test_framework-1.3.1/docs/source/images/examples/l4s_basic/html_report_udp_status.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/docs/source/images/overview/compare_latency_ccdf.png` & `byteblower_test_framework-1.3.1/docs/source/images/overview/compare_latency_ccdf.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/docs/source/images/overview/kpi_analysis.png` & `byteblower_test_framework-1.3.1/docs/source/images/overview/kpi_analysis.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/docs/source/images/overview/kpi_summary.png` & `byteblower_test_framework-1.3.1/docs/source/images/overview/kpi_summary.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/docs/source/images/overview/latency_ccdf.png` & `byteblower_test_framework-1.3.1/docs/source/images/overview/latency_ccdf.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/docs/source/images/overview/latency_cdf.png` & `byteblower_test_framework-1.3.1/docs/source/images/overview/latency_cdf.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/docs/source/images/overview/streaming_video_buffer_summary.png` & `byteblower_test_framework-1.3.1/docs/source/images/overview/streaming_video_buffer_summary.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/docs/source/images/overview/streaming_video_graph_over_time.png` & `byteblower_test_framework-1.3.1/docs/source/images/overview/streaming_video_graph_over_time.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/docs/source/images/overview/tcp_graph_over_time.png` & `byteblower_test_framework-1.3.1/docs/source/images/overview/tcp_graph_over_time.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/docs/source/images/overview/voice_graph_over_time.png` & `byteblower_test_framework-1.3.1/docs/source/images/overview/voice_graph_over_time.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/docs/source/images/overview/voice_summary.png` & `byteblower_test_framework-1.3.1/docs/source/images/overview/voice_summary.png`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/docs/source/index.rst` & `byteblower_test_framework-1.3.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/docs/source/master_index.rst` & `byteblower_test_framework-1.3.1/docs/source/master_index.rst`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/docs/source/overview.rst` & `byteblower_test_framework-1.3.1/docs/source/overview.rst`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/docs/source/quick_start.rst` & `byteblower_test_framework-1.3.1/docs/source/quick_start.rst`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/docs/source/reference/byteblower_test_framework.rst` & `byteblower_test_framework-1.3.1/docs/source/reference/byteblower_test_framework.rst`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/docs/source/todo.rst` & `byteblower_test_framework-1.3.1/docs/source/todo.rst`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/docs/source/versioning.rst` & `byteblower_test_framework-1.3.1/docs/source/versioning.rst`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/pyproject.toml` & `byteblower_test_framework-1.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `byteblower_test_framework-1.3.0/PKG-INFO` & `byteblower_test_framework-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: byteblower-test-framework
-Version: 1.3.0
+Version: 1.3.1
 Summary: Test Framework for the ByteBlower Traffic Generator.
 Keywords: ByteBlower,Test Framework
 Author-email: ByteBlower Development Team <support.byteblower@excentis.com>
 Maintainer-email: Tom Ghyselinck <tom.ghyselinck@excentis.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
```

