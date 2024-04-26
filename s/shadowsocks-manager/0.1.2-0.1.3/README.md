# Comparing `tmp/shadowsocks_manager-0.1.2.tar.gz` & `tmp/shadowsocks_manager-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shadowsocks_manager-0.1.2.tar", last modified: Fri Apr 26 19:19:38 2024, max compression
+gzip compressed data, was "shadowsocks_manager-0.1.3.tar", last modified: Fri Apr 26 20:03:28 2024, max compression
```

## Comparing `shadowsocks_manager-0.1.2.tar` & `shadowsocks_manager-0.1.3.tar`

### file list

```diff
@@ -1,124 +1,124 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:38.977722 shadowsocks_manager-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    19905 2024-04-26 19:19:38.977722 shadowsocks_manager-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15475 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:38.961722 shadowsocks_manager-0.1.2/bin/
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/bin/ssm-dev-start
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/bin/ssm-dev-stop
--rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/bin/ssm-setup
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/bin/ssm-test
--rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-04-26 19:19:35.000000 shadowsocks_manager-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-04-26 19:19:38.977722 shadowsocks_manager-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:38.961722 shadowsocks_manager-0.1.2/shadowsocks_manager/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/.env
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:38.961722 shadowsocks_manager-0.1.2/shadowsocks_manager/args_formatter/
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/args_formatter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/args_formatter/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:38.965722 shadowsocks_manager-0.1.2/shadowsocks_manager/domain/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/domain/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/domain/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:38.965722 shadowsocks_manager-0.1.2/shadowsocks_manager/domain/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/domain/fixtures/nameserver.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:38.965722 shadowsocks_manager-0.1.2/shadowsocks_manager/domain/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/domain/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8241 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/domain/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/domain/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3926 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/domain/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/domain/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/domain/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:38.965722 shadowsocks_manager-0.1.2/shadowsocks_manager/dynamicmethod/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/dynamicmethod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/dynamicmethod/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/dynamicmethod/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:38.965722 shadowsocks_manager-0.1.2/shadowsocks_manager/dynamicmethod/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/dynamicmethod/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/dynamicmethod/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/dynamicmethod/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/dynamicmethod/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:38.965722 shadowsocks_manager-0.1.2/shadowsocks_manager/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/fixtures/auth.group.json
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/fixtures/django_celery_beat.crontabschedule.json
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/fixtures/django_celery_beat.intervalschedule.json
--rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/fixtures/django_celery_beat.periodictask.json
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/fixtures/sites.site.json
--rwxr-xr-x   0 runner    (1001) docker     (127)      940 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:38.965722 shadowsocks_manager-0.1.2/shadowsocks_manager/notification/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/notification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/notification/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/notification/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:38.969722 shadowsocks_manager-0.1.2/shadowsocks_manager/notification/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/notification/fixtures/template.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:38.969722 shadowsocks_manager-0.1.2/shadowsocks_manager/notification/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/notification/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/notification/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/notification/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/notification/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/notification/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/notification/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:38.969722 shadowsocks_manager-0.1.2/shadowsocks_manager/retry/
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/retry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/retry/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:38.969722 shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocks_manager/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocks_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocks_manager/celery.py
--rw-r--r--   0 runner    (1001) docker     (127)     5771 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocks_manager/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocks_manager/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocks_manager/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:38.969722 shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocksz/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocksz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6335 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocksz/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocksz/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:38.969722 shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocksz/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocksz/fixtures/config.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:38.969722 shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocksz/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocksz/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:38.969722 shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocksz/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocksz/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocksz/management/commands/shadowsocks_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:38.969722 shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocksz/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocksz/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36547 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocksz/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocksz/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocksz/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)    19241 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocksz/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocksz/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocksz/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:38.973722 shadowsocks_manager-0.1.2/shadowsocks_manager/singleton/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/singleton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/singleton/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/singleton/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:38.973722 shadowsocks_manager-0.1.2/shadowsocks_manager/singleton/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/singleton/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/singleton/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/singleton/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/singleton/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:38.973722 shadowsocks_manager-0.1.2/shadowsocks_manager/statistic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/statistic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/statistic/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/statistic/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:38.973722 shadowsocks_manager-0.1.2/shadowsocks_manager/statistic/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/statistic/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10309 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/statistic/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/statistic/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/statistic/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/statistic/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/statistic/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/statistic/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:38.973722 shadowsocks_manager-0.1.2/shadowsocks_manager/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/utils/celery.py
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/utils/createsuperuser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/utils/dotenv.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/utils/manage.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-26 19:19:23.000000 shadowsocks_manager-0.1.2/shadowsocks_manager/utils/uwsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:19:38.973722 shadowsocks_manager-0.1.2/shadowsocks_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19905 2024-04-26 19:19:38.000000 shadowsocks_manager-0.1.2/shadowsocks_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3993 2024-04-26 19:19:38.000000 shadowsocks_manager-0.1.2/shadowsocks_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 19:19:38.000000 shadowsocks_manager-0.1.2/shadowsocks_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-26 19:19:38.000000 shadowsocks_manager-0.1.2/shadowsocks_manager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-26 19:19:38.000000 shadowsocks_manager-0.1.2/shadowsocks_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-26 19:19:38.000000 shadowsocks_manager-0.1.2/shadowsocks_manager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:28.832147 shadowsocks_manager-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    19905 2024-04-26 20:03:28.832147 shadowsocks_manager-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15475 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:28.816147 shadowsocks_manager-0.1.3/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/bin/ssm-dev-start
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/bin/ssm-dev-stop
+-rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/bin/ssm-setup
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/bin/ssm-test
+-rw-r--r--   0 runner    (1001) docker     (127)     6183 2024-04-26 20:03:25.000000 shadowsocks_manager-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-04-26 20:03:28.832147 shadowsocks_manager-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:28.820147 shadowsocks_manager-0.1.3/shadowsocks_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/.env
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:28.820147 shadowsocks_manager-0.1.3/shadowsocks_manager/args_formatter/
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/args_formatter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/args_formatter/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:28.820147 shadowsocks_manager-0.1.3/shadowsocks_manager/domain/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/domain/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/domain/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:28.820147 shadowsocks_manager-0.1.3/shadowsocks_manager/domain/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/domain/fixtures/nameserver.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:28.820147 shadowsocks_manager-0.1.3/shadowsocks_manager/domain/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/domain/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8241 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/domain/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/domain/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3926 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/domain/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/domain/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/domain/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:28.820147 shadowsocks_manager-0.1.3/shadowsocks_manager/dynamicmethod/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/dynamicmethod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/dynamicmethod/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/dynamicmethod/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:28.824147 shadowsocks_manager-0.1.3/shadowsocks_manager/dynamicmethod/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/dynamicmethod/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/dynamicmethod/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/dynamicmethod/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/dynamicmethod/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:28.824147 shadowsocks_manager-0.1.3/shadowsocks_manager/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/fixtures/auth.group.json
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/fixtures/django_celery_beat.crontabschedule.json
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/fixtures/django_celery_beat.intervalschedule.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/fixtures/django_celery_beat.periodictask.json
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/fixtures/sites.site.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)      940 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:28.824147 shadowsocks_manager-0.1.3/shadowsocks_manager/notification/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/notification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/notification/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/notification/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:28.824147 shadowsocks_manager-0.1.3/shadowsocks_manager/notification/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/notification/fixtures/template.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:28.824147 shadowsocks_manager-0.1.3/shadowsocks_manager/notification/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/notification/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/notification/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/notification/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/notification/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/notification/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/notification/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:28.824147 shadowsocks_manager-0.1.3/shadowsocks_manager/retry/
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/retry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/retry/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:28.824147 shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocks_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocks_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocks_manager/celery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5771 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocks_manager/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocks_manager/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocks_manager/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:28.828147 shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocksz/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocksz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6335 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocksz/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocksz/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:28.828147 shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocksz/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocksz/fixtures/config.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:28.828147 shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocksz/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocksz/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:28.828147 shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocksz/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocksz/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocksz/management/commands/shadowsocks_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:28.828147 shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocksz/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocksz/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36547 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocksz/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocksz/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocksz/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19241 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocksz/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocksz/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocksz/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:28.828147 shadowsocks_manager-0.1.3/shadowsocks_manager/singleton/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/singleton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/singleton/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/singleton/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:28.828147 shadowsocks_manager-0.1.3/shadowsocks_manager/singleton/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/singleton/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/singleton/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/singleton/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/singleton/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:28.832147 shadowsocks_manager-0.1.3/shadowsocks_manager/statistic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/statistic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/statistic/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/statistic/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:28.832147 shadowsocks_manager-0.1.3/shadowsocks_manager/statistic/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/statistic/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10309 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/statistic/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/statistic/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/statistic/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/statistic/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/statistic/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/statistic/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:28.832147 shadowsocks_manager-0.1.3/shadowsocks_manager/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/utils/celery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/utils/createsuperuser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/utils/dotenv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/utils/manage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/utils/uwsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:28.832147 shadowsocks_manager-0.1.3/shadowsocks_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19905 2024-04-26 20:03:28.000000 shadowsocks_manager-0.1.3/shadowsocks_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3993 2024-04-26 20:03:28.000000 shadowsocks_manager-0.1.3/shadowsocks_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 20:03:28.000000 shadowsocks_manager-0.1.3/shadowsocks_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-26 20:03:28.000000 shadowsocks_manager-0.1.3/shadowsocks_manager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-26 20:03:28.000000 shadowsocks_manager-0.1.3/shadowsocks_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-26 20:03:28.000000 shadowsocks_manager-0.1.3/shadowsocks_manager.egg-info/top_level.txt
```

### Comparing `shadowsocks_manager-0.1.2/LICENSE` & `shadowsocks_manager-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.2/PKG-INFO` & `shadowsocks_manager-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shadowsocks-manager
-Version: 0.1.2
+Version: 0.1.3
 Summary: A shadowsocks manager for multi-user and traffic statistics
 Home-page: https://github.com/alexzhangs/shadowsocks-manager
 Author: Alex
 Author-email: Alex <alexzhangs@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Alex Zhang
```

### Comparing `shadowsocks_manager-0.1.2/README.md` & `shadowsocks_manager-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.2/bin/ssm-dev-start` & `shadowsocks_manager-0.1.3/bin/ssm-dev-start`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.2/bin/ssm-setup` & `shadowsocks_manager-0.1.3/bin/ssm-setup`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.2/bin/ssm-test` & `shadowsocks_manager-0.1.3/bin/ssm-test`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.2/pyproject.toml` & `shadowsocks_manager-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "shadowsocks-manager"
-version = "0.1.2"
+version = "0.1.3"
 requires-python = ">=2.7"
 dependencies = [
     "future",
     "six",
     "boto3",
     "celery",
     "Django<4",
@@ -135,15 +135,15 @@
 [tool.setuptools.package-data]
 shadowsocks_manager = ["fixtures/*", "**/fixtures/*", ".env"]
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 [tool.bumpversion]
-current_version = "0.1.2"
+current_version = "0.1.3"
 parse = """
     (?P<major>\\d+)\\.
     (?P<minor>\\d+)\\.
     (?P<patch>\\d+)
     (
         \\-                         # separator
         (?P<suffix>[0-9]\\d*)       # suffix Number
@@ -156,15 +156,15 @@
 search = "{current_version}"
 replace = "{new_version}"
 regex = false
 ignore_missing_version = false
 ignore_missing_files = false
 tag = true
 sign_tags = false
-tag_name = "pypi-{new_version}"
+tag_name = "{new_version}"
 tag_message = "Bump version: {current_version} → {new_version}"
 allow_dirty = true
 commit = true
 message = "Bump version: {current_version} → {new_version}"
 commit_args = "--no-verify"
 
 [[tool.bumpversion.files]]
```

### Comparing `shadowsocks_manager-0.1.2/setup.cfg` & `shadowsocks_manager-0.1.3/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = shadowsocks-manager
-version = 0.1.2
+version = 0.1.3
 description = A shadowsocks manager for multi-user and traffic statistics
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Alex
 author_email = alexzhangs@gmail.com
 url = https://github.com/alexzhangs/shadowsocks-manager
 license = MIT
```

### Comparing `shadowsocks_manager-0.1.2/shadowsocks_manager/__main__.py` & `shadowsocks_manager-0.1.3/shadowsocks_manager/__main__.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.2/shadowsocks_manager/args_formatter/__init__.py` & `shadowsocks_manager-0.1.3/shadowsocks_manager/args_formatter/__init__.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.2/shadowsocks_manager/args_formatter/tests.py` & `shadowsocks_manager-0.1.3/shadowsocks_manager/args_formatter/tests.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.2/shadowsocks_manager/domain/admin.py` & `shadowsocks_manager-0.1.3/shadowsocks_manager/domain/admin.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.2/shadowsocks_manager/domain/models.py` & `shadowsocks_manager-0.1.3/shadowsocks_manager/domain/models.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.2/shadowsocks_manager/domain/serializers.py` & `shadowsocks_manager-0.1.3/shadowsocks_manager/domain/serializers.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.2/shadowsocks_manager/domain/tests.py` & `shadowsocks_manager-0.1.3/shadowsocks_manager/domain/tests.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.2/shadowsocks_manager/domain/views.py` & `shadowsocks_manager-0.1.3/shadowsocks_manager/domain/views.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.2/shadowsocks_manager/dynamicmethod/models.py` & `shadowsocks_manager-0.1.3/shadowsocks_manager/dynamicmethod/models.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.2/shadowsocks_manager/fixtures/django_celery_beat.crontabschedule.json` & `shadowsocks_manager-0.1.3/shadowsocks_manager/fixtures/django_celery_beat.crontabschedule.json`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.2/shadowsocks_manager/fixtures/django_celery_beat.periodictask.json` & `shadowsocks_manager-0.1.3/shadowsocks_manager/fixtures/django_celery_beat.periodictask.json`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.2/shadowsocks_manager/manage.py` & `shadowsocks_manager-0.1.3/shadowsocks_manager/manage.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.2/shadowsocks_manager/notification/fixtures/template.json` & `shadowsocks_manager-0.1.3/shadowsocks_manager/notification/fixtures/template.json`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.2/shadowsocks_manager/notification/models.py` & `shadowsocks_manager-0.1.3/shadowsocks_manager/notification/models.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.2/shadowsocks_manager/notification/tests.py` & `shadowsocks_manager-0.1.3/shadowsocks_manager/notification/tests.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.2/shadowsocks_manager/retry/__init__.py` & `shadowsocks_manager-0.1.3/shadowsocks_manager/retry/__init__.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.2/shadowsocks_manager/retry/tests.py` & `shadowsocks_manager-0.1.3/shadowsocks_manager/retry/tests.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocks_manager/celery.py` & `shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocks_manager/celery.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocks_manager/settings.py` & `shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocks_manager/settings.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocks_manager/urls.py` & `shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocks_manager/urls.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocksz/admin.py` & `shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocksz/admin.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocksz/management/commands/shadowsocks_config.py` & `shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocksz/management/commands/shadowsocks_config.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocksz/models.py` & `shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocksz/models.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocksz/serializers.py` & `shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocksz/serializers.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocksz/tests.py` & `shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocksz/tests.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocksz/urls.py` & `shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocksz/urls.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.2/shadowsocks_manager/shadowsocksz/views.py` & `shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocksz/views.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.2/shadowsocks_manager/singleton/models.py` & `shadowsocks_manager-0.1.3/shadowsocks_manager/singleton/models.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.2/shadowsocks_manager/statistic/admin.py` & `shadowsocks_manager-0.1.3/shadowsocks_manager/statistic/admin.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.2/shadowsocks_manager/statistic/models.py` & `shadowsocks_manager-0.1.3/shadowsocks_manager/statistic/models.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.2/shadowsocks_manager/statistic/serializers.py` & `shadowsocks_manager-0.1.3/shadowsocks_manager/statistic/serializers.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.2/shadowsocks_manager/statistic/tests.py` & `shadowsocks_manager-0.1.3/shadowsocks_manager/statistic/tests.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.2/shadowsocks_manager/statistic/views.py` & `shadowsocks_manager-0.1.3/shadowsocks_manager/statistic/views.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.2/shadowsocks_manager/utils/celery.py` & `shadowsocks_manager-0.1.3/shadowsocks_manager/utils/celery.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.2/shadowsocks_manager/utils/createsuperuser.py` & `shadowsocks_manager-0.1.3/shadowsocks_manager/utils/createsuperuser.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.2/shadowsocks_manager/utils/dotenv.py` & `shadowsocks_manager-0.1.3/shadowsocks_manager/utils/dotenv.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.2/shadowsocks_manager/utils/manage.py` & `shadowsocks_manager-0.1.3/shadowsocks_manager/utils/manage.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.2/shadowsocks_manager.egg-info/PKG-INFO` & `shadowsocks_manager-0.1.3/shadowsocks_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shadowsocks-manager
-Version: 0.1.2
+Version: 0.1.3
 Summary: A shadowsocks manager for multi-user and traffic statistics
 Home-page: https://github.com/alexzhangs/shadowsocks-manager
 Author: Alex
 Author-email: Alex <alexzhangs@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Alex Zhang
```

### Comparing `shadowsocks_manager-0.1.2/shadowsocks_manager.egg-info/SOURCES.txt` & `shadowsocks_manager-0.1.3/shadowsocks_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.2/shadowsocks_manager.egg-info/requires.txt` & `shadowsocks_manager-0.1.3/shadowsocks_manager.egg-info/requires.txt`

 * *Files identical despite different names*

