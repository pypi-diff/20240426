# Comparing `tmp/shadowsocks_manager-0.1.1.3.tar.gz` & `tmp/shadowsocks_manager-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shadowsocks_manager-0.1.1.3.tar", last modified: Thu Apr 25 16:32:47 2024, max compression
+gzip compressed data, was "shadowsocks_manager-0.1.2.tar", last modified: Fri Apr 26 19:19:38 2024, max compression
```

## Comparing `shadowsocks_manager-0.1.1.3.tar` & `shadowsocks_manager-0.1.2.tar`

### file list

```diff
@@ -1,123 +1,124 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:32:47.899717 shadowsocks_manager-0.1.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    18976 2024-04-25 16:32:47.895717 shadowsocks_manager-0.1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14618 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:32:47.879717 shadowsocks_manager-0.1.1.3/bin/
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/bin/ssm-dev-start
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/bin/ssm-dev-stop
--rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/bin/ssm-setup
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/bin/ssm-test
--rw-r--r--   0 runner    (1001) docker     (127)     6051 2024-04-25 16:32:44.000000 shadowsocks_manager-0.1.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 16:32:47.899717 shadowsocks_manager-0.1.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:32:47.883717 shadowsocks_manager-0.1.1.3/shadowsocks_manager/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/.env
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:32:47.883717 shadowsocks_manager-0.1.1.3/shadowsocks_manager/args_formatter/
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/args_formatter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/args_formatter/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:32:47.883717 shadowsocks_manager-0.1.1.3/shadowsocks_manager/domain/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/domain/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/domain/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:32:47.883717 shadowsocks_manager-0.1.1.3/shadowsocks_manager/domain/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/domain/fixtures/nameserver.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:32:47.883717 shadowsocks_manager-0.1.1.3/shadowsocks_manager/domain/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/domain/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8241 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/domain/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/domain/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3926 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/domain/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/domain/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/domain/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:32:47.887717 shadowsocks_manager-0.1.1.3/shadowsocks_manager/dynamicmethod/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/dynamicmethod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/dynamicmethod/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/dynamicmethod/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:32:47.887717 shadowsocks_manager-0.1.1.3/shadowsocks_manager/dynamicmethod/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/dynamicmethod/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/dynamicmethod/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/dynamicmethod/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/dynamicmethod/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:32:47.887717 shadowsocks_manager-0.1.1.3/shadowsocks_manager/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/fixtures/auth.group.json
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/fixtures/django_celery_beat.crontabschedule.json
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/fixtures/django_celery_beat.intervalschedule.json
--rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/fixtures/django_celery_beat.periodictask.json
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/fixtures/sites.site.json
--rwxr-xr-x   0 runner    (1001) docker     (127)      940 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:32:47.887717 shadowsocks_manager-0.1.1.3/shadowsocks_manager/notification/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/notification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/notification/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/notification/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:32:47.887717 shadowsocks_manager-0.1.1.3/shadowsocks_manager/notification/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/notification/fixtures/template.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:32:47.887717 shadowsocks_manager-0.1.1.3/shadowsocks_manager/notification/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/notification/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/notification/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/notification/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/notification/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/notification/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/notification/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:32:47.887717 shadowsocks_manager-0.1.1.3/shadowsocks_manager/retry/
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/retry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/retry/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:32:47.891717 shadowsocks_manager-0.1.1.3/shadowsocks_manager/shadowsocks_manager/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/shadowsocks_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/shadowsocks_manager/celery.py
--rw-r--r--   0 runner    (1001) docker     (127)     5771 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/shadowsocks_manager/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/shadowsocks_manager/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/shadowsocks_manager/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:32:47.891717 shadowsocks_manager-0.1.1.3/shadowsocks_manager/shadowsocksz/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/shadowsocksz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6335 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/shadowsocksz/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/shadowsocksz/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:32:47.891717 shadowsocks_manager-0.1.1.3/shadowsocks_manager/shadowsocksz/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/shadowsocksz/fixtures/config.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:32:47.891717 shadowsocks_manager-0.1.1.3/shadowsocks_manager/shadowsocksz/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/shadowsocksz/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:32:47.891717 shadowsocks_manager-0.1.1.3/shadowsocks_manager/shadowsocksz/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/shadowsocksz/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/shadowsocksz/management/commands/shadowsocks_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:32:47.891717 shadowsocks_manager-0.1.1.3/shadowsocks_manager/shadowsocksz/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/shadowsocksz/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36547 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/shadowsocksz/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/shadowsocksz/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/shadowsocksz/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)    19241 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/shadowsocksz/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/shadowsocksz/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/shadowsocksz/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:32:47.891717 shadowsocks_manager-0.1.1.3/shadowsocks_manager/singleton/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/singleton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/singleton/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/singleton/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:32:47.891717 shadowsocks_manager-0.1.1.3/shadowsocks_manager/singleton/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/singleton/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/singleton/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/singleton/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/singleton/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:32:47.895717 shadowsocks_manager-0.1.1.3/shadowsocks_manager/statistic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/statistic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/statistic/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/statistic/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:32:47.895717 shadowsocks_manager-0.1.1.3/shadowsocks_manager/statistic/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/statistic/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10309 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/statistic/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/statistic/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/statistic/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/statistic/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/statistic/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/statistic/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:32:47.895717 shadowsocks_manager-0.1.1.3/shadowsocks_manager/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/utils/celery.py
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/utils/createsuperuser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/utils/dotenv.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/utils/manage.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-25 16:32:31.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager/utils/uwsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:32:47.895717 shadowsocks_manager-0.1.1.3/shadowsocks_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18976 2024-04-25 16:32:47.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-04-25 16:32:47.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 16:32:47.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-25 16:32:47.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-25 16:32:47.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-25 16:32:47.000000 shadowsocks_manager-0.1.1.3/shadowsocks_manager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:38.977722 shadowsocks_manager-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    19905 2024-04-26 19:19:38.977722 shadowsocks_manager-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15475 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:38.961722 shadowsocks_manager-0.1.2/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/bin/ssm-dev-start
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/bin/ssm-dev-stop
+-rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/bin/ssm-setup
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/bin/ssm-test
+-rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-04-26 19:19:35.000000 shadowsocks_manager-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-04-26 19:19:38.977722 shadowsocks_manager-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:38.961722 shadowsocks_manager-0.1.2/shadowsocks_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/.env
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:38.961722 shadowsocks_manager-0.1.2/shadowsocks_manager/args_formatter/
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/args_formatter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/args_formatter/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:38.965722 shadowsocks_manager-0.1.2/shadowsocks_manager/domain/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/domain/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/domain/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:38.965722 shadowsocks_manager-0.1.2/shadowsocks_manager/domain/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/domain/fixtures/nameserver.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:38.965722 shadowsocks_manager-0.1.2/shadowsocks_manager/domain/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/domain/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8241 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/domain/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/domain/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3926 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/domain/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/domain/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/domain/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:38.965722 shadowsocks_manager-0.1.2/shadowsocks_manager/dynamicmethod/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/dynamicmethod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/dynamicmethod/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/dynamicmethod/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:38.965722 shadowsocks_manager-0.1.2/shadowsocks_manager/dynamicmethod/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/dynamicmethod/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/dynamicmethod/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/dynamicmethod/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/dynamicmethod/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:38.965722 shadowsocks_manager-0.1.2/shadowsocks_manager/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/fixtures/auth.group.json
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/fixtures/django_celery_beat.crontabschedule.json
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/fixtures/django_celery_beat.intervalschedule.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/fixtures/django_celery_beat.periodictask.json
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/fixtures/sites.site.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)      940 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:38.965722 shadowsocks_manager-0.1.2/shadowsocks_manager/notification/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/notification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/notification/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/notification/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:38.969722 shadowsocks_manager-0.1.2/shadowsocks_manager/notification/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/notification/fixtures/template.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:38.969722 shadowsocks_manager-0.1.2/shadowsocks_manager/notification/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/notification/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/notification/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/notification/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/notification/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/notification/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/notification/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:38.969722 shadowsocks_manager-0.1.2/shadowsocks_manager/retry/
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/retry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/retry/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:38.969722 shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocks_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocks_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocks_manager/celery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5771 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocks_manager/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocks_manager/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocks_manager/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:38.969722 shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocksz/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocksz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6335 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocksz/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocksz/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:38.969722 shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocksz/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocksz/fixtures/config.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:38.969722 shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocksz/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocksz/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:38.969722 shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocksz/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocksz/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocksz/management/commands/shadowsocks_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:38.969722 shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocksz/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocksz/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36547 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocksz/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocksz/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocksz/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19241 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocksz/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocksz/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocksz/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:38.973722 shadowsocks_manager-0.1.2/shadowsocks_manager/singleton/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/singleton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/singleton/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/singleton/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:38.973722 shadowsocks_manager-0.1.2/shadowsocks_manager/singleton/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/singleton/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/singleton/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/singleton/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/singleton/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:38.973722 shadowsocks_manager-0.1.2/shadowsocks_manager/statistic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/statistic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/statistic/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/statistic/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:38.973722 shadowsocks_manager-0.1.2/shadowsocks_manager/statistic/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/statistic/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10309 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/statistic/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/statistic/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/statistic/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/statistic/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/statistic/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/statistic/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:38.973722 shadowsocks_manager-0.1.2/shadowsocks_manager/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/utils/celery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/utils/createsuperuser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/utils/dotenv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/utils/manage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/utils/uwsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:38.973722 shadowsocks_manager-0.1.2/shadowsocks_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19905 2024-04-26 19:19:38.000000 shadowsocks_manager-0.1.2/shadowsocks_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3993 2024-04-26 19:19:38.000000 shadowsocks_manager-0.1.2/shadowsocks_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 19:19:38.000000 shadowsocks_manager-0.1.2/shadowsocks_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-26 19:19:38.000000 shadowsocks_manager-0.1.2/shadowsocks_manager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-26 19:19:38.000000 shadowsocks_manager-0.1.2/shadowsocks_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-26 19:19:38.000000 shadowsocks_manager-0.1.2/shadowsocks_manager.egg-info/top_level.txt
```

### Comparing `shadowsocks_manager-0.1.1.3/LICENSE` & `shadowsocks_manager-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1.3/PKG-INFO` & `shadowsocks_manager-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 Metadata-Version: 2.1
 Name: shadowsocks-manager
-Version: 0.1.1.3
+Version: 0.1.2
 Summary: A shadowsocks manager for multi-user and traffic statistics
+Home-page: https://github.com/alexzhangs/shadowsocks-manager
+Author: Alex
 Author-email: Alex <alexzhangs@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Alex Zhang
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -142,17 +144,15 @@
 ![Home › Shadowsocks › Shadowsocks Nodes](https://www.0xbeta.com/shadowsocks-manager/assets/images/shadowsocks-node-ssmanager.png)
 
 
 ## 1. Requirements
 
 * Python 2.7, Python 3.x
 * Django 1.11.x, Django 3.x
-* macOS Big Sur
-* [AWS Amazon Linux AMI](https://aws.amazon.com/amazon-linux-ami/)
-* [AWS Amazon Linux 2 AMI](https://aws.amazon.com/amazon-linux-2/)
+* Docker
 * [Shadowsocks-libev 3.2.0 for Linux (multi-user API is required)](https://github.com/shadowsocks/shadowsocks-libev)
 
 
 ## 2. Install
 
 This project is a part of an entire VPN solution, which includes the Shadowsocks server and Shadowsocks manager. The Shadowsocks server serves the traffic, the Shadowsocks manager serves the users and the traffic statistics. The solution is designed to be deployed in the AWS cloud. If you are looking for such a solution, you can refer to the repo [aws-cfn-vpn](https://github.com/alexzhangs/aws-cfn-vpn). With `aws-cfn-vpn`, you can deploy the entire solution with a few commands.
 
@@ -296,15 +296,15 @@
 ### Update for Shadowsocks Python edition on 2024-04
 
 Both the pypi version (2.8.2) and the github master branch (3.0.0) failed to start `ssserver` due to the upstream and dependency changes.
 
 Since the Python edition is pre-installed in this project, mainly for running test cases, I have to make a patch to make it work.
 
 The fix based on github master branch 3.0.0, and would be minimal, just to make the `ssserver` start without any error, no more features added.
-After the fix, the pre-installed Python edition will be changed from the pypi version to [my fork](https://github.com/alexforks/shadowsocks/tree/master).
+After the fix, the pre-installed Python edition will be changed from the [original pypi version](https://pypi.org/project/shadowsocks/) to [my fork](https://pypi.org/project/shadowsocks-alexforks/).
 
 
 ## 7. Known Issues
 
 1. DNS records matching for Node may not be accurate on macOS.
     For unknown reason sometimes DNS query returns only one IP address
 while multiple IP addresses were configured for the domain.
@@ -320,17 +320,20 @@
     Solution:
     Link the homebrew openssl library to the system library.
     ```sh
     sudo ln -s /opt/homebrew/opt/openssl/lib/libcrypto.dylib /usr/local/lib/
     sudo ln -s /opt/homebrew/opt/openssl/lib/libssl.dylib /usr/local/lib/
     ```
 
-1. Install the project with pip under Python 2.7 get error:
+1. Install the project by source with pip under Python 2.7 get error:
     ```
-    pip install -e .
+    python --version
+    Python 2.7.18
+
+    pip install .
     ```
 
     Error message:
     ```
     ...
     Collecting pyyaml
     Downloading PyYAML-5.4.1.tar.gz (175 kB)
@@ -342,20 +345,32 @@
         raise AttributeError, attr
     AttributeError: cython_sources
     ...
     ```
 
     Solution:
     ```sh
-    pip install --no-build-isolation -e .
+    pip install setuptools wheel
+    pip install --no-build-isolation .
     ```
 
 
 ## 8. Development
 
+The development of this project requires Python 3.x.
+
+However, the installation of the project is compatible with both Python 2.7 and 3.x.
+To keep the compatibility is difficult, but it's kept due to the historical reason.
+The following files are kept only for installing the source distribution of the PyPI package under Python 2.7:
+
+* setup.py
+* setup.cfg
+
+### 8.1. Development Environment Setup
+
 1. Install the dependencies
 
     ```sh
     # run memcached, used by django cache
     docker run -d -p 11211:11211 --name ssm-memcached memcached
 
     # run rabbitmq, used by celery
@@ -412,62 +427,69 @@
 1. Test the Github workflows locally
 
     ```sh
     brew install act
     act -j test
     ```
 
-1. Build the pypi package
+1. Build the PyPI package
 
     ```sh
     pip install build
 
-    # build source distribution, equivalent to `python setup.py sdist`
-    python -m build -s
-
-    # build binary distribution for py3, equivalent to `python setup.py bdist_wheel`
-    python3 -m build -w
-
-    # build binary distribution for py2
-    python2 -m build -w
+    # build source and binary distribution, equivalent to `python setup.py sdist bdist_wheel`
+    # universal wheel is enabled in the pyproject.toml to make the wheel compatible with both Python 2 and 3
+    python -m build
     ```
 
-1. Upload the pypi package
+1. Upload the PyPI package
 
     Set the ~/.pypirc file with the API token from the TestPyPI and PyPI before uploading.
 
     ```sh
     pip install twine
 
-    # upload the package to the test pypi
+    # upload the package to TestPyPI
     python -m twine upload --repository testpypi dist/*
 
-    # upload the package to the live pypi
+    # upload the package to PyPI
     python -m twine upload dist/*
     ```
 
-1. Test the pypi package
+1. Test the PyPI package
 
     ```sh
-    # install the package from the test pypi
-    # --no-deps is used to skip installing dependencies for the test pypi
+    # install the package from TestPyPI
+    # --no-deps is used to skip installing dependencies for the TestPyPI environment
     pip install -i https://test.pypi.org/simple/ --no-deps shadowsocks-manager
 
-    # install the package from the live pypi
+    # install the package from PyPI
     # --no-binary is used to force building the package from the source
     # --use-pep517 is used together to make sure the PEP 517 is tested
     pip install --no-binary shadowsocks-manager --use-pep517 shadowsocks-manager
     ```
 
 1. Build the docker image
 
     ```sh
     docker build -t alexzhangs/shadowsocks-manager .
     ```
 
+### 8.2. CI/CD
+
+Github Actions is currently used for the CI/CD.
+Travis CI is removed due to the limitation of the free plan.
+
+The CI/CD workflows are defined in the `.github/workflows` directory.
+
+* ci-unittest.yml: Run the unit tests.
+* ci-testpypi.yml: Build and upload the package to TestPyPI.
+* ci-pypi.yml: Build and upload the package to PyPI. It can be triggered by the tag: `ci-pypi` or `ci-pypi-(major|minor|patch|suffx)`.
+* ci-docker.yml: Build and push the docker image to Docker Hub. It can be triggered by the Github release.
+
 
 ## 9. Troubleshooting
 
 1. Check the logs
 
     ```
     # supervisor
```

### Comparing `shadowsocks_manager-0.1.1.3/README.md` & `shadowsocks_manager-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -48,17 +48,15 @@
 ![Home › Shadowsocks › Shadowsocks Nodes](https://www.0xbeta.com/shadowsocks-manager/assets/images/shadowsocks-node-ssmanager.png)
 
 
 ## 1. Requirements
 
 * Python 2.7, Python 3.x
 * Django 1.11.x, Django 3.x
-* macOS Big Sur
-* [AWS Amazon Linux AMI](https://aws.amazon.com/amazon-linux-ami/)
-* [AWS Amazon Linux 2 AMI](https://aws.amazon.com/amazon-linux-2/)
+* Docker
 * [Shadowsocks-libev 3.2.0 for Linux (multi-user API is required)](https://github.com/shadowsocks/shadowsocks-libev)
 
 
 ## 2. Install
 
 This project is a part of an entire VPN solution, which includes the Shadowsocks server and Shadowsocks manager. The Shadowsocks server serves the traffic, the Shadowsocks manager serves the users and the traffic statistics. The solution is designed to be deployed in the AWS cloud. If you are looking for such a solution, you can refer to the repo [aws-cfn-vpn](https://github.com/alexzhangs/aws-cfn-vpn). With `aws-cfn-vpn`, you can deploy the entire solution with a few commands.
 
@@ -202,15 +200,15 @@
 ### Update for Shadowsocks Python edition on 2024-04
 
 Both the pypi version (2.8.2) and the github master branch (3.0.0) failed to start `ssserver` due to the upstream and dependency changes.
 
 Since the Python edition is pre-installed in this project, mainly for running test cases, I have to make a patch to make it work.
 
 The fix based on github master branch 3.0.0, and would be minimal, just to make the `ssserver` start without any error, no more features added.
-After the fix, the pre-installed Python edition will be changed from the pypi version to [my fork](https://github.com/alexforks/shadowsocks/tree/master).
+After the fix, the pre-installed Python edition will be changed from the [original pypi version](https://pypi.org/project/shadowsocks/) to [my fork](https://pypi.org/project/shadowsocks-alexforks/).
 
 
 ## 7. Known Issues
 
 1. DNS records matching for Node may not be accurate on macOS.
     For unknown reason sometimes DNS query returns only one IP address
 while multiple IP addresses were configured for the domain.
@@ -226,17 +224,20 @@
     Solution:
     Link the homebrew openssl library to the system library.
     ```sh
     sudo ln -s /opt/homebrew/opt/openssl/lib/libcrypto.dylib /usr/local/lib/
     sudo ln -s /opt/homebrew/opt/openssl/lib/libssl.dylib /usr/local/lib/
     ```
 
-1. Install the project with pip under Python 2.7 get error:
+1. Install the project by source with pip under Python 2.7 get error:
     ```
-    pip install -e .
+    python --version
+    Python 2.7.18
+
+    pip install .
     ```
 
     Error message:
     ```
     ...
     Collecting pyyaml
     Downloading PyYAML-5.4.1.tar.gz (175 kB)
@@ -248,20 +249,32 @@
         raise AttributeError, attr
     AttributeError: cython_sources
     ...
     ```
 
     Solution:
     ```sh
-    pip install --no-build-isolation -e .
+    pip install setuptools wheel
+    pip install --no-build-isolation .
     ```
 
 
 ## 8. Development
 
+The development of this project requires Python 3.x.
+
+However, the installation of the project is compatible with both Python 2.7 and 3.x.
+To keep the compatibility is difficult, but it's kept due to the historical reason.
+The following files are kept only for installing the source distribution of the PyPI package under Python 2.7:
+
+* setup.py
+* setup.cfg
+
+### 8.1. Development Environment Setup
+
 1. Install the dependencies
 
     ```sh
     # run memcached, used by django cache
     docker run -d -p 11211:11211 --name ssm-memcached memcached
 
     # run rabbitmq, used by celery
@@ -318,62 +331,69 @@
 1. Test the Github workflows locally
 
     ```sh
     brew install act
     act -j test
     ```
 
-1. Build the pypi package
+1. Build the PyPI package
 
     ```sh
     pip install build
 
-    # build source distribution, equivalent to `python setup.py sdist`
-    python -m build -s
-
-    # build binary distribution for py3, equivalent to `python setup.py bdist_wheel`
-    python3 -m build -w
-
-    # build binary distribution for py2
-    python2 -m build -w
+    # build source and binary distribution, equivalent to `python setup.py sdist bdist_wheel`
+    # universal wheel is enabled in the pyproject.toml to make the wheel compatible with both Python 2 and 3
+    python -m build
     ```
 
-1. Upload the pypi package
+1. Upload the PyPI package
 
     Set the ~/.pypirc file with the API token from the TestPyPI and PyPI before uploading.
 
     ```sh
     pip install twine
 
-    # upload the package to the test pypi
+    # upload the package to TestPyPI
     python -m twine upload --repository testpypi dist/*
 
-    # upload the package to the live pypi
+    # upload the package to PyPI
     python -m twine upload dist/*
     ```
 
-1. Test the pypi package
+1. Test the PyPI package
 
     ```sh
-    # install the package from the test pypi
-    # --no-deps is used to skip installing dependencies for the test pypi
+    # install the package from TestPyPI
+    # --no-deps is used to skip installing dependencies for the TestPyPI environment
     pip install -i https://test.pypi.org/simple/ --no-deps shadowsocks-manager
 
-    # install the package from the live pypi
+    # install the package from PyPI
     # --no-binary is used to force building the package from the source
     # --use-pep517 is used together to make sure the PEP 517 is tested
     pip install --no-binary shadowsocks-manager --use-pep517 shadowsocks-manager
     ```
 
 1. Build the docker image
 
     ```sh
     docker build -t alexzhangs/shadowsocks-manager .
     ```
 
+### 8.2. CI/CD
+
+Github Actions is currently used for the CI/CD.
+Travis CI is removed due to the limitation of the free plan.
+
+The CI/CD workflows are defined in the `.github/workflows` directory.
+
+* ci-unittest.yml: Run the unit tests.
+* ci-testpypi.yml: Build and upload the package to TestPyPI.
+* ci-pypi.yml: Build and upload the package to PyPI. It can be triggered by the tag: `ci-pypi` or `ci-pypi-(major|minor|patch|suffx)`.
+* ci-docker.yml: Build and push the docker image to Docker Hub. It can be triggered by the Github release.
+
 
 ## 9. Troubleshooting
 
 1. Check the logs
 
     ```
     # supervisor
```

### Comparing `shadowsocks_manager-0.1.1.3/bin/ssm-dev-start` & `shadowsocks_manager-0.1.2/bin/ssm-dev-start`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1.3/bin/ssm-setup` & `shadowsocks_manager-0.1.2/bin/ssm-setup`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1.3/bin/ssm-test` & `shadowsocks_manager-0.1.2/bin/ssm-test`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1.3/pyproject.toml` & `shadowsocks_manager-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "shadowsocks-manager"
-version = "0.1.1.3"
+version = "0.1.2"
 requires-python = ">=2.7"
 dependencies = [
     "future",
     "six",
     "boto3",
     "celery",
     "Django<4",
@@ -135,27 +135,27 @@
 [tool.setuptools.package-data]
 shadowsocks_manager = ["fixtures/*", "**/fixtures/*", ".env"]
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 [tool.bumpversion]
-current_version = "0.1.1.3"
+current_version = "0.1.2"
 parse = """
     (?P<major>\\d+)\\.
     (?P<minor>\\d+)\\.
     (?P<patch>\\d+)
     (
-        \\.                         # separator
+        \\-                         # separator
         (?P<suffix>[0-9]\\d*)       # suffix Number
     )?                              # suffix is optional
 """
 serialize = [
+    "{major}.{minor}.{patch}-{suffix}",
     "{major}.{minor}.{patch}",
-    "{major}.{minor}.{patch}.{suffix}",
 ]
 search = "{current_version}"
 replace = "{new_version}"
 regex = false
 ignore_missing_version = false
 ignore_missing_files = false
 tag = true
@@ -169,14 +169,20 @@
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = '^version = "{current_version}"$'
 replace = 'version = "{new_version}"'
 regex = true
 
+[[tool.bumpversion.files]]
+filename = "setup.cfg"
+search = '^version = {current_version}$'
+replace = 'version = {new_version}'
+regex = true
+
 [tool.coverage.run]
 source = "."
 branch = true
 
 [tool.coverage.report]
 show_missing = true
 skip_covered = true
```

### Comparing `shadowsocks_manager-0.1.1.3/shadowsocks_manager/__main__.py` & `shadowsocks_manager-0.1.2/shadowsocks_manager/__main__.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1.3/shadowsocks_manager/args_formatter/__init__.py` & `shadowsocks_manager-0.1.2/shadowsocks_manager/args_formatter/__init__.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1.3/shadowsocks_manager/args_formatter/tests.py` & `shadowsocks_manager-0.1.2/shadowsocks_manager/args_formatter/tests.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1.3/shadowsocks_manager/domain/admin.py` & `shadowsocks_manager-0.1.2/shadowsocks_manager/domain/admin.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1.3/shadowsocks_manager/domain/models.py` & `shadowsocks_manager-0.1.2/shadowsocks_manager/domain/models.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1.3/shadowsocks_manager/domain/serializers.py` & `shadowsocks_manager-0.1.2/shadowsocks_manager/domain/serializers.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1.3/shadowsocks_manager/domain/tests.py` & `shadowsocks_manager-0.1.2/shadowsocks_manager/domain/tests.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1.3/shadowsocks_manager/domain/views.py` & `shadowsocks_manager-0.1.2/shadowsocks_manager/domain/views.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1.3/shadowsocks_manager/dynamicmethod/models.py` & `shadowsocks_manager-0.1.2/shadowsocks_manager/dynamicmethod/models.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1.3/shadowsocks_manager/fixtures/django_celery_beat.crontabschedule.json` & `shadowsocks_manager-0.1.2/shadowsocks_manager/fixtures/django_celery_beat.crontabschedule.json`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1.3/shadowsocks_manager/fixtures/django_celery_beat.periodictask.json` & `shadowsocks_manager-0.1.2/shadowsocks_manager/fixtures/django_celery_beat.periodictask.json`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1.3/shadowsocks_manager/manage.py` & `shadowsocks_manager-0.1.2/shadowsocks_manager/manage.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1.3/shadowsocks_manager/notification/fixtures/template.json` & `shadowsocks_manager-0.1.2/shadowsocks_manager/notification/fixtures/template.json`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1.3/shadowsocks_manager/notification/models.py` & `shadowsocks_manager-0.1.2/shadowsocks_manager/notification/models.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1.3/shadowsocks_manager/notification/tests.py` & `shadowsocks_manager-0.1.2/shadowsocks_manager/notification/tests.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1.3/shadowsocks_manager/retry/__init__.py` & `shadowsocks_manager-0.1.2/shadowsocks_manager/retry/__init__.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1.3/shadowsocks_manager/retry/tests.py` & `shadowsocks_manager-0.1.2/shadowsocks_manager/retry/tests.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1.3/shadowsocks_manager/shadowsocks_manager/celery.py` & `shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocks_manager/celery.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1.3/shadowsocks_manager/shadowsocks_manager/settings.py` & `shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocks_manager/settings.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1.3/shadowsocks_manager/shadowsocks_manager/urls.py` & `shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocks_manager/urls.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1.3/shadowsocks_manager/shadowsocksz/admin.py` & `shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocksz/admin.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1.3/shadowsocks_manager/shadowsocksz/management/commands/shadowsocks_config.py` & `shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocksz/management/commands/shadowsocks_config.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1.3/shadowsocks_manager/shadowsocksz/models.py` & `shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocksz/models.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1.3/shadowsocks_manager/shadowsocksz/serializers.py` & `shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocksz/serializers.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1.3/shadowsocks_manager/shadowsocksz/tests.py` & `shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocksz/tests.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1.3/shadowsocks_manager/shadowsocksz/urls.py` & `shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocksz/urls.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1.3/shadowsocks_manager/shadowsocksz/views.py` & `shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocksz/views.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1.3/shadowsocks_manager/singleton/models.py` & `shadowsocks_manager-0.1.2/shadowsocks_manager/singleton/models.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1.3/shadowsocks_manager/statistic/admin.py` & `shadowsocks_manager-0.1.2/shadowsocks_manager/statistic/admin.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1.3/shadowsocks_manager/statistic/models.py` & `shadowsocks_manager-0.1.2/shadowsocks_manager/statistic/models.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1.3/shadowsocks_manager/statistic/serializers.py` & `shadowsocks_manager-0.1.2/shadowsocks_manager/statistic/serializers.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1.3/shadowsocks_manager/statistic/tests.py` & `shadowsocks_manager-0.1.2/shadowsocks_manager/statistic/tests.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1.3/shadowsocks_manager/statistic/views.py` & `shadowsocks_manager-0.1.2/shadowsocks_manager/statistic/views.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1.3/shadowsocks_manager/utils/celery.py` & `shadowsocks_manager-0.1.2/shadowsocks_manager/utils/celery.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1.3/shadowsocks_manager/utils/createsuperuser.py` & `shadowsocks_manager-0.1.2/shadowsocks_manager/utils/createsuperuser.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1.3/shadowsocks_manager/utils/dotenv.py` & `shadowsocks_manager-0.1.2/shadowsocks_manager/utils/dotenv.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1.3/shadowsocks_manager/utils/manage.py` & `shadowsocks_manager-0.1.2/shadowsocks_manager/utils/manage.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1.3/shadowsocks_manager.egg-info/PKG-INFO` & `shadowsocks_manager-0.1.2/shadowsocks_manager.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 Metadata-Version: 2.1
 Name: shadowsocks-manager
-Version: 0.1.1.3
+Version: 0.1.2
 Summary: A shadowsocks manager for multi-user and traffic statistics
+Home-page: https://github.com/alexzhangs/shadowsocks-manager
+Author: Alex
 Author-email: Alex <alexzhangs@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Alex Zhang
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -142,17 +144,15 @@
 ![Home › Shadowsocks › Shadowsocks Nodes](https://www.0xbeta.com/shadowsocks-manager/assets/images/shadowsocks-node-ssmanager.png)
 
 
 ## 1. Requirements
 
 * Python 2.7, Python 3.x
 * Django 1.11.x, Django 3.x
-* macOS Big Sur
-* [AWS Amazon Linux AMI](https://aws.amazon.com/amazon-linux-ami/)
-* [AWS Amazon Linux 2 AMI](https://aws.amazon.com/amazon-linux-2/)
+* Docker
 * [Shadowsocks-libev 3.2.0 for Linux (multi-user API is required)](https://github.com/shadowsocks/shadowsocks-libev)
 
 
 ## 2. Install
 
 This project is a part of an entire VPN solution, which includes the Shadowsocks server and Shadowsocks manager. The Shadowsocks server serves the traffic, the Shadowsocks manager serves the users and the traffic statistics. The solution is designed to be deployed in the AWS cloud. If you are looking for such a solution, you can refer to the repo [aws-cfn-vpn](https://github.com/alexzhangs/aws-cfn-vpn). With `aws-cfn-vpn`, you can deploy the entire solution with a few commands.
 
@@ -296,15 +296,15 @@
 ### Update for Shadowsocks Python edition on 2024-04
 
 Both the pypi version (2.8.2) and the github master branch (3.0.0) failed to start `ssserver` due to the upstream and dependency changes.
 
 Since the Python edition is pre-installed in this project, mainly for running test cases, I have to make a patch to make it work.
 
 The fix based on github master branch 3.0.0, and would be minimal, just to make the `ssserver` start without any error, no more features added.
-After the fix, the pre-installed Python edition will be changed from the pypi version to [my fork](https://github.com/alexforks/shadowsocks/tree/master).
+After the fix, the pre-installed Python edition will be changed from the [original pypi version](https://pypi.org/project/shadowsocks/) to [my fork](https://pypi.org/project/shadowsocks-alexforks/).
 
 
 ## 7. Known Issues
 
 1. DNS records matching for Node may not be accurate on macOS.
     For unknown reason sometimes DNS query returns only one IP address
 while multiple IP addresses were configured for the domain.
@@ -320,17 +320,20 @@
     Solution:
     Link the homebrew openssl library to the system library.
     ```sh
     sudo ln -s /opt/homebrew/opt/openssl/lib/libcrypto.dylib /usr/local/lib/
     sudo ln -s /opt/homebrew/opt/openssl/lib/libssl.dylib /usr/local/lib/
     ```
 
-1. Install the project with pip under Python 2.7 get error:
+1. Install the project by source with pip under Python 2.7 get error:
     ```
-    pip install -e .
+    python --version
+    Python 2.7.18
+
+    pip install .
     ```
 
     Error message:
     ```
     ...
     Collecting pyyaml
     Downloading PyYAML-5.4.1.tar.gz (175 kB)
@@ -342,20 +345,32 @@
         raise AttributeError, attr
     AttributeError: cython_sources
     ...
     ```
 
     Solution:
     ```sh
-    pip install --no-build-isolation -e .
+    pip install setuptools wheel
+    pip install --no-build-isolation .
     ```
 
 
 ## 8. Development
 
+The development of this project requires Python 3.x.
+
+However, the installation of the project is compatible with both Python 2.7 and 3.x.
+To keep the compatibility is difficult, but it's kept due to the historical reason.
+The following files are kept only for installing the source distribution of the PyPI package under Python 2.7:
+
+* setup.py
+* setup.cfg
+
+### 8.1. Development Environment Setup
+
 1. Install the dependencies
 
     ```sh
     # run memcached, used by django cache
     docker run -d -p 11211:11211 --name ssm-memcached memcached
 
     # run rabbitmq, used by celery
@@ -412,62 +427,69 @@
 1. Test the Github workflows locally
 
     ```sh
     brew install act
     act -j test
     ```
 
-1. Build the pypi package
+1. Build the PyPI package
 
     ```sh
     pip install build
 
-    # build source distribution, equivalent to `python setup.py sdist`
-    python -m build -s
-
-    # build binary distribution for py3, equivalent to `python setup.py bdist_wheel`
-    python3 -m build -w
-
-    # build binary distribution for py2
-    python2 -m build -w
+    # build source and binary distribution, equivalent to `python setup.py sdist bdist_wheel`
+    # universal wheel is enabled in the pyproject.toml to make the wheel compatible with both Python 2 and 3
+    python -m build
     ```
 
-1. Upload the pypi package
+1. Upload the PyPI package
 
     Set the ~/.pypirc file with the API token from the TestPyPI and PyPI before uploading.
 
     ```sh
     pip install twine
 
-    # upload the package to the test pypi
+    # upload the package to TestPyPI
     python -m twine upload --repository testpypi dist/*
 
-    # upload the package to the live pypi
+    # upload the package to PyPI
     python -m twine upload dist/*
     ```
 
-1. Test the pypi package
+1. Test the PyPI package
 
     ```sh
-    # install the package from the test pypi
-    # --no-deps is used to skip installing dependencies for the test pypi
+    # install the package from TestPyPI
+    # --no-deps is used to skip installing dependencies for the TestPyPI environment
     pip install -i https://test.pypi.org/simple/ --no-deps shadowsocks-manager
 
-    # install the package from the live pypi
+    # install the package from PyPI
     # --no-binary is used to force building the package from the source
     # --use-pep517 is used together to make sure the PEP 517 is tested
     pip install --no-binary shadowsocks-manager --use-pep517 shadowsocks-manager
     ```
 
 1. Build the docker image
 
     ```sh
     docker build -t alexzhangs/shadowsocks-manager .
     ```
 
+### 8.2. CI/CD
+
+Github Actions is currently used for the CI/CD.
+Travis CI is removed due to the limitation of the free plan.
+
+The CI/CD workflows are defined in the `.github/workflows` directory.
+
+* ci-unittest.yml: Run the unit tests.
+* ci-testpypi.yml: Build and upload the package to TestPyPI.
+* ci-pypi.yml: Build and upload the package to PyPI. It can be triggered by the tag: `ci-pypi` or `ci-pypi-(major|minor|patch|suffx)`.
+* ci-docker.yml: Build and push the docker image to Docker Hub. It can be triggered by the Github release.
+
 
 ## 9. Troubleshooting
 
 1. Check the logs
 
     ```
     # supervisor
```

### Comparing `shadowsocks_manager-0.1.1.3/shadowsocks_manager.egg-info/SOURCES.txt` & `shadowsocks_manager-0.1.2/shadowsocks_manager.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 LICENSE
 README.md
 pyproject.toml
+setup.cfg
+setup.py
 bin/ssm-dev-start
 bin/ssm-dev-stop
 bin/ssm-setup
 bin/ssm-test
 shadowsocks_manager/.env
 shadowsocks_manager/__init__.py
 shadowsocks_manager/__main__.py
```

### Comparing `shadowsocks_manager-0.1.1.3/shadowsocks_manager.egg-info/requires.txt` & `shadowsocks_manager-0.1.2/shadowsocks_manager.egg-info/requires.txt`

 * *Files identical despite different names*

