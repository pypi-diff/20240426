# Comparing `tmp/alibabacloud_dingtalk-2.0.98.tar.gz` & `tmp/alibabacloud_dingtalk-2.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dingtalk-2.0.98.tar", last modified: Tue Apr 23 09:05:01 2024, max compression
+gzip compressed data, was "dist/alibabacloud_dingtalk-2.0.99.tar", last modified: Fri Apr 26 02:41:59 2024, max compression
```

## Comparing `alibabacloud_dingtalk-2.0.98.tar` & `alibabacloud_dingtalk-2.0.99.tar`

### file list

```diff
@@ -1,429 +1,429 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/
--rw-r--r--   0 root         (0) root         (0)   124935 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3853 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2565 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     2650 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/activity_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/activity_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8552 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/activity_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    15045 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/activity_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/ai_interaction_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/ai_interaction_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21346 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/ai_interaction_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    23757 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/ai_interaction_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/ai_paa_s_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/ai_paa_s_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    38246 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/ai_paa_s_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    50325 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/ai_paa_s_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/algo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/algo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9980 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/algo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    22974 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/algo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/alitrip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/alitrip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58254 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/alitrip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   168107 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/alitrip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/amdp_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/amdp_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12468 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/amdp_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    19568 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/amdp_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/apaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/apaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25166 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/apaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    45004 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/apaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/app_market_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/app_market_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25682 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/app_market_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    26721 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/app_market_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/ats_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/ats_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    95304 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/ats_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   142688 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/ats_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/attendance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/attendance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   204138 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/attendance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   393347 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/attendance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/badge_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/badge_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45240 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/badge_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    60886 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/badge_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/bay_max_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/bay_max_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5222 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/bay_max_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4059 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/bay_max_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/bizfinance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   250270 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/bizfinance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   651992 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/bizfinance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/bizfinance_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/bizfinance_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    71584 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/bizfinance_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   101499 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/bizfinance_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9614 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     9792 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/calendar_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/calendar_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   161860 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/calendar_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   394680 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/calendar_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/carbon_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/carbon_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27976 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/carbon_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    41039 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/carbon_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/card_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/card_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    78198 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/card_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   236838 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/card_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/check_in_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/check_in_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6044 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/check_in_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10276 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/check_in_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/chengfeng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    71632 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/chengfeng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   119949 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/chengfeng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/conference_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/conference_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   143706 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/conference_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   201875 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/conference_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/connector_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/connector_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58616 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/connector_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   122524 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/connector_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/contact_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/contact_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   334068 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/contact_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   418722 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/contact_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/content_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/content_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21270 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/content_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    41482 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/content_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/contract_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/contract_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33392 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/contract_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    44364 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/contract_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/conv_file_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/conv_file_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17934 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/conv_file_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    30172 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/conv_file_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/cool_app_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/cool_app_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19630 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/cool_app_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    25937 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/cool_app_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/cool_ops_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/cool_ops_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8944 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/cool_ops_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    14272 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/cool_ops_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/credit_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/credit_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5652 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/credit_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10226 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/credit_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/crm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/crm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   257462 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/crm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   615355 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/crm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/crm_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/crm_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4810 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/crm_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)     7215 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/crm_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/customer_service_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/customer_service_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32170 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/customer_service_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    45878 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/customer_service_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/datacenter_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/datacenter_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   391978 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/datacenter_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   499475 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/datacenter_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/devicemng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/devicemng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   112278 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/devicemng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   148230 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/devicemng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/ding_phone_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/ding_phone_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13874 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/ding_phone_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    15755 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/ding_phone_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/dingmi_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/dingmi_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56946 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/dingmi_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    54091 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/dingmi_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/diot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/diot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    64765 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/diot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    80337 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/diot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/doc_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/doc_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   259804 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/doc_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   315211 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/doc_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/doc_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/doc_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   213190 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/doc_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   379351 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/doc_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/dpaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/dpaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19496 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/dpaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    25936 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/dpaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/drive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/drive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   140210 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/drive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   190495 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/drive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/edu_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/edu_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   557050 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/edu_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   850115 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/edu_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/esign_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/esign_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    72708 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/esign_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   113146 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/esign_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/esign_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/esign_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    86294 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/esign_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   120009 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/esign_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/event_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/event_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18589 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/event_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    20432 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/event_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/exclusive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/exclusive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   378556 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/exclusive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   527163 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/exclusive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/finance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/finance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   161906 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/finance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   305557 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/finance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/flashmeeting_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17280 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/flashmeeting_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    28173 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/flashmeeting_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/flashmsg_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/flashmsg_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35856 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/flashmsg_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    52698 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/flashmsg_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/gateway_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/gateway_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4825 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/gateway_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4965 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/gateway_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/group_blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10562 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/group_blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     9402 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/group_blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/h3yun_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/h3yun_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    80133 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/h3yun_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   134962 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/h3yun_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/h5package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/h5package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17059 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/h5package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    18223 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/h5package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/hrbrain_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    68862 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/hrbrain_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   119612 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/hrbrain_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/hrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/hrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   136761 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/hrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   208587 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/hrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/im_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/im_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   303006 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/im_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   368637 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/im_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/im_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/im_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24693 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/im_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    33051 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/im_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/impaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/impaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    90230 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/impaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    89450 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/impaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/industry_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/industry_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   671658 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/industry_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   913856 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/industry_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/jzcrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    62348 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/jzcrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   152590 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/jzcrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/link_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/link_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    63194 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/link_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   105975 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/link_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/live_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/live_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    91118 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/live_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   131540 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/live_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/live_activities_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/live_activities_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9852 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/live_activities_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    14026 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/live_activities_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/mail_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/mail_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5150 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/mail_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4229 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/mail_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/manufacturing_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16181 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/manufacturing_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    22736 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/manufacturing_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/micro_app_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/micro_app_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   148979 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/micro_app_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   170469 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/micro_app_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/miniapp_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/miniapp_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    52227 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/miniapp_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    52481 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/miniapp_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/notable_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/notable_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    55948 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/notable_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    61887 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/notable_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/oauth2_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/oauth2_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    34360 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/oauth2_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    42471 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/oauth2_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/occupationauth_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8962 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/occupationauth_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     7167 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/occupationauth_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/okr_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/okr_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    89094 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/okr_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   162124 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/okr_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/org_culture_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/org_culture_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    77488 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/org_culture_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   120360 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/org_culture_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56344 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    57967 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/pedia_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/pedia_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29226 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/pedia_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    68049 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/pedia_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/project_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/project_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   265120 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/project_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   409387 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/project_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/project_integration_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/project_integration_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17983 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/project_integration_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10808 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/project_integration_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/rcs_call_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5368 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/rcs_call_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4409 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/rcs_call_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/report_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/report_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25740 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/report_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    43482 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/report_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/resident_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/resident_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   135300 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/resident_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   169147 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/resident_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/robot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/robot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    94300 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/robot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   103368 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/robot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/rooms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/rooms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    93324 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/rooms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   146182 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/rooms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/search_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/search_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39248 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/search_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    44633 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/search_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/service_group_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/service_group_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   386598 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/service_group_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   538012 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/service_group_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/smart_device_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/smart_device_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31508 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/smart_device_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    25740 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/smart_device_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/sns_storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    44726 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/sns_storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    94517 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/sns_storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   187612 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   346388 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/storage_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/storage_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58076 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/storage_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    94327 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/storage_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/swform_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/swform_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13910 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/swform_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    28049 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/swform_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/todo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/todo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    70520 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/todo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   152094 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/todo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/trade_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/trade_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14284 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/trade_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    15723 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/trade_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/trajectory_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/trajectory_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14192 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/trajectory_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    21167 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/trajectory_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/transcribe_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/transcribe_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13676 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/transcribe_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    17009 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/transcribe_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/trip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/trip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    77172 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/trip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   133813 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/trip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/village_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/village_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    75904 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/village_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   107789 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/village_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/watt_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/watt_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33103 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/watt_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    40753 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/watt_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/wiki_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/wiki_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8278 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/wiki_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    20146 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/wiki_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/wiki_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/wiki_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    66210 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/wiki_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   128063 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/wiki_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/wms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/wms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5370 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/wms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     8155 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/wms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/workbench_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/workbench_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    41320 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/workbench_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    42730 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/workbench_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/workflow_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/workflow_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   198336 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/workflow_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   413640 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/workflow_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/workrecord_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/workrecord_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4774 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/workrecord_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3602 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/workrecord_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/yida_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/yida_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   494302 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/yida_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   751756 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/yida_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/yun_shu_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/yun_shu_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5452 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/yun_shu_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4320 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/yun_shu_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3853 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    14206 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      240 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2685 2024-04-23 09:05:01.000000 alibabacloud_dingtalk-2.0.98/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/
+-rw-r--r--   0 root         (0) root         (0)   126471 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3853 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2565 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     2650 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/activity_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/activity_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8552 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/activity_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    15045 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/activity_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/ai_interaction_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/ai_interaction_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21346 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/ai_interaction_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    23757 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/ai_interaction_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/ai_paa_s_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/ai_paa_s_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    38246 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/ai_paa_s_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    50325 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/ai_paa_s_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/algo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/algo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9980 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/algo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    22974 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/algo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/alitrip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/alitrip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58254 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/alitrip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   168107 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/alitrip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/amdp_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/amdp_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12468 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/amdp_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    19568 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/amdp_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/apaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/apaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25166 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/apaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    45004 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/apaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/app_market_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/app_market_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25682 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/app_market_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    26721 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/app_market_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/ats_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/ats_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    95304 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/ats_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   142688 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/ats_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/attendance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/attendance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   204138 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/attendance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   393347 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/attendance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/badge_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/badge_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    45240 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/badge_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    60886 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/badge_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/bay_max_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/bay_max_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5222 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/bay_max_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4059 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/bay_max_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/bizfinance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   250270 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/bizfinance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   651992 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/bizfinance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/bizfinance_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/bizfinance_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    71584 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/bizfinance_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   101499 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/bizfinance_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9614 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     9792 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/calendar_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/calendar_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   161860 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/calendar_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   394680 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/calendar_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/carbon_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/carbon_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27976 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/carbon_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    41039 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/carbon_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/card_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/card_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    78198 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/card_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   236838 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/card_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/check_in_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/check_in_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6044 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/check_in_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10276 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/check_in_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/chengfeng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    71632 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/chengfeng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   119949 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/chengfeng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/conference_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/conference_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   152748 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/conference_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   221957 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/conference_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/connector_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/connector_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58616 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/connector_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   122524 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/connector_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/contact_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/contact_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   334068 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/contact_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   418722 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/contact_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/content_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/content_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21270 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/content_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    41482 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/content_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/contract_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/contract_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33392 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/contract_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    44364 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/contract_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/conv_file_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/conv_file_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17934 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/conv_file_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    30172 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/conv_file_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/cool_app_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/cool_app_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19630 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/cool_app_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    25937 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/cool_app_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/cool_ops_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/cool_ops_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8944 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/cool_ops_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    14272 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/cool_ops_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/credit_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/credit_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5652 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/credit_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10226 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/credit_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/crm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/crm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   257462 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/crm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   615355 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/crm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/crm_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/crm_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4810 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/crm_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     7215 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/crm_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/customer_service_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/customer_service_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32170 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/customer_service_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    45878 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/customer_service_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/datacenter_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/datacenter_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   391978 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/datacenter_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   499475 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/datacenter_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/devicemng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/devicemng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   112278 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/devicemng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   148230 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/devicemng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/ding_phone_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/ding_phone_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13874 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/ding_phone_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    15755 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/ding_phone_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/dingmi_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/dingmi_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56946 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/dingmi_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    54091 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/dingmi_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/diot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/diot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    64765 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/diot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    80337 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/diot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/doc_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/doc_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   259804 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/doc_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   315211 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/doc_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/doc_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/doc_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   213190 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/doc_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   379351 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/doc_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/dpaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/dpaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19496 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/dpaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    25936 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/dpaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/drive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/drive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   140210 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/drive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   190495 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/drive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/edu_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/edu_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   557050 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/edu_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   850115 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/edu_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/esign_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/esign_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    72708 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/esign_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   113146 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/esign_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/esign_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/esign_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    86294 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/esign_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   120009 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/esign_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/event_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/event_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18589 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/event_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    20432 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/event_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/exclusive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/exclusive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   378556 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/exclusive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   527163 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/exclusive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/finance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/finance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   161906 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/finance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   305557 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/finance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/flashmeeting_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17280 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/flashmeeting_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    28173 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/flashmeeting_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/flashmsg_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/flashmsg_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35856 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/flashmsg_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    52698 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/flashmsg_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/gateway_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/gateway_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4825 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/gateway_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4965 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/gateway_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/group_blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10562 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/group_blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     9402 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/group_blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/h3yun_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/h3yun_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    80133 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/h3yun_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   134962 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/h3yun_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/h5package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/h5package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17059 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/h5package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    18223 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/h5package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/hrbrain_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    68862 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/hrbrain_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   119612 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/hrbrain_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/hrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/hrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   136761 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/hrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   208587 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/hrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/im_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/im_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   303006 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/im_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   368637 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/im_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/im_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/im_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24693 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/im_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    33051 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/im_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/impaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/impaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    90230 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/impaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    89450 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/impaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/industry_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/industry_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   671658 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/industry_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   913856 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/industry_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/jzcrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    62348 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/jzcrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   152590 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/jzcrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/link_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/link_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    63194 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/link_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   105975 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/link_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/live_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/live_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    91118 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/live_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   131540 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/live_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/live_activities_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/live_activities_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9852 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/live_activities_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    14026 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/live_activities_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/mail_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/mail_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5150 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/mail_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4229 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/mail_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/manufacturing_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16181 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/manufacturing_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    22736 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/manufacturing_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/micro_app_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/micro_app_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   148979 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/micro_app_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   170469 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/micro_app_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/miniapp_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/miniapp_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    52227 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/miniapp_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    52481 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/miniapp_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/notable_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/notable_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    59878 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/notable_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    62148 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/notable_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/oauth2_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/oauth2_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    34360 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/oauth2_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    42471 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/oauth2_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/occupationauth_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8962 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/occupationauth_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     7167 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/occupationauth_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/okr_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/okr_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    89094 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/okr_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   162124 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/okr_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/org_culture_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/org_culture_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    77488 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/org_culture_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   120360 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/org_culture_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56344 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    57967 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/pedia_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/pedia_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29226 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/pedia_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    68049 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/pedia_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/project_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/project_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   265120 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/project_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   409387 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/project_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/project_integration_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/project_integration_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17983 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/project_integration_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10808 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/project_integration_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/rcs_call_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5368 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/rcs_call_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4409 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/rcs_call_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/report_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/report_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25740 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/report_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    43482 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/report_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/resident_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/resident_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   135300 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/resident_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   169147 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/resident_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/robot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/robot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    94300 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/robot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   103368 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/robot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/rooms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/rooms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    93324 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/rooms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   146182 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/rooms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/search_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/search_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39248 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/search_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    44633 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/search_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/service_group_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/service_group_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   386598 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/service_group_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   538012 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/service_group_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/smart_device_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/smart_device_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31508 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/smart_device_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    25740 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/smart_device_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/sns_storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    44726 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/sns_storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    94517 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/sns_storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   187612 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   346388 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/storage_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/storage_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58076 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/storage_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    94327 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/storage_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/swform_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/swform_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13910 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/swform_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    28049 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/swform_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/todo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/todo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    70520 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/todo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   152094 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/todo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/trade_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/trade_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14284 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/trade_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    15723 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/trade_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/trajectory_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/trajectory_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14192 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/trajectory_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    21167 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/trajectory_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/transcribe_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/transcribe_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13676 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/transcribe_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    17009 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/transcribe_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/trip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/trip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    77172 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/trip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   133813 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/trip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/village_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/village_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    75904 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/village_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   107789 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/village_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/watt_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/watt_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33103 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/watt_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    40753 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/watt_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/wiki_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/wiki_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8278 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/wiki_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    20146 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/wiki_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/wiki_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/wiki_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    66210 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/wiki_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   128063 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/wiki_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/wms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/wms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5370 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/wms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     8155 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/wms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/workbench_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/workbench_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    41320 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/workbench_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    42730 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/workbench_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/workflow_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/workflow_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   198336 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/workflow_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   413640 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/workflow_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/workrecord_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/workrecord_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4774 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/workrecord_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3602 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/workrecord_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/yida_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/yida_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   494302 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/yida_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   751756 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/yida_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/yun_shu_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/yun_shu_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5452 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/yun_shu_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4320 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/yun_shu_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3853 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    14206 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      240 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2685 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/setup.py
```

### Comparing `alibabacloud_dingtalk-2.0.98/ChangeLog.md` & `alibabacloud_dingtalk-2.0.99/ChangeLog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2024-04-23 Version: 2.0.98
+- Generated python activity_1.0,aiInteraction_1.0,aiPaaS_1.0,algo_1.0,alitest_1.0,alitrip_1.0,amdp_1.0,apaas_1.0,appMarket_1.0,ats_1.0,attendance_1.0,badge_1.0,bayMax_1.0,baymax_2.0,bipaas_1.0,bizfinance_1.0,bizfinance_2.0,blackboard_1.0,calendar_1.0,calendar_2.0,carbon_1.0,card_1.0,checkIn_1.0,chengfeng_1.0,conference_1.0,connector_1.0,contact_1.0,content_1.0,contract_1.0,convFile_1.0,convStorage_1.0,coolApp_1.0,coolOps_1.0,credit_1.0,crm_1.0,crm_2.0,customerService_1.0,datacenter_1.0,delivery_1.0,devicemng_1.0,dingmi_1.0,dingPhone_1.0,dingsport_1.0,diot_1.0,doc_1.0,doc_2.0,dpaas_1.0,drive_1.0,drive_2.0,edu_1.0,esign_1.0,event_1.0,event_2.0,exclusive_1.0,finance_1.0,flashmeeting_1.0,flashmsg_1.0,gateway_1.0,groupBlackboard_1.0,h5package_1.0,hrbrain_1.0,hrm_1.0,im_1.0,im_2.0,impaas_1.0,industry_1.0,integration_1.0,liandanlu_1.0,link_1.0,live_1.0,liveActivities_1.0,mail_1.0,manufacturing_1.0,media_1.0,medical_1.0,microApp_1.0,miniapp_1.0,notable_1.0,oauth2_1.0,occupationauth_1.0,office_1.0,okr_1.0,orgCulture_1.0,ow_1.0,package_1.0,pedia_1.0,project_1.0,projectIntegration_1.0,rcsCall_1.0,report_1.0,resident_1.0,robot_1.0,rooms_1.0,search_1.0,serviceGroup_1.0,setting_1.0,smartDevice_1.0,snsStorage_1.0,storage_1.0,storage_2.0,swform_1.0,theone_1.0,todo_1.0,trade_1.0,trajectory_1.0,transcribe_1.0,trip_1.0,village_1.0,waterMark_1.0,watt_1.0,wiki_1.0,wiki_2.0,wms_1.0,workbench_1.0,workflow_1.0,workrecord_1.0,yida_1.0,yunShu_1.0,esign_1.1,esign_2.0,h3yun_1.0,jzcrm_1.0,soke_1.0 for dingtalk.
+
 2024-04-22 Version: 2.0.97
 - Generated python activity_1.0,aiInteraction_1.0,aiPaaS_1.0,algo_1.0,alitest_1.0,alitrip_1.0,amdp_1.0,apaas_1.0,appMarket_1.0,ats_1.0,attendance_1.0,badge_1.0,bayMax_1.0,baymax_2.0,bipaas_1.0,bizfinance_1.0,bizfinance_2.0,blackboard_1.0,calendar_1.0,calendar_2.0,carbon_1.0,card_1.0,checkIn_1.0,chengfeng_1.0,conference_1.0,connector_1.0,contact_1.0,content_1.0,contract_1.0,convFile_1.0,convStorage_1.0,coolApp_1.0,coolOps_1.0,credit_1.0,crm_1.0,crm_2.0,customerService_1.0,datacenter_1.0,delivery_1.0,devicemng_1.0,dingmi_1.0,dingPhone_1.0,dingsport_1.0,diot_1.0,doc_1.0,doc_2.0,dpaas_1.0,drive_1.0,drive_2.0,edu_1.0,esign_1.0,event_1.0,event_2.0,exclusive_1.0,finance_1.0,flashmeeting_1.0,flashmsg_1.0,gateway_1.0,groupBlackboard_1.0,h5package_1.0,hrbrain_1.0,hrm_1.0,im_1.0,im_2.0,impaas_1.0,industry_1.0,integration_1.0,liandanlu_1.0,link_1.0,live_1.0,liveActivities_1.0,mail_1.0,manufacturing_1.0,media_1.0,medical_1.0,microApp_1.0,miniapp_1.0,notable_1.0,oauth2_1.0,occupationauth_1.0,office_1.0,okr_1.0,orgCulture_1.0,ow_1.0,package_1.0,pedia_1.0,project_1.0,projectIntegration_1.0,rcsCall_1.0,report_1.0,resident_1.0,robot_1.0,rooms_1.0,search_1.0,serviceGroup_1.0,setting_1.0,smartDevice_1.0,snsStorage_1.0,storage_1.0,storage_2.0,swform_1.0,theone_1.0,todo_1.0,trade_1.0,trajectory_1.0,transcribe_1.0,trip_1.0,village_1.0,waterMark_1.0,watt_1.0,wiki_1.0,wiki_2.0,wms_1.0,workbench_1.0,workflow_1.0,workrecord_1.0,yida_1.0,yunShu_1.0,esign_1.1,esign_2.0,h3yun_1.0,jzcrm_1.0,soke_1.0 for dingtalk.
 
 2024-04-18 Version: 2.0.96
 - Generated python activity_1.0,aiInteraction_1.0,aiPaaS_1.0,algo_1.0,alitest_1.0,alitrip_1.0,amdp_1.0,apaas_1.0,appMarket_1.0,ats_1.0,attendance_1.0,badge_1.0,bayMax_1.0,baymax_2.0,bipaas_1.0,bizfinance_1.0,bizfinance_2.0,blackboard_1.0,calendar_1.0,calendar_2.0,carbon_1.0,card_1.0,checkIn_1.0,chengfeng_1.0,conference_1.0,connector_1.0,contact_1.0,content_1.0,contract_1.0,convFile_1.0,convStorage_1.0,coolApp_1.0,coolOps_1.0,credit_1.0,crm_1.0,crm_2.0,customerService_1.0,datacenter_1.0,delivery_1.0,devicemng_1.0,dingmi_1.0,dingPhone_1.0,dingsport_1.0,diot_1.0,doc_1.0,doc_2.0,dpaas_1.0,drive_1.0,drive_2.0,edu_1.0,esign_1.0,event_1.0,event_2.0,exclusive_1.0,finance_1.0,flashmeeting_1.0,flashmsg_1.0,gateway_1.0,groupBlackboard_1.0,h5package_1.0,hrbrain_1.0,hrm_1.0,im_1.0,im_2.0,impaas_1.0,industry_1.0,integration_1.0,liandanlu_1.0,link_1.0,live_1.0,liveActivities_1.0,mail_1.0,manufacturing_1.0,media_1.0,medical_1.0,microApp_1.0,miniapp_1.0,notable_1.0,oauth2_1.0,occupationauth_1.0,office_1.0,okr_1.0,orgCulture_1.0,ow_1.0,package_1.0,pedia_1.0,project_1.0,projectIntegration_1.0,rcsCall_1.0,report_1.0,resident_1.0,robot_1.0,rooms_1.0,search_1.0,serviceGroup_1.0,setting_1.0,smartDevice_1.0,snsStorage_1.0,storage_1.0,storage_2.0,swform_1.0,theone_1.0,todo_1.0,trade_1.0,trajectory_1.0,transcribe_1.0,trip_1.0,village_1.0,waterMark_1.0,watt_1.0,wiki_1.0,wiki_2.0,wms_1.0,workbench_1.0,workflow_1.0,workrecord_1.0,yida_1.0,yunShu_1.0,esign_1.1,esign_2.0,h3yun_1.0,jzcrm_1.0,soke_1.0 for dingtalk.
 
 2024-04-15 Version: 2.0.95
```

### Comparing `alibabacloud_dingtalk-2.0.98/LICENSE` & `alibabacloud_dingtalk-2.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/PKG-INFO` & `alibabacloud_dingtalk-2.0.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dingtalk
-Version: 2.0.98
+Version: 2.0.99
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dingtalk-2.0.98/README-CN.md` & `alibabacloud_dingtalk-2.0.99/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/README.md` & `alibabacloud_dingtalk-2.0.99/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/activity_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/activity_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/activity_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/activity_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/ai_interaction_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/ai_interaction_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/ai_interaction_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/ai_interaction_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/ai_paa_s_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/ai_paa_s_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/ai_paa_s_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/ai_paa_s_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/algo_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/algo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/algo_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/algo_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/alitrip_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/alitrip_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/alitrip_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/alitrip_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/amdp_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/amdp_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/amdp_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/amdp_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/apaas_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/apaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/apaas_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/apaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/app_market_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/app_market_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/app_market_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/app_market_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/ats_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/ats_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/ats_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/ats_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/attendance_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/attendance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/attendance_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/attendance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/badge_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/badge_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/badge_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/badge_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/bay_max_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/bay_max_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/bay_max_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/bay_max_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/bizfinance_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/bizfinance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/bizfinance_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/bizfinance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/bizfinance_2_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/bizfinance_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/bizfinance_2_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/bizfinance_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/blackboard_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/blackboard_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/blackboard_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/blackboard_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/calendar_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/calendar_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/calendar_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/calendar_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/carbon_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/carbon_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/carbon_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/carbon_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/card_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/card_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/card_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/card_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/check_in_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/check_in_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/check_in_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/check_in_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/chengfeng_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/chengfeng_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/chengfeng_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/chengfeng_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/conference_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/conference_1_0/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -299,14 +299,116 @@
         conference_id: str,
         request: dingtalkconference__1__0_models.CohostsRequest,
     ) -> dingtalkconference__1__0_models.CohostsResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalkconference__1__0_models.CohostsHeaders()
         return await self.cohosts_with_options_async(conference_id, request, headers, runtime)
 
+    def create_custom_short_link_with_options(
+        self,
+        request: dingtalkconference__1__0_models.CreateCustomShortLinkRequest,
+        headers: dingtalkconference__1__0_models.CreateCustomShortLinkHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkconference__1__0_models.CreateCustomShortLinkResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.cool_app_code):
+            body['coolAppCode'] = request.cool_app_code
+        if not UtilClient.is_unset(request.creator_union_id):
+            body['creatorUnionId'] = request.creator_union_id
+        if not UtilClient.is_unset(request.extension_app_biz_data):
+            body['extensionAppBizData'] = request.extension_app_biz_data
+        if not UtilClient.is_unset(request.schedule_conference_id):
+            body['scheduleConferenceId'] = request.schedule_conference_id
+        if not UtilClient.is_unset(request.use_extension_app):
+            body['useExtensionApp'] = request.use_extension_app
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='CreateCustomShortLink',
+            version='conference_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/conference/customShortLinks',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkconference__1__0_models.CreateCustomShortLinkResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def create_custom_short_link_with_options_async(
+        self,
+        request: dingtalkconference__1__0_models.CreateCustomShortLinkRequest,
+        headers: dingtalkconference__1__0_models.CreateCustomShortLinkHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkconference__1__0_models.CreateCustomShortLinkResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.cool_app_code):
+            body['coolAppCode'] = request.cool_app_code
+        if not UtilClient.is_unset(request.creator_union_id):
+            body['creatorUnionId'] = request.creator_union_id
+        if not UtilClient.is_unset(request.extension_app_biz_data):
+            body['extensionAppBizData'] = request.extension_app_biz_data
+        if not UtilClient.is_unset(request.schedule_conference_id):
+            body['scheduleConferenceId'] = request.schedule_conference_id
+        if not UtilClient.is_unset(request.use_extension_app):
+            body['useExtensionApp'] = request.use_extension_app
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='CreateCustomShortLink',
+            version='conference_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/conference/customShortLinks',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkconference__1__0_models.CreateCustomShortLinkResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def create_custom_short_link(
+        self,
+        request: dingtalkconference__1__0_models.CreateCustomShortLinkRequest,
+    ) -> dingtalkconference__1__0_models.CreateCustomShortLinkResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkconference__1__0_models.CreateCustomShortLinkHeaders()
+        return self.create_custom_short_link_with_options(request, headers, runtime)
+
+    async def create_custom_short_link_async(
+        self,
+        request: dingtalkconference__1__0_models.CreateCustomShortLinkRequest,
+    ) -> dingtalkconference__1__0_models.CreateCustomShortLinkResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkconference__1__0_models.CreateCustomShortLinkHeaders()
+        return await self.create_custom_short_link_with_options_async(request, headers, runtime)
+
     def create_schedule_conference_with_options(
         self,
         request: dingtalkconference__1__0_models.CreateScheduleConferenceRequest,
         headers: dingtalkconference__1__0_models.CreateScheduleConferenceHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkconference__1__0_models.CreateScheduleConferenceResponse:
         UtilClient.validate_model(request)
@@ -2103,14 +2205,100 @@
         conference_id: str,
         request: dingtalkconference__1__0_models.QueryConferenceMembersRequest,
     ) -> dingtalkconference__1__0_models.QueryConferenceMembersResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalkconference__1__0_models.QueryConferenceMembersHeaders()
         return await self.query_conference_members_with_options_async(conference_id, request, headers, runtime)
 
+    def query_schedule_conf_settings_with_options(
+        self,
+        request: dingtalkconference__1__0_models.QueryScheduleConfSettingsRequest,
+        headers: dingtalkconference__1__0_models.QueryScheduleConfSettingsHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkconference__1__0_models.QueryScheduleConfSettingsResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.schedule_conference_id):
+            query['scheduleConferenceId'] = request.schedule_conference_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='QueryScheduleConfSettings',
+            version='conference_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/conference/scheduleConferences/settings',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkconference__1__0_models.QueryScheduleConfSettingsResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def query_schedule_conf_settings_with_options_async(
+        self,
+        request: dingtalkconference__1__0_models.QueryScheduleConfSettingsRequest,
+        headers: dingtalkconference__1__0_models.QueryScheduleConfSettingsHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkconference__1__0_models.QueryScheduleConfSettingsResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.schedule_conference_id):
+            query['scheduleConferenceId'] = request.schedule_conference_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='QueryScheduleConfSettings',
+            version='conference_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/conference/scheduleConferences/settings',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkconference__1__0_models.QueryScheduleConfSettingsResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def query_schedule_conf_settings(
+        self,
+        request: dingtalkconference__1__0_models.QueryScheduleConfSettingsRequest,
+    ) -> dingtalkconference__1__0_models.QueryScheduleConfSettingsResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkconference__1__0_models.QueryScheduleConfSettingsHeaders()
+        return self.query_schedule_conf_settings_with_options(request, headers, runtime)
+
+    async def query_schedule_conf_settings_async(
+        self,
+        request: dingtalkconference__1__0_models.QueryScheduleConfSettingsRequest,
+    ) -> dingtalkconference__1__0_models.QueryScheduleConfSettingsResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkconference__1__0_models.QueryScheduleConfSettingsHeaders()
+        return await self.query_schedule_conf_settings_with_options_async(request, headers, runtime)
+
     def query_schedule_conference_with_options(
         self,
         schedule_conference_id: str,
         request: dingtalkconference__1__0_models.QueryScheduleConferenceRequest,
         headers: dingtalkconference__1__0_models.QueryScheduleConferenceHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkconference__1__0_models.QueryScheduleConferenceResponse:
```

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/conference_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/conference_1_0/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -689,14 +689,195 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CohostsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class CreateCustomShortLinkHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class CreateCustomShortLinkRequest(TeaModel):
+    def __init__(
+        self,
+        cool_app_code: str = None,
+        creator_union_id: str = None,
+        extension_app_biz_data: str = None,
+        schedule_conference_id: str = None,
+        use_extension_app: bool = None,
+    ):
+        self.cool_app_code = cool_app_code
+        self.creator_union_id = creator_union_id
+        self.extension_app_biz_data = extension_app_biz_data
+        self.schedule_conference_id = schedule_conference_id
+        self.use_extension_app = use_extension_app
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.cool_app_code is not None:
+            result['coolAppCode'] = self.cool_app_code
+        if self.creator_union_id is not None:
+            result['creatorUnionId'] = self.creator_union_id
+        if self.extension_app_biz_data is not None:
+            result['extensionAppBizData'] = self.extension_app_biz_data
+        if self.schedule_conference_id is not None:
+            result['scheduleConferenceId'] = self.schedule_conference_id
+        if self.use_extension_app is not None:
+            result['useExtensionApp'] = self.use_extension_app
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('coolAppCode') is not None:
+            self.cool_app_code = m.get('coolAppCode')
+        if m.get('creatorUnionId') is not None:
+            self.creator_union_id = m.get('creatorUnionId')
+        if m.get('extensionAppBizData') is not None:
+            self.extension_app_biz_data = m.get('extensionAppBizData')
+        if m.get('scheduleConferenceId') is not None:
+            self.schedule_conference_id = m.get('scheduleConferenceId')
+        if m.get('useExtensionApp') is not None:
+            self.use_extension_app = m.get('useExtensionApp')
+        return self
+
+
+class CreateCustomShortLinkResponseBodyResult(TeaModel):
+    def __init__(
+        self,
+        custom_short_link: str = None,
+    ):
+        self.custom_short_link = custom_short_link
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.custom_short_link is not None:
+            result['customShortLink'] = self.custom_short_link
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('customShortLink') is not None:
+            self.custom_short_link = m.get('customShortLink')
+        return self
+
+
+class CreateCustomShortLinkResponseBody(TeaModel):
+    def __init__(
+        self,
+        result: CreateCustomShortLinkResponseBodyResult = None,
+    ):
+        self.result = result
+
+    def validate(self):
+        if self.result:
+            self.result.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.result is not None:
+            result['result'] = self.result.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('result') is not None:
+            temp_model = CreateCustomShortLinkResponseBodyResult()
+            self.result = temp_model.from_map(m['result'])
+        return self
+
+
+class CreateCustomShortLinkResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: CreateCustomShortLinkResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = CreateCustomShortLinkResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class CreateScheduleConferenceHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
@@ -4582,14 +4763,325 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = QueryConferenceMembersResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class QueryScheduleConfSettingsHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class QueryScheduleConfSettingsRequest(TeaModel):
+    def __init__(
+        self,
+        schedule_conference_id: str = None,
+    ):
+        self.schedule_conference_id = schedule_conference_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.schedule_conference_id is not None:
+            result['scheduleConferenceId'] = self.schedule_conference_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('scheduleConferenceId') is not None:
+            self.schedule_conference_id = m.get('scheduleConferenceId')
+        return self
+
+
+class QueryScheduleConfSettingsResponseBodyScheduleConfSettingModelMoziConfVirtualExtraSettingMoziConfExtensionAppSettings(TeaModel):
+    def __init__(
+        self,
+        auto_open_mode: str = None,
+        client_id: str = None,
+        cool_app_code: str = None,
+        extension_app_biz_data: str = None,
+    ):
+        self.auto_open_mode = auto_open_mode
+        self.client_id = client_id
+        self.cool_app_code = cool_app_code
+        self.extension_app_biz_data = extension_app_biz_data
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auto_open_mode is not None:
+            result['autoOpenMode'] = self.auto_open_mode
+        if self.client_id is not None:
+            result['clientId'] = self.client_id
+        if self.cool_app_code is not None:
+            result['coolAppCode'] = self.cool_app_code
+        if self.extension_app_biz_data is not None:
+            result['extensionAppBizData'] = self.extension_app_biz_data
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('autoOpenMode') is not None:
+            self.auto_open_mode = m.get('autoOpenMode')
+        if m.get('clientId') is not None:
+            self.client_id = m.get('clientId')
+        if m.get('coolAppCode') is not None:
+            self.cool_app_code = m.get('coolAppCode')
+        if m.get('extensionAppBizData') is not None:
+            self.extension_app_biz_data = m.get('extensionAppBizData')
+        return self
+
+
+class QueryScheduleConfSettingsResponseBodyScheduleConfSettingModelMoziConfVirtualExtraSetting(TeaModel):
+    def __init__(
+        self,
+        enable_chat: int = None,
+        enable_web_anonymous_join: bool = None,
+        join_before_host: int = None,
+        lock_media_status_mic_mute: int = None,
+        lock_nick: int = None,
+        mozi_conf_extension_app_settings: List[QueryScheduleConfSettingsResponseBodyScheduleConfSettingModelMoziConfVirtualExtraSettingMoziConfExtensionAppSettings] = None,
+        waiting_room: int = None,
+    ):
+        self.enable_chat = enable_chat
+        self.enable_web_anonymous_join = enable_web_anonymous_join
+        self.join_before_host = join_before_host
+        self.lock_media_status_mic_mute = lock_media_status_mic_mute
+        self.lock_nick = lock_nick
+        self.mozi_conf_extension_app_settings = mozi_conf_extension_app_settings
+        self.waiting_room = waiting_room
+
+    def validate(self):
+        if self.mozi_conf_extension_app_settings:
+            for k in self.mozi_conf_extension_app_settings:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.enable_chat is not None:
+            result['enableChat'] = self.enable_chat
+        if self.enable_web_anonymous_join is not None:
+            result['enableWebAnonymousJoin'] = self.enable_web_anonymous_join
+        if self.join_before_host is not None:
+            result['joinBeforeHost'] = self.join_before_host
+        if self.lock_media_status_mic_mute is not None:
+            result['lockMediaStatusMicMute'] = self.lock_media_status_mic_mute
+        if self.lock_nick is not None:
+            result['lockNick'] = self.lock_nick
+        result['moziConfExtensionAppSettings'] = []
+        if self.mozi_conf_extension_app_settings is not None:
+            for k in self.mozi_conf_extension_app_settings:
+                result['moziConfExtensionAppSettings'].append(k.to_map() if k else None)
+        if self.waiting_room is not None:
+            result['waitingRoom'] = self.waiting_room
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('enableChat') is not None:
+            self.enable_chat = m.get('enableChat')
+        if m.get('enableWebAnonymousJoin') is not None:
+            self.enable_web_anonymous_join = m.get('enableWebAnonymousJoin')
+        if m.get('joinBeforeHost') is not None:
+            self.join_before_host = m.get('joinBeforeHost')
+        if m.get('lockMediaStatusMicMute') is not None:
+            self.lock_media_status_mic_mute = m.get('lockMediaStatusMicMute')
+        if m.get('lockNick') is not None:
+            self.lock_nick = m.get('lockNick')
+        self.mozi_conf_extension_app_settings = []
+        if m.get('moziConfExtensionAppSettings') is not None:
+            for k in m.get('moziConfExtensionAppSettings'):
+                temp_model = QueryScheduleConfSettingsResponseBodyScheduleConfSettingModelMoziConfVirtualExtraSettingMoziConfExtensionAppSettings()
+                self.mozi_conf_extension_app_settings.append(temp_model.from_map(k))
+        if m.get('waitingRoom') is not None:
+            self.waiting_room = m.get('waitingRoom')
+        return self
+
+
+class QueryScheduleConfSettingsResponseBodyScheduleConfSettingModel(TeaModel):
+    def __init__(
+        self,
+        cohost_union_ids: List[str] = None,
+        conf_allowed_corp_id: str = None,
+        host_union_id: str = None,
+        lock_room: int = None,
+        mozi_conf_virtual_extra_setting: QueryScheduleConfSettingsResponseBodyScheduleConfSettingModelMoziConfVirtualExtraSetting = None,
+        mute_on_join: int = None,
+        screen_share_forbidden: int = None,
+    ):
+        self.cohost_union_ids = cohost_union_ids
+        self.conf_allowed_corp_id = conf_allowed_corp_id
+        self.host_union_id = host_union_id
+        self.lock_room = lock_room
+        self.mozi_conf_virtual_extra_setting = mozi_conf_virtual_extra_setting
+        self.mute_on_join = mute_on_join
+        self.screen_share_forbidden = screen_share_forbidden
+
+    def validate(self):
+        if self.mozi_conf_virtual_extra_setting:
+            self.mozi_conf_virtual_extra_setting.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.cohost_union_ids is not None:
+            result['cohostUnionIds'] = self.cohost_union_ids
+        if self.conf_allowed_corp_id is not None:
+            result['confAllowedCorpId'] = self.conf_allowed_corp_id
+        if self.host_union_id is not None:
+            result['hostUnionId'] = self.host_union_id
+        if self.lock_room is not None:
+            result['lockRoom'] = self.lock_room
+        if self.mozi_conf_virtual_extra_setting is not None:
+            result['moziConfVirtualExtraSetting'] = self.mozi_conf_virtual_extra_setting.to_map()
+        if self.mute_on_join is not None:
+            result['muteOnJoin'] = self.mute_on_join
+        if self.screen_share_forbidden is not None:
+            result['screenShareForbidden'] = self.screen_share_forbidden
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('cohostUnionIds') is not None:
+            self.cohost_union_ids = m.get('cohostUnionIds')
+        if m.get('confAllowedCorpId') is not None:
+            self.conf_allowed_corp_id = m.get('confAllowedCorpId')
+        if m.get('hostUnionId') is not None:
+            self.host_union_id = m.get('hostUnionId')
+        if m.get('lockRoom') is not None:
+            self.lock_room = m.get('lockRoom')
+        if m.get('moziConfVirtualExtraSetting') is not None:
+            temp_model = QueryScheduleConfSettingsResponseBodyScheduleConfSettingModelMoziConfVirtualExtraSetting()
+            self.mozi_conf_virtual_extra_setting = temp_model.from_map(m['moziConfVirtualExtraSetting'])
+        if m.get('muteOnJoin') is not None:
+            self.mute_on_join = m.get('muteOnJoin')
+        if m.get('screenShareForbidden') is not None:
+            self.screen_share_forbidden = m.get('screenShareForbidden')
+        return self
+
+
+class QueryScheduleConfSettingsResponseBody(TeaModel):
+    def __init__(
+        self,
+        schedule_conf_setting_model: QueryScheduleConfSettingsResponseBodyScheduleConfSettingModel = None,
+    ):
+        self.schedule_conf_setting_model = schedule_conf_setting_model
+
+    def validate(self):
+        if self.schedule_conf_setting_model:
+            self.schedule_conf_setting_model.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.schedule_conf_setting_model is not None:
+            result['scheduleConfSettingModel'] = self.schedule_conf_setting_model.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('scheduleConfSettingModel') is not None:
+            temp_model = QueryScheduleConfSettingsResponseBodyScheduleConfSettingModel()
+            self.schedule_conf_setting_model = temp_model.from_map(m['scheduleConfSettingModel'])
+        return self
+
+
+class QueryScheduleConfSettingsResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: QueryScheduleConfSettingsResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = QueryScheduleConfSettingsResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class QueryScheduleConferenceHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
@@ -5710,33 +6202,77 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
+class UpdateScheduleConfSettingsRequestScheduleConfSettingModelMoziConfVirtualExtraSettingMoziConfExtensionAppSettings(TeaModel):
+    def __init__(
+        self,
+        auto_open_mode: int = None,
+        cool_app_code: str = None,
+        extension_app_biz_data: str = None,
+    ):
+        self.auto_open_mode = auto_open_mode
+        self.cool_app_code = cool_app_code
+        self.extension_app_biz_data = extension_app_biz_data
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auto_open_mode is not None:
+            result['autoOpenMode'] = self.auto_open_mode
+        if self.cool_app_code is not None:
+            result['coolAppCode'] = self.cool_app_code
+        if self.extension_app_biz_data is not None:
+            result['extensionAppBizData'] = self.extension_app_biz_data
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('autoOpenMode') is not None:
+            self.auto_open_mode = m.get('autoOpenMode')
+        if m.get('coolAppCode') is not None:
+            self.cool_app_code = m.get('coolAppCode')
+        if m.get('extensionAppBizData') is not None:
+            self.extension_app_biz_data = m.get('extensionAppBizData')
+        return self
+
+
 class UpdateScheduleConfSettingsRequestScheduleConfSettingModelMoziConfVirtualExtraSetting(TeaModel):
     def __init__(
         self,
         enable_chat: int = None,
         enable_web_anonymous_join: bool = None,
         join_before_host: int = None,
         lock_media_status_mic_mute: int = None,
         lock_nick: int = None,
+        mozi_conf_extension_app_settings: List[UpdateScheduleConfSettingsRequestScheduleConfSettingModelMoziConfVirtualExtraSettingMoziConfExtensionAppSettings] = None,
         waiting_room: int = None,
     ):
         self.enable_chat = enable_chat
         self.enable_web_anonymous_join = enable_web_anonymous_join
         self.join_before_host = join_before_host
         self.lock_media_status_mic_mute = lock_media_status_mic_mute
         self.lock_nick = lock_nick
+        self.mozi_conf_extension_app_settings = mozi_conf_extension_app_settings
         self.waiting_room = waiting_room
 
     def validate(self):
-        pass
+        if self.mozi_conf_extension_app_settings:
+            for k in self.mozi_conf_extension_app_settings:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -5746,14 +6282,18 @@
             result['enableWebAnonymousJoin'] = self.enable_web_anonymous_join
         if self.join_before_host is not None:
             result['joinBeforeHost'] = self.join_before_host
         if self.lock_media_status_mic_mute is not None:
             result['lockMediaStatusMicMute'] = self.lock_media_status_mic_mute
         if self.lock_nick is not None:
             result['lockNick'] = self.lock_nick
+        result['moziConfExtensionAppSettings'] = []
+        if self.mozi_conf_extension_app_settings is not None:
+            for k in self.mozi_conf_extension_app_settings:
+                result['moziConfExtensionAppSettings'].append(k.to_map() if k else None)
         if self.waiting_room is not None:
             result['waitingRoom'] = self.waiting_room
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('enableChat') is not None:
@@ -5762,14 +6302,19 @@
             self.enable_web_anonymous_join = m.get('enableWebAnonymousJoin')
         if m.get('joinBeforeHost') is not None:
             self.join_before_host = m.get('joinBeforeHost')
         if m.get('lockMediaStatusMicMute') is not None:
             self.lock_media_status_mic_mute = m.get('lockMediaStatusMicMute')
         if m.get('lockNick') is not None:
             self.lock_nick = m.get('lockNick')
+        self.mozi_conf_extension_app_settings = []
+        if m.get('moziConfExtensionAppSettings') is not None:
+            for k in m.get('moziConfExtensionAppSettings'):
+                temp_model = UpdateScheduleConfSettingsRequestScheduleConfSettingModelMoziConfVirtualExtraSettingMoziConfExtensionAppSettings()
+                self.mozi_conf_extension_app_settings.append(temp_model.from_map(k))
         if m.get('waitingRoom') is not None:
             self.waiting_room = m.get('waitingRoom')
         return self
 
 
 class UpdateScheduleConfSettingsRequestScheduleConfSettingModel(TeaModel):
     def __init__(
```

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/connector_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/connector_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/connector_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/connector_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/contact_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/contact_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/contact_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/contact_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/content_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/content_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/content_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/content_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/contract_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/contract_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/contract_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/contract_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/conv_file_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/conv_file_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/conv_file_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/conv_file_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/cool_app_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/cool_app_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/cool_app_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/cool_app_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/cool_ops_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/cool_ops_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/cool_ops_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/cool_ops_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/credit_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/credit_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/credit_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/credit_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/crm_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/crm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/crm_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/crm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/crm_2_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/crm_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/crm_2_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/crm_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/customer_service_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/customer_service_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/customer_service_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/customer_service_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/datacenter_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/datacenter_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/datacenter_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/datacenter_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/devicemng_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/devicemng_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/devicemng_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/devicemng_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/ding_phone_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/ding_phone_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/ding_phone_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/ding_phone_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/dingmi_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/dingmi_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/dingmi_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/dingmi_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/diot_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/diot_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/diot_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/diot_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/doc_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/doc_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/doc_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/doc_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/doc_2_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/doc_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/doc_2_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/doc_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/dpaas_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/dpaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/dpaas_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/dpaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/drive_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/drive_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/drive_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/drive_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/edu_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/edu_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/edu_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/edu_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/esign_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/esign_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/esign_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/esign_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/esign_2_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/esign_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/esign_2_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/esign_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/event_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/event_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/event_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/event_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/exclusive_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/exclusive_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/exclusive_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/exclusive_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/finance_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/finance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/finance_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/finance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/flashmeeting_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/flashmeeting_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/flashmeeting_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/flashmeeting_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/flashmsg_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/flashmsg_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/flashmsg_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/flashmsg_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/gateway_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/gateway_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/gateway_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/gateway_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/group_blackboard_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/group_blackboard_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/group_blackboard_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/group_blackboard_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/h3yun_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/h3yun_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/h3yun_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/h3yun_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/h5package_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/h5package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/h5package_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/h5package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/hrbrain_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/hrbrain_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/hrbrain_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/hrbrain_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/hrm_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/hrm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/hrm_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/hrm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/im_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/im_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/im_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/im_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/im_2_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/im_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/im_2_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/im_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/impaas_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/impaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/impaas_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/impaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/industry_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/industry_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/industry_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/industry_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/jzcrm_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/jzcrm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/jzcrm_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/jzcrm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/link_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/link_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/link_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/link_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/live_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/live_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/live_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/live_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/live_activities_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/live_activities_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/live_activities_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/live_activities_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/mail_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/mail_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/mail_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/mail_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/manufacturing_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/manufacturing_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/manufacturing_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/manufacturing_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/micro_app_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/micro_app_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/micro_app_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/micro_app_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/miniapp_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/miniapp_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/miniapp_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/miniapp_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/notable_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/notable_1_0/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -138,30 +138,35 @@
         runtime = util_models.RuntimeOptions()
         headers = dingtalknotable__1__0_models.CreateFieldHeaders()
         return await self.create_field_with_options_async(base_id, sheet_id_or_name, request, headers, runtime)
 
     def create_sheet_with_options(
         self,
         base_id: str,
-        name: str,
         request: dingtalknotable__1__0_models.CreateSheetRequest,
         headers: dingtalknotable__1__0_models.CreateSheetHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalknotable__1__0_models.CreateSheetResponse:
         UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.operator_id):
+            query['operatorId'] = request.operator_id
         body = {}
         if not UtilClient.is_unset(request.fields):
             body['fields'] = request.fields
+        if not UtilClient.is_unset(request.name):
+            body['name'] = request.name
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
+            query=OpenApiUtilClient.query(query),
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='CreateSheet',
             version='notable_1.0',
             protocol='HTTP',
             pathname=f'/v1.0/notable/bases/{base_id}/sheets',
@@ -175,30 +180,35 @@
             dingtalknotable__1__0_models.CreateSheetResponse(),
             self.execute(params, req, runtime)
         )
 
     async def create_sheet_with_options_async(
         self,
         base_id: str,
-        name: str,
         request: dingtalknotable__1__0_models.CreateSheetRequest,
         headers: dingtalknotable__1__0_models.CreateSheetHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalknotable__1__0_models.CreateSheetResponse:
         UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.operator_id):
+            query['operatorId'] = request.operator_id
         body = {}
         if not UtilClient.is_unset(request.fields):
             body['fields'] = request.fields
+        if not UtilClient.is_unset(request.name):
+            body['name'] = request.name
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
+            query=OpenApiUtilClient.query(query),
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='CreateSheet',
             version='notable_1.0',
             protocol='HTTP',
             pathname=f'/v1.0/notable/bases/{base_id}/sheets',
@@ -212,30 +222,28 @@
             dingtalknotable__1__0_models.CreateSheetResponse(),
             await self.execute_async(params, req, runtime)
         )
 
     def create_sheet(
         self,
         base_id: str,
-        name: str,
         request: dingtalknotable__1__0_models.CreateSheetRequest,
     ) -> dingtalknotable__1__0_models.CreateSheetResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalknotable__1__0_models.CreateSheetHeaders()
-        return self.create_sheet_with_options(base_id, name, request, headers, runtime)
+        return self.create_sheet_with_options(base_id, request, headers, runtime)
 
     async def create_sheet_async(
         self,
         base_id: str,
-        name: str,
         request: dingtalknotable__1__0_models.CreateSheetRequest,
     ) -> dingtalknotable__1__0_models.CreateSheetResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalknotable__1__0_models.CreateSheetHeaders()
-        return await self.create_sheet_with_options_async(base_id, name, request, headers, runtime)
+        return await self.create_sheet_with_options_async(base_id, request, headers, runtime)
 
     def delete_field_with_options(
         self,
         base_id: str,
         sheet_id_or_name: str,
         field_id_or_name: str,
         request: dingtalknotable__1__0_models.DeleteFieldRequest,
@@ -433,24 +441,30 @@
         headers = dingtalknotable__1__0_models.DeleteRecordsHeaders()
         return await self.delete_records_with_options_async(base_id, sheet_id_or_name, request, headers, runtime)
 
     def delete_sheet_with_options(
         self,
         base_id: str,
         sheet_id_or_name: str,
+        request: dingtalknotable__1__0_models.DeleteSheetRequest,
         headers: dingtalknotable__1__0_models.DeleteSheetHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalknotable__1__0_models.DeleteSheetResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.operator_id):
+            query['operatorId'] = request.operator_id
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
-            headers=real_headers
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DeleteSheet',
             version='notable_1.0',
             protocol='HTTP',
             pathname=f'/v1.0/notable/bases/{base_id}/sheets/{sheet_id_or_name}',
             method='DELETE',
@@ -464,24 +478,30 @@
             self.execute(params, req, runtime)
         )
 
     async def delete_sheet_with_options_async(
         self,
         base_id: str,
         sheet_id_or_name: str,
+        request: dingtalknotable__1__0_models.DeleteSheetRequest,
         headers: dingtalknotable__1__0_models.DeleteSheetHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalknotable__1__0_models.DeleteSheetResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.operator_id):
+            query['operatorId'] = request.operator_id
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
-            headers=real_headers
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DeleteSheet',
             version='notable_1.0',
             protocol='HTTP',
             pathname=f'/v1.0/notable/bases/{base_id}/sheets/{sheet_id_or_name}',
             method='DELETE',
@@ -495,27 +515,29 @@
             await self.execute_async(params, req, runtime)
         )
 
     def delete_sheet(
         self,
         base_id: str,
         sheet_id_or_name: str,
+        request: dingtalknotable__1__0_models.DeleteSheetRequest,
     ) -> dingtalknotable__1__0_models.DeleteSheetResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalknotable__1__0_models.DeleteSheetHeaders()
-        return self.delete_sheet_with_options(base_id, sheet_id_or_name, headers, runtime)
+        return self.delete_sheet_with_options(base_id, sheet_id_or_name, request, headers, runtime)
 
     async def delete_sheet_async(
         self,
         base_id: str,
         sheet_id_or_name: str,
+        request: dingtalknotable__1__0_models.DeleteSheetRequest,
     ) -> dingtalknotable__1__0_models.DeleteSheetResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalknotable__1__0_models.DeleteSheetHeaders()
-        return await self.delete_sheet_with_options_async(base_id, sheet_id_or_name, headers, runtime)
+        return await self.delete_sheet_with_options_async(base_id, sheet_id_or_name, request, headers, runtime)
 
     def get_all_fields_with_options(
         self,
         base_id: str,
         sheet_id_or_name: str,
         request: dingtalknotable__1__0_models.GetAllFieldsRequest,
         headers: dingtalknotable__1__0_models.GetAllFieldsHeaders,
@@ -606,24 +628,30 @@
         runtime = util_models.RuntimeOptions()
         headers = dingtalknotable__1__0_models.GetAllFieldsHeaders()
         return await self.get_all_fields_with_options_async(base_id, sheet_id_or_name, request, headers, runtime)
 
     def get_all_sheets_with_options(
         self,
         base_id: str,
+        request: dingtalknotable__1__0_models.GetAllSheetsRequest,
         headers: dingtalknotable__1__0_models.GetAllSheetsHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalknotable__1__0_models.GetAllSheetsResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.operator_id):
+            query['operatorId'] = request.operator_id
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
-            headers=real_headers
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetAllSheets',
             version='notable_1.0',
             protocol='HTTP',
             pathname=f'/v1.0/notable/bases/{base_id}/sheets',
             method='GET',
@@ -636,24 +664,30 @@
             dingtalknotable__1__0_models.GetAllSheetsResponse(),
             self.execute(params, req, runtime)
         )
 
     async def get_all_sheets_with_options_async(
         self,
         base_id: str,
+        request: dingtalknotable__1__0_models.GetAllSheetsRequest,
         headers: dingtalknotable__1__0_models.GetAllSheetsHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalknotable__1__0_models.GetAllSheetsResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.operator_id):
+            query['operatorId'] = request.operator_id
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
-            headers=real_headers
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetAllSheets',
             version='notable_1.0',
             protocol='HTTP',
             pathname=f'/v1.0/notable/bases/{base_id}/sheets',
             method='GET',
@@ -666,42 +700,50 @@
             dingtalknotable__1__0_models.GetAllSheetsResponse(),
             await self.execute_async(params, req, runtime)
         )
 
     def get_all_sheets(
         self,
         base_id: str,
+        request: dingtalknotable__1__0_models.GetAllSheetsRequest,
     ) -> dingtalknotable__1__0_models.GetAllSheetsResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalknotable__1__0_models.GetAllSheetsHeaders()
-        return self.get_all_sheets_with_options(base_id, headers, runtime)
+        return self.get_all_sheets_with_options(base_id, request, headers, runtime)
 
     async def get_all_sheets_async(
         self,
         base_id: str,
+        request: dingtalknotable__1__0_models.GetAllSheetsRequest,
     ) -> dingtalknotable__1__0_models.GetAllSheetsResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalknotable__1__0_models.GetAllSheetsHeaders()
-        return await self.get_all_sheets_with_options_async(base_id, headers, runtime)
+        return await self.get_all_sheets_with_options_async(base_id, request, headers, runtime)
 
     def get_record_with_options(
         self,
         base_id: str,
         sheet_id_or_name: str,
         record_id: str,
+        request: dingtalknotable__1__0_models.GetRecordRequest,
         headers: dingtalknotable__1__0_models.GetRecordHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalknotable__1__0_models.GetRecordResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.operator_id):
+            query['operatorId'] = request.operator_id
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
-            headers=real_headers
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetRecord',
             version='notable_1.0',
             protocol='HTTP',
             pathname=f'/v1.0/notable/bases/{base_id}/sheets/{sheet_id_or_name}/records/{record_id}',
             method='GET',
@@ -716,24 +758,30 @@
         )
 
     async def get_record_with_options_async(
         self,
         base_id: str,
         sheet_id_or_name: str,
         record_id: str,
+        request: dingtalknotable__1__0_models.GetRecordRequest,
         headers: dingtalknotable__1__0_models.GetRecordHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalknotable__1__0_models.GetRecordResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.operator_id):
+            query['operatorId'] = request.operator_id
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
-            headers=real_headers
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetRecord',
             version='notable_1.0',
             protocol='HTTP',
             pathname=f'/v1.0/notable/bases/{base_id}/sheets/{sheet_id_or_name}/records/{record_id}',
             method='GET',
@@ -748,28 +796,30 @@
         )
 
     def get_record(
         self,
         base_id: str,
         sheet_id_or_name: str,
         record_id: str,
+        request: dingtalknotable__1__0_models.GetRecordRequest,
     ) -> dingtalknotable__1__0_models.GetRecordResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalknotable__1__0_models.GetRecordHeaders()
-        return self.get_record_with_options(base_id, sheet_id_or_name, record_id, headers, runtime)
+        return self.get_record_with_options(base_id, sheet_id_or_name, record_id, request, headers, runtime)
 
     async def get_record_async(
         self,
         base_id: str,
         sheet_id_or_name: str,
         record_id: str,
+        request: dingtalknotable__1__0_models.GetRecordRequest,
     ) -> dingtalknotable__1__0_models.GetRecordResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalknotable__1__0_models.GetRecordHeaders()
-        return await self.get_record_with_options_async(base_id, sheet_id_or_name, record_id, headers, runtime)
+        return await self.get_record_with_options_async(base_id, sheet_id_or_name, record_id, request, headers, runtime)
 
     def get_records_with_options(
         self,
         base_id: str,
         sheet_id_or_name: str,
         request: dingtalknotable__1__0_models.GetRecordsRequest,
         headers: dingtalknotable__1__0_models.GetRecordsHeaders,
@@ -777,14 +827,16 @@
     ) -> dingtalknotable__1__0_models.GetRecordsResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.max_results):
             query['maxResults'] = request.max_results
         if not UtilClient.is_unset(request.next_token):
             query['nextToken'] = request.next_token
+        if not UtilClient.is_unset(request.operator_id):
+            query['operatorId'] = request.operator_id
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
@@ -816,14 +868,16 @@
     ) -> dingtalknotable__1__0_models.GetRecordsResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.max_results):
             query['maxResults'] = request.max_results
         if not UtilClient.is_unset(request.next_token):
             query['nextToken'] = request.next_token
+        if not UtilClient.is_unset(request.operator_id):
+            query['operatorId'] = request.operator_id
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
@@ -865,24 +919,30 @@
         headers = dingtalknotable__1__0_models.GetRecordsHeaders()
         return await self.get_records_with_options_async(base_id, sheet_id_or_name, request, headers, runtime)
 
     def get_sheet_with_options(
         self,
         base_id: str,
         sheet_id_or_name: str,
+        request: dingtalknotable__1__0_models.GetSheetRequest,
         headers: dingtalknotable__1__0_models.GetSheetHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalknotable__1__0_models.GetSheetResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.operator_id):
+            query['operatorId'] = request.operator_id
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
-            headers=real_headers
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetSheet',
             version='notable_1.0',
             protocol='HTTP',
             pathname=f'/v1.0/notable/bases/{base_id}/sheets/{sheet_id_or_name}',
             method='GET',
@@ -896,24 +956,30 @@
             self.execute(params, req, runtime)
         )
 
     async def get_sheet_with_options_async(
         self,
         base_id: str,
         sheet_id_or_name: str,
+        request: dingtalknotable__1__0_models.GetSheetRequest,
         headers: dingtalknotable__1__0_models.GetSheetHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalknotable__1__0_models.GetSheetResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.operator_id):
+            query['operatorId'] = request.operator_id
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
-            headers=real_headers
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetSheet',
             version='notable_1.0',
             protocol='HTTP',
             pathname=f'/v1.0/notable/bases/{base_id}/sheets/{sheet_id_or_name}',
             method='GET',
@@ -927,47 +993,53 @@
             await self.execute_async(params, req, runtime)
         )
 
     def get_sheet(
         self,
         base_id: str,
         sheet_id_or_name: str,
+        request: dingtalknotable__1__0_models.GetSheetRequest,
     ) -> dingtalknotable__1__0_models.GetSheetResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalknotable__1__0_models.GetSheetHeaders()
-        return self.get_sheet_with_options(base_id, sheet_id_or_name, headers, runtime)
+        return self.get_sheet_with_options(base_id, sheet_id_or_name, request, headers, runtime)
 
     async def get_sheet_async(
         self,
         base_id: str,
         sheet_id_or_name: str,
+        request: dingtalknotable__1__0_models.GetSheetRequest,
     ) -> dingtalknotable__1__0_models.GetSheetResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalknotable__1__0_models.GetSheetHeaders()
-        return await self.get_sheet_with_options_async(base_id, sheet_id_or_name, headers, runtime)
+        return await self.get_sheet_with_options_async(base_id, sheet_id_or_name, request, headers, runtime)
 
     def insert_records_with_options(
         self,
         base_id: str,
         sheet_id_or_name: str,
         request: dingtalknotable__1__0_models.InsertRecordsRequest,
         headers: dingtalknotable__1__0_models.InsertRecordsHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalknotable__1__0_models.InsertRecordsResponse:
         UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.operator_id):
+            query['operatorId'] = request.operator_id
         body = {}
         if not UtilClient.is_unset(request.records):
             body['records'] = request.records
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
+            query=OpenApiUtilClient.query(query),
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='InsertRecords',
             version='notable_1.0',
             protocol='HTTP',
             pathname=f'/v1.0/notable/bases/{base_id}/sheets/{sheet_id_or_name}/records',
@@ -987,24 +1059,28 @@
         base_id: str,
         sheet_id_or_name: str,
         request: dingtalknotable__1__0_models.InsertRecordsRequest,
         headers: dingtalknotable__1__0_models.InsertRecordsHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalknotable__1__0_models.InsertRecordsResponse:
         UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.operator_id):
+            query['operatorId'] = request.operator_id
         body = {}
         if not UtilClient.is_unset(request.records):
             body['records'] = request.records
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
+            query=OpenApiUtilClient.query(query),
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='InsertRecords',
             version='notable_1.0',
             protocol='HTTP',
             pathname=f'/v1.0/notable/bases/{base_id}/sheets/{sheet_id_or_name}/records',
```

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/notable_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/notable_1_0/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -240,16 +240,20 @@
         return self
 
 
 class CreateSheetRequest(TeaModel):
     def __init__(
         self,
         fields: List[CreateSheetRequestFields] = None,
+        name: str = None,
+        operator_id: str = None,
     ):
         self.fields = fields
+        self.name = name
+        self.operator_id = operator_id
 
     def validate(self):
         if self.fields:
             for k in self.fields:
                 if k:
                     k.validate()
 
@@ -259,23 +263,31 @@
             return _map
 
         result = dict()
         result['fields'] = []
         if self.fields is not None:
             for k in self.fields:
                 result['fields'].append(k.to_map() if k else None)
+        if self.name is not None:
+            result['name'] = self.name
+        if self.operator_id is not None:
+            result['operatorId'] = self.operator_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         self.fields = []
         if m.get('fields') is not None:
             for k in m.get('fields'):
                 temp_model = CreateSheetRequestFields()
                 self.fields.append(temp_model.from_map(k))
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('operatorId') is not None:
+            self.operator_id = m.get('operatorId')
         return self
 
 
 class CreateSheetResponseBody(TeaModel):
     def __init__(
         self,
         id: str = None,
@@ -640,14 +652,41 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
+class DeleteSheetRequest(TeaModel):
+    def __init__(
+        self,
+        operator_id: str = None,
+    ):
+        self.operator_id = operator_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.operator_id is not None:
+            result['operatorId'] = self.operator_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('operatorId') is not None:
+            self.operator_id = m.get('operatorId')
+        return self
+
+
 class DeleteSheetResponseBody(TeaModel):
     def __init__(
         self,
         success: bool = None,
     ):
         self.success = success
 
@@ -922,99 +961,67 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class GetAllSheetsResponseBodyValueFields(TeaModel):
+class GetAllSheetsRequest(TeaModel):
     def __init__(
         self,
-        id: str = None,
-        name: str = None,
-        property: Dict[str, Any] = None,
-        type: str = None,
+        operator_id: str = None,
     ):
-        self.id = id
-        self.name = name
-        self.property = property
-        self.type = type
+        self.operator_id = operator_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.id is not None:
-            result['id'] = self.id
-        if self.name is not None:
-            result['name'] = self.name
-        if self.property is not None:
-            result['property'] = self.property
-        if self.type is not None:
-            result['type'] = self.type
+        if self.operator_id is not None:
+            result['operatorId'] = self.operator_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('id') is not None:
-            self.id = m.get('id')
-        if m.get('name') is not None:
-            self.name = m.get('name')
-        if m.get('property') is not None:
-            self.property = m.get('property')
-        if m.get('type') is not None:
-            self.type = m.get('type')
+        if m.get('operatorId') is not None:
+            self.operator_id = m.get('operatorId')
         return self
 
 
 class GetAllSheetsResponseBodyValue(TeaModel):
     def __init__(
         self,
-        fields: List[GetAllSheetsResponseBodyValueFields] = None,
         id: str = None,
         name: str = None,
     ):
-        self.fields = fields
         self.id = id
         self.name = name
 
     def validate(self):
-        if self.fields:
-            for k in self.fields:
-                if k:
-                    k.validate()
+        pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        result['fields'] = []
-        if self.fields is not None:
-            for k in self.fields:
-                result['fields'].append(k.to_map() if k else None)
         if self.id is not None:
             result['id'] = self.id
         if self.name is not None:
             result['name'] = self.name
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        self.fields = []
-        if m.get('fields') is not None:
-            for k in m.get('fields'):
-                temp_model = GetAllSheetsResponseBodyValueFields()
-                self.fields.append(temp_model.from_map(k))
         if m.get('id') is not None:
             self.id = m.get('id')
         if m.get('name') is not None:
             self.name = m.get('name')
         return self
 
 
@@ -1123,14 +1130,41 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
+class GetRecordRequest(TeaModel):
+    def __init__(
+        self,
+        operator_id: str = None,
+    ):
+        self.operator_id = operator_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.operator_id is not None:
+            result['operatorId'] = self.operator_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('operatorId') is not None:
+            self.operator_id = m.get('operatorId')
+        return self
+
+
 class GetRecordResponseBody(TeaModel):
     def __init__(
         self,
         fields: Dict[str, Any] = None,
         id: str = None,
     ):
         self.fields = fields
@@ -1235,39 +1269,45 @@
 
 
 class GetRecordsRequest(TeaModel):
     def __init__(
         self,
         max_results: int = None,
         next_token: str = None,
+        operator_id: str = None,
     ):
         self.max_results = max_results
         self.next_token = next_token
+        self.operator_id = operator_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.max_results is not None:
             result['maxResults'] = self.max_results
         if self.next_token is not None:
             result['nextToken'] = self.next_token
+        if self.operator_id is not None:
+            result['operatorId'] = self.operator_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('maxResults') is not None:
             self.max_results = m.get('maxResults')
         if m.get('nextToken') is not None:
             self.next_token = m.get('nextToken')
+        if m.get('operatorId') is not None:
+            self.operator_id = m.get('operatorId')
         return self
 
 
 class GetRecordsResponseBodyRecords(TeaModel):
     def __init__(
         self,
         fields: Dict[str, Any] = None,
@@ -1417,91 +1457,71 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class GetSheetResponseBodyFields(TeaModel):
+class GetSheetRequest(TeaModel):
     def __init__(
         self,
-        id: str = None,
-        name: str = None,
-        property: Dict[str, Any] = None,
-        type: str = None,
+        operator_id: str = None,
     ):
-        self.id = id
-        self.name = name
-        self.property = property
-        self.type = type
+        self.operator_id = operator_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.id is not None:
-            result['id'] = self.id
-        if self.name is not None:
-            result['name'] = self.name
-        if self.property is not None:
-            result['property'] = self.property
-        if self.type is not None:
-            result['type'] = self.type
+        if self.operator_id is not None:
+            result['operatorId'] = self.operator_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('id') is not None:
-            self.id = m.get('id')
-        if m.get('name') is not None:
-            self.name = m.get('name')
-        if m.get('property') is not None:
-            self.property = m.get('property')
-        if m.get('type') is not None:
-            self.type = m.get('type')
+        if m.get('operatorId') is not None:
+            self.operator_id = m.get('operatorId')
         return self
 
 
 class GetSheetResponseBody(TeaModel):
     def __init__(
         self,
-        fields: List[GetSheetResponseBodyFields] = None,
+        id: str = None,
+        name: str = None,
     ):
-        self.fields = fields
+        self.id = id
+        self.name = name
 
     def validate(self):
-        if self.fields:
-            for k in self.fields:
-                if k:
-                    k.validate()
+        pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        result['fields'] = []
-        if self.fields is not None:
-            for k in self.fields:
-                result['fields'].append(k.to_map() if k else None)
+        if self.id is not None:
+            result['id'] = self.id
+        if self.name is not None:
+            result['name'] = self.name
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        self.fields = []
-        if m.get('fields') is not None:
-            for k in m.get('fields'):
-                temp_model = GetSheetResponseBodyFields()
-                self.fields.append(temp_model.from_map(k))
+        if m.get('id') is not None:
+            self.id = m.get('id')
+        if m.get('name') is not None:
+            self.name = m.get('name')
         return self
 
 
 class GetSheetResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
@@ -1602,16 +1622,18 @@
         return self
 
 
 class InsertRecordsRequest(TeaModel):
     def __init__(
         self,
         records: List[InsertRecordsRequestRecords] = None,
+        operator_id: str = None,
     ):
         self.records = records
+        self.operator_id = operator_id
 
     def validate(self):
         if self.records:
             for k in self.records:
                 if k:
                     k.validate()
 
@@ -1621,23 +1643,27 @@
             return _map
 
         result = dict()
         result['records'] = []
         if self.records is not None:
             for k in self.records:
                 result['records'].append(k.to_map() if k else None)
+        if self.operator_id is not None:
+            result['operatorId'] = self.operator_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         self.records = []
         if m.get('records') is not None:
             for k in m.get('records'):
                 temp_model = InsertRecordsRequestRecords()
                 self.records.append(temp_model.from_map(k))
+        if m.get('operatorId') is not None:
+            self.operator_id = m.get('operatorId')
         return self
 
 
 class InsertRecordsResponseBodyValue(TeaModel):
     def __init__(
         self,
         id: str = None,
```

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/oauth2_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/oauth2_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/oauth2_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/oauth2_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/occupationauth_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/occupationauth_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/occupationauth_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/occupationauth_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/okr_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/okr_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/okr_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/okr_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/org_culture_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/org_culture_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/org_culture_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/org_culture_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/package_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/package_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/pedia_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/pedia_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/pedia_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/pedia_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/project_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/project_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/project_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/project_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/project_integration_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/project_integration_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/project_integration_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/project_integration_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/rcs_call_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/rcs_call_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/rcs_call_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/rcs_call_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/report_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/report_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/report_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/report_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/resident_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/resident_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/resident_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/resident_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/robot_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/robot_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/robot_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/robot_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/rooms_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/rooms_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/rooms_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/rooms_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/search_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/search_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/search_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/search_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/service_group_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/service_group_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/service_group_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/service_group_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/smart_device_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/smart_device_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/smart_device_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/smart_device_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/sns_storage_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/sns_storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/sns_storage_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/sns_storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/storage_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/storage_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/storage_2_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/storage_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/storage_2_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/storage_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/swform_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/swform_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/swform_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/swform_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/todo_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/todo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/todo_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/todo_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/trade_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/trade_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/trade_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/trade_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/trajectory_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/trajectory_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/trajectory_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/trajectory_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/transcribe_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/transcribe_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/transcribe_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/transcribe_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/trip_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/trip_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/trip_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/trip_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/village_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/village_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/village_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/village_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/watt_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/watt_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/watt_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/watt_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/wiki_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/wiki_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/wiki_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/wiki_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/wiki_2_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/wiki_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/wiki_2_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/wiki_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/wms_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/wms_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/wms_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/wms_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/workbench_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/workbench_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/workbench_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/workbench_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/workflow_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/workflow_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/workflow_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/workflow_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/workrecord_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/workrecord_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/workrecord_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/workrecord_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/yida_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/yida_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/yida_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/yida_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/yun_shu_1_0/client.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/yun_shu_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk/yun_shu_1_0/models.py` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/yun_shu_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk.egg-info/PKG-INFO` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dingtalk
-Version: 2.0.98
+Version: 2.0.99
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dingtalk-2.0.98/alibabacloud_dingtalk.egg-info/SOURCES.txt` & `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.98/setup.py` & `alibabacloud_dingtalk-2.0.99/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dingtalk.
 
-Created on 23/04/2024
+Created on 26/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dingtalk"
 NAME = "alibabacloud_dingtalk" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Dingtalk SDK Library for Python"
```

