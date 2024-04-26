# Comparing `tmp/edumfa-2.0.1.tar.gz` & `tmp/edumfa-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edumfa-2.0.1.tar", last modified: Fri Apr 12 11:16:16 2024, max compression
+gzip compressed data, was "edumfa-2.0.2.tar", last modified: Fri Apr 26 10:25:15 2024, max compression
```

## Comparing `edumfa-2.0.1.tar` & `edumfa-2.0.2.tar`

### file list

```diff
@@ -1,1013 +1,1013 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.099623 edumfa-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     8120 2024-04-12 11:16:12.000000 edumfa-2.0.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)    32387 2024-04-12 11:16:12.000000 edumfa-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-12 11:16:12.000000 edumfa-2.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8588 2024-04-12 11:16:16.099623 edumfa-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-04-12 11:16:12.000000 edumfa-2.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.947622 edumfa-2.0.1/deploy/
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-12 11:16:12.000000 edumfa-2.0.1/deploy/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.947622 edumfa-2.0.1/deploy/apache/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-12 11:16:12.000000 edumfa-2.0.1/deploy/apache/edumfaapp.wsgi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.947622 edumfa-2.0.1/deploy/apache/sites-available/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-12 11:16:12.000000 edumfa-2.0.1/deploy/apache/sites-available/edumfa-venv.conf
--rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-04-12 11:16:12.000000 edumfa-2.0.1/deploy/apache/sites-available/edumfa.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.927622 edumfa-2.0.1/deploy/config/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.947622 edumfa-2.0.1/deploy/config/freeradius2/
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-12 11:16:12.000000 edumfa-2.0.1/deploy/config/freeradius2/edumfa
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-12 11:16:12.000000 edumfa-2.0.1/deploy/config/freeradius2/mods-perl-edumfa
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.947622 edumfa-2.0.1/deploy/config/freeradius3/
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-12 11:16:12.000000 edumfa-2.0.1/deploy/config/freeradius3/edumfa
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-12 11:16:12.000000 edumfa-2.0.1/deploy/config/freeradius3/mods-perl-edumfa
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.947622 edumfa-2.0.1/deploy/crontab/
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-12 11:16:12.000000 edumfa-2.0.1/deploy/crontab/edumfa
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-12 11:16:12.000000 edumfa-2.0.1/deploy/docker-compose-example.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.951622 edumfa-2.0.1/deploy/docker-example/
--rw-r--r--   0 runner    (1001) docker     (127)     6424 2024-04-12 11:16:12.000000 edumfa-2.0.1/deploy/docker-example/edumfa-policy.conf
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-12 11:16:12.000000 edumfa-2.0.1/deploy/docker-example/edumfa-setup.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-12 11:16:12.000000 edumfa-2.0.1/deploy/docker-example/edumfa.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      726 2024-04-12 11:16:12.000000 edumfa-2.0.1/deploy/docker-setup.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.951622 edumfa-2.0.1/deploy/edumfa/
--rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-04-12 11:16:12.000000 edumfa-2.0.1/deploy/edumfa/dictionary
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-12 11:16:12.000000 edumfa-2.0.1/deploy/edumfa/edumfa.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    21848 2024-04-12 11:16:12.000000 edumfa-2.0.1/deploy/edumfa_radius.pm
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.951622 edumfa-2.0.1/deploy/gunicorn/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-12 11:16:12.000000 edumfa-2.0.1/deploy/gunicorn/edumfaapp.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-12 11:16:12.000000 edumfa-2.0.1/deploy/logging.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.951622 edumfa-2.0.1/deploy/nginx/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-12 11:16:12.000000 edumfa-2.0.1/deploy/nginx/edumfaapp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.951622 edumfa-2.0.1/deploy/nginx/sites-available/
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-12 11:16:12.000000 edumfa-2.0.1/deploy/nginx/sites-available/edumfa
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-12 11:16:12.000000 edumfa-2.0.1/deploy/rlm_perl.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.951622 edumfa-2.0.1/deploy/ubuntu/
--rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-04-12 11:16:12.000000 edumfa-2.0.1/deploy/ubuntu/changelog
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-12 11:16:12.000000 edumfa-2.0.1/deploy/ubuntu/clean
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-12 11:16:12.000000 edumfa-2.0.1/deploy/ubuntu/compat
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-12 11:16:12.000000 edumfa-2.0.1/deploy/ubuntu/control
--rw-r--r--   0 runner    (1001) docker     (127)    32387 2024-04-12 11:16:12.000000 edumfa-2.0.1/deploy/ubuntu/copyright
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-12 11:16:12.000000 edumfa-2.0.1/deploy/ubuntu/rules
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.955622 edumfa-2.0.1/deploy/ubuntu/source/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-12 11:16:12.000000 edumfa-2.0.1/deploy/ubuntu/source/format
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-12 11:16:12.000000 edumfa-2.0.1/deploy/ubuntu/source/options
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.951622 edumfa-2.0.1/deploy/ubuntu-radius/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-12 11:16:12.000000 edumfa-2.0.1/deploy/ubuntu-radius/changelog
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-12 11:16:12.000000 edumfa-2.0.1/deploy/ubuntu-radius/compat
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-12 11:16:12.000000 edumfa-2.0.1/deploy/ubuntu-radius/control
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-12 11:16:12.000000 edumfa-2.0.1/deploy/ubuntu-radius/copyright
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-12 11:16:12.000000 edumfa-2.0.1/deploy/ubuntu-radius/edumfa-radius.install
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-12 11:16:12.000000 edumfa-2.0.1/deploy/ubuntu-radius/edumfa-radius.postinst
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-12 11:16:12.000000 edumfa-2.0.1/deploy/ubuntu-radius/edumfa-radius.postrm
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-12 11:16:12.000000 edumfa-2.0.1/deploy/ubuntu-radius/rules
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.951622 edumfa-2.0.1/deploy/ubuntu-radius/source/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-12 11:16:12.000000 edumfa-2.0.1/deploy/ubuntu-radius/source/format
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.955622 edumfa-2.0.1/deploy/ubuntu-server/
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-12 11:16:12.000000 edumfa-2.0.1/deploy/ubuntu-server/changelog
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-12 11:16:12.000000 edumfa-2.0.1/deploy/ubuntu-server/clean
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-12 11:16:12.000000 edumfa-2.0.1/deploy/ubuntu-server/compat
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-12 11:16:12.000000 edumfa-2.0.1/deploy/ubuntu-server/control
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-12 11:16:12.000000 edumfa-2.0.1/deploy/ubuntu-server/edumfa-apache2.install
--rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-04-12 11:16:12.000000 edumfa-2.0.1/deploy/ubuntu-server/edumfa-apache2.postinst
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-12 11:16:12.000000 edumfa-2.0.1/deploy/ubuntu-server/edumfa-apache2.postrm
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-12 11:16:12.000000 edumfa-2.0.1/deploy/ubuntu-server/edumfa-nginx.install
--rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-04-12 11:16:12.000000 edumfa-2.0.1/deploy/ubuntu-server/edumfa-nginx.postinst
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-12 11:16:12.000000 edumfa-2.0.1/deploy/ubuntu-server/edumfa-nginx.postrm
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-12 11:16:12.000000 edumfa-2.0.1/deploy/ubuntu-server/rules
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.955622 edumfa-2.0.1/deploy/ubuntu-server/source/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-12 11:16:12.000000 edumfa-2.0.1/deploy/ubuntu-server/source/format
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-12 11:16:12.000000 edumfa-2.0.1/deploy/ubuntu-server/source/options
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.931622 edumfa-2.0.1/deploy/uwsgi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.955622 edumfa-2.0.1/deploy/uwsgi/apps-available/
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-12 11:16:12.000000 edumfa-2.0.1/deploy/uwsgi/apps-available/edumfa.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.955622 edumfa-2.0.1/doc/
--rw-r--r--   0 runner    (1001) docker     (127)     9459 2024-04-12 11:16:12.000000 edumfa-2.0.1/doc/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.955622 edumfa-2.0.1/edumfa/
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.963622 edumfa-2.0.1/edumfa/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/api/application.py
--rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/api/audit.py
--rw-r--r--   0 runner    (1001) docker     (127)    18346 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/api/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    16376 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/api/before_after.py
--rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/api/caconnector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/api/clienttype.py
--rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/api/edumfaserver.py
--rw-r--r--   0 runner    (1001) docker     (127)     7416 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/api/event.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.963622 edumfa-2.0.1/edumfa/api/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/api/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/api/lib/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/api/lib/policyhelper.py
--rw-r--r--   0 runner    (1001) docker     (127)    41925 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/api/lib/postpolicy.py
--rw-r--r--   0 runner    (1001) docker     (127)   101628 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/api/lib/prepolicy.py
--rw-r--r--   0 runner    (1001) docker     (127)    17919 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/api/lib/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15527 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/api/machine.py
--rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/api/machineresolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/api/monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     7937 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/api/periodictask.py
--rw-r--r--   0 runner    (1001) docker     (127)    18770 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/api/policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5065 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/api/radiusserver.py
--rw-r--r--   0 runner    (1001) docker     (127)    10790 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/api/realm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3436 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/api/recover.py
--rw-r--r--   0 runner    (1001) docker     (127)     7117 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/api/register.py
--rw-r--r--   0 runner    (1001) docker     (127)     6730 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/api/resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     5232 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/api/serviceid.py
--rw-r--r--   0 runner    (1001) docker     (127)     5462 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/api/smsgateway.py
--rw-r--r--   0 runner    (1001) docker     (127)     5678 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/api/smtpserver.py
--rw-r--r--   0 runner    (1001) docker     (127)    12631 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/api/system.py
--rw-r--r--   0 runner    (1001) docker     (127)    55749 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/api/token.py
--rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/api/tokengroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/api/ttype.py
--rw-r--r--   0 runner    (1001) docker     (127)    12293 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/api/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    29126 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/api/validate.py
--rw-r--r--   0 runner    (1001) docker     (127)    10347 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/app.py
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/babel.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.963622 edumfa-2.0.1/edumfa/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.967622 edumfa-2.0.1/edumfa/commands/manage/
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/commands/manage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/commands/manage/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/commands/manage/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7876 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/commands/manage/audit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/commands/manage/authcache.py
--rw-r--r--   0 runner    (1001) docker     (127)     7905 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/commands/manage/backup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/commands/manage/ca.py
--rw-r--r--   0 runner    (1001) docker     (127)     8434 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/commands/manage/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9125 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/commands/manage/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/commands/manage/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     8604 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/commands/manage/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/commands/manage/hsm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/commands/manage/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     6113 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/commands/manage/policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/commands/manage/realm.py
--rw-r--r--   0 runner    (1001) docker     (127)     7407 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/commands/manage/resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/commands/manage/token.py
--rw-r--r--   0 runner    (1001) docker     (127)     6727 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.971622 edumfa-2.0.1/edumfa/lib/
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.975622 edumfa-2.0.1/edumfa/lib/applications/
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5830 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/applications/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/applications/luks.py
--rw-r--r--   0 runner    (1001) docker     (127)     8071 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/applications/offline.py
--rw-r--r--   0 runner    (1001) docker     (127)     4624 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/applications/ssh.py
--rw-r--r--   0 runner    (1001) docker     (127)     7274 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/audit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.975622 edumfa-2.0.1/edumfa/lib/auditmodules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/auditmodules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8769 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/auditmodules/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4803 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/auditmodules/containeraudit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/auditmodules/loggeraudit.py
--rw-r--r--   0 runner    (1001) docker     (127)    26334 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/auditmodules/sqlaudit.py
--rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     6116 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/authcache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.975622 edumfa-2.0.1/edumfa/lib/cache/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11818 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/caconnector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.975622 edumfa-2.0.1/edumfa/lib/caconnectors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/caconnectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5415 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/caconnectors/baseca.py
--rw-r--r--   0 runner    (1001) docker     (127)    10664 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/caconnectors/caservice_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    11729 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/caconnectors/caservice_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    27145 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/caconnectors/localca.py
--rw-r--r--   0 runner    (1001) docker     (127)    17292 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/caconnectors/msca.py
--rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/challenge.py
--rw-r--r--   0 runner    (1001) docker     (127)     9658 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/challengeresponsedecorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     4216 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/clientapplication.py
--rw-r--r--   0 runner    (1001) docker     (127)    37215 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/counter.py
--rw-r--r--   0 runner    (1001) docker     (127)    28674 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/crypto.py
--rw-r--r--   0 runner    (1001) docker     (127)     5180 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     8921 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/edumfaserver.py
--rw-r--r--   0 runner    (1001) docker     (127)     6314 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/error.py
--rw-r--r--   0 runner    (1001) docker     (127)    13496 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/event.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.979622 edumfa-2.0.1/edumfa/lib/eventhandler/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/eventhandler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24840 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/eventhandler/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/eventhandler/counterhandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/eventhandler/customuserattributeshandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     7332 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/eventhandler/federationhandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     6358 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/eventhandler/logginghandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     7509 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/eventhandler/requestmangler.py
--rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/eventhandler/responsemangler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8919 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/eventhandler/scripthandler.py
--rw-r--r--   0 runner    (1001) docker     (127)    30653 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/eventhandler/tokenhandler.py
--rw-r--r--   0 runner    (1001) docker     (127)    21561 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/eventhandler/usernotification.py
--rw-r--r--   0 runner    (1001) docker     (127)     6898 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/eventhandler/webhookeventhandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/framework.py
--rw-r--r--   0 runner    (1001) docker     (127)    29337 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/importotp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/lifecycle.py
--rw-r--r--   0 runner    (1001) docker     (127)     7419 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/log.py
--rw-r--r--   0 runner    (1001) docker     (127)    19552 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/machine.py
--rw-r--r--   0 runner    (1001) docker     (127)    11009 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/machineresolver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.979622 edumfa-2.0.1/edumfa/lib/machines/
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/machines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5809 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/machines/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5828 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/machines/hosts.py
--rw-r--r--   0 runner    (1001) docker     (127)    14366 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/machines/ldap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.979622 edumfa-2.0.1/edumfa/lib/monitoringmodules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/monitoringmodules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/monitoringmodules/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7803 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/monitoringmodules/sqlstats.py
--rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/monitoringstats.py
--rw-r--r--   0 runner    (1001) docker     (127)     5598 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/passwordreset.py
--rw-r--r--   0 runner    (1001) docker     (127)    12715 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/periodictask.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.979622 edumfa-2.0.1/edumfa/lib/pinhandling/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/pinhandling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/pinhandling/base.py
--rw-r--r--   0 runner    (1001) docker     (127)   146757 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    28842 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/policydecorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     5010 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/pooling.py
--rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/queue.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.979622 edumfa-2.0.1/edumfa/lib/queues/
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/queues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/queues/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/queues/huey_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/radiusserver.py
--rw-r--r--   0 runner    (1001) docker     (127)     8015 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/realm.py
--rw-r--r--   0 runner    (1001) docker     (127)    14818 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.979622 edumfa-2.0.1/edumfa/lib/resolvers/
--rw-r--r--   0 runner    (1001) docker     (127)     7221 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/resolvers/HTTPResolver.py
--rw-r--r--   0 runner    (1001) docker     (127)    56725 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/resolvers/LDAPIdResolver.py
--rw-r--r--   0 runner    (1001) docker     (127)    15166 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/resolvers/PasswdIdResolver.py
--rw-r--r--   0 runner    (1001) docker     (127)    10885 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/resolvers/SCIMIdResolver.py
--rw-r--r--   0 runner    (1001) docker     (127)    28267 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/resolvers/SQLIdResolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     8590 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/resolvers/UserIdResolver.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/resolvers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.983622 edumfa-2.0.1/edumfa/lib/security/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13784 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/security/aeshsm.py
--rw-r--r--   0 runner    (1001) docker     (127)    16464 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/security/default.py
--rw-r--r--   0 runner    (1001) docker     (127)    14478 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/security/encryptkey.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.983622 edumfa-2.0.1/edumfa/lib/security/password/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/security/password/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/serviceid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.983622 edumfa-2.0.1/edumfa/lib/smsprovider/
--rw-r--r--   0 runner    (1001) docker     (127)     9043 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/smsprovider/FirebaseProvider.py
--rw-r--r--   0 runner    (1001) docker     (127)    11897 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/smsprovider/HttpMessageToUidProvider.py
--rw-r--r--   0 runner    (1001) docker     (127)    12084 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/smsprovider/HttpSMSProvider.py
--rw-r--r--   0 runner    (1001) docker     (127)    12565 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/smsprovider/SMSProvider.py
--rw-r--r--   0 runner    (1001) docker     (127)     5560 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/smsprovider/ScriptSMSProvider.py
--rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/smsprovider/SipgateSMSProvider.py
--rw-r--r--   0 runner    (1001) docker     (127)     6344 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/smsprovider/SmppSMSProvider.py
--rw-r--r--   0 runner    (1001) docker     (127)     5552 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/smsprovider/SmtpSMSProvider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/smsprovider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13922 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/smtpserver.py
--rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/sqlutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5206 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/subscriptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.983622 edumfa-2.0.1/edumfa/lib/task/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/task/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/task/eventcounter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/task/simplestats.py
--rw-r--r--   0 runner    (1001) docker     (127)    96840 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/token.py
--rw-r--r--   0 runner    (1001) docker     (127)    68419 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/tokenclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/tokengroup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.991622 edumfa-2.0.1/edumfa/lib/tokens/
--rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/tokens/HMAC.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/tokens/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/tokens/applicationspecificpasswordtoken.py
--rw-r--r--   0 runner    (1001) docker     (127)    25837 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/tokens/certificatetoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     8437 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/tokens/daplugtoken.py
--rw-r--r--   0 runner    (1001) docker     (127)    16746 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/tokens/daypasswordtoken.py
--rw-r--r--   0 runner    (1001) docker     (127)    22719 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/tokens/emailtoken.py
--rw-r--r--   0 runner    (1001) docker     (127)    18983 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/tokens/foureyestoken.py
--rw-r--r--   0 runner    (1001) docker     (127)    33207 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/tokens/hotptoken.py
--rw-r--r--   0 runner    (1001) docker     (127)    15903 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/tokens/indexedsecrettoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/tokens/mOTP.py
--rw-r--r--   0 runner    (1001) docker     (127)     8233 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/tokens/motptoken.py
--rw-r--r--   0 runner    (1001) docker     (127)    14133 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/tokens/ocra.py
--rw-r--r--   0 runner    (1001) docker     (127)    10863 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/tokens/ocratoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     5179 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/tokens/papertoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     6723 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/tokens/passwordtoken.py
--rw-r--r--   0 runner    (1001) docker     (127)    46777 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/tokens/pushtoken.py
--rw-r--r--   0 runner    (1001) docker     (127)    14249 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/tokens/questionnairetoken.py
--rw-r--r--   0 runner    (1001) docker     (127)    22143 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/tokens/radiustoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     5709 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/tokens/registrationtoken.py
--rw-r--r--   0 runner    (1001) docker     (127)    12204 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/tokens/remotetoken.py
--rw-r--r--   0 runner    (1001) docker     (127)    25368 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/tokens/smstoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     5253 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/tokens/spasstoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     5806 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/tokens/sshkeytoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     8130 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/tokens/tantoken.py
--rw-r--r--   0 runner    (1001) docker     (127)    19949 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/tokens/tiqrtoken.py
--rw-r--r--   0 runner    (1001) docker     (127)    27633 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/tokens/totptoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     9775 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/tokens/u2f.py
--rw-r--r--   0 runner    (1001) docker     (127)    23127 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/tokens/u2ftoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/tokens/vasco.py
--rw-r--r--   0 runner    (1001) docker     (127)     7039 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/tokens/vascotoken.py
--rw-r--r--   0 runner    (1001) docker     (127)    89138 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/tokens/webauthn.py
--rw-r--r--   0 runner    (1001) docker     (127)    66757 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/tokens/webauthntoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     8523 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/tokens/yubicotoken.py
--rw-r--r--   0 runner    (1001) docker     (127)    16984 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/tokens/yubikeytoken.py
--rw-r--r--   0 runner    (1001) docker     (127)    30149 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     9668 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/usercache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.991622 edumfa-2.0.1/edumfa/lib/utils/
--rw-r--r--   0 runner    (1001) docker     (127)    55043 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8077 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/utils/compare.py
--rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/lib/utils/export.py
--rw-r--r--   0 runner    (1001) docker     (127)    71279 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/messages.pot
--rw-r--r--   0 runner    (1001) docker     (127)   121706 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.991622 edumfa-2.0.1/edumfa/static/
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     8220 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/app.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.939622 edumfa-2.0.1/edumfa/static/components/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.935622 edumfa-2.0.1/edumfa/static/components/audit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.991622 edumfa-2.0.1/edumfa/static/components/audit/controllers/
--rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/audit/controllers/auditControllers.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.991622 edumfa-2.0.1/edumfa/static/components/audit/factories/
--rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/audit/factories/audit.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.991622 edumfa-2.0.1/edumfa/static/components/audit/states/
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/audit/states/states.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.991622 edumfa-2.0.1/edumfa/static/components/audit/views/
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/audit/views/audit.html
--rw-r--r--   0 runner    (1001) docker     (127)    11055 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/audit/views/audit.log.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.935622 edumfa-2.0.1/edumfa/static/components/components/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.991622 edumfa-2.0.1/edumfa/static/components/components/controllers/
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/components/controllers/componentControllers.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.991622 edumfa-2.0.1/edumfa/static/components/components/factories/
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/components/factories/component.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.991622 edumfa-2.0.1/edumfa/static/components/components/states/
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/components/states/states.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.995622 edumfa-2.0.1/edumfa/static/components/components/views/
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/components/views/component.clienttype.html
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/components/views/component.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.935622 edumfa-2.0.1/edumfa/static/components/config/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.995622 edumfa-2.0.1/edumfa/static/components/config/controllers/
--rw-r--r--   0 runner    (1001) docker     (127)    50570 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/controllers/configControllers.js
--rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/controllers/eduMfaServerController.js
--rw-r--r--   0 runner    (1001) docker     (127)    11316 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/controllers/eventController.js
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/controllers/ldapMachineResolverController.js
--rw-r--r--   0 runner    (1001) docker     (127)     7474 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/controllers/periodicTaskController.js
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/controllers/radiusServerController.js
--rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/controllers/serviceidController.js
--rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/controllers/smsgatewayController.js
--rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/controllers/smtpServerController.js
--rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/controllers/tokengroupController.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.995622 edumfa-2.0.1/edumfa/static/components/config/factories/
--rw-r--r--   0 runner    (1001) docker     (127)    32353 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/factories/config.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.995622 edumfa-2.0.1/edumfa/static/components/config/states/
--rw-r--r--   0 runner    (1001) docker     (127)    19924 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/states/states.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.003622 edumfa-2.0.1/edumfa/static/components/config/views/
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/views/config.caconnectors.list.html
--rw-r--r--   0 runner    (1001) docker     (127)     6518 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/views/config.caconnectors.local.html
--rw-r--r--   0 runner    (1001) docker     (127)     6204 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/views/config.caconnectors.microsoft.html
--rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/views/config.edumfaserver.edit.html
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/views/config.edumfaserver.list.html
--rw-r--r--   0 runner    (1001) docker     (127)    15020 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/views/config.events.details.html
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/views/config.events.html
--rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/views/config.events.list.html
--rw-r--r--   0 runner    (1001) docker     (127)     4497 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/views/config.html
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/views/config.machineresolvers.html
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/views/config.mresolvers.hosts.html
--rw-r--r--   0 runner    (1001) docker     (127)     8217 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/views/config.mresolvers.ldap.html
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/views/config.mresolvers.list.html
--rw-r--r--   0 runner    (1001) docker     (127)     7503 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/views/config.periodictasks.details.html
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/views/config.periodictasks.html
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/views/config.periodictasks.list.html
--rw-r--r--   0 runner    (1001) docker     (127)    22234 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/views/config.policies.details.html
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/views/config.policies.html
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/views/config.policies.list.html
--rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/views/config.radius.edit.html
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/views/config.radius.list.html
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/views/config.realms.html
--rw-r--r--   0 runner    (1001) docker     (127)     6002 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/views/config.realms.list.html
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/views/config.resolvers.html
--rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/views/config.resolvers.http.html
--rw-r--r--   0 runner    (1001) docker     (127)    14914 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/views/config.resolvers.ldap.html
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/views/config.resolvers.list.html
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/views/config.resolvers.passwd.html
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/views/config.resolvers.scim.html
--rw-r--r--   0 runner    (1001) docker     (127)    10128 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/views/config.resolvers.sql.html
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/views/config.serviceid.edit.html
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/views/config.serviceid.list.html
--rw-r--r--   0 runner    (1001) docker     (127)     5797 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/views/config.smsgateway.edit.html
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/views/config.smsgateway.list.html
--rw-r--r--   0 runner    (1001) docker     (127)     5506 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/views/config.smtp.edit.html
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/views/config.smtp.list.html
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/views/config.system.doc.html
--rw-r--r--   0 runner    (1001) docker     (127)     8912 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/views/config.system.edit.html
--rw-r--r--   0 runner    (1001) docker     (127)    13600 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/views/config.system.html
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/views/config.token.daypassword.html
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/views/config.token.email.html
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/views/config.token.hotp.html
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/views/config.token.question.html
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/views/config.token.radius.html
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/views/config.token.remote.html
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/views/config.token.sms.html
--rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/views/config.token.tiqr.html
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/views/config.token.totp.html
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/views/config.token.u2f.html
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/views/config.token.webauthn.html
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/views/config.token.yubico.html
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/views/config.token.yubikey.html
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/views/config.tokengroup.edit.html
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/views/config.tokengroup.list.html
--rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/views/config.tokens.html
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/config/views/dialog.confirm_delete.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.935622 edumfa-2.0.1/edumfa/static/components/dashboard/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.007623 edumfa-2.0.1/edumfa/static/components/dashboard/controllers/
--rw-r--r--   0 runner    (1001) docker     (127)     8518 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/dashboard/controllers/dashboardControllers.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.007623 edumfa-2.0.1/edumfa/static/components/dashboard/states/
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/dashboard/states/states.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.007623 edumfa-2.0.1/edumfa/static/components/dashboard/views/
--rw-r--r--   0 runner    (1001) docker     (127)     8881 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/dashboard/views/dashboard.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.935622 edumfa-2.0.1/edumfa/static/components/dialogs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.007623 edumfa-2.0.1/edumfa/static/components/dialogs/views/
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/dialogs/views/dialog.about.html
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/dialogs/views/dialog.autocreate_realm.html
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/dialogs/views/dialog.lock.html
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/dialogs/views/dialog.no.token.html
--rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/dialogs/views/dialog.welcome.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.935622 edumfa-2.0.1/edumfa/static/components/directives/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.007623 edumfa-2.0.1/edumfa/static/components/directives/controllers/
--rw-r--r--   0 runner    (1001) docker     (127)    19746 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/directives/controllers/directives.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.007623 edumfa-2.0.1/edumfa/static/components/directives/views/
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/directives/views/directive.assigntoken.html
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/directives/views/directive.assignuser.html
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/directives/views/directive.attachmachine.html
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/directives/views/directive.attachtoken.html
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/directives/views/directive.csvdownload.html
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/directives/views/directive.filter.table.html
--rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/directives/views/directive.policyconditions.html
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/directives/views/directive.tokendata.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.007623 edumfa-2.0.1/edumfa/static/components/filters/
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/filters/filters.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.935622 edumfa-2.0.1/edumfa/static/components/login/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.007623 edumfa-2.0.1/edumfa/static/components/login/controllers/
--rw-r--r--   0 runner    (1001) docker     (127)    30344 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/login/controllers/loginControllers.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.007623 edumfa-2.0.1/edumfa/static/components/login/factories/
--rw-r--r--   0 runner    (1001) docker     (127)     5789 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/login/factories/auth.js
--rw-r--r--   0 runner    (1001) docker     (127)     5225 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/login/factories/u2f.js
--rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/login/factories/webauthn.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.011623 edumfa-2.0.1/edumfa/static/components/login/states/
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/login/states/states.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.011623 edumfa-2.0.1/edumfa/static/components/login/views/
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/login/views/enter-response.html
--rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/login/views/login.html
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/login/views/offline.html
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/login/views/pinchange.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.939622 edumfa-2.0.1/edumfa/static/components/machine/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.011623 edumfa-2.0.1/edumfa/static/components/machine/controllers/
--rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/machine/controllers/machineController.js
--rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/machine/controllers/machineDetailsController.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.011623 edumfa-2.0.1/edumfa/static/components/machine/factories/
--rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/machine/factories/machine.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.011623 edumfa-2.0.1/edumfa/static/components/machine/states/
--rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/machine/states/states.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.011623 edumfa-2.0.1/edumfa/static/components/machine/views/
--rw-r--r--   0 runner    (1001) docker     (127)     7085 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/machine/views/machine.details.html
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/machine/views/machine.html
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/machine/views/machine.list.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.939622 edumfa-2.0.1/edumfa/static/components/recovery/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.011623 edumfa-2.0.1/edumfa/static/components/recovery/controllers/
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/recovery/controllers/recoveryControllers.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.011623 edumfa-2.0.1/edumfa/static/components/recovery/factories/
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/recovery/factories/recoveryFactory.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.011623 edumfa-2.0.1/edumfa/static/components/recovery/states/
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/recovery/states/states.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.011623 edumfa-2.0.1/edumfa/static/components/recovery/views/
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/recovery/views/recovery.html
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/recovery/views/recovery.reset.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.939622 edumfa-2.0.1/edumfa/static/components/register/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.011623 edumfa-2.0.1/edumfa/static/components/register/controllers/
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/register/controllers/registerControllers.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.011623 edumfa-2.0.1/edumfa/static/components/register/factories/
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/register/factories/registerFactory.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.011623 edumfa-2.0.1/edumfa/static/components/register/states/
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/register/states/states.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.011623 edumfa-2.0.1/edumfa/static/components/register/views/
--rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/register/views/register.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.939622 edumfa-2.0.1/edumfa/static/components/token/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.015622 edumfa-2.0.1/edumfa/static/components/token/controllers/
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/token/controllers/tokenApplicationsController.js
--rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/token/controllers/tokenChallengesController.js
--rw-r--r--   0 runner    (1001) docker     (127)    29864 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/token/controllers/tokenControllers.js
--rw-r--r--   0 runner    (1001) docker     (127)    17169 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/token/controllers/tokenDetailController.js
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/token/controllers/tokenGetSerialController.js
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/token/controllers/tokenLostController.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.015622 edumfa-2.0.1/edumfa/static/components/token/factories/
--rw-r--r--   0 runner    (1001) docker     (127)    12956 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/token/factories/token.js
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/token/factories/validate.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.015622 edumfa-2.0.1/edumfa/static/components/token/states/
--rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/token/states/states.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.023623 edumfa-2.0.1/edumfa/static/components/token/views/
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/token/views/dialog.ask_token_delete.html
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/token/views/token.applications.html
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/token/views/token.applications.offline.html
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/token/views/token.applications.ssh.html
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/token/views/token.assign.html
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/token/views/token.challenges.html
--rw-r--r--   0 runner    (1001) docker     (127)    32395 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/token/views/token.details.html
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/token/views/token.display.apps.html
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/token/views/token.enroll.4eyes.html
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/token/views/token.enroll.applspec.html
--rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/token/views/token.enroll.certificate.html
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/token/views/token.enroll.daypassword.html
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/token/views/token.enroll.email.html
--rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/token/views/token.enroll.hotp.html
--rw-r--r--   0 runner    (1001) docker     (127)    10466 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/token/views/token.enroll.html
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/token/views/token.enroll.indexedsecret.html
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/token/views/token.enroll.motp.html
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/token/views/token.enroll.paper.html
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/token/views/token.enroll.push.html
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/token/views/token.enroll.question.html
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/token/views/token.enroll.radius.html
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/token/views/token.enroll.registration.html
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/token/views/token.enroll.remote.html
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/token/views/token.enroll.sms.html
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/token/views/token.enroll.spass.html
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/token/views/token.enroll.sshkey.html
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/token/views/token.enroll.tan.html
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/token/views/token.enroll.tiqr.html
--rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/token/views/token.enroll.totp.html
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/token/views/token.enroll.u2f.html
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/token/views/token.enroll.vasco.html
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/token/views/token.enroll.webauthn.html
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/token/views/token.enroll.yubico.html
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/token/views/token.enroll.yubikey.html
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/token/views/token.enrolled.applspec.html
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/token/views/token.enrolled.certificate.html
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/token/views/token.enrolled.daypassword.html
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/token/views/token.enrolled.hotp.html
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/token/views/token.enrolled.motp.html
--rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/token/views/token.enrolled.paper.html
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/token/views/token.enrolled.push.html
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/token/views/token.enrolled.registration.html
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/token/views/token.enrolled.tan.html
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/token/views/token.enrolled.tiqr.html
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/token/views/token.enrolled.totp.html
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/token/views/token.enrolled.u2f.html
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/token/views/token.enrolled.webauthn.html
--rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/token/views/token.getserial.html
--rw-r--r--   0 runner    (1001) docker     (127)     7095 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/token/views/token.html
--rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/token/views/token.import.html
--rw-r--r--   0 runner    (1001) docker     (127)     6263 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/token/views/token.list.html
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/token/views/token.lost.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.023623 edumfa-2.0.1/edumfa/static/components/translation/
--rw-r--r--   0 runner    (1001) docker     (127)   557560 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/translation/translations.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.939622 edumfa-2.0.1/edumfa/static/components/user/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.023623 edumfa-2.0.1/edumfa/static/components/user/controllers/
--rw-r--r--   0 runner    (1001) docker     (127)    19169 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/user/controllers/userControllers.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.023623 edumfa-2.0.1/edumfa/static/components/user/factories/
--rw-r--r--   0 runner    (1001) docker     (127)     5507 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/user/factories/user.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.023623 edumfa-2.0.1/edumfa/static/components/user/states/
--rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/user/states/states.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.023623 edumfa-2.0.1/edumfa/static/components/user/views/
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/user/views/dialog.ask_user_delete.html
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/user/views/user.add.dynamic.form.fields.html
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/user/views/user.add.html
--rw-r--r--   0 runner    (1001) docker     (127)     8616 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/user/views/user.details.html
--rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/user/views/user.html
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/user/views/user.list.html
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/components/user/views/user.password.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.939622 edumfa-2.0.1/edumfa/static/contrib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.027623 edumfa-2.0.1/edumfa/static/contrib/css/
--rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/contrib/css/angular-inform.css
--rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/contrib/css/angular-inform.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    25682 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/contrib/css/bootstrap-theme.css
--rw-r--r--   0 runner    (1001) docker     (127)    48005 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/contrib/css/bootstrap-theme.css.map
--rw-r--r--   0 runner    (1001) docker     (127)   145933 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/contrib/css/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)   390887 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/contrib/css/bootstrap.css.map
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/contrib/css/hotkeys.css
--rw-r--r--   0 runner    (1001) docker     (127)     7021 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/contrib/css/isteven-multi-select.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.027623 edumfa-2.0.1/edumfa/static/contrib/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)    20127 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/contrib/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 runner    (1001) docker     (127)   108738 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/contrib/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 runner    (1001) docker     (127)    45404 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/contrib/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    23424 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/contrib/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 runner    (1001) docker     (127)    18028 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/contrib/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.031623 edumfa-2.0.1/edumfa/static/contrib/js/
--rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/contrib/js/angular-inform.js
--rw-r--r--   0 runner    (1001) docker     (127)     6360 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/contrib/js/angular-inform.js.map
--rw-r--r--   0 runner    (1001) docker     (127)  1377909 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/contrib/js/angular.js
--rw-r--r--   0 runner    (1001) docker     (127)    75484 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/contrib/js/bootstrap.js
--rw-r--r--   0 runner    (1001) docker     (127)    53486 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/contrib/js/hotkeys.js
--rw-r--r--   0 runner    (1001) docker     (127)   288580 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/contrib/js/jquery.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.035623 edumfa-2.0.1/edumfa/static/contrib/js/ngmodules/
--rw-r--r--   0 runner    (1001) docker     (127)    32388 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/contrib/js/ngmodules/angular-gettext.js
--rw-r--r--   0 runner    (1001) docker     (127)    16000 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/contrib/js/ngmodules/angular-idle.js
--rw-r--r--   0 runner    (1001) docker     (127)    33197 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/contrib/js/ngmodules/angular-sanitize.js
--rw-r--r--   0 runner    (1001) docker     (127)   487964 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/contrib/js/ngmodules/angular-ui-router.js
--rw-r--r--   0 runner    (1001) docker     (127)   760134 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/contrib/js/ngmodules/angular-ui-router.js.map
--rw-r--r--   0 runner    (1001) docker     (127)    53338 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/contrib/js/ngmodules/isteven-multi-select.js
--rw-r--r--   0 runner    (1001) docker     (127)    81683 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/contrib/js/ngmodules/ng-file-upload.js
--rw-r--r--   0 runner    (1001) docker     (127)    20905 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/contrib/js/u2f-api.js
--rw-r--r--   0 runner    (1001) docker     (127)   276562 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/contrib/js/ui-bootstrap-tpls.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.035623 edumfa-2.0.1/edumfa/static/contrib/js/webauthn-client/
--rw-r--r--   0 runner    (1001) docker     (127)    20759 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/contrib/js/webauthn-client/edumfa-webauthn.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.035623 edumfa-2.0.1/edumfa/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/css/baseline.css
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/css/content.css
--rw-r--r--   0 runner    (1001) docker     (127)    24602 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/css/eduMFA-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/css/highlight.css
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/css/menu.css
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/css/papertoken.css
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/css/signin.css
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/css/table-ui.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.035623 edumfa-2.0.1/edumfa/static/customize/
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/customize/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8145 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/favicon.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.035623 edumfa-2.0.1/edumfa/static/img/
--rw-r--r--   0 runner    (1001) docker     (127)   195931 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/img/FIDO-U2F-Security-Key-444x444.png
--rw-r--r--   0 runner    (1001) docker     (127)    47610 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/img/plugup.jpg
--rw-r--r--   0 runner    (1001) docker     (127)   336777 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/img/solokeys.png
--rw-r--r--   0 runner    (1001) docker     (127)   107999 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/img/u2fzero.png
--rw-r--r--   0 runner    (1001) docker     (127)     8044 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.039623 edumfa-2.0.1/edumfa/static/providers/
--rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/providers/errorMessageProvider.js
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/providers/versioningProvider.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.039623 edumfa-2.0.1/edumfa/static/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/templates/baseline.html
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/templates/cert_request_form.html
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/templates/deactivated.html
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/templates/documentation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7950 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/templates/footer.html
--rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/templates/header.html
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     7838 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/templates/menu.html
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/templates/token_enrolled.html
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/static/update_contrib.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.943622 edumfa-2.0.1/edumfa/translations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.943622 edumfa-2.0.1/edumfa/translations/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.039623 edumfa-2.0.1/edumfa/translations/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    23376 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/translations/cs/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    84098 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/translations/cs/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.943622 edumfa-2.0.1/edumfa/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.039623 edumfa-2.0.1/edumfa/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    95309 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/translations/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)   127521 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/translations/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.943622 edumfa-2.0.1/edumfa/translations/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.039623 edumfa-2.0.1/edumfa/translations/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    81449 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)   118619 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.943622 edumfa-2.0.1/edumfa/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.039623 edumfa-2.0.1/edumfa/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    53719 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/translations/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)   104451 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/translations/fr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.943622 edumfa-2.0.1/edumfa/translations/it/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.043623 edumfa-2.0.1/edumfa/translations/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    26784 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/translations/it/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    87343 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/translations/it/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.943622 edumfa-2.0.1/edumfa/translations/nl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.043623 edumfa-2.0.1/edumfa/translations/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    85965 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/translations/nl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)   120848 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/translations/nl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.943622 edumfa-2.0.1/edumfa/translations/pl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.043623 edumfa-2.0.1/edumfa/translations/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/translations/pl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    73216 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/translations/pl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.943622 edumfa-2.0.1/edumfa/translations/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.043623 edumfa-2.0.1/edumfa/translations/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    78400 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/translations/pt_BR/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)   115604 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/translations/pt_BR/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.943622 edumfa-2.0.1/edumfa/translations/ro/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.043623 edumfa-2.0.1/edumfa/translations/ro/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    10507 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/translations/ro/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    79882 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/translations/ro/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.943622 edumfa-2.0.1/edumfa/translations/ru/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.043623 edumfa-2.0.1/edumfa/translations/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    33313 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/translations/ru/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    96048 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/translations/ru/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.943622 edumfa-2.0.1/edumfa/translations/si/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.043623 edumfa-2.0.1/edumfa/translations/si/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/translations/si/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    73291 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/translations/si/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.943622 edumfa-2.0.1/edumfa/translations/tr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.043623 edumfa-2.0.1/edumfa/translations/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    82030 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/translations/tr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)   117846 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/translations/tr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.943622 edumfa-2.0.1/edumfa/translations/zh_Hans/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.043623 edumfa-2.0.1/edumfa/translations/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    68507 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/translations/zh_Hans/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)   104457 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/translations/zh_Hans/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.943622 edumfa-2.0.1/edumfa/translations/zh_Hant/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.047623 edumfa-2.0.1/edumfa/translations/zh_Hant/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    70327 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/translations/zh_Hant/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)   105843 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/translations/zh_Hant/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.047623 edumfa-2.0.1/edumfa/webui/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/webui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/webui/certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)     9124 2024-04-12 11:16:12.000000 edumfa-2.0.1/edumfa/webui/login.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.095623 edumfa-2.0.1/edumfa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8588 2024-04-12 11:16:15.000000 edumfa-2.0.1/edumfa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    33263 2024-04-12 11:16:15.000000 edumfa-2.0.1/edumfa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 11:16:15.000000 edumfa-2.0.1/edumfa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-12 11:16:15.000000 edumfa-2.0.1/edumfa.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 11:16:15.000000 edumfa-2.0.1/edumfa.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-12 11:16:15.000000 edumfa-2.0.1/edumfa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-12 11:16:15.000000 edumfa-2.0.1/edumfa.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.047623 edumfa-2.0.1/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/README
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/alembic.ini
--rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/env.py
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/script.py.mako
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.059623 edumfa-2.0.1/migrations/versions/
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/006d4747f858_.py
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/00762b3f7a60_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/0c7123345224_.py
--rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/0d011e94a8e8_.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/140ba0ca4f07_.py
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/145ce80decd_.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/14a1bcb10018_.py
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/19f727d285e2_.py
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/1a0710df148b_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/1a69e5e5e2ac_.py
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/1edda52b619f_.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/204d8d4f351e_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/205bda834127_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/20969b4cbf06_.py
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/2118e566df16_.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/2181294eed0b_.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/22558d9f3178_.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/239995464c48_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/2551ee982544_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/2ac117d0a6f5_.py
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/2c9430cfc66b_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/307a4fbe8a05_.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/3236a1abf1c6_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/3429d523e51f_.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/36428afb2457_.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/37e6b49fc686_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/3ae3c668f444_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/3ba618f6b820_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/3c6e9dd7fbac_.py
--rw-r--r--   0 runner    (1001) docker     (127)     3711 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/3d7f8b29cbb1_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/3f7e8583ea2_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/4023571658f8_.py
--rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/4238eac8ccab_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/449903fb6e35_.py
--rw-r--r--   0 runner    (1001) docker     (127)    10211 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/48ee74b8a7c8_.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/49a04e560d96_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/4a0aec37e7cf_.py
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/4d9178fa8336_.py
--rw-r--r--   0 runner    (1001) docker     (127)    19377 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/4f32a4e1bf33_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/50adc980d625_.py
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/5402fd96fbca_.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/58e4f7ebb705_.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/59ef3e03bc62_.py
--rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/5cb310101a1f_.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/631ec59e1ca6_.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/849170064430_.py
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/86f40f535d7c_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/888b56ed5dcb_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/89e57ed16379_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/8d40dbcfda25_.py
--rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/9155f0d3d028_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/a28f2733897b_.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/a63df077051a_.py
--rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/a7e91b18a460_.py
--rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/b9131d0686eb_.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/cb6d7b7bae63_.py
--rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/d2ae8e54b628_.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/d3c0f0403a84_.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/d415d490eb05_.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/d5870fd2f2a4_.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/d6b40a745e5_.py
--rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/d756b34061ff_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/dceb6cd3c41e_.py
--rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/e360c56bcf8c_.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/e5cbeb7c177_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/ef29ba43e290_.py
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/fa07bd604a75.py
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/fabcf24d9304_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-12 11:16:12.000000 edumfa-2.0.1/migrations/versions/ff26585932ec_.py
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-12 11:16:12.000000 edumfa-2.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 11:16:16.099623 edumfa-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4862 2024-04-12 11:16:12.000000 edumfa-2.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.079623 edumfa-2.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10018 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    28189 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/ldap3mock.py
--rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/mscamock.py
--rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/pkcs11mock.py
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/queuemock.py
--rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/radiusmock.py
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/redismock.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5066 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/smppmock.py
--rw-r--r--   0 runner    (1001) docker     (127)     7723 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/smtpmock.py
--rw-r--r--   0 runner    (1001) docker     (127)    35694 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_api_2stepinit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_api_applications.py
--rw-r--r--   0 runner    (1001) docker     (127)    20710 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_api_audit.py
--rw-r--r--   0 runner    (1001) docker     (127)    48907 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_api_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     9180 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_api_caconnector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_api_clienttype.py
--rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_api_edumfaserver.py
--rw-r--r--   0 runner    (1001) docker     (127)    35517 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_api_events.py
--rw-r--r--   0 runner    (1001) docker     (127)   193396 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_api_lib_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    19077 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_api_lib_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7403 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_api_machineresolver.py
--rw-r--r--   0 runner    (1001) docker     (127)    38769 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_api_machines.py
--rw-r--r--   0 runner    (1001) docker     (127)    16166 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_api_machines_serviceid.py
--rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_api_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     5127 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_api_offline_no_token.py
--rw-r--r--   0 runner    (1001) docker     (127)    13094 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_api_periodictask.py
--rw-r--r--   0 runner    (1001) docker     (127)    36128 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_api_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    26177 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_api_push_validate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6776 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_api_radiusserver.py
--rw-r--r--   0 runner    (1001) docker     (127)     8398 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_api_register.py
--rw-r--r--   0 runner    (1001) docker     (127)    76125 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_api_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_api_serviceids.py
--rw-r--r--   0 runner    (1001) docker     (127)    14259 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_api_smsgateway.py
--rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_api_smtpserver.py
--rw-r--r--   0 runner    (1001) docker     (127)    62186 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_api_system.py
--rw-r--r--   0 runner    (1001) docker     (127)   195170 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_api_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     4649 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_api_tokengroup.py
--rw-r--r--   0 runner    (1001) docker     (127)    21541 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_api_ttype.py
--rw-r--r--   0 runner    (1001) docker     (127)    29544 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_api_u2f.py
--rw-r--r--   0 runner    (1001) docker     (127)    33099 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_api_users.py
--rw-r--r--   0 runner    (1001) docker     (127)   302927 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_api_validate.py
--rw-r--r--   0 runner    (1001) docker     (127)     9130 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (127)    45689 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_db_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9078 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_applications.py
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)    23056 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_audit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     7745 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_authcache.py
--rw-r--r--   0 runner    (1001) docker     (127)    31138 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_caconnector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_challenges.py
--rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_clientapplication.py
--rw-r--r--   0 runner    (1001) docker     (127)    11734 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5797 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_counter.py
--rw-r--r--   0 runner    (1001) docker     (127)    35302 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_crypto.py
--rw-r--r--   0 runner    (1001) docker     (127)    13267 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_edumfaserver.py
--rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_eventhandler_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)    60534 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_eventhandler_usernotification.py
--rw-r--r--   0 runner    (1001) docker     (127)   113340 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_framework.py
--rw-r--r--   0 runner    (1001) docker     (127)    29545 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_importotp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_lifecycle.py
--rw-r--r--   0 runner    (1001) docker     (127)     7147 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_machine_resolver_ldap.py
--rw-r--r--   0 runner    (1001) docker     (127)     8642 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_machines.py
--rw-r--r--   0 runner    (1001) docker     (127)     9378 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_machinetokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     5020 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_monitoringstats.py
--rw-r--r--   0 runner    (1001) docker     (127)    20699 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_periodictask.py
--rw-r--r--   0 runner    (1001) docker     (127)    75326 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    36401 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_policydecorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_pooling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_radiusserver.py
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_realm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_recovery.py
--rw-r--r--   0 runner    (1001) docker     (127)   123815 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_serviceid.py
--rw-r--r--   0 runner    (1001) docker     (127)    32074 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_smsprovider.py
--rw-r--r--   0 runner    (1001) docker     (127)    10949 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_smtpserver.py
--rw-r--r--   0 runner    (1001) docker     (127)     4110 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_sqlutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_task_eventcounter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_task_simplestats.py
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)    97908 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_token.py
--rw-r--r--   0 runner    (1001) docker     (127)    38128 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_tokenclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_tokengroup.py
--rw-r--r--   0 runner    (1001) docker     (127)    36699 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_tokens_certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)    25260 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_tokens_daplug.py
--rw-r--r--   0 runner    (1001) docker     (127)    27651 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_tokens_daypassword.py
--rw-r--r--   0 runner    (1001) docker     (127)    21128 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_tokens_email.py
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_tokens_foureyes.py
--rw-r--r--   0 runner    (1001) docker     (127)    34350 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_tokens_hotp.py
--rw-r--r--   0 runner    (1001) docker     (127)     5500 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_tokens_indexedsecret.py
--rw-r--r--   0 runner    (1001) docker     (127)     7183 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_tokens_motp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_tokens_paper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_tokens_passwordtoken.py
--rw-r--r--   0 runner    (1001) docker     (127)    75419 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_tokens_push.py
--rw-r--r--   0 runner    (1001) docker     (127)     5476 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_tokens_questionnaire.py
--rw-r--r--   0 runner    (1001) docker     (127)    16576 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_tokens_radius.py
--rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_tokens_registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     9417 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_tokens_remote.py
--rw-r--r--   0 runner    (1001) docker     (127)    20806 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_tokens_sms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_tokens_spass.py
--rw-r--r--   0 runner    (1001) docker     (127)     5902 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_tokens_ssh.py
--rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_tokens_tan.py
--rw-r--r--   0 runner    (1001) docker     (127)    31214 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_tokens_tiqr.py
--rw-r--r--   0 runner    (1001) docker     (127)    34079 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_tokens_totp.py
--rw-r--r--   0 runner    (1001) docker     (127)    22536 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_tokens_u2f.py
--rw-r--r--   0 runner    (1001) docker     (127)    10413 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_tokens_vasco.py
--rw-r--r--   0 runner    (1001) docker     (127)    50926 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_tokens_webauthn.py
--rw-r--r--   0 runner    (1001) docker     (127)     4177 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_tokens_yubico.py
--rw-r--r--   0 runner    (1001) docker     (127)    10230 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_tokens_yubikey.py
--rw-r--r--   0 runner    (1001) docker     (127)    22413 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    26644 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_usercache.py
--rw-r--r--   0 runner    (1001) docker     (127)    45888 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_lib_utils_compare.py
--rw-r--r--   0 runner    (1001) docker     (127)    38033 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_mock_ldap3.py
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_resolver_realm.py
--rw-r--r--   0 runner    (1001) docker     (127)    11157 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_scripts.py
--rw-r--r--   0 runner    (1001) docker     (127)     6367 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_ui_certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6702 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/test_ui_login.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.087623 edumfa-2.0.1/tests/testdata/
--rw-r--r--   0 runner    (1001) docker     (127)   195931 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/testdata/FIDO-U2F-Security-Key-444x444.png
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/testdata/NetKnights.pem
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/testdata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:15.943622 edumfa-2.0.1/tests/testdata/altstatic/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.087623 edumfa-2.0.1/tests/testdata/altstatic/templates/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/testdata/altstatic/templates/testui.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.087623 edumfa-2.0.1/tests/testdata/attestation/
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/testdata/attestation/yubico.pem
--rw-r--r--   0 runner    (1001) docker     (127)    16384 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/testdata/audit.sqlite
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.087623 edumfa-2.0.1/tests/testdata/ca/
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/testdata/ca/cacert.pem
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/testdata/ca/cakey.pem
--rw-r--r--   0 runner    (1001) docker     (127)    15874 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/testdata/ca/index.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/testdata/ca/index.txt.attr
--rw-r--r--   0 runner    (1001) docker     (127)     8644 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/testdata/ca/openssl.cnf
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/testdata/ca/serial
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/testdata/ca/templates.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/testdata/dictionary
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/testdata/does_not_exist
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/testdata/emailtemplate.html
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/testdata/empty.oath
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/testdata/enckey
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/testdata/enckey.enc
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/testdata/event.conf
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/testdata/fancytoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/testdata/firebase-test.json
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/testdata/google-services.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.087623 edumfa-2.0.1/tests/testdata/gpg/
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/testdata/gpg/public.pem
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/testdata/gpg/pubring.gpg
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/testdata/gpg/random_seed
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/testdata/gpg/secring.gpg
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/testdata/gpg/trustdb.gpg
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/testdata/hosts
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/testdata/import.oath
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/testdata/import.oath.asc
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/testdata/jwt_sign.key
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/testdata/logging.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/testdata/logging.yml
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/testdata/logging_broken.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.087623 edumfa-2.0.1/tests/testdata/msca-connector/
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/testdata/msca-connector/ca.pem
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/testdata/msca-connector/privacyidea-encrypted.key
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/testdata/msca-connector/privacyidea.key
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/testdata/msca-connector/privacyidea.pem
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/testdata/ocra.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/testdata/passwd
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/testdata/passwd-duplicate-name
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/testdata/passwords
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/testdata/policy.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/testdata/policy.conf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/testdata/policy_empty_file.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/testdata/private.pem
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/testdata/pskc-aes.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/testdata/pskc-password.xml
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/testdata/public.pem
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/testdata/pw-2nd-resolver
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.091623 edumfa-2.0.1/tests/testdata/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)       19 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/testdata/scripts/fail.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)       20 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/testdata/scripts/ls.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)       19 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/testdata/scripts/success.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/testdata/test.sub
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/testdata/test2.sub
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/testdata/testuser-api.sqlite
--rw-r--r--   0 runner    (1001) docker     (127)     5120 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/testdata/testuser.sqlite
--rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/testdata/testusercache.sqlite
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.091623 edumfa-2.0.1/tests/testdata/trusted_attestation_roots/
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/testdata/trusted_attestation_roots/solokeys_device_attestation_ca.pem
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/testdata/trusted_attestation_roots/yubico_u2f_device_attestation_ca.pem
--rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/testdata/yubico-oath-long.csv
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/testdata/yubico-oath.csv
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-12 11:16:12.000000 edumfa-2.0.1/tests/testdata/yubico.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:16.095623 edumfa-2.0.1/tools/
--rwxr-xr-x   0 runner    (1001) docker     (127)      768 2024-04-12 11:16:12.000000 edumfa-2.0.1/tools/creategoogleauthenticator-file
--rwxr-xr-x   0 runner    (1001) docker     (127)     2551 2024-04-12 11:16:12.000000 edumfa-2.0.1/tools/edumfa-authorizedkeys
--rwxr-xr-x   0 runner    (1001) docker     (127)     1766 2024-04-12 11:16:12.000000 edumfa-2.0.1/tools/edumfa-convert-base32.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2876 2024-04-12 11:16:12.000000 edumfa-2.0.1/tools/edumfa-convert-token
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-12 11:16:12.000000 edumfa-2.0.1/tools/edumfa-convert-token.1
--rwxr-xr-x   0 runner    (1001) docker     (127)     3230 2024-04-12 11:16:12.000000 edumfa-2.0.1/tools/edumfa-convert-xml-to-csv
--rwxr-xr-x   0 runner    (1001) docker     (127)     2440 2024-04-12 11:16:12.000000 edumfa-2.0.1/tools/edumfa-create-ad-users
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-12 11:16:12.000000 edumfa-2.0.1/tools/edumfa-create-ad-users.1
--rwxr-xr-x   0 runner    (1001) docker     (127)     1940 2024-04-12 11:16:12.000000 edumfa-2.0.1/tools/edumfa-create-certificate
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-12 11:16:12.000000 edumfa-2.0.1/tools/edumfa-create-certificate.1
--rwxr-xr-x   0 runner    (1001) docker     (127)     1985 2024-04-12 11:16:12.000000 edumfa-2.0.1/tools/edumfa-create-pwidresolver-user
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-12 11:16:12.000000 edumfa-2.0.1/tools/edumfa-create-pwidresolver-user.1
--rwxr-xr-x   0 runner    (1001) docker     (127)     1608 2024-04-12 11:16:12.000000 edumfa-2.0.1/tools/edumfa-create-sqlidresolver-user
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-12 11:16:12.000000 edumfa-2.0.1/tools/edumfa-create-sqlidresolver-user.1
--rwxr-xr-x   0 runner    (1001) docker     (127)      795 2024-04-12 11:16:12.000000 edumfa-2.0.1/tools/edumfa-create-userdb
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-12 11:16:12.000000 edumfa-2.0.1/tools/edumfa-create-userdb.1
--rwxr-xr-x   0 runner    (1001) docker     (127)     6795 2024-04-12 11:16:12.000000 edumfa-2.0.1/tools/edumfa-cron
--rwxr-xr-x   0 runner    (1001) docker     (127)     7030 2024-04-12 11:16:12.000000 edumfa-2.0.1/tools/edumfa-diag
--rwxr-xr-x   0 runner    (1001) docker     (127)     7372 2024-04-12 11:16:12.000000 edumfa-2.0.1/tools/edumfa-expired-users
--rwxr-xr-x   0 runner    (1001) docker     (127)     1354 2024-04-12 11:16:12.000000 edumfa-2.0.1/tools/edumfa-export-edumfa-counter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4514 2024-04-12 11:16:12.000000 edumfa-2.0.1/tools/edumfa-export-linotp-counter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3719 2024-04-12 11:16:12.000000 edumfa-2.0.1/tools/edumfa-fetchssh
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-12 11:16:12.000000 edumfa-2.0.1/tools/edumfa-fetchssh.1
--rwxr-xr-x   0 runner    (1001) docker     (127)     2500 2024-04-12 11:16:12.000000 edumfa-2.0.1/tools/edumfa-fix-access-rights
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-12 11:16:12.000000 edumfa-2.0.1/tools/edumfa-fix-access-rights.1
--rwxr-xr-x   0 runner    (1001) docker     (127)     4303 2024-04-12 11:16:12.000000 edumfa-2.0.1/tools/edumfa-get-serial
--rwxr-xr-x   0 runner    (1001) docker     (127)     5191 2024-04-12 11:16:12.000000 edumfa-2.0.1/tools/edumfa-get-unused-tokens
--rwxr-xr-x   0 runner    (1001) docker     (127)    25361 2024-04-12 11:16:12.000000 edumfa-2.0.1/tools/edumfa-migrate-linotp.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2525 2024-04-12 11:16:12.000000 edumfa-2.0.1/tools/edumfa-pip-update
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-12 11:16:12.000000 edumfa-2.0.1/tools/edumfa-pip-update.1
--rwxr-xr-x   0 runner    (1001) docker     (127)     5761 2024-04-12 11:16:12.000000 edumfa-2.0.1/tools/edumfa-queue-huey
--rwxr-xr-x   0 runner    (1001) docker     (127)      643 2024-04-12 11:16:12.000000 edumfa-2.0.1/tools/edumfa-schema-upgrade
--rwxr-xr-x   0 runner    (1001) docker     (127)    12070 2024-04-12 11:16:12.000000 edumfa-2.0.1/tools/edumfa-standalone
--rwxr-xr-x   0 runner    (1001) docker     (127)     8176 2024-04-12 11:16:12.000000 edumfa-2.0.1/tools/edumfa-sync-owncloud.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    31000 2024-04-12 11:16:12.000000 edumfa-2.0.1/tools/edumfa-token-janitor
--rwxr-xr-x   0 runner    (1001) docker     (127)     3746 2024-04-12 11:16:12.000000 edumfa-2.0.1/tools/edumfa-update-counter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5391 2024-04-12 11:16:12.000000 edumfa-2.0.1/tools/edumfa-update-linotp-counter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5471 2024-04-12 11:16:12.000000 edumfa-2.0.1/tools/edumfa-user-action
--rwxr-xr-x   0 runner    (1001) docker     (127)     4203 2024-04-12 11:16:12.000000 edumfa-2.0.1/tools/edumfa-usercache-cleanup
--rwxr-xr-x   0 runner    (1001) docker     (127)     1476 2024-04-12 11:16:12.000000 edumfa-2.0.1/tools/getgooglecodes
--rwxr-xr-x   0 runner    (1001) docker     (127)     3049 2024-04-12 11:16:12.000000 edumfa-2.0.1/tools/reset-edumfa
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-12 11:16:12.000000 edumfa-2.0.1/tools/ssha.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.992269 edumfa-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     8120 2024-04-26 10:25:09.000000 edumfa-2.0.2/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)    32387 2024-04-26 10:25:09.000000 edumfa-2.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-26 10:25:09.000000 edumfa-2.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8588 2024-04-26 10:25:15.992269 edumfa-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-04-26 10:25:09.000000 edumfa-2.0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.812270 edumfa-2.0.2/deploy/
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-26 10:25:09.000000 edumfa-2.0.2/deploy/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.812270 edumfa-2.0.2/deploy/apache/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-26 10:25:09.000000 edumfa-2.0.2/deploy/apache/edumfaapp.wsgi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.812270 edumfa-2.0.2/deploy/apache/sites-available/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-26 10:25:09.000000 edumfa-2.0.2/deploy/apache/sites-available/edumfa-venv.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-04-26 10:25:09.000000 edumfa-2.0.2/deploy/apache/sites-available/edumfa.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.792270 edumfa-2.0.2/deploy/config/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.812270 edumfa-2.0.2/deploy/config/freeradius2/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-26 10:25:09.000000 edumfa-2.0.2/deploy/config/freeradius2/edumfa
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-26 10:25:09.000000 edumfa-2.0.2/deploy/config/freeradius2/mods-perl-edumfa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.816269 edumfa-2.0.2/deploy/config/freeradius3/
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-26 10:25:09.000000 edumfa-2.0.2/deploy/config/freeradius3/edumfa
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-26 10:25:09.000000 edumfa-2.0.2/deploy/config/freeradius3/mods-perl-edumfa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.816269 edumfa-2.0.2/deploy/crontab/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-26 10:25:09.000000 edumfa-2.0.2/deploy/crontab/edumfa
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-26 10:25:09.000000 edumfa-2.0.2/deploy/docker-compose-example.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.816269 edumfa-2.0.2/deploy/docker-example/
+-rw-r--r--   0 runner    (1001) docker     (127)     6424 2024-04-26 10:25:09.000000 edumfa-2.0.2/deploy/docker-example/edumfa-policy.conf
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-26 10:25:09.000000 edumfa-2.0.2/deploy/docker-example/edumfa-setup.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-26 10:25:09.000000 edumfa-2.0.2/deploy/docker-example/edumfa.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      726 2024-04-26 10:25:09.000000 edumfa-2.0.2/deploy/docker-setup.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.816269 edumfa-2.0.2/deploy/edumfa/
+-rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-04-26 10:25:09.000000 edumfa-2.0.2/deploy/edumfa/dictionary
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-26 10:25:09.000000 edumfa-2.0.2/deploy/edumfa/edumfa.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    21848 2024-04-26 10:25:09.000000 edumfa-2.0.2/deploy/edumfa_radius.pm
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.816269 edumfa-2.0.2/deploy/gunicorn/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-26 10:25:09.000000 edumfa-2.0.2/deploy/gunicorn/edumfaapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-26 10:25:09.000000 edumfa-2.0.2/deploy/logging.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.816269 edumfa-2.0.2/deploy/nginx/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-26 10:25:09.000000 edumfa-2.0.2/deploy/nginx/edumfaapp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.816269 edumfa-2.0.2/deploy/nginx/sites-available/
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-26 10:25:09.000000 edumfa-2.0.2/deploy/nginx/sites-available/edumfa
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-26 10:25:09.000000 edumfa-2.0.2/deploy/rlm_perl.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.816269 edumfa-2.0.2/deploy/ubuntu/
+-rw-r--r--   0 runner    (1001) docker     (127)     5110 2024-04-26 10:25:09.000000 edumfa-2.0.2/deploy/ubuntu/changelog
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-26 10:25:09.000000 edumfa-2.0.2/deploy/ubuntu/clean
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-26 10:25:09.000000 edumfa-2.0.2/deploy/ubuntu/compat
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-26 10:25:09.000000 edumfa-2.0.2/deploy/ubuntu/control
+-rw-r--r--   0 runner    (1001) docker     (127)    32387 2024-04-26 10:25:09.000000 edumfa-2.0.2/deploy/ubuntu/copyright
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-26 10:25:09.000000 edumfa-2.0.2/deploy/ubuntu/rules
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.820269 edumfa-2.0.2/deploy/ubuntu/source/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-26 10:25:09.000000 edumfa-2.0.2/deploy/ubuntu/source/format
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-26 10:25:09.000000 edumfa-2.0.2/deploy/ubuntu/source/options
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.820269 edumfa-2.0.2/deploy/ubuntu-radius/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-26 10:25:09.000000 edumfa-2.0.2/deploy/ubuntu-radius/changelog
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-26 10:25:09.000000 edumfa-2.0.2/deploy/ubuntu-radius/compat
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-26 10:25:09.000000 edumfa-2.0.2/deploy/ubuntu-radius/control
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-26 10:25:09.000000 edumfa-2.0.2/deploy/ubuntu-radius/copyright
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-26 10:25:09.000000 edumfa-2.0.2/deploy/ubuntu-radius/edumfa-radius.install
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-26 10:25:09.000000 edumfa-2.0.2/deploy/ubuntu-radius/edumfa-radius.postinst
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-26 10:25:09.000000 edumfa-2.0.2/deploy/ubuntu-radius/edumfa-radius.postrm
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-26 10:25:09.000000 edumfa-2.0.2/deploy/ubuntu-radius/rules
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.820269 edumfa-2.0.2/deploy/ubuntu-radius/source/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-26 10:25:09.000000 edumfa-2.0.2/deploy/ubuntu-radius/source/format
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.820269 edumfa-2.0.2/deploy/ubuntu-server/
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-26 10:25:09.000000 edumfa-2.0.2/deploy/ubuntu-server/changelog
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-26 10:25:09.000000 edumfa-2.0.2/deploy/ubuntu-server/clean
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-26 10:25:09.000000 edumfa-2.0.2/deploy/ubuntu-server/compat
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-26 10:25:09.000000 edumfa-2.0.2/deploy/ubuntu-server/control
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-26 10:25:09.000000 edumfa-2.0.2/deploy/ubuntu-server/edumfa-apache2.install
+-rw-r--r--   0 runner    (1001) docker     (127)     5936 2024-04-26 10:25:09.000000 edumfa-2.0.2/deploy/ubuntu-server/edumfa-apache2.postinst
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-26 10:25:09.000000 edumfa-2.0.2/deploy/ubuntu-server/edumfa-apache2.postrm
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-26 10:25:09.000000 edumfa-2.0.2/deploy/ubuntu-server/edumfa-nginx.install
+-rw-r--r--   0 runner    (1001) docker     (127)     5498 2024-04-26 10:25:09.000000 edumfa-2.0.2/deploy/ubuntu-server/edumfa-nginx.postinst
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-26 10:25:09.000000 edumfa-2.0.2/deploy/ubuntu-server/edumfa-nginx.postrm
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-26 10:25:09.000000 edumfa-2.0.2/deploy/ubuntu-server/rules
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.820269 edumfa-2.0.2/deploy/ubuntu-server/source/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-26 10:25:09.000000 edumfa-2.0.2/deploy/ubuntu-server/source/format
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-26 10:25:09.000000 edumfa-2.0.2/deploy/ubuntu-server/source/options
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.792270 edumfa-2.0.2/deploy/uwsgi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.820269 edumfa-2.0.2/deploy/uwsgi/apps-available/
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-26 10:25:09.000000 edumfa-2.0.2/deploy/uwsgi/apps-available/edumfa.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.820269 edumfa-2.0.2/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)     9578 2024-04-26 10:25:09.000000 edumfa-2.0.2/doc/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.824269 edumfa-2.0.2/edumfa/
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.828270 edumfa-2.0.2/edumfa/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/api/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/api/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18346 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/api/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16376 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/api/before_after.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/api/caconnector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/api/clienttype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/api/edumfaserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7416 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/api/event.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.832270 edumfa-2.0.2/edumfa/api/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/api/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/api/lib/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/api/lib/policyhelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41909 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/api/lib/postpolicy.py
+-rw-r--r--   0 runner    (1001) docker     (127)   101620 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/api/lib/prepolicy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17919 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/api/lib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15527 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/api/machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/api/machineresolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/api/monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7937 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/api/periodictask.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18770 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/api/policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5065 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/api/radiusserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10790 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/api/realm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3436 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/api/recover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7117 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/api/register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6730 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/api/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5232 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/api/serviceid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5462 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/api/smsgateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5678 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/api/smtpserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12631 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/api/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55749 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/api/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/api/tokengroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/api/ttype.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12293 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/api/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29126 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/api/validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10347 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/babel.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.832270 edumfa-2.0.2/edumfa/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.832270 edumfa-2.0.2/edumfa/commands/manage/
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/commands/manage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/commands/manage/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/commands/manage/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7876 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/commands/manage/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/commands/manage/authcache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8679 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/commands/manage/backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/commands/manage/ca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8434 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/commands/manage/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9125 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/commands/manage/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/commands/manage/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8604 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/commands/manage/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/commands/manage/hsm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/commands/manage/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6113 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/commands/manage/policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/commands/manage/realm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7407 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/commands/manage/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/commands/manage/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6719 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.844269 edumfa-2.0.2/edumfa/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.844269 edumfa-2.0.2/edumfa/lib/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5822 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/applications/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/applications/luks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8071 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/applications/offline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4624 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/applications/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7274 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/audit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.844269 edumfa-2.0.2/edumfa/lib/auditmodules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/auditmodules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8753 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/auditmodules/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4803 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/auditmodules/containeraudit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/auditmodules/loggeraudit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26334 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/auditmodules/sqlaudit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6116 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/authcache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.844269 edumfa-2.0.2/edumfa/lib/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11818 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/caconnector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.848270 edumfa-2.0.2/edumfa/lib/caconnectors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/caconnectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5407 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/caconnectors/baseca.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10664 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/caconnectors/caservice_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11705 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/caconnectors/caservice_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27129 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/caconnectors/localca.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17276 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/caconnectors/msca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/challenge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9650 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/challengeresponsedecorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4216 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/clientapplication.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37191 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/counter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28650 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5172 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8913 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/edumfaserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6314 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13480 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/event.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.848270 edumfa-2.0.2/edumfa/lib/eventhandler/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/eventhandler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24816 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/eventhandler/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/eventhandler/counterhandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/eventhandler/customuserattributeshandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7324 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/eventhandler/federationhandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6350 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/eventhandler/logginghandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7501 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/eventhandler/requestmangler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/eventhandler/responsemangler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8919 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/eventhandler/scripthandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30629 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/eventhandler/tokenhandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21553 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/eventhandler/usernotification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6882 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/eventhandler/webhookeventhandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/framework.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29329 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/importotp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/lifecycle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7411 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19552 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11009 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/machineresolver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.848270 edumfa-2.0.2/edumfa/lib/machines/
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/machines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5793 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/machines/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5828 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/machines/hosts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14366 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/machines/ldap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.848270 edumfa-2.0.2/edumfa/lib/monitoringmodules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/monitoringmodules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/monitoringmodules/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7803 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/monitoringmodules/sqlstats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/monitoringstats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5598 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/passwordreset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12715 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/periodictask.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.848270 edumfa-2.0.2/edumfa/lib/pinhandling/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/pinhandling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/pinhandling/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)   146637 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28834 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/policydecorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5002 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/queue.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.852270 edumfa-2.0.2/edumfa/lib/queues/
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/queues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/queues/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/queues/huey_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/radiusserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8015 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/realm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14818 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.852270 edumfa-2.0.2/edumfa/lib/resolvers/
+-rw-r--r--   0 runner    (1001) docker     (127)     7221 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/resolvers/HTTPResolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56717 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/resolvers/LDAPIdResolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15166 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/resolvers/PasswdIdResolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10885 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/resolvers/SCIMIdResolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28267 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/resolvers/SQLIdResolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8582 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/resolvers/UserIdResolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/resolvers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.852270 edumfa-2.0.2/edumfa/lib/security/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13784 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/security/aeshsm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16456 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/security/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14478 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/security/encryptkey.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.852270 edumfa-2.0.2/edumfa/lib/security/password/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/security/password/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/serviceid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.856269 edumfa-2.0.2/edumfa/lib/smsprovider/
+-rw-r--r--   0 runner    (1001) docker     (127)     9043 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/smsprovider/FirebaseProvider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11897 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/smsprovider/HttpMessageToUidProvider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12084 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/smsprovider/HttpSMSProvider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12557 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/smsprovider/SMSProvider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5560 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/smsprovider/ScriptSMSProvider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/smsprovider/SipgateSMSProvider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6344 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/smsprovider/SmppSMSProvider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5552 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/smsprovider/SmtpSMSProvider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/smsprovider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13914 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/smtpserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/sqlutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5198 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/subscriptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.856269 edumfa-2.0.2/edumfa/lib/task/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/task/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/task/eventcounter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/task/simplestats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    96840 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68371 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/tokenclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/tokengroup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.860269 edumfa-2.0.2/edumfa/lib/tokens/
+-rw-r--r--   0 runner    (1001) docker     (127)     4835 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/tokens/HMAC.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/tokens/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/tokens/applicationspecificpasswordtoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25829 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/tokens/certificatetoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8437 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/tokens/daplugtoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16746 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/tokens/daypasswordtoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22711 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/tokens/emailtoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18983 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/tokens/foureyestoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33207 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/tokens/hotptoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15895 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/tokens/indexedsecrettoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5147 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/tokens/mOTP.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8233 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/tokens/motptoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14117 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/tokens/ocra.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10863 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/tokens/ocratoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5171 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/tokens/papertoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6715 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/tokens/passwordtoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46761 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/tokens/pushtoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14241 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/tokens/questionnairetoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22143 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/tokens/radiustoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5709 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/tokens/registrationtoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12204 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/tokens/remotetoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25360 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/tokens/smstoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5253 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/tokens/spasstoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5806 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/tokens/sshkeytoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8122 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/tokens/tantoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19941 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/tokens/tiqrtoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27633 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/tokens/totptoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9775 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/tokens/u2f.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23119 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/tokens/u2ftoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/tokens/vasco.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7039 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/tokens/vascotoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)    88978 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/tokens/webauthn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66725 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/tokens/webauthntoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8523 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/tokens/yubicotoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16984 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/tokens/yubikeytoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30141 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9660 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/usercache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.864269 edumfa-2.0.2/edumfa/lib/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)    55043 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8069 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/utils/compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/lib/utils/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71279 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/messages.pot
+-rw-r--r--   0 runner    (1001) docker     (127)   121690 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.864269 edumfa-2.0.2/edumfa/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8220 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/app.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.804270 edumfa-2.0.2/edumfa/static/components/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.796270 edumfa-2.0.2/edumfa/static/components/audit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.864269 edumfa-2.0.2/edumfa/static/components/audit/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/audit/controllers/auditControllers.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.864269 edumfa-2.0.2/edumfa/static/components/audit/factories/
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/audit/factories/audit.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.864269 edumfa-2.0.2/edumfa/static/components/audit/states/
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/audit/states/states.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.864269 edumfa-2.0.2/edumfa/static/components/audit/views/
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/audit/views/audit.html
+-rw-r--r--   0 runner    (1001) docker     (127)    11055 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/audit/views/audit.log.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.796270 edumfa-2.0.2/edumfa/static/components/components/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.864269 edumfa-2.0.2/edumfa/static/components/components/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/components/controllers/componentControllers.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.864269 edumfa-2.0.2/edumfa/static/components/components/factories/
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/components/factories/component.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.864269 edumfa-2.0.2/edumfa/static/components/components/states/
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/components/states/states.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.864269 edumfa-2.0.2/edumfa/static/components/components/views/
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/components/views/component.clienttype.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/components/views/component.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.800269 edumfa-2.0.2/edumfa/static/components/config/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.868269 edumfa-2.0.2/edumfa/static/components/config/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)    50570 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/controllers/configControllers.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/controllers/eduMfaServerController.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11316 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/controllers/eventController.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/controllers/ldapMachineResolverController.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7474 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/controllers/periodicTaskController.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/controllers/radiusServerController.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/controllers/serviceidController.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/controllers/smsgatewayController.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/controllers/smtpServerController.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/controllers/tokengroupController.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.868269 edumfa-2.0.2/edumfa/static/components/config/factories/
+-rw-r--r--   0 runner    (1001) docker     (127)    32353 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/factories/config.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.868269 edumfa-2.0.2/edumfa/static/components/config/states/
+-rw-r--r--   0 runner    (1001) docker     (127)    19924 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/states/states.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.876269 edumfa-2.0.2/edumfa/static/components/config/views/
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/views/config.caconnectors.list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6518 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/views/config.caconnectors.local.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6204 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/views/config.caconnectors.microsoft.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/views/config.edumfaserver.edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/views/config.edumfaserver.list.html
+-rw-r--r--   0 runner    (1001) docker     (127)    15020 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/views/config.events.details.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/views/config.events.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/views/config.events.list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4497 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/views/config.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/views/config.machineresolvers.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/views/config.mresolvers.hosts.html
+-rw-r--r--   0 runner    (1001) docker     (127)     8217 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/views/config.mresolvers.ldap.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/views/config.mresolvers.list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7503 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/views/config.periodictasks.details.html
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/views/config.periodictasks.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/views/config.periodictasks.list.html
+-rw-r--r--   0 runner    (1001) docker     (127)    22234 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/views/config.policies.details.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/views/config.policies.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/views/config.policies.list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/views/config.radius.edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/views/config.radius.list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/views/config.realms.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6002 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/views/config.realms.list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/views/config.resolvers.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/views/config.resolvers.http.html
+-rw-r--r--   0 runner    (1001) docker     (127)    14914 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/views/config.resolvers.ldap.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/views/config.resolvers.list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/views/config.resolvers.passwd.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/views/config.resolvers.scim.html
+-rw-r--r--   0 runner    (1001) docker     (127)    10128 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/views/config.resolvers.sql.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/views/config.serviceid.edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/views/config.serviceid.list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5797 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/views/config.smsgateway.edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/views/config.smsgateway.list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5506 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/views/config.smtp.edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/views/config.smtp.list.html
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/views/config.system.doc.html
+-rw-r--r--   0 runner    (1001) docker     (127)     8912 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/views/config.system.edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)    13600 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/views/config.system.html
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/views/config.token.daypassword.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/views/config.token.email.html
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/views/config.token.hotp.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/views/config.token.question.html
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/views/config.token.radius.html
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/views/config.token.remote.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/views/config.token.sms.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/views/config.token.tiqr.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/views/config.token.totp.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/views/config.token.u2f.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/views/config.token.webauthn.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/views/config.token.yubico.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/views/config.token.yubikey.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/views/config.tokengroup.edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/views/config.tokengroup.list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/views/config.tokens.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/config/views/dialog.confirm_delete.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.800269 edumfa-2.0.2/edumfa/static/components/dashboard/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.880269 edumfa-2.0.2/edumfa/static/components/dashboard/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)     8518 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/dashboard/controllers/dashboardControllers.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.880269 edumfa-2.0.2/edumfa/static/components/dashboard/states/
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/dashboard/states/states.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.880269 edumfa-2.0.2/edumfa/static/components/dashboard/views/
+-rw-r--r--   0 runner    (1001) docker     (127)     8881 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/dashboard/views/dashboard.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.800269 edumfa-2.0.2/edumfa/static/components/dialogs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.880269 edumfa-2.0.2/edumfa/static/components/dialogs/views/
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/dialogs/views/dialog.about.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/dialogs/views/dialog.autocreate_realm.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/dialogs/views/dialog.lock.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/dialogs/views/dialog.no.token.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/dialogs/views/dialog.welcome.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.800269 edumfa-2.0.2/edumfa/static/components/directives/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.880269 edumfa-2.0.2/edumfa/static/components/directives/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)    19746 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/directives/controllers/directives.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.880269 edumfa-2.0.2/edumfa/static/components/directives/views/
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/directives/views/directive.assigntoken.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/directives/views/directive.assignuser.html
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/directives/views/directive.attachmachine.html
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/directives/views/directive.attachtoken.html
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/directives/views/directive.csvdownload.html
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/directives/views/directive.filter.table.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/directives/views/directive.policyconditions.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/directives/views/directive.tokendata.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.880269 edumfa-2.0.2/edumfa/static/components/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/filters/filters.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.800269 edumfa-2.0.2/edumfa/static/components/login/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.880269 edumfa-2.0.2/edumfa/static/components/login/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)    30344 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/login/controllers/loginControllers.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.884269 edumfa-2.0.2/edumfa/static/components/login/factories/
+-rw-r--r--   0 runner    (1001) docker     (127)     5789 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/login/factories/auth.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5225 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/login/factories/u2f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/login/factories/webauthn.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.884269 edumfa-2.0.2/edumfa/static/components/login/states/
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/login/states/states.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.884269 edumfa-2.0.2/edumfa/static/components/login/views/
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/login/views/enter-response.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/login/views/login.html
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/login/views/offline.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/login/views/pinchange.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.800269 edumfa-2.0.2/edumfa/static/components/machine/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.884269 edumfa-2.0.2/edumfa/static/components/machine/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/machine/controllers/machineController.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/machine/controllers/machineDetailsController.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.884269 edumfa-2.0.2/edumfa/static/components/machine/factories/
+-rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/machine/factories/machine.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.884269 edumfa-2.0.2/edumfa/static/components/machine/states/
+-rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/machine/states/states.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.884269 edumfa-2.0.2/edumfa/static/components/machine/views/
+-rw-r--r--   0 runner    (1001) docker     (127)     7085 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/machine/views/machine.details.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/machine/views/machine.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/machine/views/machine.list.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.800269 edumfa-2.0.2/edumfa/static/components/recovery/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.884269 edumfa-2.0.2/edumfa/static/components/recovery/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/recovery/controllers/recoveryControllers.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.884269 edumfa-2.0.2/edumfa/static/components/recovery/factories/
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/recovery/factories/recoveryFactory.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.884269 edumfa-2.0.2/edumfa/static/components/recovery/states/
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/recovery/states/states.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.884269 edumfa-2.0.2/edumfa/static/components/recovery/views/
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/recovery/views/recovery.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/recovery/views/recovery.reset.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.804270 edumfa-2.0.2/edumfa/static/components/register/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.884269 edumfa-2.0.2/edumfa/static/components/register/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/register/controllers/registerControllers.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.884269 edumfa-2.0.2/edumfa/static/components/register/factories/
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/register/factories/registerFactory.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.888269 edumfa-2.0.2/edumfa/static/components/register/states/
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/register/states/states.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.888269 edumfa-2.0.2/edumfa/static/components/register/views/
+-rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/register/views/register.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.804270 edumfa-2.0.2/edumfa/static/components/token/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.888269 edumfa-2.0.2/edumfa/static/components/token/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/token/controllers/tokenApplicationsController.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/token/controllers/tokenChallengesController.js
+-rw-r--r--   0 runner    (1001) docker     (127)    29864 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/token/controllers/tokenControllers.js
+-rw-r--r--   0 runner    (1001) docker     (127)    17169 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/token/controllers/tokenDetailController.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/token/controllers/tokenGetSerialController.js
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/token/controllers/tokenLostController.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.888269 edumfa-2.0.2/edumfa/static/components/token/factories/
+-rw-r--r--   0 runner    (1001) docker     (127)    12956 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/token/factories/token.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/token/factories/validate.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.888269 edumfa-2.0.2/edumfa/static/components/token/states/
+-rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/token/states/states.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.896269 edumfa-2.0.2/edumfa/static/components/token/views/
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/token/views/dialog.ask_token_delete.html
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/token/views/token.applications.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/token/views/token.applications.offline.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/token/views/token.applications.ssh.html
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/token/views/token.assign.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/token/views/token.challenges.html
+-rw-r--r--   0 runner    (1001) docker     (127)    32395 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/token/views/token.details.html
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/token/views/token.display.apps.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/token/views/token.enroll.4eyes.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/token/views/token.enroll.applspec.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/token/views/token.enroll.certificate.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/token/views/token.enroll.daypassword.html
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/token/views/token.enroll.email.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/token/views/token.enroll.hotp.html
+-rw-r--r--   0 runner    (1001) docker     (127)    10466 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/token/views/token.enroll.html
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/token/views/token.enroll.indexedsecret.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/token/views/token.enroll.motp.html
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/token/views/token.enroll.paper.html
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/token/views/token.enroll.push.html
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/token/views/token.enroll.question.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/token/views/token.enroll.radius.html
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/token/views/token.enroll.registration.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/token/views/token.enroll.remote.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/token/views/token.enroll.sms.html
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/token/views/token.enroll.spass.html
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/token/views/token.enroll.sshkey.html
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/token/views/token.enroll.tan.html
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/token/views/token.enroll.tiqr.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/token/views/token.enroll.totp.html
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/token/views/token.enroll.u2f.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/token/views/token.enroll.vasco.html
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/token/views/token.enroll.webauthn.html
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/token/views/token.enroll.yubico.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/token/views/token.enroll.yubikey.html
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/token/views/token.enrolled.applspec.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/token/views/token.enrolled.certificate.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/token/views/token.enrolled.daypassword.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/token/views/token.enrolled.hotp.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/token/views/token.enrolled.motp.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/token/views/token.enrolled.paper.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/token/views/token.enrolled.push.html
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/token/views/token.enrolled.registration.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/token/views/token.enrolled.tan.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/token/views/token.enrolled.tiqr.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/token/views/token.enrolled.totp.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/token/views/token.enrolled.u2f.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/token/views/token.enrolled.webauthn.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/token/views/token.getserial.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7095 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/token/views/token.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/token/views/token.import.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6263 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/token/views/token.list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/token/views/token.lost.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.900269 edumfa-2.0.2/edumfa/static/components/translation/
+-rw-r--r--   0 runner    (1001) docker     (127)   557560 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/translation/translations.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.804270 edumfa-2.0.2/edumfa/static/components/user/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.900269 edumfa-2.0.2/edumfa/static/components/user/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)    19169 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/user/controllers/userControllers.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.900269 edumfa-2.0.2/edumfa/static/components/user/factories/
+-rw-r--r--   0 runner    (1001) docker     (127)     5507 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/user/factories/user.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.900269 edumfa-2.0.2/edumfa/static/components/user/states/
+-rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/user/states/states.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.900269 edumfa-2.0.2/edumfa/static/components/user/views/
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/user/views/dialog.ask_user_delete.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/user/views/user.add.dynamic.form.fields.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/user/views/user.add.html
+-rw-r--r--   0 runner    (1001) docker     (127)     8616 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/user/views/user.details.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/user/views/user.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/user/views/user.list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/components/user/views/user.password.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.804270 edumfa-2.0.2/edumfa/static/contrib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.904269 edumfa-2.0.2/edumfa/static/contrib/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/contrib/css/angular-inform.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/contrib/css/angular-inform.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    25682 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/contrib/css/bootstrap-theme.css
+-rw-r--r--   0 runner    (1001) docker     (127)    48005 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/contrib/css/bootstrap-theme.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)   145933 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/contrib/css/bootstrap.css
+-rw-r--r--   0 runner    (1001) docker     (127)   390887 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/contrib/css/bootstrap.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/contrib/css/hotkeys.css
+-rw-r--r--   0 runner    (1001) docker     (127)     7021 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/contrib/css/isteven-multi-select.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.904269 edumfa-2.0.2/edumfa/static/contrib/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)    20127 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/contrib/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   108738 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/contrib/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    45404 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/contrib/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    23424 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/contrib/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    18028 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/contrib/fonts/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.908269 edumfa-2.0.2/edumfa/static/contrib/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/contrib/js/angular-inform.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6360 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/contrib/js/angular-inform.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)  1377909 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/contrib/js/angular.js
+-rw-r--r--   0 runner    (1001) docker     (127)    75484 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/contrib/js/bootstrap.js
+-rw-r--r--   0 runner    (1001) docker     (127)    53486 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/contrib/js/hotkeys.js
+-rw-r--r--   0 runner    (1001) docker     (127)   288580 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/contrib/js/jquery.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.912269 edumfa-2.0.2/edumfa/static/contrib/js/ngmodules/
+-rw-r--r--   0 runner    (1001) docker     (127)    32388 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/contrib/js/ngmodules/angular-gettext.js
+-rw-r--r--   0 runner    (1001) docker     (127)    16000 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/contrib/js/ngmodules/angular-idle.js
+-rw-r--r--   0 runner    (1001) docker     (127)    33197 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/contrib/js/ngmodules/angular-sanitize.js
+-rw-r--r--   0 runner    (1001) docker     (127)   487964 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/contrib/js/ngmodules/angular-ui-router.js
+-rw-r--r--   0 runner    (1001) docker     (127)   760134 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/contrib/js/ngmodules/angular-ui-router.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)    53338 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/contrib/js/ngmodules/isteven-multi-select.js
+-rw-r--r--   0 runner    (1001) docker     (127)    81683 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/contrib/js/ngmodules/ng-file-upload.js
+-rw-r--r--   0 runner    (1001) docker     (127)    20905 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/contrib/js/u2f-api.js
+-rw-r--r--   0 runner    (1001) docker     (127)   276562 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/contrib/js/ui-bootstrap-tpls.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.912269 edumfa-2.0.2/edumfa/static/contrib/js/webauthn-client/
+-rw-r--r--   0 runner    (1001) docker     (127)    20759 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/contrib/js/webauthn-client/edumfa-webauthn.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.912269 edumfa-2.0.2/edumfa/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/css/baseline.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/css/content.css
+-rw-r--r--   0 runner    (1001) docker     (127)    24602 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/css/eduMFA-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/css/highlight.css
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/css/menu.css
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/css/papertoken.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/css/signin.css
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/css/table-ui.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.912269 edumfa-2.0.2/edumfa/static/customize/
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/customize/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8145 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/favicon.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.916269 edumfa-2.0.2/edumfa/static/img/
+-rw-r--r--   0 runner    (1001) docker     (127)   195931 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/img/FIDO-U2F-Security-Key-444x444.png
+-rw-r--r--   0 runner    (1001) docker     (127)    47610 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/img/plugup.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)   336777 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/img/solokeys.png
+-rw-r--r--   0 runner    (1001) docker     (127)   107999 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/img/u2fzero.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8044 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.916269 edumfa-2.0.2/edumfa/static/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/providers/errorMessageProvider.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/providers/versioningProvider.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.916269 edumfa-2.0.2/edumfa/static/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/templates/baseline.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/templates/cert_request_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/templates/deactivated.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/templates/documentation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7950 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/templates/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/templates/header.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7838 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/templates/menu.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/templates/token_enrolled.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/static/update_contrib.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.808270 edumfa-2.0.2/edumfa/translations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.804270 edumfa-2.0.2/edumfa/translations/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.916269 edumfa-2.0.2/edumfa/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    23376 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/translations/cs/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    84098 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.804270 edumfa-2.0.2/edumfa/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.916269 edumfa-2.0.2/edumfa/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    95309 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/translations/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   127521 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/translations/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.804270 edumfa-2.0.2/edumfa/translations/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.920269 edumfa-2.0.2/edumfa/translations/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    81449 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/translations/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   118619 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.808270 edumfa-2.0.2/edumfa/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.920269 edumfa-2.0.2/edumfa/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    53719 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/translations/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   104451 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/translations/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.808270 edumfa-2.0.2/edumfa/translations/it/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.920269 edumfa-2.0.2/edumfa/translations/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    26784 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/translations/it/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    87343 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/translations/it/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.808270 edumfa-2.0.2/edumfa/translations/nl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.920269 edumfa-2.0.2/edumfa/translations/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    85965 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/translations/nl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   120848 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/translations/nl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.808270 edumfa-2.0.2/edumfa/translations/pl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.920269 edumfa-2.0.2/edumfa/translations/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/translations/pl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    73216 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/translations/pl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.808270 edumfa-2.0.2/edumfa/translations/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.920269 edumfa-2.0.2/edumfa/translations/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    78400 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/translations/pt_BR/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   115604 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/translations/pt_BR/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.808270 edumfa-2.0.2/edumfa/translations/ro/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.924269 edumfa-2.0.2/edumfa/translations/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    10507 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/translations/ro/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    79882 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/translations/ro/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.808270 edumfa-2.0.2/edumfa/translations/ru/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.924269 edumfa-2.0.2/edumfa/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    33313 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/translations/ru/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    96048 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/translations/ru/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.808270 edumfa-2.0.2/edumfa/translations/si/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.924269 edumfa-2.0.2/edumfa/translations/si/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/translations/si/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    73291 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/translations/si/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.808270 edumfa-2.0.2/edumfa/translations/tr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.924269 edumfa-2.0.2/edumfa/translations/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    82030 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/translations/tr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   117846 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/translations/tr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.808270 edumfa-2.0.2/edumfa/translations/zh_Hans/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.924269 edumfa-2.0.2/edumfa/translations/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    68507 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/translations/zh_Hans/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   104457 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/translations/zh_Hans/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.808270 edumfa-2.0.2/edumfa/translations/zh_Hant/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.924269 edumfa-2.0.2/edumfa/translations/zh_Hant/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    70327 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/translations/zh_Hant/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   105843 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/translations/zh_Hant/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.928269 edumfa-2.0.2/edumfa/webui/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/webui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/webui/certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9124 2024-04-26 10:25:09.000000 edumfa-2.0.2/edumfa/webui/login.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.988269 edumfa-2.0.2/edumfa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8588 2024-04-26 10:25:15.000000 edumfa-2.0.2/edumfa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    33263 2024-04-26 10:25:15.000000 edumfa-2.0.2/edumfa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 10:25:15.000000 edumfa-2.0.2/edumfa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-26 10:25:15.000000 edumfa-2.0.2/edumfa.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 10:25:15.000000 edumfa-2.0.2/edumfa.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-26 10:25:15.000000 edumfa-2.0.2/edumfa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-26 10:25:15.000000 edumfa-2.0.2/edumfa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.928269 edumfa-2.0.2/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/README
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/alembic.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/script.py.mako
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.940269 edumfa-2.0.2/migrations/versions/
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/006d4747f858_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/00762b3f7a60_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/0c7123345224_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/0d011e94a8e8_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/140ba0ca4f07_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/145ce80decd_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/14a1bcb10018_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/19f727d285e2_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/1a0710df148b_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/1a69e5e5e2ac_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/1edda52b619f_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/204d8d4f351e_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/205bda834127_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/20969b4cbf06_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/2118e566df16_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/2181294eed0b_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/22558d9f3178_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/239995464c48_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/2551ee982544_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/2ac117d0a6f5_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/2c9430cfc66b_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/307a4fbe8a05_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/3236a1abf1c6_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/3429d523e51f_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/36428afb2457_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/37e6b49fc686_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/3ae3c668f444_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/3ba618f6b820_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/3c6e9dd7fbac_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3711 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/3d7f8b29cbb1_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/3f7e8583ea2_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/4023571658f8_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/4238eac8ccab_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/449903fb6e35_.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10211 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/48ee74b8a7c8_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/49a04e560d96_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/4a0aec37e7cf_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/4d9178fa8336_.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19377 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/4f32a4e1bf33_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/50adc980d625_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/5402fd96fbca_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/58e4f7ebb705_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/59ef3e03bc62_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/5cb310101a1f_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/631ec59e1ca6_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/849170064430_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/86f40f535d7c_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/888b56ed5dcb_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/89e57ed16379_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/8d40dbcfda25_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/9155f0d3d028_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/a28f2733897b_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/a63df077051a_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/a7e91b18a460_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/b9131d0686eb_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/cb6d7b7bae63_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/d2ae8e54b628_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/d3c0f0403a84_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/d415d490eb05_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/d5870fd2f2a4_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/d6b40a745e5_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/d756b34061ff_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/dceb6cd3c41e_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/e360c56bcf8c_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/e5cbeb7c177_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/ef29ba43e290_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/fa07bd604a75.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/fabcf24d9304_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-26 10:25:09.000000 edumfa-2.0.2/migrations/versions/ff26585932ec_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-04-26 10:25:09.000000 edumfa-2.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 10:25:15.992269 edumfa-2.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4862 2024-04-26 10:25:09.000000 edumfa-2.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.968269 edumfa-2.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10010 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28157 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/ldap3mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/mscamock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6840 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/pkcs11mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/queuemock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/radiusmock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/redismock.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/smppmock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7715 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/smtpmock.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35694 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_api_2stepinit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_api_applications.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20710 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_api_audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48907 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_api_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9180 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_api_caconnector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_api_clienttype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_api_edumfaserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35517 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_api_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)   193308 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_api_lib_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19077 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_api_lib_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7403 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_api_machineresolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38769 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_api_machines.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16166 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_api_machines_serviceid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_api_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5127 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_api_offline_no_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13094 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_api_periodictask.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36128 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_api_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26177 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_api_push_validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6776 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_api_radiusserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8398 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_api_register.py
+-rw-r--r--   0 runner    (1001) docker     (127)    76125 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_api_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_api_serviceids.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14259 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_api_smsgateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_api_smtpserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62186 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_api_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)   195170 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_api_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4649 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_api_tokengroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21541 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_api_ttype.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29544 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_api_u2f.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33099 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_api_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)   302927 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_api_validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9130 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45689 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_db_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9078 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_applications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23056 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7745 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_authcache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31138 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_caconnector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_challenges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_clientapplication.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11734 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5797 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_counter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35302 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_crypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13267 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_edumfaserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_eventhandler_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60534 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_eventhandler_usernotification.py
+-rw-r--r--   0 runner    (1001) docker     (127)   113340 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_framework.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29545 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_importotp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_lifecycle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7147 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_machine_resolver_ldap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8642 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_machines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9378 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_machinetokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5020 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_monitoringstats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20699 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_periodictask.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75286 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36401 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_policydecorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_pooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_radiusserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_realm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_recovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)   123815 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_serviceid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41034 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_smsprovider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10949 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_smtpserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4110 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_sqlutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_task_eventcounter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_task_simplestats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    97900 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38128 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_tokenclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_tokengroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36699 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_tokens_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25260 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_tokens_daplug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27651 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_tokens_daypassword.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21128 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_tokens_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_tokens_foureyes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34350 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_tokens_hotp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5500 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_tokens_indexedsecret.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7183 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_tokens_motp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_tokens_paper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_tokens_passwordtoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75419 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_tokens_push.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5476 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_tokens_questionnaire.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16576 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_tokens_radius.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_tokens_registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9417 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_tokens_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20806 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_tokens_sms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_tokens_spass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5902 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_tokens_ssh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_tokens_tan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31214 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_tokens_tiqr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34079 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_tokens_totp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22536 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_tokens_u2f.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10413 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_tokens_vasco.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50926 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_tokens_webauthn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4177 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_tokens_yubico.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10230 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_tokens_yubikey.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22413 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26644 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_usercache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45888 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_lib_utils_compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38033 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_mock_ldap3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_resolver_realm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11157 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6367 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_ui_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6702 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/test_ui_login.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.976269 edumfa-2.0.2/tests/testdata/
+-rw-r--r--   0 runner    (1001) docker     (127)   195931 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/testdata/FIDO-U2F-Security-Key-444x444.png
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/testdata/NetKnights.pem
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/testdata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.808270 edumfa-2.0.2/tests/testdata/altstatic/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.976269 edumfa-2.0.2/tests/testdata/altstatic/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/testdata/altstatic/templates/testui.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.976269 edumfa-2.0.2/tests/testdata/attestation/
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/testdata/attestation/yubico.pem
+-rw-r--r--   0 runner    (1001) docker     (127)    16384 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/testdata/audit.sqlite
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.980269 edumfa-2.0.2/tests/testdata/ca/
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/testdata/ca/cacert.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/testdata/ca/cakey.pem
+-rw-r--r--   0 runner    (1001) docker     (127)    15874 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/testdata/ca/index.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/testdata/ca/index.txt.attr
+-rw-r--r--   0 runner    (1001) docker     (127)     8644 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/testdata/ca/openssl.cnf
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/testdata/ca/serial
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/testdata/ca/templates.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/testdata/dictionary
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/testdata/does_not_exist
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/testdata/emailtemplate.html
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/testdata/empty.oath
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/testdata/enckey
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/testdata/enckey.enc
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/testdata/event.conf
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/testdata/fancytoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/testdata/firebase-test.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/testdata/google-services.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.980269 edumfa-2.0.2/tests/testdata/gpg/
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/testdata/gpg/public.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/testdata/gpg/pubring.gpg
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/testdata/gpg/random_seed
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/testdata/gpg/secring.gpg
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/testdata/gpg/trustdb.gpg
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/testdata/hosts
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/testdata/import.oath
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/testdata/import.oath.asc
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/testdata/jwt_sign.key
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/testdata/logging.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/testdata/logging.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/testdata/logging_broken.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.980269 edumfa-2.0.2/tests/testdata/msca-connector/
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/testdata/msca-connector/ca.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/testdata/msca-connector/privacyidea-encrypted.key
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/testdata/msca-connector/privacyidea.key
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/testdata/msca-connector/privacyidea.pem
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/testdata/ocra.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/testdata/passwd
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/testdata/passwd-duplicate-name
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/testdata/passwords
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/testdata/policy.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/testdata/policy.conf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/testdata/policy_empty_file.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/testdata/private.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/testdata/pskc-aes.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/testdata/pskc-password.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/testdata/public.pem
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/testdata/pw-2nd-resolver
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.980269 edumfa-2.0.2/tests/testdata/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       19 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/testdata/scripts/fail.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)       20 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/testdata/scripts/ls.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)       19 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/testdata/scripts/success.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/testdata/test.sub
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/testdata/test2.sub
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/testdata/testuser-api.sqlite
+-rw-r--r--   0 runner    (1001) docker     (127)     5120 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/testdata/testuser.sqlite
+-rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/testdata/testusercache.sqlite
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.980269 edumfa-2.0.2/tests/testdata/trusted_attestation_roots/
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/testdata/trusted_attestation_roots/solokeys_device_attestation_ca.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/testdata/trusted_attestation_roots/yubico_u2f_device_attestation_ca.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/testdata/yubico-oath-long.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/testdata/yubico-oath.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-26 10:25:09.000000 edumfa-2.0.2/tests/testdata/yubico.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:25:15.988269 edumfa-2.0.2/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      768 2024-04-26 10:25:09.000000 edumfa-2.0.2/tools/creategoogleauthenticator-file
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2551 2024-04-26 10:25:09.000000 edumfa-2.0.2/tools/edumfa-authorizedkeys
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1766 2024-04-26 10:25:09.000000 edumfa-2.0.2/tools/edumfa-convert-base32.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2876 2024-04-26 10:25:09.000000 edumfa-2.0.2/tools/edumfa-convert-token
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-26 10:25:09.000000 edumfa-2.0.2/tools/edumfa-convert-token.1
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3230 2024-04-26 10:25:09.000000 edumfa-2.0.2/tools/edumfa-convert-xml-to-csv
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2440 2024-04-26 10:25:09.000000 edumfa-2.0.2/tools/edumfa-create-ad-users
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-26 10:25:09.000000 edumfa-2.0.2/tools/edumfa-create-ad-users.1
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1940 2024-04-26 10:25:09.000000 edumfa-2.0.2/tools/edumfa-create-certificate
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-26 10:25:09.000000 edumfa-2.0.2/tools/edumfa-create-certificate.1
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1985 2024-04-26 10:25:09.000000 edumfa-2.0.2/tools/edumfa-create-pwidresolver-user
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-26 10:25:09.000000 edumfa-2.0.2/tools/edumfa-create-pwidresolver-user.1
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1608 2024-04-26 10:25:09.000000 edumfa-2.0.2/tools/edumfa-create-sqlidresolver-user
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-26 10:25:09.000000 edumfa-2.0.2/tools/edumfa-create-sqlidresolver-user.1
+-rwxr-xr-x   0 runner    (1001) docker     (127)      795 2024-04-26 10:25:09.000000 edumfa-2.0.2/tools/edumfa-create-userdb
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-26 10:25:09.000000 edumfa-2.0.2/tools/edumfa-create-userdb.1
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6823 2024-04-26 10:25:09.000000 edumfa-2.0.2/tools/edumfa-cron
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7030 2024-04-26 10:25:09.000000 edumfa-2.0.2/tools/edumfa-diag
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7372 2024-04-26 10:25:09.000000 edumfa-2.0.2/tools/edumfa-expired-users
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1354 2024-04-26 10:25:09.000000 edumfa-2.0.2/tools/edumfa-export-edumfa-counter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4514 2024-04-26 10:25:09.000000 edumfa-2.0.2/tools/edumfa-export-linotp-counter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3719 2024-04-26 10:25:09.000000 edumfa-2.0.2/tools/edumfa-fetchssh
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-26 10:25:09.000000 edumfa-2.0.2/tools/edumfa-fetchssh.1
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2500 2024-04-26 10:25:09.000000 edumfa-2.0.2/tools/edumfa-fix-access-rights
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-26 10:25:09.000000 edumfa-2.0.2/tools/edumfa-fix-access-rights.1
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4303 2024-04-26 10:25:09.000000 edumfa-2.0.2/tools/edumfa-get-serial
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5191 2024-04-26 10:25:09.000000 edumfa-2.0.2/tools/edumfa-get-unused-tokens
+-rwxr-xr-x   0 runner    (1001) docker     (127)    25353 2024-04-26 10:25:09.000000 edumfa-2.0.2/tools/edumfa-migrate-linotp.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2525 2024-04-26 10:25:09.000000 edumfa-2.0.2/tools/edumfa-pip-update
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-26 10:25:09.000000 edumfa-2.0.2/tools/edumfa-pip-update.1
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5761 2024-04-26 10:25:09.000000 edumfa-2.0.2/tools/edumfa-queue-huey
+-rwxr-xr-x   0 runner    (1001) docker     (127)      643 2024-04-26 10:25:09.000000 edumfa-2.0.2/tools/edumfa-schema-upgrade
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12070 2024-04-26 10:25:09.000000 edumfa-2.0.2/tools/edumfa-standalone
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8168 2024-04-26 10:25:09.000000 edumfa-2.0.2/tools/edumfa-sync-owncloud.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    31000 2024-04-26 10:25:09.000000 edumfa-2.0.2/tools/edumfa-token-janitor
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3746 2024-04-26 10:25:09.000000 edumfa-2.0.2/tools/edumfa-update-counter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5391 2024-04-26 10:25:09.000000 edumfa-2.0.2/tools/edumfa-update-linotp-counter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5471 2024-04-26 10:25:09.000000 edumfa-2.0.2/tools/edumfa-user-action
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4203 2024-04-26 10:25:09.000000 edumfa-2.0.2/tools/edumfa-usercache-cleanup
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1476 2024-04-26 10:25:09.000000 edumfa-2.0.2/tools/getgooglecodes
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3049 2024-04-26 10:25:09.000000 edumfa-2.0.2/tools/reset-edumfa
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-26 10:25:09.000000 edumfa-2.0.2/tools/ssha.py
```

### Comparing `edumfa-2.0.1/AUTHORS.md` & `edumfa-2.0.2/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/LICENSE` & `edumfa-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/PKG-INFO` & `edumfa-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edumfa
-Version: 2.0.1
+Version: 2.0.2
 Summary: eduMFA: identity, multifactor authentication (OTP), authorization, audit
 Home-page: https://www.edumfa.io
 Author: edumfa.io
 Author-email: edumfa@listserv.dfn.de
 License: AGPLv3
 Keywords: OTP,two factor authentication,management,security
 Classifier: Framework :: Flask
@@ -136,16 +136,15 @@
 
 
 
 Setup
 =====
 
 For setting up the system to *run* it, please read install instructions 
-at `edumfa.readthedocs.io <http://edumfa.readthedocs.io/en/latest/installation/index
-.html>`_.
+at `edumfa.readthedocs.io <http://edumfa.readthedocs.io/en/latest/installation/index.html>`_.
 
 If you want to setup a development environment start like this::
 
     git clone https://github.com/edumfa/edumfa.git
     cd edumfa
     virtualenv venv
     source venv/bin/activate
@@ -173,16 +172,15 @@
 submodules, by running::
 
    git pull --recurse-submodules
 
 Running it
 ==========
 
-First You need to create a `config-file <https://edumfa.readthedocs
-.io/en/latest/installation/system/inifile.html>`_.
+First You need to create a `config-file <https://edumfa.readthedocs.io/en/latest/installation/system/inifile.html>`_.
 
 Then create the database tables and the encryption key::
 
     ./edumfa-manage create_tables
     ./edumfa-manage create_enckey
 
 If You want to keep the development database upgradable, You should `stamp
@@ -199,15 +197,15 @@
 
     ./edumfa-manage admin add <username>
 
 Run it::
 
     ./edumfa-manage runserver
 
-Now you can connect to http://localhost:5000 with your browser and login
+Now you can connect to ``http://localhost:5000`` with your browser and login
 as administrator.
 
 Run tests
 =========
 
 If you have followed the steps above to set up your
 `environment for testing <#testing-env>`__, running the test suite should be as
@@ -220,15 +218,15 @@
 
 There are a lot of different ways to contribute to eduMFA, even
 if you are not a developer.
 
 If you found a security vulnerability please report it to us using the reporting form provided by GitHub
 
 You can find detailed information about contributing here:
-https://github.com/eduMFA/eduMFA/blob/master/CONTRIBUTING.md
+https://github.com/eduMFA/eduMFA/blob/main/CONTRIBUTING.md
 
 Code structure
 ==============
 
 The database models are defined in ``models.py`` and tested in 
 tests/test_db_model.py.
```

### Comparing `edumfa-2.0.1/README.rst` & `edumfa-2.0.2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -57,16 +57,15 @@
 
 
 
 Setup
 =====
 
 For setting up the system to *run* it, please read install instructions 
-at `edumfa.readthedocs.io <http://edumfa.readthedocs.io/en/latest/installation/index
-.html>`_.
+at `edumfa.readthedocs.io <http://edumfa.readthedocs.io/en/latest/installation/index.html>`_.
 
 If you want to setup a development environment start like this::
 
     git clone https://github.com/edumfa/edumfa.git
     cd edumfa
     virtualenv venv
     source venv/bin/activate
@@ -94,16 +93,15 @@
 submodules, by running::
 
    git pull --recurse-submodules
 
 Running it
 ==========
 
-First You need to create a `config-file <https://edumfa.readthedocs
-.io/en/latest/installation/system/inifile.html>`_.
+First You need to create a `config-file <https://edumfa.readthedocs.io/en/latest/installation/system/inifile.html>`_.
 
 Then create the database tables and the encryption key::
 
     ./edumfa-manage create_tables
     ./edumfa-manage create_enckey
 
 If You want to keep the development database upgradable, You should `stamp
@@ -120,15 +118,15 @@
 
     ./edumfa-manage admin add <username>
 
 Run it::
 
     ./edumfa-manage runserver
 
-Now you can connect to http://localhost:5000 with your browser and login
+Now you can connect to ``http://localhost:5000`` with your browser and login
 as administrator.
 
 Run tests
 =========
 
 If you have followed the steps above to set up your
 `environment for testing <#testing-env>`__, running the test suite should be as
@@ -141,15 +139,15 @@
 
 There are a lot of different ways to contribute to eduMFA, even
 if you are not a developer.
 
 If you found a security vulnerability please report it to us using the reporting form provided by GitHub
 
 You can find detailed information about contributing here:
-https://github.com/eduMFA/eduMFA/blob/master/CONTRIBUTING.md
+https://github.com/eduMFA/eduMFA/blob/main/CONTRIBUTING.md
 
 Code structure
 ==============
 
 The database models are defined in ``models.py`` and tested in 
 tests/test_db_model.py.
```

### Comparing `edumfa-2.0.1/deploy/apache/sites-available/edumfa.conf` & `edumfa-2.0.2/deploy/apache/sites-available/edumfa.conf`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/deploy/docker-compose-example.yml` & `edumfa-2.0.2/deploy/docker-compose-example.yml`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/deploy/docker-example/edumfa-policy.conf` & `edumfa-2.0.2/deploy/docker-example/edumfa-policy.conf`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/deploy/docker-example/edumfa.cfg` & `edumfa-2.0.2/deploy/docker-example/edumfa.cfg`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/deploy/docker-setup.sh` & `edumfa-2.0.2/deploy/docker-setup.sh`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/deploy/edumfa/dictionary` & `edumfa-2.0.2/deploy/edumfa/dictionary`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/deploy/edumfa/edumfa.cfg` & `edumfa-2.0.2/deploy/edumfa/edumfa.cfg`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/deploy/edumfa_radius.pm` & `edumfa-2.0.2/deploy/edumfa_radius.pm`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/deploy/logging.cfg` & `edumfa-2.0.2/deploy/logging.cfg`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/deploy/nginx/sites-available/edumfa` & `edumfa-2.0.2/deploy/nginx/sites-available/edumfa`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/deploy/rlm_perl.ini` & `edumfa-2.0.2/deploy/rlm_perl.ini`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/deploy/ubuntu/control` & `edumfa-2.0.2/deploy/ubuntu/control`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/deploy/ubuntu/copyright` & `edumfa-2.0.2/deploy/ubuntu/copyright`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/deploy/ubuntu-radius/control` & `edumfa-2.0.2/deploy/ubuntu-radius/control`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/deploy/ubuntu-radius/copyright` & `edumfa-2.0.2/deploy/ubuntu-radius/copyright`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/deploy/ubuntu-radius/edumfa-radius.postinst` & `edumfa-2.0.2/deploy/ubuntu-radius/edumfa-radius.postinst`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/deploy/ubuntu-server/changelog` & `edumfa-2.0.2/deploy/ubuntu-server/changelog`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+edumfa-server (2.0.2{{CODENAME}}) {{CODENAME}}; urgency=medium
+ 
+  * update version number
+
+ -- eduMFA <edumfa-dev@listserv.dfn.de>  Fri, 26 Apr 2024 13:01:00 +0200
+
 edumfa-server (2.0.1{{CODENAME}}) {{CODENAME}}; urgency=medium
  
   * update version number
 
  -- eduMFA <edumfa-dev@listserv.dfn.de>  Fri, 12 Apr 2024 12:01:00 +0200
 
 edumfa-server (2.0.0{{CODENAME}}) {{CODENAME}}; urgency=medium
```

### Comparing `edumfa-2.0.1/deploy/ubuntu-server/control` & `edumfa-2.0.2/deploy/ubuntu-server/control`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/deploy/ubuntu-server/edumfa-apache2.postinst` & `edumfa-2.0.2/deploy/ubuntu-server/edumfa-apache2.postinst`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 fi
 
 USERNAME=edumfa
 CERTDAYS=1095
 CERTKEYSIZE=4096
 MIGRATIONSDIR=/opt/edumfa/lib/edumfa/migrations/
 MYSQLFIX=/etc/mysql/conf.d/edumfa-maxkeylengthfix.cnf
-DB_CREATED=0
+DB_CREATED=false
 
 if test -f /etc/default/edumfa; then
   . /etc/default/edumfa
   # If the daemon user was changed,
   # we set other access rights
   USERNAME=$USER
 fi
@@ -105,15 +105,15 @@
     NPW="$(tr -dc A-Za-z0-9_ < /dev/urandom | head -c12)"
     mysql -u "$USER" --password="$PASSWORD" -e "create database edumfa;" || true
     mysql -u "$USER" --password="$PASSWORD" -e "create user 'edumfa'@'localhost' IDENTIFIED BY '$NPW';"
     mysql -u "$USER" --password="$PASSWORD" -e "grant all privileges on edumfa.* to 'edumfa'@'localhost';"
     echo "SQLALCHEMY_DATABASE_URI = 'mysql+pymysql://edumfa:$NPW@localhost/edumfa?charset=utf8'" >> /etc/edumfa/edumfa.cfg
     echo "DB created"
     /opt/edumfa/bin/edumfa-manage create_tables || true
-    DB_CREATED=1
+    DB_CREATED=true
   fi
 }
 
 enable_apache() {
   a2enmod wsgi headers ssl rewrite
   if [ ! -h /etc/apache2/sites-enabled/edumfa.conf ]; then
     rm -f /etc/apache2/sites-enabled/*
@@ -158,15 +158,15 @@
     adapt_edumfa_cfg
     create_files
     create_database
     enable_apache
     create_certificate
     #update-rc.d apache2 defaults
     service apache2 restart
-    if [ "$DB_CREATED" ]; then
+    if [ "$DB_CREATED" = true ]; then
       # We've created the DB, so we stamp the DB
       touch /tmp/edumfa-install
       /opt/edumfa/bin/edumfa-manage db stamp -d $MIGRATIONSDIR head
     else
       # The DB was already created, so a update might be necessary
       touch /tmp/edumfa-upgrade
       update_db
```

### Comparing `edumfa-2.0.1/deploy/ubuntu-server/edumfa-apache2.postrm` & `edumfa-2.0.2/deploy/ubuntu-server/edumfa-apache2.postrm`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/deploy/ubuntu-server/edumfa-nginx.postinst` & `edumfa-2.0.2/deploy/ubuntu-server/edumfa-nginx.postinst`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 fi
 
 USERNAME=edumfa
 CERTDAYS=1095
 CERTKEYSIZE=4096
 MIGRATIONSDIR=/opt/edumfa/lib/edumfa/migrations/
 MYSQLFIX=/etc/mysql/conf.d/edumfa-maxkeylengthfix.cnf
-DB_CREATED=0
+DB_CREATED=false
 
 
 if test -f /etc/default/edumfa; then
   . /etc/default/edumfa
   # If the daemon user was changed,
   # we set other access rights
   USERNAME=$USER
@@ -106,15 +106,15 @@
     NPW="$(tr -dc A-Za-z0-9_ < /dev/urandom | head -c12)"
     mysql -u "$USER" --password="$PASSWORD" -e "create database edumfa;" || true
     mysql -u "$USER" --password="$PASSWORD" -e "create user 'edumfa'@'localhost' IDENTIFIED BY '$NPW';"
     mysql -u "$USER" --password="$PASSWORD" -e "grant all privileges on edumfa.* to 'edumfa'@'localhost';"
     echo "SQLALCHEMY_DATABASE_URI = 'mysql+pymysql://edumfa:$NPW@localhost/edumfa?charset=utf8'" >> /etc/edumfa/edumfa.cfg
     echo "DB created"
     /opt/edumfa/bin/edumfa-manage create_tables || true
-    DB_CREATED=1
+    DB_CREATED=true
   fi
 }
 
 enable_nginx_uwsgi() {
   rm -f /etc/nginx/sites-enabled/*
   rm -f /etc/uwsgi/apps-enabled/*
   ln -sf /etc/nginx/sites-available/edumfa /etc/nginx/sites-enabled/
@@ -142,15 +142,15 @@
     set_path
     create_user
     adapt_edumfa_cfg
     create_files
     create_database
     enable_nginx_uwsgi
     create_certificate
-    if [ "$DB_CREATED" ]; then
+    if [ "$DB_CREATED" = true ]; then
       # We've created the DB, so we stamp the DB
       /opt/edumfa/bin/edumfa-manage db stamp -d $MIGRATIONSDIR head
     else
       # The DB was already created, so a update might be necessary
       update_db
     fi
     #update-rc.d nginx defaults
```

### Comparing `edumfa-2.0.1/deploy/ubuntu-server/edumfa-nginx.postrm` & `edumfa-2.0.2/deploy/ubuntu-server/edumfa-nginx.postrm`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/deploy/uwsgi/apps-available/edumfa.xml` & `edumfa-2.0.2/deploy/uwsgi/apps-available/edumfa.xml`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/doc/conf.py` & `edumfa-2.0.2/doc/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import functools
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = '2.0.1'
+version = '2.0.2'
 # The full version, including alpha/beta/rc tags.
 #release = '2.16dev5'
 release = version
 
 
 def no_op_wraps(func, assigned=None, updated=None):
     """Replaces functools.wraps in order to undo wrapping.
@@ -54,16 +54,16 @@
 # If your documentation needs a minimal Sphinx version, state it here.
 #needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be extensions
 # coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
 extensions = ['sphinx.ext.autodoc', 'sphinx.ext.imgmath', 'sphinx.ext.viewcode',
               'sphinxcontrib.autohttp.flask', 'sphinxcontrib.plantuml',
-              'sphinxcontrib.spelling', 'sphinx.ext.todo',
-              'pallets_sphinx_themes']
+              'sphinxcontrib.spelling', 'sphinx.ext.todo', 'sphinx_copybutton',
+              'sphinx_inline_tabs']
 http_index_ignore_prefixes = ['/token']
 
 # Add any paths that contain templates here, relative to this directory.
 #templates_path = ['_templates']
 
 # The suffix of source filenames.
 source_suffix = '.rst'
@@ -117,40 +117,43 @@
 # -- Options for HTML output ---------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #html_theme = 'sphinxdoc'
 #html_theme = 'sphinx_rtd_theme'
 #html_theme = 'agogo'
-html_theme = 'flask'
+html_theme = 'furo'
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
-#html_theme_options = {}
+html_theme_options = {
+    "light_logo": "images/edumfa-logo.png",
+    "dark_logo": "images/edumfa-logo-dark.png",
+}
 
 # Add any paths that contain custom themes here, relative to this directory.
 #html_theme_path = ['_themes/flask-sphinx-themes']
 
 
 # The name for this set of Sphinx documents.  If None, it defaults to
 # "<project> v<release> documentation".
 #html_title = None
 
 # A shorter title for the navigation bar.  Default is the same as html_title.
 #html_short_title = None
 
 # The name of an image file (relative to this directory) to place at the top
 # of the sidebar.
-html_logo = "images/eduMFA-logo.png"
+# html_logo = "images/edumfa-logo.png"
 
 # The name of an image file (within the static path) to use as favicon of the
 # docs.  This file should be a Windows icon file (.ico) being 16x16 or 32x32
 # pixels large.
-html_favicon = "images/eduMFA-icon.png"
+html_favicon = "_static/images/edumfa-icon.png"
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ['_static']
 
 html_css_files = [
```

### Comparing `edumfa-2.0.1/edumfa/__init__.py` & `edumfa-2.0.2/edumfa/__init__.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/api/__init__.py` & `edumfa-2.0.2/edumfa/api/__init__.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/api/application.py` & `edumfa-2.0.2/edumfa/api/application.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/api/audit.py` & `edumfa-2.0.2/edumfa/api/audit.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/api/auth.py` & `edumfa-2.0.2/edumfa/api/auth.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/api/before_after.py` & `edumfa-2.0.2/edumfa/api/before_after.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/api/caconnector.py` & `edumfa-2.0.2/edumfa/api/caconnector.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/api/clienttype.py` & `edumfa-2.0.2/edumfa/api/clienttype.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/api/edumfaserver.py` & `edumfa-2.0.2/edumfa/api/edumfaserver.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/api/event.py` & `edumfa-2.0.2/edumfa/api/event.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/api/lib/decorators.py` & `edumfa-2.0.2/edumfa/api/lib/decorators.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/api/lib/policyhelper.py` & `edumfa-2.0.2/edumfa/api/lib/policyhelper.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/api/lib/postpolicy.py` & `edumfa-2.0.2/edumfa/api/lib/postpolicy.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 DEFAULT_PAGE_SIZE = 15
 DEFAULT_TOKENTYPE = "hotp"
 DEFAULT_TIMEOUT_ACTION = "lockscreeen"
 DEFAULT_POLICY_TEMPLATE_URL = "https://raw.githubusercontent.com/edumfa/" \
                               "policy-templates/main/templates/"
 
 
-class postpolicy(object):
+class postpolicy:
     """
     Decorator that allows one to call a specific function after the decorated
     function.
     The postpolicy decorator is to be used in the API calls.
     """
     def __init__(self, function, request=None):
         """
@@ -100,15 +100,15 @@
         def policy_wrapper(*args, **kwds):
             response = wrapped_function(*args, **kwds)
             return self.function(self.request, response, *args, **kwds)
 
         return policy_wrapper
 
 
-class postrequest(object):
+class postrequest:
     """
     Decorator that is supposed to be used with after_request.
     """
     def __init__(self, function, request=None):
         """
         :param function: This is the policy function the is to be called
         :type function: function
```

### Comparing `edumfa-2.0.1/edumfa/api/lib/prepolicy.py` & `edumfa-2.0.2/edumfa/api/lib/prepolicy.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 
 log = logging.getLogger(__name__)
 
 optional = True
 required = False
 
 
-class prepolicy(object):
+class prepolicy:
     """
     This is the decorator wrapper to call a specific function before an API
     call.
     The prepolicy decorator is to be used in the API calls.
     A prepolicy decorator then will modify the request data or raise an
     exception
     """
```

### Comparing `edumfa-2.0.1/edumfa/api/lib/utils.py` & `edumfa-2.0.2/edumfa/api/lib/utils.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/api/machine.py` & `edumfa-2.0.2/edumfa/api/machine.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/api/machineresolver.py` & `edumfa-2.0.2/edumfa/api/machineresolver.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/api/monitoring.py` & `edumfa-2.0.2/edumfa/api/monitoring.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/api/periodictask.py` & `edumfa-2.0.2/edumfa/api/periodictask.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/api/policy.py` & `edumfa-2.0.2/edumfa/api/policy.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/api/radiusserver.py` & `edumfa-2.0.2/edumfa/api/radiusserver.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/api/realm.py` & `edumfa-2.0.2/edumfa/api/realm.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/api/recover.py` & `edumfa-2.0.2/edumfa/api/recover.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/api/register.py` & `edumfa-2.0.2/edumfa/api/register.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/api/resolver.py` & `edumfa-2.0.2/edumfa/api/resolver.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/api/serviceid.py` & `edumfa-2.0.2/edumfa/api/serviceid.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/api/smsgateway.py` & `edumfa-2.0.2/edumfa/api/smsgateway.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/api/smtpserver.py` & `edumfa-2.0.2/edumfa/api/smtpserver.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/api/system.py` & `edumfa-2.0.2/edumfa/api/system.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/api/token.py` & `edumfa-2.0.2/edumfa/api/token.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/api/tokengroup.py` & `edumfa-2.0.2/edumfa/api/tokengroup.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/api/ttype.py` & `edumfa-2.0.2/edumfa/api/ttype.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/api/user.py` & `edumfa-2.0.2/edumfa/api/user.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/api/validate.py` & `edumfa-2.0.2/edumfa/api/validate.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/app.py` & `edumfa-2.0.2/edumfa/app.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/commands/__init__.py` & `edumfa-2.0.2/edumfa/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/commands/manage/__init__.py` & `edumfa-2.0.2/edumfa/commands/manage/__init__.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/commands/manage/admin.py` & `edumfa-2.0.2/edumfa/commands/manage/admin.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/commands/manage/api.py` & `edumfa-2.0.2/edumfa/commands/manage/api.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/commands/manage/audit.py` & `edumfa-2.0.2/edumfa/commands/manage/audit.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/commands/manage/authcache.py` & `edumfa-2.0.2/edumfa/commands/manage/authcache.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/commands/manage/backup.py` & `edumfa-2.0.2/edumfa/commands/manage/backup.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,25 +18,26 @@
 # License along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 import os
 import re
 import sys
 from datetime import datetime
 from shlex import quote as shlex_quote
-from subprocess import Popen, PIPE, call
-from urllib.parse import urlparse
+from subprocess import Popen, PIPE, call, run
 
 import click
 import sqlalchemy
 from flask import current_app
 from flask.cli import AppGroup
 
 backup_cli = AppGroup("backup", help="Perform backup operations")
 
 MYSQL_DIALECTS = ["mysql", "pymysql", "mysql+pymysql", "mariadb+pymysql"]
+PSQL_DIALECTS = ["postgresql+psycopg", "postgresql+psycopg2", "postgresql+pg8000",
+                 "postgresql+asyncpg", "postgresql+psycopg2cffi"]
 
 
 def _write_mysql_defaults(filename, username, password):
     """
     Write the defaults_file for mysql commands
 
     :param filename: THe name of the file
@@ -106,26 +107,33 @@
     sqltype = sqluri.split(":")[0]
     if sqltype == "sqlite":
         productive_file = sqluri[len("sqlite:///"):]
         click.echo("Restore SQLite %s" % productive_file)
         call(["cp", sqlfile, productive_file])
         os.unlink(sqlfile)
     elif sqltype in MYSQL_DIALECTS:
-        parsed_sqluri = sqlalchemy.make_url(sqluri)
+        parsed_sqluri = sqlalchemy.engine.url.make_url(sqluri)
         username = parsed_sqluri.username
         password = parsed_sqluri.password
         hostname = parsed_sqluri.host
         database = parsed_sqluri.database
         defaults_file = "/etc/edumfa/mysql.cnf"
         _write_mysql_defaults(defaults_file, username, password)
         # Rewriting database
         click.echo("Restoring database.")
         call("mysql --defaults-file=%s -h %s %s < %s" % (
             shlex_quote(defaults_file), shlex_quote(hostname), shlex_quote(database), shlex_quote(sqlfile)), shell=True)
         os.unlink(sqlfile)
+    elif sqltype in PSQL_DIALECTS:
+        parsed_sqluri = sqlalchemy.engine.url.make_url(sqluri)
+        env = os.environ.copy()
+        env["PGPASSWORD"] = parsed_sqluri.password
+        cmd = ['psql', '-U', parsed_sqluri.username, '-d', parsed_sqluri.database,
+               '-h', parsed_sqluri.host, '-f', sqlfile]
+        run(cmd, env=env)
     else:
         click.echo("unsupported SQL syntax: %s" % sqltype)
         sys.exit(2)
 
 
 @backup_cli.command("create")
 @click.option("-d", "--directory", "target_dir", type=click.Path(file_okay=False, writable=True),
@@ -156,15 +164,15 @@
         encfile_stat = os.stat(current_app.config.get("EDUMFA_ENCFILE"))
         os.chown(target_dir, encfile_stat.st_uid, encfile_stat.st_gid)
 
     sqlfile = "%s/dbdump-%s.sql" % (target_dir, DATE)
     backup_file = "%s/%s-%s.tgz" % (target_dir, BASE_NAME, DATE)
 
     sqluri = current_app.config.get("SQLALCHEMY_DATABASE_URI")
-    parsed_sqluri = sqlalchemy.make_url(sqluri)
+    parsed_sqluri = sqlalchemy.engine.url.make_url(sqluri)
     sqltype = parsed_sqluri.drivername
 
     if sqltype == "sqlite":
         productive_file = sqluri[len("sqlite:///"):]
         click.echo(f"Backup SQLite {productive_file}")
         sqlfile = "%s/db-%s.sqlite" % (target_dir, DATE)
         call(["cp", productive_file, sqlfile])
@@ -176,14 +184,20 @@
         defaults_file = "{0!s}/mysql.cnf".format(config_dir)
         _write_mysql_defaults(defaults_file, username, password)
         cmd = ['mysqldump', '--defaults-file={!s}'.format(shlex_quote(defaults_file)), '-h', shlex_quote(hostname)]
         if parsed_sqluri.port:
             cmd.extend(['-P', str(parsed_sqluri.port)])
         cmd.extend(['-B', shlex_quote(database), '-r', shlex_quote(sqlfile)])
         call(cmd, shell=False)
+    elif sqltype in PSQL_DIALECTS:
+        env = os.environ.copy()
+        env["PGPASSWORD"] = parsed_sqluri.password
+        cmd = ['pg_dump', '-U', parsed_sqluri.username, '-d', parsed_sqluri.database,
+               '-h', parsed_sqluri.host, '-f', sqlfile]
+        run(cmd, env=env)
     else:
         click.echo(f"unsupported SQL syntax: {sqltype}")
         sys.exit(2)
     enc_file = current_app.config.get("EDUMFA_ENCFILE")
 
     backup_call = ["tar", "-zcf", backup_file, CONF_DIR, sqlfile]
```

### Comparing `edumfa-2.0.1/edumfa/commands/manage/ca.py` & `edumfa-2.0.2/edumfa/commands/manage/ca.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/commands/manage/config.py` & `edumfa-2.0.2/edumfa/commands/manage/config.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/commands/manage/core.py` & `edumfa-2.0.2/edumfa/commands/manage/core.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/commands/manage/event.py` & `edumfa-2.0.2/edumfa/commands/manage/event.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/commands/manage/helper.py` & `edumfa-2.0.2/edumfa/commands/manage/helper.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/commands/manage/hsm.py` & `edumfa-2.0.2/edumfa/commands/manage/hsm.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/commands/manage/main.py` & `edumfa-2.0.2/edumfa/commands/manage/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     click.echo(r"""
                _       __  __ ______      
               | |     |  \/  |  ____/\    
        ___  __| |_   _| \  / | |__ /  \   
       / _ \/ _` | | | | |\/| |  __/ /\ \  
      |  __/ (_| | |_| | |  | | | / ____ \ 
       \___|\__,_|\__,_|_|  |_|_|/_/    \_\ {0!s:>12}
-    """.format('v{0!s}'.format(get_version_number())))
+    """.format('v{0!s}'.format(get_version_number())), err=True)
 
 
 cli.add_command(audit_cli)
 cli.add_command(authcache_cli)
 cli.add_command(admin_cli)
 cli.add_command(api_cli)
 cli.add_command(backup_cli)
```

### Comparing `edumfa-2.0.1/edumfa/commands/manage/policy.py` & `edumfa-2.0.2/edumfa/commands/manage/policy.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/commands/manage/realm.py` & `edumfa-2.0.2/edumfa/commands/manage/realm.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/commands/manage/resolver.py` & `edumfa-2.0.2/edumfa/commands/manage/resolver.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/commands/manage/token.py` & `edumfa-2.0.2/edumfa/commands/manage/token.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/config.py` & `edumfa-2.0.2/edumfa/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 def _random_password(size):
     log.info("SECRET_KEY not set in config. Generating a random key.")
     passwd = [secrets.choice(string.ascii_lowercase + \
                              string.ascii_uppercase + string.digits) for _x in range(size)]
     return "".join(passwd)
 
 
-class Config(object):
+class Config:
     SECRET_KEY = os.environ.get('SECRET_KEY')
     # SQL_ALCHEMY_DATABASE_URI = "mysql://privacyidea:XmbSrlqy5d4IS08zjz"
     # "GG5HTt40Cpf5@localhost/privacyidea"
     EDUMFA_ENCFILE = os.path.join(basedir, "tests/testdata/enckey")
     EDUMFA_HSM = "default"
     EDUMFA_AUDIT_MODULE = "edumfa.lib.auditmodules.sqlaudit"
     EDUMFA_AUDIT_KEY_PRIVATE = os.path.join(basedir, "tests/testdata/private.pem")
```

### Comparing `edumfa-2.0.1/edumfa/lib/__init__.py` & `edumfa-2.0.2/edumfa/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/applications/__init__.py` & `edumfa-2.0.2/edumfa/lib/applications/__init__.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/applications/base.py` & `edumfa-2.0.2/edumfa/lib/applications/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         auth_class = mod.MachineApplication
         mtype = auth_class.application_name
 
         ret[mtype] = auth_class
     return ret
 
 
-class MachineApplication(object):
+class MachineApplication:
 
     application_name = "base"
     '''If bulk_call is false, the administrator may
     only retrieve authentication items for the
     very host he is starting the request.
     '''
     allow_bulk_call = False
```

### Comparing `edumfa-2.0.1/edumfa/lib/applications/luks.py` & `edumfa-2.0.2/edumfa/lib/applications/luks.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/applications/offline.py` & `edumfa-2.0.2/edumfa/lib/applications/offline.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/applications/ssh.py` & `edumfa-2.0.2/edumfa/lib/applications/ssh.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/apps.py` & `edumfa-2.0.2/edumfa/lib/apps.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/audit.py` & `edumfa-2.0.2/edumfa/lib/audit.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/auditmodules/base.py` & `edumfa-2.0.2/edumfa/lib/auditmodules/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 import traceback
 from edumfa.lib.log import log_with
 import datetime
 
 log = logging.getLogger(__name__)
 
 
-class Paginate(object):
+class Paginate:
     """
     This is a pagination object, that is used for searching audit trails.
     """
     def __init__(self):
         # The audit data
         self.auditdata = []
         # The number of the previous page
@@ -69,15 +69,15 @@
         # the number of the current page
         self.current = 1
         self.page = 1
         # the total entry numbers
         self.total = 0
     
 
-class Audit(object):  # pragma: no cover
+class Audit:  # pragma: no cover
 
     is_readable = False
 
     def __init__(self, config=None, startdate=None):
         """
         Create a new audit object.
```

### Comparing `edumfa-2.0.1/edumfa/lib/auditmodules/containeraudit.py` & `edumfa-2.0.2/edumfa/lib/auditmodules/containeraudit.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/auditmodules/loggeraudit.py` & `edumfa-2.0.2/edumfa/lib/auditmodules/loggeraudit.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/auditmodules/sqlaudit.py` & `edumfa-2.0.2/edumfa/lib/auditmodules/sqlaudit.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/auth.py` & `edumfa-2.0.2/edumfa/lib/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 from edumfa.lib.crypto import hash_with_pepper, verify_with_pepper
 from edumfa.lib.utils import fetch_one_resource
 import logging
 
 log = logging.getLogger(__name__)
 
 
-class ROLE(object):
+class ROLE:
     ADMIN = "admin"
     USER = "user"
     VALIDATE = "validate"
 
 
 def verify_db_admin(username, password):
     """
```

### Comparing `edumfa-2.0.1/edumfa/lib/authcache.py` & `edumfa-2.0.2/edumfa/lib/authcache.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/caconnector.py` & `edumfa-2.0.2/edumfa/lib/caconnector.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/caconnectors/baseca.py` & `edumfa-2.0.2/edumfa/lib/caconnectors/baseca.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 This module is tested in tests/test_lib_caconnector.py
 """
 
 # This takes a set of all CA Connector modules.
 AvailableCAConnectors = []
 
 
-class BaseCAConnector(object):
+class BaseCAConnector:
     def revoke_cert(self, certificate, request_id=None, reason=None):
         """
         Revoke the specified certificate. At this point only the database
         index.txt is updated.
 
         :param certificate: The certificate to revoke
         :type certificate: Either takes X509 object or a PEM encoded
```

### Comparing `edumfa-2.0.1/edumfa/lib/caconnectors/caservice_pb2.py` & `edumfa-2.0.2/edumfa/lib/caconnectors/caservice_pb2.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/caconnectors/caservice_pb2_grpc.py` & `edumfa-2.0.2/edumfa/lib/caconnectors/caservice_pb2_grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
 import eduMFA.lib.caconnectors.caservice_pb2 as caservice__pb2
 
 
-class CAServiceStub(object):
+class CAServiceStub:
     """Disposition values:
     0 - Incomplete
     1 - Error
     2 - Denied
     3 - Issued
     4 - Issued out of band
     5 - Under Submission
@@ -55,15 +55,15 @@
         self.GetOptions = channel.unary_unary(
                 '/CAService/GetOptions',
                 request_serializer=caservice__pb2.GetOptionsRequest.SerializeToString,
                 response_deserializer=caservice__pb2.GetOptionsReply.FromString,
                 )
 
 
-class CAServiceServicer(object):
+class CAServiceServicer:
     """Disposition values:
     0 - Incomplete
     1 - Error
     2 - Denied
     3 - Issued
     4 - Issued out of band
     5 - Under Submission
@@ -153,15 +153,15 @@
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'CAService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
-class CAService(object):
+class CAService:
     """Disposition values:
     0 - Incomplete
     1 - Error
     2 - Denied
     3 - Issued
     4 - Issued out of band
     5 - Under Submission
```

### Comparing `edumfa-2.0.1/edumfa/lib/caconnectors/localca.py` & `edumfa-2.0.2/edumfa/lib/caconnectors/localca.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,15 +208,15 @@
             key, value = line.split(":", 1)
             date = value.strip()
             dt = datetime.datetime.strptime(date, "%b %d %X %Y %Z")
             break
     return dt
 
 
-class CONFIG(object):
+class CONFIG:
 
     def __init__(self, name):
         self.directory = "./ca"
         self.keysize = 4096
         self.validity_ca = 1800
         self.validity_cert = 365
         self.crl_days = 30
@@ -234,15 +234,15 @@
 
         CRL validity: {ca.crl_days}
         CRL overlap : {ca.crl_overlap}
         """.format(ca=self)
         return s
 
 
-class ATTR(object):
+class ATTR:
     __doc__ = """This is the list Attributes of the Local CA."""
     CAKEY = "cakey"
     CACERT = "cacert"
     OPENSSL_CNF = "openssl.cnf"
     WORKING_DIR = "WorkingDir"
     CSR_DIR = "CSRDir"
     CERT_DIR = "CertificateDir"
```

### Comparing `edumfa-2.0.1/edumfa/lib/caconnectors/msca.py` & `edumfa-2.0.2/edumfa/lib/caconnectors/msca.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
 CRL_REASONS = ["unspecified", "keyCompromise", "CACompromise",
                "affiliationChanged", "superseded", "cessationOfOperation"]
 
 TIMEOUT = 3
 
 
-class CONFIG(object):  # pragma: no cover
+class CONFIG:  # pragma: no cover
     # Only needed for command line creation
 
     def __init__(self, name):
         self.hostname = "foo.bar"
         self.port = 5000
         self.http_proxy = 0
         self.ca = "hostname\\caname"
@@ -77,15 +77,15 @@
         Connect via HTTP Proxy      : {ca.http_proxy}
         CA               : {ca.ca}
         Use SSL          : {ca.use_ssl}
         """.format(ca=self)
         return s
 
 
-class ATTR(object):
+class ATTR:
     __doc__ = """This is the list Attributes of the Microsoft CA connector."""
     HOSTNAME = "hostname"
     PORT = "port"
     HTTP_PROXY = "http_proxy"
     CA = "ca"
     USE_SSL = "use_ssl"
     SSL_CA_CERT = "ssl_ca_cert"
```

### Comparing `edumfa-2.0.1/edumfa/lib/challenge.py` & `edumfa-2.0.2/edumfa/lib/challenge.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/challengeresponsedecorators.py` & `edumfa-2.0.2/edumfa/lib/challengeresponsedecorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 log = logging.getLogger(__name__)
 
 
 SEED_LENGTH = 16
 
 
-class CHALLENGE_TYPE(object):
+class CHALLENGE_TYPE:
     PIN_RESET = "generic_pin_reset"
     RESYNC = "generic_resync"
 
 
 def _create_challenge(token_obj, challenge_type, message, challenge_data=None):
     validity = int(get_from_config('DefaultChallengeValidityTime', 120))
     if challenge_type == CHALLENGE_TYPE.PIN_RESET:
```

### Comparing `edumfa-2.0.1/edumfa/lib/clientapplication.py` & `edumfa-2.0.2/edumfa/lib/clientapplication.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/config.py` & `edumfa-2.0.2/edumfa/lib/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
 # this is a pointer to the module object instance itself.
 this = sys.modules[__name__]
 
 this.config = {}
 
 
-class SharedConfigClass(object):
+class SharedConfigClass:
     """
     A shared config class object is shared between threads and is supposed
     to store the current configuration with resolvers, realms, policies
     and event handler definitions along with the timestamp of the configuration.
 
     The method ``_reload_from_db()`` compares this timestamp against the
     timestamp in the database (while taking the EDUMFA_CHECK_RELOAD_CONFIG
@@ -194,15 +194,15 @@
         EDUMFA_CHECK_RELOAD_CONFIG setting), reload it if needed and return a
         ``LocalConfigClass`` object containing the current configuration state
         """
         self._reload_from_db()
         return self._clone()
 
 
-class LocalConfigClass(object):
+class LocalConfigClass:
     """
     The Config_Object will contain all database configuration of system
     config, resolvers, realms, policies and event handler definitions.
 
     It will be cloned from the shared config object at the beginning of the
     request and is supposed to stay alive and unchanged during the request.
     """
@@ -266,15 +266,15 @@
                 r_config = r_config > 0
             if isinstance(r_config, str):
                 r_config = is_true(r_config.lower())
 
         return r_config
 
 
-class SYSCONF(object):
+class SYSCONF:
     __doc__ = """This is a list of system config attributes"""
     OVERRIDECLIENT = "OverrideAuthorizationClient"
     PREPENDPIN = "PrependPin"
     SPLITATSIGN = "splitAtSign"
     INCFAILCOUNTER = "IncFailCountOnFalsePin"
     RETURNSAML = "ReturnSamlAttributes"
     RETURNSAMLONFAIL = "ReturnSamlAttributesOnFail"
```

### Comparing `edumfa-2.0.1/edumfa/lib/counter.py` & `edumfa-2.0.2/edumfa/lib/counter.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/crypto.py` & `edumfa-2.0.2/edumfa/lib/crypto.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 DEFAULT_HASH_ALGO_PARAMS = {'argon2__rounds': ROUNDS}
 
 FAILED_TO_DECRYPT_PASSWORD = "FAILED TO DECRYPT PASSWORD!"  # nosec B105 # placeholder in case of error
 
 log = logging.getLogger(__name__)
 
 
-class SecretObj(object):
+class SecretObj:
     def __init__(self, val, iv, preserve=True):
         self.val = val
         self.iv = iv
         self.bkey = None
         self.preserve = preserve
 
     def getKey(self):
@@ -499,15 +499,15 @@
     if hex:
         ret = to_unicode(binascii.hexlify(ret))
     return ret
 
 # some random functions based on geturandom #################################
 
 
-class urandom(object):
+class urandom:
 
     precision = 12
 
     @staticmethod
     def random():
         """
         get random float value between 0.0 and 1.0
@@ -677,15 +677,15 @@
     else:  # pragma: no cover
         raise TypeError('No public key')
 
     # compute m**d (mod n) and compare the two integers
     return msg == pow(sig, pn.e, pn.n)
 
 
-class Sign(object):
+class Sign:
     """
     Signing class that is used to sign Audit Entries and to sign API responses.
     """
     sig_ver = 'rsa_sha256_pss'
 
     def __init__(self, private_key=None, public_key=None, check_private_key=True):
         """
```

### Comparing `edumfa-2.0.1/edumfa/lib/decorators.py` & `edumfa-2.0.2/edumfa/lib/decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
         f_result = func(*args, **kwds)
         return f_result
 
     return user_or_serial_wrapper
 
 
-class check_user_or_serial_in_request(object):
+class check_user_or_serial_in_request:
     """
     Decorator to check user and serial in a request.
     If the request does not contain a serial number (serial) or a user
     (user) it will throw a ParameterError.
     """
     def __init__(self, request):
         self.request = request
```

### Comparing `edumfa-2.0.1/edumfa/lib/edumfaserver.py` & `edumfa-2.0.2/edumfa/lib/edumfaserver.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 module can be tested standalone without any webservices.
 This module is tested in tests/test_lib_edumfaserver.py
 """
 
 log = logging.getLogger(__name__)
 
 
-class eduMFAServer(object):
+class eduMFAServer:
     """
     eduMFA Server object with configuration. The eduMFA Server object
     contains a test functionality so that the configuration can be tested.
     """
 
     def __init__(self, db_edumfaserver_object):
         """
```

### Comparing `edumfa-2.0.1/edumfa/lib/error.py` & `edumfa-2.0.2/edumfa/lib/error.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/event.py` & `edumfa-2.0.2/edumfa/lib/event.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 import functools
 import logging
 log = logging.getLogger(__name__)
 
 AVAILABLE_EVENTS = []
 
 
-class event(object):
+class event:
     """
     This is the event decorator that calls the event handler in the handler
     module. This event decorator can be used at any API call
     """
 
     def __init__(self, eventname, request, g):
         self.eventname = eventname
@@ -253,15 +253,15 @@
     :type event_id: int
     :return:
     """
     event_id = int(event_id)
     return fetch_one_resource(EventHandler, id=event_id).delete()
 
 
-class EventConfiguration(object):
+class EventConfiguration:
     """
     This class is supposed to contain the event handling configuration during
     the Request.
     The currently defined events are fetched from the request-local config object.
     """
 
     def __init__(self):
```

### Comparing `edumfa-2.0.1/edumfa/lib/eventhandler/base.py` & `edumfa-2.0.2/edumfa/lib/eventhandler/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 import re
 import logging
 from edumfa.lib.tokenclass import DATE_FORMAT
 
 log = logging.getLogger(__name__)
 
 
-class CONDITION(object):
+class CONDITION:
     """
     Possible conditions
     """
     TOKEN_HAS_OWNER = "token_has_owner"  # nosec B105 # condition name
     TOKEN_IS_ORPHANED = "token_is_orphaned"  # nosec B105 # condition name
     TOKEN_VALIDITY_PERIOD = "token_validity_period"  # nosec B105 # condition name
     USER_TOKEN_NUMBER = "user_token_number"  # nosec B105 # condition name
@@ -75,26 +75,26 @@
     TOKENRESOLVER = "tokenresolver"
     REALM = "realm"
     RESOLVER = "resolver"
     CLIENT_IP = "client_ip"
     ROLLOUT_STATE = "rollout_state"
 
 
-class GROUP(object):
+class GROUP:
     """
     These are the event handler groups. The conditions
     will be grouped in the UI.
     """
     TOKEN = "token"  # nosec B105 # group name
     GENERAL = "general"
     USER = "user"
     COUNTER = "counter"
 
 
-class BaseEventHandler(object):
+class BaseEventHandler:
     """
     An Eventhandler needs to return a list of actions, which it can handle.
 
     It also returns a list of allowed action and conditions
 
     It returns an identifier, which can be used in the eventhandlig definitions
     """
```

### Comparing `edumfa-2.0.1/edumfa/lib/eventhandler/counterhandler.py` & `edumfa-2.0.2/edumfa/lib/eventhandler/counterhandler.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/eventhandler/customuserattributeshandler.py` & `edumfa-2.0.2/edumfa/lib/eventhandler/customuserattributeshandler.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 import logging
 
 from edumfa.lib.user import User
 
 log = logging.getLogger(__name__)
 
 
-class ACTION_TYPE(object):
+class ACTION_TYPE:
     """
     Allowed actions
     """
     SET_CUSTOM_USER_ATTRIBUTES = "set_custom_user_attributes"
     DELETE_CUSTOM_USER_ATTRIBUTES = "delete_custom_user_attributes"
 
 
-class USER_TYPE(object):
+class USER_TYPE:
     """
     Allowed user types
     """
     TOKENOWNER = "tokenowner"
     LOGGED_IN_USER = "logged_in_user"
```

### Comparing `edumfa-2.0.1/edumfa/lib/eventhandler/federationhandler.py` & `edumfa-2.0.2/edumfa/lib/eventhandler/federationhandler.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 import requests
 from flask import current_app
 
 
 log = logging.getLogger(__name__)
 
 
-class ACTION_TYPE(object):
+class ACTION_TYPE:
     """
     Allowed actions
     """
     FORWARD = "forward"
 
 
 class FederationEventHandler(BaseEventHandler):
```

### Comparing `edumfa-2.0.1/edumfa/lib/eventhandler/logginghandler.py` & `edumfa-2.0.2/edumfa/lib/eventhandler/logginghandler.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 from edumfa.lib.utils import create_tag_dict, to_unicode, is_true
 from edumfa.lib import _
 import logging
 
 log = logging.getLogger(__name__)
 
 
-class LOGGING_LEVEL(object):
+class LOGGING_LEVEL:
     """
     Allowed logging levels
     """
     ERROR = logging.getLevelName(logging.ERROR)
     WARNING = logging.getLevelName(logging.WARNING)
     INFO = logging.getLevelName(logging.INFO)
     DEBUG = logging.getLevelName(logging.DEBUG)
```

### Comparing `edumfa-2.0.1/edumfa/lib/eventhandler/requestmangler.py` & `edumfa-2.0.2/edumfa/lib/eventhandler/requestmangler.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 import yaml
 from dateutil.parser import parse as parse_date_string
 from dateutil.tz import tzlocal
 
 log = logging.getLogger(__name__)
 
 
-class ACTION_TYPE(object):
+class ACTION_TYPE:
     """
     Allowed actions
     """
     SET = "set"
     DELETE = "delete"
```

### Comparing `edumfa-2.0.1/edumfa/lib/eventhandler/responsemangler.py` & `edumfa-2.0.2/edumfa/lib/eventhandler/responsemangler.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 import json
 import logging
 
 
 log = logging.getLogger(__name__)
 
 
-class ACTION_TYPE(object):
+class ACTION_TYPE:
     """
     Allowed actions
     """
     SET = "set"
     DELETE = "delete"
```

### Comparing `edumfa-2.0.1/edumfa/lib/eventhandler/scripthandler.py` & `edumfa-2.0.2/edumfa/lib/eventhandler/scripthandler.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/eventhandler/tokenhandler.py` & `edumfa-2.0.2/edumfa/lib/eventhandler/tokenhandler.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 import yaml
 import json
 from dateutil.tz import tzlocal
 
 log = logging.getLogger(__name__)
 
 
-class ACTION_TYPE(object):
+class ACTION_TYPE:
     """
     Allowed actions
     """
     SET_TOKENREALM = "set tokenrealm"
     DELETE = "delete"
     UNASSIGN = "unassign"
     DISABLE = "disable"
@@ -79,21 +79,21 @@
     CHANGE_FAILCOUNTER = "change failcounter"
     DELETE_TOKENINFO = "delete tokeninfo"
     SET_RANDOM_PIN = "set random pin"
     ADD_TOKENGROUP = "add tokengroup"
     REMOVE_TOKENGROUP = "remove tokengroup"
     ATTACH_APPLICATION = "attach application"
 
-class TOKEN_APPLICATIONS(object):
+class TOKEN_APPLICATIONS:
     SSH = "ssh"
     OFFLINE = "offline"
     LUKS = "luks"
 
 
-class VALIDITY(object):
+class VALIDITY:
     """
     Allowed validity options
     """
     START = "valid from"
     END = "valid till"
```

### Comparing `edumfa-2.0.1/edumfa/lib/eventhandler/usernotification.py` & `edumfa-2.0.2/edumfa/lib/eventhandler/usernotification.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 {action} on your token {serial}.
 
 To check your tokens you may login to the Web UI:
 {url}
 """
 
 
-class NOTIFY_TYPE(object):
+class NOTIFY_TYPE:
     """
     Allowed token owner
     """
     TOKENOWNER = "tokenowner"
     LOGGED_IN_USER = "logged_in_user"
     INTERNAL_ADMIN = "internal admin"
     ADMIN_REALM = "admin realm"
```

### Comparing `edumfa-2.0.1/edumfa/lib/eventhandler/webhookeventhandler.py` & `edumfa-2.0.2/edumfa/lib/eventhandler/webhookeventhandler.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,23 +34,23 @@
 from edumfa.lib.error import UserError
 
 
 log = logging.getLogger(__name__)
 TIMEOUT = 10
 
 
-class CONTENT_TYPE(object):
+class CONTENT_TYPE:
     """
     Allowed type off content
     """
     JSON = "json"
     URLENCODED = "urlendcode"
 
 
-class ACTION_TYPE(object):
+class ACTION_TYPE:
     """
     Allowed actions
     """
     POST_WEBHOOK = "post_webhook"
 
 
 class WebHookHandler(BaseEventHandler):
```

### Comparing `edumfa-2.0.1/edumfa/lib/framework.py` & `edumfa-2.0.2/edumfa/lib/framework.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/importotp.py` & `edumfa-2.0.2/edumfa/lib/importotp.py`

 * *Files 1% similar despite different names*

```diff
@@ -577,15 +577,15 @@
     if abort:
         not_imported_serials = tokens.keys()
         tokens = {}  # reset tokens
 
     return tokens, not_imported_serials
 
 
-class GPGImport(object):
+class GPGImport:
     """
     This class is used to decrypt GPG encrypted import files.
 
     The decrypt method returns the unencrpyted files.
 
     Create the keypair like this:
```

### Comparing `edumfa-2.0.1/edumfa/lib/lifecycle.py` & `edumfa-2.0.2/edumfa/lib/lifecycle.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/log.py` & `edumfa-2.0.2/edumfa/lib/log.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 
         if secured:
             s = "!!!Log Entry Secured by SecureFormatter!!! " + s
 
         return s
 
 
-class log_with(object):
+class log_with:
     """
     Logging decorator that allows you to log with a
     specific logger.
     """
     # Customize these messages
     ENTRY_MESSAGE = 'Entering {0} with arguments {1} and keywords {2}'
     EXIT_MESSAGE = 'Exiting {0} with result {1}'
```

### Comparing `edumfa-2.0.1/edumfa/lib/machine.py` & `edumfa-2.0.2/edumfa/lib/machine.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/machineresolver.py` & `edumfa-2.0.2/edumfa/lib/machineresolver.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/machines/__init__.py` & `edumfa-2.0.2/edumfa/lib/machines/__init__.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/machines/base.py` & `edumfa-2.0.2/edumfa/lib/machines/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 machine ID.
 
 This file is tested in tests/test_lib_machines.py
 """
 import netaddr
 
 
-class Machine(object):
+class Machine:
 
     """
     The Machine object is returned by the resolver for a given machine_id.
     It contains data like the hostname, the ip address and additional
     information like expiry or decommission...
     """
 
@@ -96,15 +96,15 @@
              "id": self.id}
         return d
 
 class MachineResolverError(Exception):
     pass
 
 
-class BaseMachineResolver(object):
+class BaseMachineResolver:
 
     type = "base"
 
     def __init__(self, name, config=None):
         """
 
         :param name: The identifying name of the resolver
```

### Comparing `edumfa-2.0.1/edumfa/lib/machines/hosts.py` & `edumfa-2.0.2/edumfa/lib/machines/hosts.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/machines/ldap.py` & `edumfa-2.0.2/edumfa/lib/machines/ldap.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/monitoringmodules/base.py` & `edumfa-2.0.2/edumfa/lib/monitoringmodules/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 return all available keys, return the last data. 
 """
 import logging
 log = logging.getLogger(__name__)
 from edumfa.lib.log import log_with
 
 
-class Monitoring(object):
+class Monitoring:
 
     def __init__(self, config=None):
         pass
 
     def get_keys(self):
         """
         Return a list of the available statistic keys.
```

### Comparing `edumfa-2.0.1/edumfa/lib/monitoringmodules/sqlstats.py` & `edumfa-2.0.2/edumfa/lib/monitoringmodules/sqlstats.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/monitoringstats.py` & `edumfa-2.0.2/edumfa/lib/monitoringstats.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/passwordreset.py` & `edumfa-2.0.2/edumfa/lib/passwordreset.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/periodictask.py` & `edumfa-2.0.2/edumfa/lib/periodictask.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/pinhandling/base.py` & `edumfa-2.0.2/edumfa/lib/pinhandling/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 It is tested in conjunction with the policy decorator init_random_pin in
 tests/test_api_lib_policy.py
 """
 import logging
 log = logging.getLogger(__name__)
 
 
-class PinHandler(object):
+class PinHandler:
     """
     A PinHandler Class is responsible for handling the OTP PIN during
     enrollment.
 
     It receives the necessary data like
       * the PIN
       * the serial number of the token
```

### Comparing `edumfa-2.0.1/edumfa/lib/policy.py` & `edumfa-2.0.2/edumfa/lib/policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,29 +125,29 @@
 required = False
 
 DEFAULT_ANDROID_APP_URL = "https://play.google.com/store/apps/details?id=it.netknights.piauthenticator"
 DEFAULT_IOS_APP_URL = "https://apps.apple.com/us/app/privacyidea-authenticator/id1445401301"
 DEFAULT_PREFERRED_CLIENT_MODE_LIST = ['interactive', 'webauthn', 'poll', 'u2f']
 
 
-class SCOPE(object):
+class SCOPE:
     __doc__ = """This is the list of the allowed scopes that can be used in
     policy definitions.
     """
     AUTHZ = "authorization"
     ADMIN = "admin"
     AUTH = "authentication"
     AUDIT = "audit"
     USER = "user"   # was selfservice
     ENROLL = "enrollment"
     WEBUI = "webui"
     REGISTER = "register"
 
 
-class ACTION(object):
+class ACTION:
     __doc__ = """This is the list of usual actions."""
     ADMIN_DASHBOARD = "admin_dashboard"
     ASSIGN = "assign"
     APPIMAGEURL = "appimageurl"
     APPLICATION_TOKENTYPE = "application_tokentype"
     AUDIT = "auditlog"
     AUDIT_AGE = "auditlog_age"
@@ -314,26 +314,26 @@
     SERVICEID_LIST = "serviceid_list"
     SERVICEID_ADD = "serviceid_add"
     SERVICEID_DELETE = "serviceid_delete"
     PREFERREDCLIENTMODE = "preferred_client_mode"
     REQUIRE_DESCRIPTION = "require_description"
 
 
-class TYPE(object):
+class TYPE:
     INT = "int"
     STRING = "str"
     BOOL = "bool"
 
 
-class AUTHORIZED(object):
+class AUTHORIZED:
     ALLOW = "grant_access"
     DENY = "deny_access"
 
 
-class GROUP(object):
+class GROUP:
     __doc__ = """These are the allowed policy action groups. The policies
     will be grouped in the UI."""
     TOOLS = "tools"
     SYSTEM = "system"
     TOKEN = "token"  # nosec B105 # group name
     ENROLLMENT = "enrollment"
     GENERAL = "general"
@@ -343,78 +343,78 @@
     MODIFYING_RESPONSE = "modifying response"
     CONDITIONS = "conditions"
     SETTING_ACTIONS = "setting actions"
     TOKENGROUP = "tokengroup"
     SERVICEID = "service ID"
 
 
-class MAIN_MENU(object):
+class MAIN_MENU:
     __doc__ = """These are the allowed top level menu items. These are used
     to toggle the visibility of the menu items depending on the rights of the
     user"""
     TOKENS = "tokens"
     USERS = "users"
     MACHINES = "machines"
     CONFIG = "config"
     AUDIT = "audit"
     COMPONENTS = "components"
 
 
-class LOGINMODE(object):
+class LOGINMODE:
     __doc__ = """This is the list of possible values for the login mode."""
     USERSTORE = "userstore"
     EDUMFA = "eduMFA"
     DISABLE = "disable"
 
 
-class REMOTE_USER(object):
+class REMOTE_USER:
     __doc__ = """The list of possible values for the remote_user policy."""
     DISABLE = "disable"
     ACTIVE = "allowed"
     FORCE = "force"
 
 
-class ACTIONVALUE(object):
+class ACTIONVALUE:
     __doc__ = """This is a list of usual action values for e.g. policy
     action-values like otppin."""
     TOKENPIN = "tokenpin"
     USERSTORE = "userstore"
     DISABLE = "disable"
     NONE = "none"
 
 
-class AUTOASSIGNVALUE(object):
+class AUTOASSIGNVALUE:
     __doc__ = """This is the possible values for autoassign"""
     USERSTORE = "userstore"
     NONE = "any_pin"
 
 
-class TIMEOUT_ACTION(object):
+class TIMEOUT_ACTION:
     __doc__ = """This is a list of actions values for idle users"""
     LOGOUT = "logout"
     LOCKSCREEN = 'lockscreen'
 
 
-class CONDITION_SECTION(object):
+class CONDITION_SECTION:
     __doc__ = """This is a list of available sections for conditions of policies """
     USERINFO = "userinfo"
     TOKENINFO = "tokeninfo"
     TOKEN = "token"  # nosec B105 # section name
     HTTP_REQUEST_HEADER = "HTTP Request header"
     HTTP_ENVIRONMENT = "HTTP Environment"
 
 
-class CONDITION_CHECK(object):
+class CONDITION_CHECK:
     __doc__ = """The available check methods for extended conditions"""
     DO_NOT_CHECK_AT_ALL = 1
     ONLY_CHECK_USERINFO = [CONDITION_SECTION.USERINFO]
     CHECK_AND_RAISE_EXCEPTION_ON_MISSING = None
 
 
-class PolicyClass(object):
+class PolicyClass:
     """
     A policy object can be used to query the current set of policies.
     The policy object itself does not store any policies.
     Instead, every query uses ``get_config_object`` to retrieve the request-local
     config object which contains the current set of policies.
 
     Hence, reloading the request-local config object also reloads the set of policies.
@@ -2615,15 +2615,15 @@
             for comparator, description in COMPARATOR_DESCRIPTIONS.items()}
 
 
 class MatchingError(ServerError):
     pass
 
 
-class Match(object):
+class Match:
     """
     This class provides a high-level API for policy matching.
 
     It should not be instantiated directly. Instead, code should use one of the
     provided classmethods to construct a ``Match`` object. See the respective
     classmethods for details.
```

### Comparing `edumfa-2.0.1/edumfa/lib/policydecorators.py` & `edumfa-2.0.2/edumfa/lib/policydecorators.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 import datetime
 from dateutil.tz import tzlocal
 from edumfa.lib.radiusserver import get_radius
 
 log = logging.getLogger(__name__)
 
 
-class libpolicy(object):
+class libpolicy:
     """
     This is the decorator wrapper to call a specific function before a
     library call in contrast to prepolicy and postpolicy, which are to be
     called in API Calls.
 
     The decorator expects a named parameter "options". In this options dict
     it will look for the flask global "g".
```

### Comparing `edumfa-2.0.1/edumfa/lib/pooling.py` & `edumfa-2.0.2/edumfa/lib/pooling.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 from threading import Lock
 
 from edumfa.lib.framework import get_app_local_store, get_app_config_value
 
 log = logging.getLogger(__name__)
 
 
-class BaseEngineRegistry(object):
+class BaseEngineRegistry:
     """
     Abstract base class for engine registries.
     """
     def get_engine(self, key, creator):
         """
         Return the engine associated with the key ``key``.
         :param key: An arbitrary hashable Python object
```

### Comparing `edumfa-2.0.1/edumfa/lib/queue.py` & `edumfa-2.0.2/edumfa/lib/queue.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 log = logging.getLogger(__name__)
 
 JOB_QUEUE_CLASS = "EDUMFA_JOB_QUEUE_CLASS"
 JOB_QUEUE_OPTION_PREFIX = "EDUMFA_JOB_QUEUE_"
 
 
-class JobCollector(object):
+class JobCollector:
     """
     For most third-party job queue modules, the jobs are discovered by tracking all
     functions decorated with a ``@job`` decorator. However, in order
     to invoke the decorator, one usually needs to provide the queue
     configuration (e.g. the redis server) already.
     In eduMFA, we cannot do that, because the app config is not known
     yet -- it will be known when ``create_app`` is called!
```

### Comparing `edumfa-2.0.1/edumfa/lib/queues/__init__.py` & `edumfa-2.0.2/edumfa/lib/queues/__init__.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/queues/base.py` & `edumfa-2.0.2/edumfa/lib/queues/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 #
 
 
 class QueueError(Exception):
     pass
 
 
-class BaseQueue(object):
+class BaseQueue:
     """
     A queue object represents an external job queue and is configured with
     a dictionary of options.
     It allows to register jobs, which are Python functions that may
     be executed outside of the request lifecycle. Every job is identified by
     a unique job name.
     It then allows to delegate (or "enqueue") an invocation of a job
```

### Comparing `edumfa-2.0.1/edumfa/lib/queues/huey_queue.py` & `edumfa-2.0.2/edumfa/lib/queues/huey_queue.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/radiusserver.py` & `edumfa-2.0.2/edumfa/lib/radiusserver.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 be tested standalone without any webservices.
 This module is tested in tests/test_lib_radiusserver.py
 """
 
 log = logging.getLogger(__name__)
 
 
-class RADIUSServer(object):
+class RADIUSServer:
     """
     RADIUS Server object with configuration. The RADIUS Server object
     contains a test functionality so that the configuration can be tested.
     """
 
     def __init__(self, db_radius_object):
         """
```

### Comparing `edumfa-2.0.1/edumfa/lib/realm.py` & `edumfa-2.0.2/edumfa/lib/realm.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/resolver.py` & `edumfa-2.0.2/edumfa/lib/resolver.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/resolvers/HTTPResolver.py` & `edumfa-2.0.2/edumfa/lib/resolvers/HTTPResolver.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/resolvers/LDAPIdResolver.py` & `edumfa-2.0.2/edumfa/lib/resolvers/LDAPIdResolver.py`

 * *Files 1% similar despite different names*

```diff
@@ -256,15 +256,15 @@
                 "timestamp": now}
 
         return f_result
 
     return cache_wrapper
 
 
-class AUTHTYPE(object):
+class AUTHTYPE:
     SIMPLE = "Simple"
     SASL_DIGEST_MD5 = "SASL Digest-MD5"
     NTLM = "NTLM"
     SASL_KERBEROS = "SASL Kerberos"
 
 
 class IdResolver (UserIdResolver):
```

### Comparing `edumfa-2.0.1/edumfa/lib/resolvers/PasswdIdResolver.py` & `edumfa-2.0.2/edumfa/lib/resolvers/PasswdIdResolver.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/resolvers/SCIMIdResolver.py` & `edumfa-2.0.2/edumfa/lib/resolvers/SCIMIdResolver.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/resolvers/SQLIdResolver.py` & `edumfa-2.0.2/edumfa/lib/resolvers/SQLIdResolver.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/resolvers/UserIdResolver.py` & `edumfa-2.0.2/edumfa/lib/resolvers/UserIdResolver.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 - for /etc/passwd this will be the uid
 - for ldap this might be the DN
 - for SQL the unique index ( what's the right name here (tm))
 
 """
 
 
-class UserIdResolver(object):
+class UserIdResolver:
 
     fields = {"username": 1, "userid": 1,
               "description": 0,
               "phone": 0, "mobile": 0, "email": 0,
               "givenname": 0, "surname": 0, "gender": 0
               }
     name = ""
```

### Comparing `edumfa-2.0.1/edumfa/lib/security/aeshsm.py` & `edumfa-2.0.2/edumfa/lib/security/aeshsm.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/security/default.py` & `edumfa-2.0.2/edumfa/lib/security/default.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     return key
 
 
 def int_list_to_bytestring(int_list):  # pragma: no cover
     return b"".join([bytes((i, )) for i in int_list])
 
 
-class SecurityModule(object):
+class SecurityModule:
     TOKEN_KEY = 0
     CONFIG_KEY = 1
     VALUE_KEY = 2
     DEFAULT_KEY = 3
 
     mapping = {
         'token': TOKEN_KEY,
```

### Comparing `edumfa-2.0.1/edumfa/lib/security/encryptkey.py` & `edumfa-2.0.2/edumfa/lib/security/encryptkey.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/serviceid.py` & `edumfa-2.0.2/edumfa/lib/serviceid.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/smsprovider/FirebaseProvider.py` & `edumfa-2.0.2/edumfa/lib/smsprovider/FirebaseProvider.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/smsprovider/HttpMessageToUidProvider.py` & `edumfa-2.0.2/edumfa/lib/smsprovider/HttpMessageToUidProvider.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/smsprovider/HttpSMSProvider.py` & `edumfa-2.0.2/edumfa/lib/smsprovider/HttpSMSProvider.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/smsprovider/SMSProvider.py` & `edumfa-2.0.2/edumfa/lib/smsprovider/SMSProvider.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         return ret
 
     def __str__(self):
         ret = '{0!s}'.format(self.description)
         return ret
 
 
-class ISMSProvider(object):
+class ISMSProvider:
     """ the SMS Provider Interface - BaseClass """
 
     regexp_description = _("Regular expression to modify the phone number to make it compatible with provider. "
                            "For example to remove pluses and slashes enter something like '/[\\+/]//'.")
 
     def __init__(self, db_smsprovider_object=None, smsgateway=None):
         """
```

### Comparing `edumfa-2.0.1/edumfa/lib/smsprovider/ScriptSMSProvider.py` & `edumfa-2.0.2/edumfa/lib/smsprovider/ScriptSMSProvider.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/smsprovider/SipgateSMSProvider.py` & `edumfa-2.0.2/edumfa/lib/smsprovider/SipgateSMSProvider.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/smsprovider/SmppSMSProvider.py` & `edumfa-2.0.2/edumfa/lib/smsprovider/SmppSMSProvider.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/smsprovider/SmtpSMSProvider.py` & `edumfa-2.0.2/edumfa/lib/smsprovider/SmtpSMSProvider.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/smsprovider/__init__.py` & `edumfa-2.0.2/edumfa/lib/smsprovider/__init__.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/smtpserver.py` & `edumfa-2.0.2/edumfa/lib/smtpserver.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
 log = logging.getLogger(__name__)
 TIMEOUT = 10
 
 SEND_EMAIL_JOB_NAME = "smtpserver.send_email"
 
 
-class SMTPServer(object):
+class SMTPServer:
     """
     SMTP Object that holds a SMTP Database Object but can also send emails.
     """
 
     def __init__(self, db_smtpserver_object):
         """
         Creates a new SMTPServer instance from a DB Server Object
```

### Comparing `edumfa-2.0.1/edumfa/lib/sqlutils.py` & `edumfa-2.0.2/edumfa/lib/sqlutils.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/subscriptions.py` & `edumfa-2.0.2/edumfa/lib/subscriptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,15 +164,15 @@
 
     :param subscription: The dict of the subscription
     :return: True
     """
     return True
 
 
-class CheckSubscription(object):
+class CheckSubscription:
     """
     Decorator to decorate an API request and check if the subscription is valid.
     For this, we evaluate the requesting client.
     If the subscription for this client is not valid, we raise an exception.
     """
 
     def __init__(self, request):
```

### Comparing `edumfa-2.0.1/edumfa/lib/task/base.py` & `edumfa-2.0.2/edumfa/lib/task/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 __doc__ = """This is the base class for a task module.
 
 Tasks may be run periodically. Upon execution, a task
 can be given a set of options.
 """
 
 
-class BaseTask(object):
+class BaseTask:
     """
     A BaseTask returns a list of supported options.
     """
 
     identifier = "BaseTask"
     description = "This is the base class of a task with no functionality"
```

### Comparing `edumfa-2.0.1/edumfa/lib/task/eventcounter.py` & `edumfa-2.0.2/edumfa/lib/task/eventcounter.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/task/simplestats.py` & `edumfa-2.0.2/edumfa/lib/task/simplestats.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/token.py` & `edumfa-2.0.2/edumfa/lib/token.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/tokenclass.py` & `edumfa-2.0.2/edumfa/lib/tokenclass.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,55 +90,55 @@
 
 TWOSTEP_DEFAULT_CLIENTSIZE = 8
 TWOSTEP_DEFAULT_DIFFICULTY = 10000
 
 log = logging.getLogger(__name__)
 
 
-class CHALLENGE_SESSION(object):
+class CHALLENGE_SESSION:
     ENROLLMENT = "enrollment"
 
 
-class TOKENKIND(object):
+class TOKENKIND:
     SOFTWARE = "software"
     HARDWARE = "hardware"
     VIRTUAL = "virtual"
 
 
-class AUTHENTICATIONMODE(object):
+class AUTHENTICATIONMODE:
     AUTHENTICATE = 'authenticate'
     CHALLENGE = 'challenge'
     # If the challenge is answered out of band
     OUTOFBAND = 'outofband'
 
 
-class CLIENTMODE(object):
+class CLIENTMODE:
     """
     This informs eduMFA clients how to
     handle challenge-responses
     """
     INTERACTIVE = 'interactive'
     POLL = 'poll'
     U2F = 'u2f'
     WEBAUTHN = 'webauthn'
 
     
-class ROLLOUTSTATE(object):
+class ROLLOUTSTATE:
     CLIENTWAIT = 'clientwait'
     # The rollout is pending in the backend, like CSRs that need to be approved
     PENDING = 'pending'
     # This means the user needs to authenticate to verify that the token was successfully enrolled.
     VERIFYPENDING = 'verify'
     ENROLLED = 'enrolled'
     BROKEN = 'broken'
     FAILED = 'failed'
     DENIED = 'denied'
 
 
-class TokenClass(object):
+class TokenClass:
 
     # Class properties
     using_pin = True
     hKeyRequired = False
     mode = [AUTHENTICATIONMODE.AUTHENTICATE, AUTHENTICATIONMODE.CHALLENGE]
     client_mode = CLIENTMODE.INTERACTIVE
     # If the token provides means that the user has to prove/verify that the token was successfully enrolled.
```

### Comparing `edumfa-2.0.1/edumfa/lib/tokengroup.py` & `edumfa-2.0.2/edumfa/lib/tokengroup.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/tokens/HMAC.py` & `edumfa-2.0.2/edumfa/lib/tokens/HMAC.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 from edumfa.lib.log import log_with
 from edumfa.lib.crypto import safe_compare
 
 
 log = logging.getLogger(__name__)
 
 
-class HmacOtp(object):
+class HmacOtp:
 
     def __init__(self, secObj=None, counter=0, digits=6, hashfunc=sha1):
         self.secretObj = secObj
         self.counter = int(counter)
         self.digits = digits
         self.hashfunc = hashfunc
```

### Comparing `edumfa-2.0.1/edumfa/lib/tokens/applicationspecificpasswordtoken.py` & `edumfa-2.0.2/edumfa/lib/tokens/applicationspecificpasswordtoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/tokens/certificatetoken.py` & `edumfa-2.0.2/edumfa/lib/tokens/certificatetoken.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     TRUSTED_CA_PATH = "certificate_trusted_Attestation_CA_path"
     REQUIRE_ATTESTATION = "certificate_require_attestation"
     CA_CONNECTOR = "certificate_ca_connector"
     CERTIFICATE_TEMPLATE = "certificate_template"
     CERTIFICATE_REQUEST_SUBJECT_COMPONENT = "certificate_request_subject_component"
 
 
-class REQUIRE_ACTIONS(object):
+class REQUIRE_ACTIONS:
     IGNORE = "ignore"
     VERIFY = "verify"
     REQUIRE_AND_VERIFY = "require_and_verify"
 
 
 def verify_certificate_path(certificate, trusted_ca_paths):
     """
```

### Comparing `edumfa-2.0.1/edumfa/lib/tokens/daplugtoken.py` & `edumfa-2.0.2/edumfa/lib/tokens/daplugtoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/tokens/daypasswordtoken.py` & `edumfa-2.0.2/edumfa/lib/tokens/daypasswordtoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/tokens/emailtoken.py` & `edumfa-2.0.2/edumfa/lib/tokens/emailtoken.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 from edumfa.lib.crypto import safe_compare
 
 
 log = logging.getLogger(__name__)
 TEST_SUCCESSFUL = "Successfully sent email. Please check your inbox."
 
 
-class EMAILACTION(object):
+class EMAILACTION:
     EMAILTEXT = "emailtext"
     EMAILSUBJECT = "emailsubject"
     EMAILAUTO = "emailautosend"
 
 
 class EmailTokenClass(HotpTokenClass):
     """
```

### Comparing `edumfa-2.0.1/edumfa/lib/tokens/foureyestoken.py` & `edumfa-2.0.2/edumfa/lib/tokens/foureyestoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/tokens/hotptoken.py` & `edumfa-2.0.2/edumfa/lib/tokens/hotptoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/tokens/indexedsecrettoken.py` & `edumfa-2.0.2/edumfa/lib/tokens/indexedsecrettoken.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
 log = logging.getLogger(__name__)
 
 DEFAULT_CHALLENGE_TEXT = _("Please enter the positions {0!s} from your secret.")
 DEFAULT_POSITION_COUNT = 2
 
 
-class PIIXACTION(object):
+class PIIXACTION:
     COUNT = "count"
     PRESET_ATTRIBUTE = "preset_attribute"
     FORCE_ATTRIBUTE = "force_attribute"
 
 
 class IndexedSecretTokenClass(TokenClass):
     """
```

### Comparing `edumfa-2.0.1/edumfa/lib/tokens/mOTP.py` & `edumfa-2.0.2/edumfa/lib/tokens/mOTP.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 from edumfa.lib.crypto import zerome, safe_compare
 from edumfa.lib.log import log_with
 
 
 log = logging.getLogger(__name__)
 
 
-class mTimeOtp(object):
+class mTimeOtp:
     '''
     implements the motp timebased check_otp
     - s. https://github.com/neush/otpn900/blob/master/src/test_motp.c
     '''
 
     def __init__(self, secObj=None, secPin=None, oldtime=0, digits=6,
                  key=None, pin=None):
```

### Comparing `edumfa-2.0.1/edumfa/lib/tokens/motptoken.py` & `edumfa-2.0.2/edumfa/lib/tokens/motptoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/tokens/ocra.py` & `edumfa-2.0.2/edumfa/lib/tokens/ocra.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 import struct
 
 SHA_FUNC = {"SHA1": sha1,
             "SHA256": sha256,
             "SHA512": sha512}
 
 
-class OCRASuite(object):
+class OCRASuite:
 
     def __init__(self, ocrasuite):
         """
         Check if the given *ocrasuite* is a valid ocrasuite according to
         chapter 6 of RFC6287.
 
         If it is not a valid OCRA Suite an exception is raised.
@@ -195,15 +195,15 @@
         if not ret:  # pragma: no cover
             raise Exception("OCRA.create_challenge failed. Obviously no good "
                             "challenge_type!")
 
         return ret
 
 
-class OCRA(object):
+class OCRA:
 
     def __init__(self, ocrasuite, key=None, security_object=None):
         """
         Creates an OCRA Object that can be used to calculate OTP response or
         verify a response.
 
         :param ocrasuite: The ocrasuite description
```

### Comparing `edumfa-2.0.1/edumfa/lib/tokens/ocratoken.py` & `edumfa-2.0.2/edumfa/lib/tokens/ocratoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/tokens/papertoken.py` & `edumfa-2.0.2/edumfa/lib/tokens/papertoken.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 from edumfa.lib.policy import SCOPE, ACTION, GROUP
 from edumfa.lib import _
 
 log = logging.getLogger(__name__)
 DEFAULT_COUNT = 100
 
 
-class PAPERACTION(object):
+class PAPERACTION:
     PAPERTOKEN_COUNT = "papertoken_count"
 
 
 class PaperTokenClass(HotpTokenClass):
 
     """
     The Paper Token allows to print out the next e.g. 100 OTP values.
```

### Comparing `edumfa-2.0.1/edumfa/lib/tokens/passwordtoken.py` & `edumfa-2.0.2/edumfa/lib/tokens/passwordtoken.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     This Token can be used for a scenario like losttoken
     """
 
     password_detail_key = "password"  # nosec B105 # key name
     default_length = DEFAULT_LENGTH
     default_contents = DEFAULT_CONTENTS
 
-    class SecretPassword(object):
+    class SecretPassword:
 
         def __init__(self, secObj):
             self.secretObject = secObj
 
         def get_password(self):
             return self.secretObject.getKey()
```

### Comparing `edumfa-2.0.1/edumfa/lib/tokens/pushtoken.py` & `edumfa-2.0.2/edumfa/lib/tokens/pushtoken.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,26 +83,26 @@
 
 # Timedelta in minutes
 POLL_TIME_WINDOW = 1
 UPDATE_FB_TOKEN_WINDOW = 5
 POLL_ONLY = "poll only"
 
 
-class PUSH_ACTION(object):
+class PUSH_ACTION:
     FIREBASE_CONFIG = "push_firebase_configuration"
     REGISTRATION_URL = "push_registration_url"
     TTL = "push_ttl"
     MOBILE_TEXT = "push_text_on_mobile"
     MOBILE_TITLE = "push_title_on_mobile"
     SSL_VERIFY = "push_ssl_verify"
     WAIT = "push_wait"
     ALLOW_POLLING = "push_allow_polling"
 
 
-class PushAllowPolling(object):
+class PushAllowPolling:
     ALLOW = 'allow'
     DENY = 'deny'
     TOKEN = 'token'  # nosec B105 # key name
 
 
 def strip_key(key):
     """
```

### Comparing `edumfa-2.0.1/edumfa/lib/tokens/questionnairetoken.py` & `edumfa-2.0.2/edumfa/lib/tokens/questionnairetoken.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
 log = logging.getLogger(__name__)
 optional = True
 required = False
 DEFAULT_NUM_ANSWERS = 5
 
 
-class QUESTACTION(object):
+class QUESTACTION:
     NUM_QUESTIONS = "number"
 
 
 class QuestionnaireTokenClass(TokenClass):
 
     """
     This is a Questionnaire Token. The token stores a list of questions and
```

### Comparing `edumfa-2.0.1/edumfa/lib/tokens/radiustoken.py` & `edumfa-2.0.2/edumfa/lib/tokens/radiustoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/tokens/registrationtoken.py` & `edumfa-2.0.2/edumfa/lib/tokens/registrationtoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/tokens/remotetoken.py` & `edumfa-2.0.2/edumfa/lib/tokens/remotetoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/tokens/smstoken.py` & `edumfa-2.0.2/edumfa/lib/tokens/smstoken.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 log = logging.getLogger(__name__)
 
 keylen = {'sha1': 20,
           'sha256': 32,
           'sha512': 64}
 
 
-class SMSACTION(object):
+class SMSACTION:
     SMSTEXT = "smstext"
     SMSPOSTCHECKTEXT = "smspostchecktext"
     SMSAUTO = "smsautosend"
     GATEWAYS = "sms_gateways"
 
 
 class SmsTokenClass(HotpTokenClass):
```

### Comparing `edumfa-2.0.1/edumfa/lib/tokens/spasstoken.py` & `edumfa-2.0.2/edumfa/lib/tokens/spasstoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/tokens/sshkeytoken.py` & `edumfa-2.0.2/edumfa/lib/tokens/sshkeytoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/tokens/tantoken.py` & `edumfa-2.0.2/edumfa/lib/tokens/tantoken.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 from edumfa.lib.crypto import geturandom, hash
 
 log = logging.getLogger(__name__)
 DEFAULT_COUNT = 100
 SALT_LENGTH = 4
 
 
-class TANACTION(object):
+class TANACTION:
     TANTOKEN_COUNT = "tantoken_count"
 
 
 class TanTokenClass(PaperTokenClass):
     """
     The TAN token allows to print out the next e.g. 100 OTP values.
     This sheet of paper can be used to authenticate and strike out the used
```

### Comparing `edumfa-2.0.1/edumfa/lib/tokens/tiqrtoken.py` & `edumfa-2.0.2/edumfa/lib/tokens/tiqrtoken.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
 optional = True
 required = False
 
 
 OCRA_DEFAULT_SUITE = "OCRA-1:HOTP-SHA1-6:QN10"
 
 
-class API_ACTIONS(object):
+class API_ACTIONS:
     METADATA = "metadata"
     ENROLLMENT = "enrollment"
     AUTHENTICATION = "authentication"
     ALLOWED_ACTIONS = [METADATA, ENROLLMENT, AUTHENTICATION]
 
 
 class TiqrTokenClass(OcraTokenClass):
```

### Comparing `edumfa-2.0.1/edumfa/lib/tokens/totptoken.py` & `edumfa-2.0.2/edumfa/lib/tokens/totptoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/tokens/u2f.py` & `edumfa-2.0.2/edumfa/lib/tokens/u2f.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/tokens/u2ftoken.py` & `edumfa-2.0.2/edumfa/lib/tokens/u2ftoken.py`

 * *Files 0% similar despite different names*

```diff
@@ -190,15 +190,15 @@
 U2F_Version = "U2F_V2"
 
 log = logging.getLogger(__name__)
 optional = True
 required = False
 
 
-class U2FACTION(object):
+class U2FACTION:
     FACETS = "u2f_facets"
     REQ = "u2f_req"
     NO_VERIFY_CERT = "u2f_no_verify_certificate"
 
 
 class U2fTokenClass(TokenClass):
     """
```

### Comparing `edumfa-2.0.1/edumfa/lib/tokens/vasco.py` & `edumfa-2.0.2/edumfa/lib/tokens/vasco.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/tokens/vascotoken.py` & `edumfa-2.0.2/edumfa/lib/tokens/vascotoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/tokens/webauthn.py` & `edumfa-2.0.2/edumfa/lib/tokens/webauthn.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,27 +91,27 @@
 # Default authenticator extensions
 #
 DEFAULT_AUTHENTICATOR_EXTENSIONS = {"credProtect": None}
 
 log = logging.getLogger(__name__)
 
 
-class COSE_PUBLIC_KEY(object):
+class COSE_PUBLIC_KEY:
     """
     The indices of the various parameters in a COSE-formatted public key.
     """
 
     ALG = 3
     X = -2
     Y = -3
     E = -2
     N = -1
 
 
-class ATTESTATION_TYPE(object):
+class ATTESTATION_TYPE:
     """
     Attestation types known to this implementation.
     """
 
     BASIC = 'Basic'
     ECDAA = 'ECDAA'
     NONE = 'None'
@@ -123,15 +123,15 @@
 SUPPORTED_ATTESTATION_TYPES = (
     ATTESTATION_TYPE.BASIC,
     ATTESTATION_TYPE.NONE,
     ATTESTATION_TYPE.SELF_ATTESTATION
 )
 
 
-class ATTESTATION_FORMAT(object):
+class ATTESTATION_FORMAT:
     """
     Attestation format identifiers as registered in the IANA WebAuthn attestation statement format identifiers registry.
     """
 
     PACKED = 'packed'
     TPM = 'tpm'
     ANDROID_KEY = 'android-key'
@@ -157,30 +157,30 @@
     ATTESTATION_FORMAT.ANDROID_SAFETYNET,
     ATTESTATION_FORMAT.APPLE,
     ATTESTATION_FORMAT.FIDO_U2F,
     ATTESTATION_FORMAT.NONE
 )
 
 
-class CLIENT_DATA_TYPE(object):
+class CLIENT_DATA_TYPE:
     """
     Client data types used by this implementation.
     """
 
     CREATE = 'webauthn.create'
     GET = 'webauthn.get'
 
 
 SUPPORTED_CLIENT_DATA_TYPES = (
     CLIENT_DATA_TYPE.CREATE,
     CLIENT_DATA_TYPE.GET
 )
 
 
-class COSE_ALGORITHM(object):
+class COSE_ALGORITHM:
     """
     IANA-assigned identifiers of supported COSE algorithms.
     """
 
     ES256 = -7
     PS256 = -37
     RS256 = -257
@@ -190,15 +190,15 @@
 SUPPORTED_COSE_ALGORITHMS = (
     COSE_ALGORITHM.ES256,
     COSE_ALGORITHM.PS256,
     COSE_ALGORITHM.RS256,
 )
 
 
-class ATTESTATION_FORM(object):
+class ATTESTATION_FORM:
     """
     The different forms of attestation.
     """
 
     NONE = 'none'
     INDIRECT = 'indirect'
     DIRECT = 'direct'
@@ -207,15 +207,15 @@
 ATTESTATION_FORMS = (
     ATTESTATION_FORM.NONE,
     ATTESTATION_FORM.INDIRECT,
     ATTESTATION_FORM.DIRECT
 )
 
 
-class USER_VERIFICATION_LEVEL(object):
+class USER_VERIFICATION_LEVEL:
     """
     The different levels of user verification.
     """
 
     REQUIRED = 'required'
     PREFERRED = 'preferred'
     DISCOURAGED = 'discouraged'
@@ -224,15 +224,15 @@
 USER_VERIFICATION_LEVELS = (
     USER_VERIFICATION_LEVEL.REQUIRED,
     USER_VERIFICATION_LEVEL.PREFERRED,
     USER_VERIFICATION_LEVEL.DISCOURAGED
 )
 
 
-class ATTESTATION_LEVEL(object):
+class ATTESTATION_LEVEL:
     """
     The different levels of attestation requirement.
     """
 
     TRUSTED = 'trusted'
     UNTRUSTED = 'untrusted'
     NONE = 'none'
@@ -264,30 +264,30 @@
 ATTESTATION_REQUIREMENT_LEVELS = (
     ATTESTATION_REQUIREMENT_LEVEL[ATTESTATION_LEVEL.TRUSTED],
     ATTESTATION_REQUIREMENT_LEVEL[ATTESTATION_LEVEL.UNTRUSTED],
     ATTESTATION_REQUIREMENT_LEVEL[ATTESTATION_LEVEL.NONE]
 )
 
 
-class AUTHENTICATOR_ATTACHMENT_TYPE(object):
+class AUTHENTICATOR_ATTACHMENT_TYPE:
     """
     The different types of authenticator attachment.
     """
 
     PLATFORM = 'platform'
     CROSS_PLATFORM = 'cross-platform'
 
 
 AUTHENTICATOR_ATTACHMENT_TYPES = (
     AUTHENTICATOR_ATTACHMENT_TYPE.PLATFORM,
     AUTHENTICATOR_ATTACHMENT_TYPE.CROSS_PLATFORM
 )
 
 
-class TRANSPORT(object):
+class TRANSPORT:
     """
     The standard transports.
     """
 
     USB = 'usb'
     BLE = 'ble'
     NFC = 'nfc'
@@ -297,41 +297,41 @@
 TRANSPORTS = (
     TRANSPORT.USB,
     TRANSPORT.BLE,
     TRANSPORT.NFC,
     TRANSPORT.INTERNAL,
 )
 
-class RESIDENT_KEY_LEVEL(object):
+class RESIDENT_KEY_LEVEL:
     """
     The different resident key levels
     """
     DISCOURAGED = 'discouraged'
     REQUIRED = 'required'
     PREFERRED = 'preferred'
 
 RESIDENT_KEY_LEVELS = (
     RESIDENT_KEY_LEVEL.DISCOURAGED,
     RESIDENT_KEY_LEVEL.REQUIRED,
     RESIDENT_KEY_LEVEL.PREFERRED
 )
 
-class USERNAMELESS_AUTHN(object):
+class USERNAMELESS_AUTHN:
     """
     Whether to allow username-less authentication.
     """
     ENABLED = True
     DISABLED = False
 
 USERNAMELESS_AUTHNS = (
     USERNAMELESS_AUTHN.ENABLED,
     USERNAMELESS_AUTHN.DISABLED
 )
 
-class USERNAMELESS_REALM_POLICY(object):
+class USERNAMELESS_REALM_POLICY:
     """
     Whether to enable realm-specific policies in username-less authentication scenarios.
     """
     ENABLED = True
     DISABLED = False
 
 USERNAMELESS_REALM_POLICYS = (
@@ -367,15 +367,15 @@
     """
     The user data is missing.
     """
 
     pass
 
 
-class AuthenticatorDataFlags(object):
+class AuthenticatorDataFlags:
     """
     Authenticator data flags:
 
     https://www.w3.org/TR/webauthn/#authenticator-data
     """
 
     USER_PRESENT = 1 << 0
@@ -428,15 +428,15 @@
         :return: Whether the authenticator response included extension data.
         :rtype: bool
         """
 
         return (self.flags & self.EXTENSION_DATA_INCLUDED) == self.EXTENSION_DATA_INCLUDED
 
 
-class WebAuthnMakeCredentialOptions(object):
+class WebAuthnMakeCredentialOptions:
     """
     Generate the options passed to navigator.credentials.create()
     """
 
     def __init__(self,
                  challenge,
                  rp_name,
@@ -600,15 +600,15 @@
         :return: The publicKeyCredentialCreationOptions dictionary encoded as JSON.
         :rtype: basestring
         """
 
         return json.dumps(self.registration_dict)
 
 
-class WebAuthnAssertionOptions(object):
+class WebAuthnAssertionOptions:
     """
     Generate the options passed to navigator.credentials.get()
     """
 
     def __init__(self,
                  challenge,
                  webauthn_user,
@@ -721,15 +721,15 @@
         :return: The publicKeyCredentialRequestOptions dictionary encoded as JSON.
         :rtype: basestring
         """
 
         return json.dumps(self.assertion_dict)
 
 
-class WebAuthnUser(object):
+class WebAuthnUser:
     """
     A single WebAuthn user credential.
     """
 
     def __init__(self,
                  user_id,
                  user_name,
@@ -779,15 +779,15 @@
         self.rp_id = rp_id
 
     def __str__(self):
         return '{!r} ({}, {}, {})'.format(self.user_id, self.user_name,
                                           self.user_display_name, self.sign_count)
 
 
-class WebAuthnCredential(object):
+class WebAuthnCredential:
     """
     A single WebAuthn credential.
     """
 
     def __init__(self,
                  rp_id,
                  origin,
@@ -852,15 +852,15 @@
         return not ATTESTATION_REQUIREMENT_LEVEL[self.attestation_level]['self_attestation_permitted']
 
     def __str__(self):
         return '{!r} ({}, {}, {})'.format(self.credential_id, self.rp_id,
                                           self.origin, self.sign_count)
 
 
-class WebAuthnRegistrationResponse(object):
+class WebAuthnRegistrationResponse:
     """
     The WebAuthn registration response containing all information needed to verify the registration ceremony.
     """
 
     def __init__(self,
                  rp_id,
                  origin,
@@ -1593,15 +1593,15 @@
                 raise RegistrationRejectedException('No (or unsupported) attestation certificate.')
             return credential
 
         except Exception as e:
             raise RegistrationRejectedException('Registration rejected. Error: {}'.format(e))
 
 
-class WebAuthnAssertionResponse(object):
+class WebAuthnAssertionResponse:
     """
     The WebAuthn assertion response containing all information needed to verify the authentication ceremony.
     """
 
     def __init__(self,
                  webauthn_user,
                  assertion_response,
```

### Comparing `edumfa-2.0.1/edumfa/lib/tokens/webauthntoken.py` & `edumfa-2.0.2/edumfa/lib/tokens/webauthntoken.py`

 * *Files 0% similar despite different names*

```diff
@@ -490,15 +490,15 @@
 PUBKEY_CRED_ALGORITHMS_ORDER = ['ecdsa', 'rsassa-pss', 'rsassa-pkcs1v1_5']
 
 log = logging.getLogger(__name__)
 optional = True
 required = False
 
 
-class WEBAUTHNCONFIG(object):
+class WEBAUTHNCONFIG:
     """
     Config options defined for WebAuthn
     """
 
     TRUST_ANCHOR_DIR = 'webauthn.trust_anchor_dir'
     APP_ID = 'webauthn.appid'
     CHALLENGE_VALIDITY_TIME = 'WebauthnChallengeValidityTime'
@@ -506,15 +506,15 @@
 
 WEBAUTHN_TOKEN_SPECIFIC_SETTINGS = {
     WEBAUTHNCONFIG.TRUST_ANCHOR_DIR: 'public',
     WEBAUTHNCONFIG.APP_ID: 'public'
 }
 
 
-class WEBAUTHNACTION(object):
+class WEBAUTHNACTION:
     """
     Policy actions defined for WebAuthn
     """
 
     ALLOWED_TRANSPORTS = 'webauthn_allowed_transports'
     TIMEOUT = 'webauthn_timeout'
     RELYING_PARTY_NAME = 'webauthn_relying_party_name'
@@ -529,15 +529,15 @@
     USERNAMELESS_AUTHN = 'webauthn_usernameless_authn'
     USERNAMELESS_REALM_POLICY = 'webauthn_usernameless_realm_policy'
     TOKENLABEL = 'webauthn_tokenlabel'
     REQ = 'webauthn_req'
     AVOID_DOUBLE_REGISTRATION = 'webauthn_avoid_double_registration'
 
 
-class WEBAUTHNINFO(object):
+class WEBAUTHNINFO:
     """
     Token info fields used by WebAuthn
     """
 
     PUB_KEY = "pubKey"
     ORIGIN = "origin"
     AAGUID = "aaguid"
@@ -546,15 +546,15 @@
     ATTESTATION_SERIAL = "attestation_serial"
     ATTESTATION_SUBJECT = "attestation_subject"
     RELYING_PARTY_ID = "relying_party_id"
     RELYING_PARTY_NAME = "relying_party_name"
     RESIDENT_KEY = "resident_key"
 
 
-class WEBAUTHNGROUP(object):
+class WEBAUTHNGROUP:
     """
     Categories used to group WebAuthn token actions.
     """
 
     WEBAUTHN = "WebAuthn"
```

### Comparing `edumfa-2.0.1/edumfa/lib/tokens/yubicotoken.py` & `edumfa-2.0.2/edumfa/lib/tokens/yubicotoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/tokens/yubikeytoken.py` & `edumfa-2.0.2/edumfa/lib/tokens/yubikeytoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/user.py` & `edumfa-2.0.2/edumfa/lib/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 from .config import get_from_config, SYSCONF
 from .usercache import (user_cache, cache_username, user_init, delete_user_cache)
 from edumfa.models import CustomUserAttribute, db
 
 log = logging.getLogger(__name__)
 
 
-class User(object):
+class User:
     """
     The user has the attributes
       login, realm and resolver.
     Usually a user can be found via "login@realm".
     
     A user object with an empty login and realm should not exist,
     whereas a user object could have an empty resolver.
```

### Comparing `edumfa-2.0.1/edumfa/lib/usercache.py` & `edumfa-2.0.2/edumfa/lib/usercache.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from edumfa.models import UserCache, db
 from sqlalchemy import and_
 
 log = logging.getLogger(__name__)
 EXPIRATION_SECONDS = "UserCacheExpiration"
 
 
-class user_cache(object):
+class user_cache:
     """
     This is the decorator wrapper to call a specific resolver function to
     allow user caching.
     If the user cache is disabled, the decorator wrapper is not called and
     the original function's result is returned instead.
     """
```

### Comparing `edumfa-2.0.1/edumfa/lib/utils/__init__.py` & `edumfa-2.0.2/edumfa/lib/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/lib/utils/compare.py` & `edumfa-2.0.2/edumfa/lib/utils/compare.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,15 +148,15 @@
         return not func(left, comparator, right)
     return negated
 
 
 #: This class enumerates all available comparators.
 #: In order to add a comparator to this module, add a suitable member to COMPARATORS
 #: and suitable entries to COMPARATOR_FUNCTIONS and COMPARATOR_DESCRIPTIONS.
-class COMPARATORS(object):
+class COMPARATORS:
     EQUALS = "equals"
     NOT_EQUALS = "!equals"
 
     CONTAINS = "contains"
     NOT_CONTAINS = "!contains"
 
     MATCHES = "matches"
```

### Comparing `edumfa-2.0.1/edumfa/lib/utils/export.py` & `edumfa-2.0.2/edumfa/lib/utils/export.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/messages.pot` & `edumfa-2.0.2/edumfa/messages.pot`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/models.py` & `edumfa-2.0.2/edumfa/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 @compiles(CreateSequence, 'mariadb')
 def increment_by_zero(element, compiler, **kw):  # pragma: no cover
     text = compiler.visit_create_sequence(element, **kw)
     text = text + " INCREMENT BY 0"
     return text
 
 
-class MethodsMixin(object):
+class MethodsMixin:
     """
     This class mixes in some common Class table functions like
     delete and save
     """
 
     def save(self):
         db.session.add(self)
@@ -118,15 +118,15 @@
         # the current request-local config object. The next access to the config
         # during this request will reload the config from the database and create
         # a new request-local config object, which holds the *new* config.
         from edumfa.lib.config import invalidate_config_object
         invalidate_config_object()
 
 
-class TimestampMethodsMixin(object):
+class TimestampMethodsMixin:
     """
     This class mixes in the table functions including update of the timestamp
     """
 
     def save(self):
         db.session.add(self)
         save_config_timestamp()
```

### Comparing `edumfa-2.0.1/edumfa/static/README.md` & `edumfa-2.0.2/edumfa/static/README.md`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/app.js` & `edumfa-2.0.2/edumfa/static/app.js`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/audit/controllers/auditControllers.js` & `edumfa-2.0.2/edumfa/static/components/audit/controllers/auditControllers.js`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/audit/factories/audit.js` & `edumfa-2.0.2/edumfa/static/components/audit/factories/audit.js`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/audit/states/states.js` & `edumfa-2.0.2/edumfa/static/components/audit/states/states.js`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/audit/views/audit.html` & `edumfa-2.0.2/edumfa/static/components/audit/views/audit.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/audit/views/audit.log.html` & `edumfa-2.0.2/edumfa/static/components/audit/views/audit.log.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/components/controllers/componentControllers.js` & `edumfa-2.0.2/edumfa/static/components/components/controllers/componentControllers.js`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/components/factories/component.js` & `edumfa-2.0.2/edumfa/static/components/components/factories/component.js`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/components/states/states.js` & `edumfa-2.0.2/edumfa/static/components/components/states/states.js`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/components/views/component.clienttype.html` & `edumfa-2.0.2/edumfa/static/components/components/views/component.clienttype.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/components/views/component.html` & `edumfa-2.0.2/edumfa/static/components/components/views/component.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/config/controllers/configControllers.js` & `edumfa-2.0.2/edumfa/static/components/config/controllers/configControllers.js`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/config/controllers/eduMfaServerController.js` & `edumfa-2.0.2/edumfa/static/components/config/controllers/eduMfaServerController.js`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/config/controllers/eventController.js` & `edumfa-2.0.2/edumfa/static/components/config/controllers/eventController.js`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/config/controllers/ldapMachineResolverController.js` & `edumfa-2.0.2/edumfa/static/components/config/controllers/ldapMachineResolverController.js`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/config/controllers/periodicTaskController.js` & `edumfa-2.0.2/edumfa/static/components/config/controllers/periodicTaskController.js`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/config/controllers/radiusServerController.js` & `edumfa-2.0.2/edumfa/static/components/config/controllers/radiusServerController.js`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/config/controllers/serviceidController.js` & `edumfa-2.0.2/edumfa/static/components/config/controllers/serviceidController.js`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/config/controllers/smsgatewayController.js` & `edumfa-2.0.2/edumfa/static/components/config/controllers/smsgatewayController.js`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/config/controllers/smtpServerController.js` & `edumfa-2.0.2/edumfa/static/components/config/controllers/smtpServerController.js`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/config/controllers/tokengroupController.js` & `edumfa-2.0.2/edumfa/static/components/config/controllers/tokengroupController.js`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/config/factories/config.js` & `edumfa-2.0.2/edumfa/static/components/config/factories/config.js`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/config/states/states.js` & `edumfa-2.0.2/edumfa/static/components/config/states/states.js`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/config/views/config.caconnectors.list.html` & `edumfa-2.0.2/edumfa/static/components/config/views/config.caconnectors.list.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/config/views/config.caconnectors.local.html` & `edumfa-2.0.2/edumfa/static/components/config/views/config.caconnectors.local.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/config/views/config.caconnectors.microsoft.html` & `edumfa-2.0.2/edumfa/static/components/config/views/config.caconnectors.microsoft.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/config/views/config.edumfaserver.edit.html` & `edumfa-2.0.2/edumfa/static/components/config/views/config.edumfaserver.edit.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/config/views/config.edumfaserver.list.html` & `edumfa-2.0.2/edumfa/static/components/config/views/config.edumfaserver.list.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/config/views/config.events.details.html` & `edumfa-2.0.2/edumfa/static/components/config/views/config.events.details.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/config/views/config.events.html` & `edumfa-2.0.2/edumfa/static/components/config/views/config.events.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/config/views/config.events.list.html` & `edumfa-2.0.2/edumfa/static/components/config/views/config.events.list.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/config/views/config.html` & `edumfa-2.0.2/edumfa/static/components/config/views/config.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/config/views/config.machineresolvers.html` & `edumfa-2.0.2/edumfa/static/components/config/views/config.machineresolvers.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/config/views/config.mresolvers.hosts.html` & `edumfa-2.0.2/edumfa/static/components/config/views/config.mresolvers.hosts.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/config/views/config.mresolvers.ldap.html` & `edumfa-2.0.2/edumfa/static/components/config/views/config.mresolvers.ldap.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/config/views/config.mresolvers.list.html` & `edumfa-2.0.2/edumfa/static/components/config/views/config.mresolvers.list.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/config/views/config.periodictasks.details.html` & `edumfa-2.0.2/edumfa/static/components/config/views/config.periodictasks.details.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/config/views/config.periodictasks.html` & `edumfa-2.0.2/edumfa/static/components/config/views/config.periodictasks.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/config/views/config.periodictasks.list.html` & `edumfa-2.0.2/edumfa/static/components/config/views/config.periodictasks.list.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/config/views/config.policies.details.html` & `edumfa-2.0.2/edumfa/static/components/config/views/config.policies.details.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/config/views/config.policies.html` & `edumfa-2.0.2/edumfa/static/components/config/views/config.policies.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/config/views/config.policies.list.html` & `edumfa-2.0.2/edumfa/static/components/config/views/config.policies.list.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/config/views/config.radius.edit.html` & `edumfa-2.0.2/edumfa/static/components/config/views/config.radius.edit.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/config/views/config.radius.list.html` & `edumfa-2.0.2/edumfa/static/components/config/views/config.radius.list.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/config/views/config.realms.html` & `edumfa-2.0.2/edumfa/static/components/config/views/config.realms.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/config/views/config.realms.list.html` & `edumfa-2.0.2/edumfa/static/components/config/views/config.realms.list.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/config/views/config.resolvers.html` & `edumfa-2.0.2/edumfa/static/components/config/views/config.resolvers.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/config/views/config.resolvers.http.html` & `edumfa-2.0.2/edumfa/static/components/config/views/config.resolvers.http.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/config/views/config.resolvers.ldap.html` & `edumfa-2.0.2/edumfa/static/components/config/views/config.resolvers.ldap.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/config/views/config.resolvers.list.html` & `edumfa-2.0.2/edumfa/static/components/config/views/config.resolvers.list.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/config/views/config.resolvers.passwd.html` & `edumfa-2.0.2/edumfa/static/components/config/views/config.resolvers.passwd.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/config/views/config.resolvers.scim.html` & `edumfa-2.0.2/edumfa/static/components/config/views/config.resolvers.scim.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/config/views/config.resolvers.sql.html` & `edumfa-2.0.2/edumfa/static/components/config/views/config.resolvers.sql.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/config/views/config.serviceid.edit.html` & `edumfa-2.0.2/edumfa/static/components/config/views/config.serviceid.edit.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/config/views/config.serviceid.list.html` & `edumfa-2.0.2/edumfa/static/components/config/views/config.serviceid.list.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/config/views/config.smsgateway.edit.html` & `edumfa-2.0.2/edumfa/static/components/config/views/config.smsgateway.edit.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/config/views/config.smsgateway.list.html` & `edumfa-2.0.2/edumfa/static/components/config/views/config.smsgateway.list.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/config/views/config.smtp.edit.html` & `edumfa-2.0.2/edumfa/static/components/config/views/config.smtp.edit.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/config/views/config.smtp.list.html` & `edumfa-2.0.2/edumfa/static/components/config/views/config.smtp.list.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/config/views/config.system.edit.html` & `edumfa-2.0.2/edumfa/static/components/config/views/config.system.edit.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/config/views/config.system.html` & `edumfa-2.0.2/edumfa/static/components/config/views/config.system.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/config/views/config.token.daypassword.html` & `edumfa-2.0.2/edumfa/static/components/config/views/config.token.daypassword.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/config/views/config.token.email.html` & `edumfa-2.0.2/edumfa/static/components/config/views/config.token.email.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/config/views/config.token.hotp.html` & `edumfa-2.0.2/edumfa/static/components/config/views/config.token.hotp.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/config/views/config.token.question.html` & `edumfa-2.0.2/edumfa/static/components/config/views/config.token.question.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/config/views/config.token.radius.html` & `edumfa-2.0.2/edumfa/static/components/config/views/config.token.radius.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/config/views/config.token.remote.html` & `edumfa-2.0.2/edumfa/static/components/config/views/config.token.remote.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/config/views/config.token.sms.html` & `edumfa-2.0.2/edumfa/static/components/config/views/config.token.sms.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/config/views/config.token.tiqr.html` & `edumfa-2.0.2/edumfa/static/components/config/views/config.token.tiqr.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/config/views/config.token.totp.html` & `edumfa-2.0.2/edumfa/static/components/config/views/config.token.totp.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/config/views/config.token.u2f.html` & `edumfa-2.0.2/edumfa/static/components/config/views/config.token.u2f.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/config/views/config.token.webauthn.html` & `edumfa-2.0.2/edumfa/static/components/config/views/config.token.webauthn.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/config/views/config.token.yubico.html` & `edumfa-2.0.2/edumfa/static/components/config/views/config.token.yubico.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/config/views/config.token.yubikey.html` & `edumfa-2.0.2/edumfa/static/components/config/views/config.token.yubikey.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/config/views/config.tokengroup.edit.html` & `edumfa-2.0.2/edumfa/static/components/config/views/config.tokengroup.edit.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/config/views/config.tokengroup.list.html` & `edumfa-2.0.2/edumfa/static/components/config/views/config.tokengroup.list.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/config/views/config.tokens.html` & `edumfa-2.0.2/edumfa/static/components/config/views/config.tokens.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/config/views/dialog.confirm_delete.html` & `edumfa-2.0.2/edumfa/static/components/config/views/dialog.confirm_delete.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/dashboard/controllers/dashboardControllers.js` & `edumfa-2.0.2/edumfa/static/components/dashboard/controllers/dashboardControllers.js`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/dashboard/states/states.js` & `edumfa-2.0.2/edumfa/static/components/dashboard/states/states.js`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/dashboard/views/dashboard.html` & `edumfa-2.0.2/edumfa/static/components/dashboard/views/dashboard.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/dialogs/views/dialog.about.html` & `edumfa-2.0.2/edumfa/static/components/dialogs/views/dialog.about.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/dialogs/views/dialog.autocreate_realm.html` & `edumfa-2.0.2/edumfa/static/components/dialogs/views/dialog.autocreate_realm.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/dialogs/views/dialog.lock.html` & `edumfa-2.0.2/edumfa/static/components/dialogs/views/dialog.lock.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/dialogs/views/dialog.no.token.html` & `edumfa-2.0.2/edumfa/static/components/dialogs/views/dialog.no.token.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/dialogs/views/dialog.welcome.html` & `edumfa-2.0.2/edumfa/static/components/dialogs/views/dialog.welcome.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/directives/controllers/directives.js` & `edumfa-2.0.2/edumfa/static/components/directives/controllers/directives.js`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/directives/views/directive.assigntoken.html` & `edumfa-2.0.2/edumfa/static/components/directives/views/directive.assigntoken.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/directives/views/directive.assignuser.html` & `edumfa-2.0.2/edumfa/static/components/directives/views/directive.assignuser.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/directives/views/directive.attachmachine.html` & `edumfa-2.0.2/edumfa/static/components/directives/views/directive.attachmachine.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/directives/views/directive.attachtoken.html` & `edumfa-2.0.2/edumfa/static/components/directives/views/directive.attachtoken.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/directives/views/directive.policyconditions.html` & `edumfa-2.0.2/edumfa/static/components/directives/views/directive.policyconditions.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/directives/views/directive.tokendata.html` & `edumfa-2.0.2/edumfa/static/components/directives/views/directive.tokendata.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/filters/filters.js` & `edumfa-2.0.2/edumfa/static/components/filters/filters.js`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/login/controllers/loginControllers.js` & `edumfa-2.0.2/edumfa/static/components/login/controllers/loginControllers.js`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/login/factories/auth.js` & `edumfa-2.0.2/edumfa/static/components/login/factories/auth.js`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/login/factories/u2f.js` & `edumfa-2.0.2/edumfa/static/components/login/factories/u2f.js`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/login/factories/webauthn.js` & `edumfa-2.0.2/edumfa/static/components/login/factories/webauthn.js`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/login/states/states.js` & `edumfa-2.0.2/edumfa/static/components/login/states/states.js`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/login/views/enter-response.html` & `edumfa-2.0.2/edumfa/static/components/login/views/enter-response.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/login/views/login.html` & `edumfa-2.0.2/edumfa/static/components/login/views/login.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/login/views/pinchange.html` & `edumfa-2.0.2/edumfa/static/components/login/views/pinchange.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/machine/controllers/machineController.js` & `edumfa-2.0.2/edumfa/static/components/machine/controllers/machineController.js`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/machine/controllers/machineDetailsController.js` & `edumfa-2.0.2/edumfa/static/components/machine/controllers/machineDetailsController.js`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/machine/factories/machine.js` & `edumfa-2.0.2/edumfa/static/components/machine/factories/machine.js`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/machine/states/states.js` & `edumfa-2.0.2/edumfa/static/components/machine/states/states.js`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/machine/views/machine.details.html` & `edumfa-2.0.2/edumfa/static/components/machine/views/machine.details.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/machine/views/machine.html` & `edumfa-2.0.2/edumfa/static/components/machine/views/machine.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/machine/views/machine.list.html` & `edumfa-2.0.2/edumfa/static/components/machine/views/machine.list.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/recovery/controllers/recoveryControllers.js` & `edumfa-2.0.2/edumfa/static/components/recovery/controllers/recoveryControllers.js`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/recovery/factories/recoveryFactory.js` & `edumfa-2.0.2/edumfa/static/components/recovery/factories/recoveryFactory.js`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/recovery/states/states.js` & `edumfa-2.0.2/edumfa/static/components/recovery/states/states.js`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/recovery/views/recovery.html` & `edumfa-2.0.2/edumfa/static/components/recovery/views/recovery.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/recovery/views/recovery.reset.html` & `edumfa-2.0.2/edumfa/static/components/recovery/views/recovery.reset.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/register/controllers/registerControllers.js` & `edumfa-2.0.2/edumfa/static/components/register/controllers/registerControllers.js`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/register/factories/registerFactory.js` & `edumfa-2.0.2/edumfa/static/components/register/factories/registerFactory.js`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/register/states/states.js` & `edumfa-2.0.2/edumfa/static/components/register/states/states.js`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/register/views/register.html` & `edumfa-2.0.2/edumfa/static/components/register/views/register.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/token/controllers/tokenApplicationsController.js` & `edumfa-2.0.2/edumfa/static/components/token/controllers/tokenApplicationsController.js`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/token/controllers/tokenChallengesController.js` & `edumfa-2.0.2/edumfa/static/components/token/controllers/tokenChallengesController.js`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/token/controllers/tokenControllers.js` & `edumfa-2.0.2/edumfa/static/components/token/controllers/tokenControllers.js`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/token/controllers/tokenDetailController.js` & `edumfa-2.0.2/edumfa/static/components/token/controllers/tokenDetailController.js`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/token/controllers/tokenGetSerialController.js` & `edumfa-2.0.2/edumfa/static/components/token/controllers/tokenGetSerialController.js`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/token/controllers/tokenLostController.js` & `edumfa-2.0.2/edumfa/static/components/token/controllers/tokenLostController.js`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/token/factories/token.js` & `edumfa-2.0.2/edumfa/static/components/token/factories/token.js`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/token/factories/validate.js` & `edumfa-2.0.2/edumfa/static/components/token/factories/validate.js`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/token/states/states.js` & `edumfa-2.0.2/edumfa/static/components/token/states/states.js`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/token/views/dialog.ask_token_delete.html` & `edumfa-2.0.2/edumfa/static/components/token/views/dialog.ask_token_delete.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/token/views/token.applications.html` & `edumfa-2.0.2/edumfa/static/components/token/views/token.applications.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/token/views/token.applications.offline.html` & `edumfa-2.0.2/edumfa/static/components/token/views/token.applications.offline.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/token/views/token.applications.ssh.html` & `edumfa-2.0.2/edumfa/static/components/token/views/token.applications.ssh.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/token/views/token.assign.html` & `edumfa-2.0.2/edumfa/static/components/token/views/token.assign.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/token/views/token.challenges.html` & `edumfa-2.0.2/edumfa/static/components/token/views/token.challenges.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/token/views/token.details.html` & `edumfa-2.0.2/edumfa/static/components/token/views/token.details.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/token/views/token.enroll.4eyes.html` & `edumfa-2.0.2/edumfa/static/components/token/views/token.enroll.4eyes.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/token/views/token.enroll.applspec.html` & `edumfa-2.0.2/edumfa/static/components/token/views/token.enroll.applspec.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/token/views/token.enroll.certificate.html` & `edumfa-2.0.2/edumfa/static/components/token/views/token.enroll.certificate.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/token/views/token.enroll.daypassword.html` & `edumfa-2.0.2/edumfa/static/components/token/views/token.enroll.daypassword.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/token/views/token.enroll.email.html` & `edumfa-2.0.2/edumfa/static/components/token/views/token.enroll.email.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/token/views/token.enroll.hotp.html` & `edumfa-2.0.2/edumfa/static/components/token/views/token.enroll.hotp.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/token/views/token.enroll.html` & `edumfa-2.0.2/edumfa/static/components/token/views/token.enroll.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/token/views/token.enroll.indexedsecret.html` & `edumfa-2.0.2/edumfa/static/components/token/views/token.enroll.indexedsecret.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/token/views/token.enroll.motp.html` & `edumfa-2.0.2/edumfa/static/components/token/views/token.enroll.motp.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/token/views/token.enroll.push.html` & `edumfa-2.0.2/edumfa/static/components/token/views/token.enroll.push.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/token/views/token.enroll.question.html` & `edumfa-2.0.2/edumfa/static/components/token/views/token.enroll.question.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/token/views/token.enroll.radius.html` & `edumfa-2.0.2/edumfa/static/components/token/views/token.enroll.radius.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/token/views/token.enroll.remote.html` & `edumfa-2.0.2/edumfa/static/components/token/views/token.enroll.remote.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/token/views/token.enroll.sms.html` & `edumfa-2.0.2/edumfa/static/components/token/views/token.enroll.sms.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/token/views/token.enroll.sshkey.html` & `edumfa-2.0.2/edumfa/static/components/token/views/token.enroll.sshkey.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/token/views/token.enroll.totp.html` & `edumfa-2.0.2/edumfa/static/components/token/views/token.enroll.totp.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/token/views/token.enroll.vasco.html` & `edumfa-2.0.2/edumfa/static/components/token/views/token.enroll.vasco.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/token/views/token.enroll.yubico.html` & `edumfa-2.0.2/edumfa/static/components/token/views/token.enroll.yubico.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/token/views/token.enroll.yubikey.html` & `edumfa-2.0.2/edumfa/static/components/token/views/token.enroll.yubikey.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/token/views/token.enrolled.certificate.html` & `edumfa-2.0.2/edumfa/static/components/token/views/token.enrolled.certificate.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/token/views/token.enrolled.daypassword.html` & `edumfa-2.0.2/edumfa/static/components/token/views/token.enrolled.daypassword.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/token/views/token.enrolled.hotp.html` & `edumfa-2.0.2/edumfa/static/components/token/views/token.enrolled.hotp.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/token/views/token.enrolled.motp.html` & `edumfa-2.0.2/edumfa/static/components/token/views/token.enrolled.motp.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/token/views/token.enrolled.paper.html` & `edumfa-2.0.2/edumfa/static/components/token/views/token.enrolled.paper.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/token/views/token.enrolled.push.html` & `edumfa-2.0.2/edumfa/static/components/token/views/token.enrolled.push.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/token/views/token.enrolled.registration.html` & `edumfa-2.0.2/edumfa/static/components/token/views/token.enrolled.registration.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/token/views/token.enrolled.tan.html` & `edumfa-2.0.2/edumfa/static/components/token/views/token.enrolled.tan.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/token/views/token.enrolled.tiqr.html` & `edumfa-2.0.2/edumfa/static/components/token/views/token.enrolled.tiqr.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/token/views/token.enrolled.totp.html` & `edumfa-2.0.2/edumfa/static/components/token/views/token.enrolled.totp.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/token/views/token.enrolled.u2f.html` & `edumfa-2.0.2/edumfa/static/components/token/views/token.enrolled.u2f.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/token/views/token.enrolled.webauthn.html` & `edumfa-2.0.2/edumfa/static/components/token/views/token.enrolled.webauthn.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/token/views/token.getserial.html` & `edumfa-2.0.2/edumfa/static/components/token/views/token.getserial.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/token/views/token.html` & `edumfa-2.0.2/edumfa/static/components/token/views/token.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/token/views/token.import.html` & `edumfa-2.0.2/edumfa/static/components/token/views/token.import.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/token/views/token.list.html` & `edumfa-2.0.2/edumfa/static/components/token/views/token.list.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/token/views/token.lost.html` & `edumfa-2.0.2/edumfa/static/components/token/views/token.lost.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/translation/translations.js` & `edumfa-2.0.2/edumfa/static/components/translation/translations.js`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/user/controllers/userControllers.js` & `edumfa-2.0.2/edumfa/static/components/user/controllers/userControllers.js`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/user/factories/user.js` & `edumfa-2.0.2/edumfa/static/components/user/factories/user.js`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/user/states/states.js` & `edumfa-2.0.2/edumfa/static/components/user/states/states.js`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/user/views/dialog.ask_user_delete.html` & `edumfa-2.0.2/edumfa/static/components/user/views/dialog.ask_user_delete.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/user/views/user.add.dynamic.form.fields.html` & `edumfa-2.0.2/edumfa/static/components/user/views/user.add.dynamic.form.fields.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/user/views/user.add.html` & `edumfa-2.0.2/edumfa/static/components/user/views/user.add.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/user/views/user.details.html` & `edumfa-2.0.2/edumfa/static/components/user/views/user.details.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/user/views/user.html` & `edumfa-2.0.2/edumfa/static/components/user/views/user.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/user/views/user.list.html` & `edumfa-2.0.2/edumfa/static/components/user/views/user.list.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/components/user/views/user.password.html` & `edumfa-2.0.2/edumfa/static/components/user/views/user.password.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/contrib/css/angular-inform.css` & `edumfa-2.0.2/edumfa/static/contrib/css/angular-inform.css`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/contrib/css/angular-inform.css.map` & `edumfa-2.0.2/edumfa/static/contrib/css/angular-inform.css.map`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/contrib/css/bootstrap-theme.css` & `edumfa-2.0.2/edumfa/static/contrib/css/bootstrap-theme.css`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/contrib/css/bootstrap-theme.css.map` & `edumfa-2.0.2/edumfa/static/contrib/css/bootstrap-theme.css.map`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/contrib/css/bootstrap.css` & `edumfa-2.0.2/edumfa/static/contrib/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/contrib/css/bootstrap.css.map` & `edumfa-2.0.2/edumfa/static/contrib/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/contrib/css/hotkeys.css` & `edumfa-2.0.2/edumfa/static/contrib/css/hotkeys.css`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/contrib/css/isteven-multi-select.css` & `edumfa-2.0.2/edumfa/static/contrib/css/isteven-multi-select.css`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/contrib/fonts/glyphicons-halflings-regular.eot` & `edumfa-2.0.2/edumfa/static/contrib/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/contrib/fonts/glyphicons-halflings-regular.svg` & `edumfa-2.0.2/edumfa/static/contrib/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/contrib/fonts/glyphicons-halflings-regular.ttf` & `edumfa-2.0.2/edumfa/static/contrib/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/contrib/fonts/glyphicons-halflings-regular.woff` & `edumfa-2.0.2/edumfa/static/contrib/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/contrib/fonts/glyphicons-halflings-regular.woff2` & `edumfa-2.0.2/edumfa/static/contrib/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/contrib/js/angular-inform.js` & `edumfa-2.0.2/edumfa/static/contrib/js/angular-inform.js`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/contrib/js/angular-inform.js.map` & `edumfa-2.0.2/edumfa/static/contrib/js/angular-inform.js.map`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/contrib/js/angular.js` & `edumfa-2.0.2/edumfa/static/contrib/js/angular.js`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/contrib/js/bootstrap.js` & `edumfa-2.0.2/edumfa/static/contrib/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/contrib/js/hotkeys.js` & `edumfa-2.0.2/edumfa/static/contrib/js/hotkeys.js`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/contrib/js/jquery.js` & `edumfa-2.0.2/edumfa/static/contrib/js/jquery.js`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/contrib/js/ngmodules/angular-gettext.js` & `edumfa-2.0.2/edumfa/static/contrib/js/ngmodules/angular-gettext.js`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/contrib/js/ngmodules/angular-idle.js` & `edumfa-2.0.2/edumfa/static/contrib/js/ngmodules/angular-idle.js`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/contrib/js/ngmodules/angular-sanitize.js` & `edumfa-2.0.2/edumfa/static/contrib/js/ngmodules/angular-sanitize.js`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/contrib/js/ngmodules/angular-ui-router.js` & `edumfa-2.0.2/edumfa/static/contrib/js/ngmodules/angular-ui-router.js`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/contrib/js/ngmodules/angular-ui-router.js.map` & `edumfa-2.0.2/edumfa/static/contrib/js/ngmodules/angular-ui-router.js.map`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/contrib/js/ngmodules/isteven-multi-select.js` & `edumfa-2.0.2/edumfa/static/contrib/js/ngmodules/isteven-multi-select.js`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/contrib/js/ngmodules/ng-file-upload.js` & `edumfa-2.0.2/edumfa/static/contrib/js/ngmodules/ng-file-upload.js`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/contrib/js/u2f-api.js` & `edumfa-2.0.2/edumfa/static/contrib/js/u2f-api.js`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/contrib/js/ui-bootstrap-tpls.js` & `edumfa-2.0.2/edumfa/static/contrib/js/ui-bootstrap-tpls.js`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/contrib/js/webauthn-client/edumfa-webauthn.js` & `edumfa-2.0.2/edumfa/static/contrib/js/webauthn-client/edumfa-webauthn.js`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/css/content.css` & `edumfa-2.0.2/edumfa/static/css/content.css`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/css/eduMFA-logo.png` & `edumfa-2.0.2/edumfa/static/css/eduMFA-logo.png`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/css/menu.css` & `edumfa-2.0.2/edumfa/static/css/menu.css`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/css/papertoken.css` & `edumfa-2.0.2/edumfa/static/css/papertoken.css`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/css/signin.css` & `edumfa-2.0.2/edumfa/static/css/signin.css`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/customize/README.rst` & `edumfa-2.0.2/edumfa/static/customize/README.rst`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/favicon.png` & `edumfa-2.0.2/edumfa/static/favicon.png`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/img/FIDO-U2F-Security-Key-444x444.png` & `edumfa-2.0.2/edumfa/static/img/FIDO-U2F-Security-Key-444x444.png`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/img/plugup.jpg` & `edumfa-2.0.2/edumfa/static/img/plugup.jpg`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/img/solokeys.png` & `edumfa-2.0.2/edumfa/static/img/solokeys.png`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/img/u2fzero.png` & `edumfa-2.0.2/edumfa/static/img/u2fzero.png`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/package-lock.json` & `edumfa-2.0.2/edumfa/static/package-lock.json`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/package.json` & `edumfa-2.0.2/edumfa/static/package.json`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/providers/errorMessageProvider.js` & `edumfa-2.0.2/edumfa/static/providers/errorMessageProvider.js`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/providers/versioningProvider.js` & `edumfa-2.0.2/edumfa/static/providers/versioningProvider.js`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/templates/cert_request_form.html` & `edumfa-2.0.2/edumfa/static/templates/cert_request_form.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/templates/documentation.rst` & `edumfa-2.0.2/edumfa/static/templates/documentation.rst`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/templates/footer.html` & `edumfa-2.0.2/edumfa/static/templates/footer.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/templates/header.html` & `edumfa-2.0.2/edumfa/static/templates/header.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/templates/index.html` & `edumfa-2.0.2/edumfa/static/templates/index.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/templates/menu.html` & `edumfa-2.0.2/edumfa/static/templates/menu.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/templates/token_enrolled.html` & `edumfa-2.0.2/edumfa/static/templates/token_enrolled.html`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/static/update_contrib.sh` & `edumfa-2.0.2/edumfa/static/update_contrib.sh`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/translations/cs/LC_MESSAGES/messages.mo` & `edumfa-2.0.2/edumfa/translations/cs/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/translations/cs/LC_MESSAGES/messages.po` & `edumfa-2.0.2/edumfa/translations/cs/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/translations/de/LC_MESSAGES/messages.mo` & `edumfa-2.0.2/edumfa/translations/de/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/translations/de/LC_MESSAGES/messages.po` & `edumfa-2.0.2/edumfa/translations/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/translations/es/LC_MESSAGES/messages.mo` & `edumfa-2.0.2/edumfa/translations/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/translations/es/LC_MESSAGES/messages.po` & `edumfa-2.0.2/edumfa/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/translations/fr/LC_MESSAGES/messages.mo` & `edumfa-2.0.2/edumfa/translations/fr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/translations/fr/LC_MESSAGES/messages.po` & `edumfa-2.0.2/edumfa/translations/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/translations/it/LC_MESSAGES/messages.mo` & `edumfa-2.0.2/edumfa/translations/it/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/translations/it/LC_MESSAGES/messages.po` & `edumfa-2.0.2/edumfa/translations/it/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/translations/nl/LC_MESSAGES/messages.mo` & `edumfa-2.0.2/edumfa/translations/nl/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/translations/nl/LC_MESSAGES/messages.po` & `edumfa-2.0.2/edumfa/translations/nl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/translations/pl/LC_MESSAGES/messages.po` & `edumfa-2.0.2/edumfa/translations/pl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/translations/pt_BR/LC_MESSAGES/messages.mo` & `edumfa-2.0.2/edumfa/translations/pt_BR/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/translations/pt_BR/LC_MESSAGES/messages.po` & `edumfa-2.0.2/edumfa/translations/pt_BR/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/translations/ro/LC_MESSAGES/messages.mo` & `edumfa-2.0.2/edumfa/translations/ro/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/translations/ro/LC_MESSAGES/messages.po` & `edumfa-2.0.2/edumfa/translations/ro/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/translations/ru/LC_MESSAGES/messages.mo` & `edumfa-2.0.2/edumfa/translations/ru/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/translations/ru/LC_MESSAGES/messages.po` & `edumfa-2.0.2/edumfa/translations/ru/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/translations/si/LC_MESSAGES/messages.mo` & `edumfa-2.0.2/edumfa/translations/si/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/translations/si/LC_MESSAGES/messages.po` & `edumfa-2.0.2/edumfa/translations/si/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/translations/tr/LC_MESSAGES/messages.mo` & `edumfa-2.0.2/edumfa/translations/tr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/translations/tr/LC_MESSAGES/messages.po` & `edumfa-2.0.2/edumfa/translations/tr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/translations/zh_Hans/LC_MESSAGES/messages.mo` & `edumfa-2.0.2/edumfa/translations/zh_Hans/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/translations/zh_Hans/LC_MESSAGES/messages.po` & `edumfa-2.0.2/edumfa/translations/zh_Hans/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/translations/zh_Hant/LC_MESSAGES/messages.mo` & `edumfa-2.0.2/edumfa/translations/zh_Hant/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/translations/zh_Hant/LC_MESSAGES/messages.po` & `edumfa-2.0.2/edumfa/translations/zh_Hant/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/webui/certificate.py` & `edumfa-2.0.2/edumfa/webui/certificate.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa/webui/login.py` & `edumfa-2.0.2/edumfa/webui/login.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa.egg-info/PKG-INFO` & `edumfa-2.0.2/edumfa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edumfa
-Version: 2.0.1
+Version: 2.0.2
 Summary: eduMFA: identity, multifactor authentication (OTP), authorization, audit
 Home-page: https://www.edumfa.io
 Author: edumfa.io
 Author-email: edumfa@listserv.dfn.de
 License: AGPLv3
 Keywords: OTP,two factor authentication,management,security
 Classifier: Framework :: Flask
@@ -136,16 +136,15 @@
 
 
 
 Setup
 =====
 
 For setting up the system to *run* it, please read install instructions 
-at `edumfa.readthedocs.io <http://edumfa.readthedocs.io/en/latest/installation/index
-.html>`_.
+at `edumfa.readthedocs.io <http://edumfa.readthedocs.io/en/latest/installation/index.html>`_.
 
 If you want to setup a development environment start like this::
 
     git clone https://github.com/edumfa/edumfa.git
     cd edumfa
     virtualenv venv
     source venv/bin/activate
@@ -173,16 +172,15 @@
 submodules, by running::
 
    git pull --recurse-submodules
 
 Running it
 ==========
 
-First You need to create a `config-file <https://edumfa.readthedocs
-.io/en/latest/installation/system/inifile.html>`_.
+First You need to create a `config-file <https://edumfa.readthedocs.io/en/latest/installation/system/inifile.html>`_.
 
 Then create the database tables and the encryption key::
 
     ./edumfa-manage create_tables
     ./edumfa-manage create_enckey
 
 If You want to keep the development database upgradable, You should `stamp
@@ -199,15 +197,15 @@
 
     ./edumfa-manage admin add <username>
 
 Run it::
 
     ./edumfa-manage runserver
 
-Now you can connect to http://localhost:5000 with your browser and login
+Now you can connect to ``http://localhost:5000`` with your browser and login
 as administrator.
 
 Run tests
 =========
 
 If you have followed the steps above to set up your
 `environment for testing <#testing-env>`__, running the test suite should be as
@@ -220,15 +218,15 @@
 
 There are a lot of different ways to contribute to eduMFA, even
 if you are not a developer.
 
 If you found a security vulnerability please report it to us using the reporting form provided by GitHub
 
 You can find detailed information about contributing here:
-https://github.com/eduMFA/eduMFA/blob/master/CONTRIBUTING.md
+https://github.com/eduMFA/eduMFA/blob/main/CONTRIBUTING.md
 
 Code structure
 ==============
 
 The database models are defined in ``models.py`` and tested in 
 tests/test_db_model.py.
```

### Comparing `edumfa-2.0.1/edumfa.egg-info/SOURCES.txt` & `edumfa-2.0.2/edumfa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/edumfa.egg-info/requires.txt` & `edumfa-2.0.2/edumfa.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/alembic.ini` & `edumfa-2.0.2/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/env.py` & `edumfa-2.0.2/migrations/env.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/versions/006d4747f858_.py` & `edumfa-2.0.2/migrations/versions/006d4747f858_.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/versions/00762b3f7a60_.py` & `edumfa-2.0.2/migrations/versions/00762b3f7a60_.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/versions/0c7123345224_.py` & `edumfa-2.0.2/migrations/versions/0c7123345224_.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/versions/0d011e94a8e8_.py` & `edumfa-2.0.2/migrations/versions/0d011e94a8e8_.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/versions/145ce80decd_.py` & `edumfa-2.0.2/migrations/versions/145ce80decd_.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/versions/14a1bcb10018_.py` & `edumfa-2.0.2/migrations/versions/14a1bcb10018_.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/versions/19f727d285e2_.py` & `edumfa-2.0.2/migrations/versions/19f727d285e2_.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/versions/1a0710df148b_.py` & `edumfa-2.0.2/migrations/versions/1a0710df148b_.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/versions/1a69e5e5e2ac_.py` & `edumfa-2.0.2/migrations/versions/1a69e5e5e2ac_.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/versions/1edda52b619f_.py` & `edumfa-2.0.2/migrations/versions/1edda52b619f_.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/versions/204d8d4f351e_.py` & `edumfa-2.0.2/migrations/versions/204d8d4f351e_.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/versions/205bda834127_.py` & `edumfa-2.0.2/migrations/versions/205bda834127_.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/versions/20969b4cbf06_.py` & `edumfa-2.0.2/migrations/versions/20969b4cbf06_.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/versions/2118e566df16_.py` & `edumfa-2.0.2/migrations/versions/2118e566df16_.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/versions/2181294eed0b_.py` & `edumfa-2.0.2/migrations/versions/2181294eed0b_.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/versions/22558d9f3178_.py` & `edumfa-2.0.2/migrations/versions/22558d9f3178_.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/versions/239995464c48_.py` & `edumfa-2.0.2/migrations/versions/239995464c48_.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/versions/2551ee982544_.py` & `edumfa-2.0.2/migrations/versions/2551ee982544_.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/versions/2ac117d0a6f5_.py` & `edumfa-2.0.2/migrations/versions/2ac117d0a6f5_.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/versions/2c9430cfc66b_.py` & `edumfa-2.0.2/migrations/versions/2c9430cfc66b_.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/versions/307a4fbe8a05_.py` & `edumfa-2.0.2/migrations/versions/307a4fbe8a05_.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/versions/3236a1abf1c6_.py` & `edumfa-2.0.2/migrations/versions/3236a1abf1c6_.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/versions/3429d523e51f_.py` & `edumfa-2.0.2/migrations/versions/3429d523e51f_.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/versions/36428afb2457_.py` & `edumfa-2.0.2/migrations/versions/36428afb2457_.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/versions/37e6b49fc686_.py` & `edumfa-2.0.2/migrations/versions/37e6b49fc686_.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/versions/3ae3c668f444_.py` & `edumfa-2.0.2/migrations/versions/3ae3c668f444_.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/versions/3ba618f6b820_.py` & `edumfa-2.0.2/migrations/versions/3ba618f6b820_.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/versions/3c6e9dd7fbac_.py` & `edumfa-2.0.2/migrations/versions/3c6e9dd7fbac_.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/versions/3d7f8b29cbb1_.py` & `edumfa-2.0.2/migrations/versions/3d7f8b29cbb1_.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/versions/3f7e8583ea2_.py` & `edumfa-2.0.2/migrations/versions/3f7e8583ea2_.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/versions/4023571658f8_.py` & `edumfa-2.0.2/migrations/versions/4023571658f8_.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/versions/4238eac8ccab_.py` & `edumfa-2.0.2/migrations/versions/4238eac8ccab_.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/versions/449903fb6e35_.py` & `edumfa-2.0.2/migrations/versions/449903fb6e35_.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/versions/48ee74b8a7c8_.py` & `edumfa-2.0.2/migrations/versions/48ee74b8a7c8_.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/versions/49a04e560d96_.py` & `edumfa-2.0.2/migrations/versions/49a04e560d96_.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/versions/4a0aec37e7cf_.py` & `edumfa-2.0.2/migrations/versions/4a0aec37e7cf_.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/versions/4d9178fa8336_.py` & `edumfa-2.0.2/migrations/versions/4d9178fa8336_.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/versions/4f32a4e1bf33_.py` & `edumfa-2.0.2/migrations/versions/4f32a4e1bf33_.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/versions/50adc980d625_.py` & `edumfa-2.0.2/migrations/versions/50adc980d625_.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/versions/5402fd96fbca_.py` & `edumfa-2.0.2/migrations/versions/5402fd96fbca_.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/versions/58e4f7ebb705_.py` & `edumfa-2.0.2/migrations/versions/58e4f7ebb705_.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/versions/59ef3e03bc62_.py` & `edumfa-2.0.2/migrations/versions/59ef3e03bc62_.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/versions/5cb310101a1f_.py` & `edumfa-2.0.2/migrations/versions/5cb310101a1f_.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/versions/631ec59e1ca6_.py` & `edumfa-2.0.2/migrations/versions/631ec59e1ca6_.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/versions/849170064430_.py` & `edumfa-2.0.2/migrations/versions/849170064430_.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/versions/86f40f535d7c_.py` & `edumfa-2.0.2/migrations/versions/86f40f535d7c_.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/versions/888b56ed5dcb_.py` & `edumfa-2.0.2/migrations/versions/888b56ed5dcb_.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/versions/89e57ed16379_.py` & `edumfa-2.0.2/migrations/versions/89e57ed16379_.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/versions/8d40dbcfda25_.py` & `edumfa-2.0.2/migrations/versions/8d40dbcfda25_.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/versions/9155f0d3d028_.py` & `edumfa-2.0.2/migrations/versions/9155f0d3d028_.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/versions/a28f2733897b_.py` & `edumfa-2.0.2/migrations/versions/a28f2733897b_.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/versions/a63df077051a_.py` & `edumfa-2.0.2/migrations/versions/a63df077051a_.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/versions/a7e91b18a460_.py` & `edumfa-2.0.2/migrations/versions/a7e91b18a460_.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/versions/b9131d0686eb_.py` & `edumfa-2.0.2/migrations/versions/b9131d0686eb_.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/versions/cb6d7b7bae63_.py` & `edumfa-2.0.2/migrations/versions/cb6d7b7bae63_.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/versions/d2ae8e54b628_.py` & `edumfa-2.0.2/migrations/versions/d2ae8e54b628_.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/versions/d415d490eb05_.py` & `edumfa-2.0.2/migrations/versions/d415d490eb05_.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/versions/d6b40a745e5_.py` & `edumfa-2.0.2/migrations/versions/d6b40a745e5_.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/versions/d756b34061ff_.py` & `edumfa-2.0.2/migrations/versions/d756b34061ff_.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/versions/dceb6cd3c41e_.py` & `edumfa-2.0.2/migrations/versions/dceb6cd3c41e_.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/versions/e360c56bcf8c_.py` & `edumfa-2.0.2/migrations/versions/e360c56bcf8c_.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/versions/e5cbeb7c177_.py` & `edumfa-2.0.2/migrations/versions/e5cbeb7c177_.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/versions/ef29ba43e290_.py` & `edumfa-2.0.2/migrations/versions/ef29ba43e290_.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/versions/fa07bd604a75.py` & `edumfa-2.0.2/migrations/versions/fa07bd604a75.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/versions/fabcf24d9304_.py` & `edumfa-2.0.2/migrations/versions/fabcf24d9304_.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/migrations/versions/ff26585932ec_.py` & `edumfa-2.0.2/migrations/versions/ff26585932ec_.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/requirements.txt` & `edumfa-2.0.2/requirements.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,167 +1,167 @@
 #
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
 #    pip-compile --allow-unsafe --output-file=requirements.txt --strip-extras
 #
-alembic==1.10.2
+alembic==1.13.1
     # via flask-migrate
 argon2-cffi==21.3.0
     # via edumfa (setup.py)
 argon2-cffi-bindings==21.2.0
     # via argon2-cffi
-async-timeout==4.0.2
+async-timeout==4.0.3
     # via redis
-babel==2.12.1
+babel==2.14.0
     # via flask-babel
-bcrypt==4.0.1
+bcrypt==4.1.2
     # via passlib
 beautifulsoup4==4.12.3
     # via edumfa (setup.py)
 blinker==1.7.0
     # via flask
-cachetools==5.3.0
+cachetools==5.3.3
     # via google-auth
-cbor2==5.4.6
+cbor2==5.6.3
     # via edumfa (setup.py)
 certifi==2023.7.22
     # via requests
-cffi==1.15.1
+cffi==1.16.0
     # via
     #   argon2-cffi-bindings
     #   cryptography
-charset-normalizer==3.1.0
+charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via flask
 configobj==5.0.8
     # via edumfa (setup.py)
-croniter==1.3.8
+croniter==1.4.1
     # via edumfa (setup.py)
 cryptography==42.0.5
     # via
     #   edumfa (setup.py)
     #   pyopenssl
 defusedxml==0.7.1
     # via edumfa (setup.py)
-flask==3.0.2
+flask==3.0.3
     # via
     #   edumfa (setup.py)
     #   flask-babel
     #   flask-migrate
     #   flask-sqlalchemy
     #   flask-versioned
 flask-babel==4.0.0
     # via edumfa (setup.py)
-flask-migrate==4.0.5
+flask-migrate==4.0.7
     # via edumfa (setup.py)
 flask-sqlalchemy==3.0.5
     # via
     #   edumfa (setup.py)
     #   flask-migrate
 flask-versioned==0.9.4.post20101221
     # via edumfa (setup.py)
 google-auth==2.17.0
     # via edumfa (setup.py)
 grpcio==1.62.1
     # via edumfa (setup.py)
 huey==2.4.5
     # via edumfa (setup.py)
-idna==3.4
+idna==3.7
     # via requests
 importlib-metadata==6.1.0
     # via edumfa (setup.py)
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.3
     # via
     #   flask
     #   flask-babel
 ldap3==2.9.1
     # via edumfa (setup.py)
-lxml==5.1.0
+lxml==5.2.1
     # via
     #   beautifulsoup4
     #   edumfa (setup.py)
 mako==1.2.4
     # via alembic
 markupsafe==2.1.5
     # via
     #   jinja2
     #   mako
     #   werkzeug
-netaddr==0.8.0
+netaddr==0.10.1
     # via
     #   edumfa (setup.py)
     #   pyrad
 passlib==1.7.4
     # via edumfa (setup.py)
 pyasn1==0.4.8
     # via
     #   ldap3
     #   pyasn1-modules
     #   rsa
 pyasn1-modules==0.2.8
     # via google-auth
 pycparser==2.21
     # via cffi
-pydash==6.0.2
+pydash==8.0.0
     # via edumfa (setup.py)
-pyjwt==2.6.0
+pyjwt==2.8.0
     # via edumfa (setup.py)
 pymysql==1.0.3
     # via edumfa (setup.py)
 pyopenssl==24.0.0
     # via edumfa (setup.py)
 pyrad==2.4
     # via edumfa (setup.py)
 python-dateutil==2.8.2
     # via
     #   croniter
     #   edumfa (setup.py)
 python-gnupg==0.5.0
     # via edumfa (setup.py)
-pytz==2023.3
+pytz==2024.1
     # via flask-babel
 pyyaml==6.0.1
     # via edumfa (setup.py)
-redis==4.4.4
+redis==4.6.0
     # via huey
 requests==2.31.0
     # via edumfa (setup.py)
 rsa==4.9
     # via google-auth
 segno==1.5.2
     # via edumfa (setup.py)
 six==1.16.0
     # via
     #   configobj
     #   google-auth
     #   pyrad
     #   python-dateutil
     #   smpplib
-smpplib==2.2.2
+smpplib==2.2.3
     # via edumfa (setup.py)
 soupsieve==2.4
     # via beautifulsoup4
-sqlalchemy==1.4.47
+sqlalchemy==1.4.52
     # via
     #   alembic
     #   edumfa (setup.py)
     #   flask-sqlalchemy
 typing-extensions==4.10.0
     # via
     #   alembic
     #   edumfa (setup.py)
 urllib3==2.2.1
     # via
     #   edumfa (setup.py)
     #   requests
-werkzeug==3.0.1
+werkzeug==3.0.2
     # via flask
 zipp==3.15.0
     # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 setuptools==69.1.1
     # via flask-versioned
```

### Comparing `edumfa-2.0.1/setup.py` & `edumfa-2.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup, find_packages, find_namespace_packages
 import os
 import stat
 import sys
 
-VERSION = "2.0.1"
+VERSION = "2.0.2"
 
 # Taken from kennethreitz/requests/setup.py
 package_directory = os.path.realpath(os.path.dirname(__file__))
 
 
 def get_file_contents(file_path):
     """Get the context of the file using full path name."""
```

### Comparing `edumfa-2.0.1/tests/base.py` & `edumfa-2.0.2/tests/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from edumfa.lib.lifecycle import call_finalizers
 
 
 PWFILE = "tests/testdata/passwords"
 PWFILE2 = "tests/testdata/passwd"
 
 
-class FakeFlaskG(object):
+class FakeFlaskG:
     policy_object = None
     logged_in_user = {}
     audit_object = None
     client_ip = None
     request_headers = None
     serial = None
```

### Comparing `edumfa-2.0.1/tests/ldap3mock.py` & `edumfa-2.0.2/tests/ldap3mock.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,19 +72,19 @@
     def setdata(self, request, response):
         self._calls.append(Call(request, response))
 
     def reset(self):
         self._calls = []
 
 
-class Connection(object):
+class Connection:
 
-    class Extend(object):
+    class Extend:
 
-        class Standard(object):
+        class Standard:
 
             def __init__(self, connection):
                 self.connection = connection
 
             def paged_search(self, **kwargs):
                 self.connection.search(search_base=kwargs.get("search_base"),
                                        search_scope=kwargs.get("search_scope"),
@@ -634,15 +634,15 @@
 
         return True
 
     def unbind(self):
         return True
 
 
-class Ldap3Mock(object):
+class Ldap3Mock:
 
     def __init__(self):
         self._calls = CallList()
         self._server_mock = None
         self.directory = []
         self.exception = None
         self.reset()
```

### Comparing `edumfa-2.0.1/tests/mscamock.py` & `edumfa-2.0.2/tests/mscamock.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,47 +18,47 @@
 # GNU AFFERO GENERAL PUBLIC LICENSE for more details.
 #
 # You should have received a copy of the GNU Affero General Public
 # License along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 
 
-class MyTemplateReply(object):
+class MyTemplateReply:
     def __init__(self, templates):
         self.templateNames = templates
 
 
-class MyCAReply(object):
+class MyCAReply:
     def __init__(self, ca_list=None):
         self.caNames = ca_list or []
 
 
-class MyCSRReply(object):
+class MyCSRReply:
     def __init__(self, disposition=0, request_id=None, message="CSR invalid"):
         self.disposition = disposition
         self.dispositionMessage = message
         self.requestId = request_id or 4711
 
 
-class MyCertReply(object):
+class MyCertReply:
     def __init__(self, certificate):
         self.cert = certificate
 
 
-class MyCSRStatusReply(object):
+class MyCSRStatusReply:
     def __init__(self, disposition):
         self.disposition = disposition
 
 
-class MyCertificateReply(object):
+class MyCertificateReply:
     def __init__(self, certificate):
         self.cert = certificate
 
 
-class CAServiceMock(object):
+class CAServiceMock:
 
     def __init__(self, config, mock_config=None):
         self.cas = mock_config.get("available_cas") or []
         self.templates = mock_config.get("ca_templates") or []
         self.disposition = mock_config.get("csr_disposition") or 0
         self.certificate = mock_config.get("certificate")
```

### Comparing `edumfa-2.0.1/tests/pkcs11mock.py` & `edumfa-2.0.2/tests/pkcs11mock.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     """
     simple fake decrypt function for testing: substract 1 from each byte
     :return: a list of integers
     """
     return [(c - 1) % 256 for c in data]
 
 
-class PKCS11Mock(object):
+class PKCS11Mock:
     """
     Mock helper to simulate a HSM. Usage::
 
         with PKCS11Mock():
             hsm = AESHardwareSecurityModule(...)
 
             crypted = hsm.encrypt_password(...)
```

### Comparing `edumfa-2.0.1/tests/queuemock.py` & `edumfa-2.0.2/tests/queuemock.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/radiusmock.py` & `edumfa-2.0.2/tests/radiusmock.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     def setdata(self, request, response):
         self._calls.append(Call(request, response))
 
     def reset(self):
         self._calls = []
 
 
-class RadiusMock(object):
+class RadiusMock:
 
     def __init__(self):
         self._calls = CallList()
         self.reset()
 
     def reset(self):
         self._request_data = {}
```

### Comparing `edumfa-2.0.1/tests/redismock.py` & `edumfa-2.0.2/tests/redismock.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     def setdata(self, request, response):
         self._calls.append(Call(request, response))
 
     def reset(self):
         self._calls = []
 
 
-class Redis(object):
+class Redis:
 
     def __init__(self):
         self.dictionary = {}
 
     def get(self, value):
         return self.dictionary.get(value)
 
@@ -65,15 +65,15 @@
         self.dictionary[key] = value
         return True
 
     def set_data(self, data):
         self.dictionary = data
 
 
-class RedisMock(object):
+class RedisMock:
 
     def __init__(self):
         self._calls = CallList()
         self.data = {}
         self.reset()
 
     def reset(self):
```

### Comparing `edumfa-2.0.1/tests/smppmock.py` & `edumfa-2.0.2/tests/smppmock.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     def setdata(self, request, response):
         self._calls.append(Call(request, response))
 
     def reset(self):
         self._calls = []
 
 
-class SmppMock(object):
+class SmppMock:
 
     def __init__(self):
         self._calls = CallList()
         self.connect_successful = True
         self.systemid = None
         self.password = None
         self.reset()
```

### Comparing `edumfa-2.0.1/tests/smtpmock.py` & `edumfa-2.0.2/tests/smtpmock.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 
     def setdata(self, request, response):
         self._calls.append(Call(request, response))
 
     def reset(self):
         self._calls = []
 
-class SmtpMock(object):
+class SmtpMock:
 
     def __init__(self):
         self._calls = CallList()
         self.sent_message = None
         self.smtp_ssl = False
         self.reset()
```

### Comparing `edumfa-2.0.1/tests/test_api_2stepinit.py` & `edumfa-2.0.2/tests/test_api_2stepinit.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_api_applications.py` & `edumfa-2.0.2/tests/test_api_applications.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_api_audit.py` & `edumfa-2.0.2/tests/test_api_audit.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_api_auth.py` & `edumfa-2.0.2/tests/test_api_auth.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_api_caconnector.py` & `edumfa-2.0.2/tests/test_api_caconnector.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_api_clienttype.py` & `edumfa-2.0.2/tests/test_api_clienttype.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_api_edumfaserver.py` & `edumfa-2.0.2/tests/test_api_edumfaserver.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_api_events.py` & `edumfa-2.0.2/tests/test_api_events.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_api_lib_policy.py` & `edumfa-2.0.2/tests/test_api_lib_policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -2014,15 +2014,15 @@
         pushtoken_wait(req, None)
         self.assertEqual(req.all_data.get(PUSH_ACTION.WAIT), 10)
 
         delete_policy("push1")
 
     def test_24b_push_disable_wait_policy(self):
         # We send a fake push_wait that is not in the policies
-        class RequestMock(object):
+        class RequestMock:
             pass
         req = RequestMock()
         req.all_data = {"push_wait": "120"}
         pushtoken_disable_wait(req, None)
         self.assertEqual(req.all_data.get(PUSH_ACTION.WAIT), False)
 
         # But even with a policy, the function still sets PUSH_ACTION.WAIT to False
@@ -2127,15 +2127,15 @@
         # Now the request.all_data contains the otpkey from the user attributes.
         self.assertIn("otpkey", req.all_data)
         self.assertEqual("cornelius", req.all_data.get("otpkey"))
 
         delete_policy("Indexed")
 
     def test_26a_webauthn_auth_validate_triggerchallenge(self):
-        class RequestMock(object):
+        class RequestMock:
             pass
 
         # Normal request
         request = RequestMock()
         request.all_data = {
             'user': 'foo'
         }
@@ -2190,15 +2190,15 @@
         set_policy(
             name="WebAuthn",
             scope=SCOPE.AUTH,
             action=''
         )
 
     def test_26b_webauthn_auth_validate_check(self):
-        class RequestMock(object):
+        class RequestMock:
             pass
         # Normal request
         request = RequestMock()
         request.all_data = {
             'user': 'foo',
             'pass': '1234'
         }
@@ -2258,15 +2258,15 @@
         set_policy(
             name="WebAuthn",
             scope=SCOPE.AUTH,
             action=''
         )
 
     def test_26c_webauthn_auth_auth(self):
-        class RequestMock(object):
+        class RequestMock:
             pass
 
         # Normal request
         request = RequestMock()
         request.all_data = {
             'username': 'foo',
             'password': '1234'
@@ -2301,15 +2301,15 @@
         set_policy(
             name="WebAuthn",
             scope=SCOPE.AUTH,
             action=''
         )
 
     def test_27a_webauthn_authz_validate_check(self):
-        class RequestMock(object):
+        class RequestMock:
             pass
 
         # Normal request
         request = RequestMock()
         request.all_data = {
             "credentialid": CRED_ID,
             "authenticatordata": ASSERTION_RESPONSE_TMPL['authData'],
@@ -2414,15 +2414,15 @@
         set_policy(
             name="WebAuthn",
             scope=SCOPE.AUTHZ,
             action=''
         )
 
     def test_28_webauthn_enroll(self):
-        class RequestMock(object):
+        class RequestMock:
             pass
 
         rp_id = RP_ID
         rp_name = RP_NAME
 
         # Missing RP_ID
         request = RequestMock()
@@ -2750,15 +2750,15 @@
         set_policy(
             name="WebAuthn",
             scope=SCOPE.AUTH,
             action=''
         )
 
     def test_29c_webauthn_request_auth_authn(self):
-        class RequestMock(object):
+        class RequestMock:
             pass
 
         # Normal request
         request = RequestMock()
         request.all_data = {
             'username': 'foo',
             'password': '1234'
@@ -2855,15 +2855,15 @@
         set_policy(
             name="WebAuthn",
             scope=SCOPE.AUTHZ,
             action=''
         )
 
     def test_29e_webauthn_request_validate_check_authn(self):
-        class RequestMock(object):
+        class RequestMock:
             pass
 
         # Normal request
         request = RequestMock()
         request.all_data = {
             'user': 'foo',
             'pass': '1234'
@@ -2998,15 +2998,15 @@
         set_policy(
             name="WebAuthn",
             scope=SCOPE.ENROLL,
             action=''
         )
 
     def test_31_webauthn_disallowed_req(self):
-        class RequestMock(object):
+        class RequestMock:
             pass
 
         allowed_certs = "subject/.*Frobnicate.*/"
 
         request = RequestMock()
         request.all_data = {
             "type": WebAuthnTokenClass.get_class_type(),
@@ -3026,28 +3026,28 @@
         set_policy(
             name="WebAuthn",
             scope=SCOPE.ENROLL,
             action=''
         )
 
     def test_32_webauthn_allowed_aaguid(self):
-        class RequestMock(object):
+        class RequestMock:
             pass
 
         request = RequestMock()
         request.all_data = {
             "type": WebAuthnTokenClass.get_class_type(),
             "serial": WebAuthnTokenClass.get_class_prefix() + "123",
             "regdata": REGISTRATION_RESPONSE_TMPL['attObj']
         }
 
         self.assertTrue(webauthntoken_allowed(request, None))
 
     def test_33_webauthn_disallowed_aaguid(self):
-        class RequestMock(object):
+        class RequestMock:
             pass
 
         authenticator_selection_list = 'foo bar baz'
 
         request = RequestMock()
         request.all_data = {
             "type": WebAuthnTokenClass.get_class_type(),
```

### Comparing `edumfa-2.0.1/tests/test_api_lib_utils.py` & `edumfa-2.0.2/tests/test_api_lib_utils.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_api_machineresolver.py` & `edumfa-2.0.2/tests/test_api_machineresolver.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_api_machines.py` & `edumfa-2.0.2/tests/test_api_machines.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_api_machines_serviceid.py` & `edumfa-2.0.2/tests/test_api_machines_serviceid.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_api_monitoring.py` & `edumfa-2.0.2/tests/test_api_monitoring.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_api_offline_no_token.py` & `edumfa-2.0.2/tests/test_api_offline_no_token.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_api_periodictask.py` & `edumfa-2.0.2/tests/test_api_periodictask.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_api_policy.py` & `edumfa-2.0.2/tests/test_api_policy.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_api_push_validate.py` & `edumfa-2.0.2/tests/test_api_push_validate.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_api_radiusserver.py` & `edumfa-2.0.2/tests/test_api_radiusserver.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_api_register.py` & `edumfa-2.0.2/tests/test_api_register.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_api_roles.py` & `edumfa-2.0.2/tests/test_api_roles.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_api_serviceids.py` & `edumfa-2.0.2/tests/test_api_serviceids.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_api_smsgateway.py` & `edumfa-2.0.2/tests/test_api_smsgateway.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_api_smtpserver.py` & `edumfa-2.0.2/tests/test_api_smtpserver.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_api_system.py` & `edumfa-2.0.2/tests/test_api_system.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_api_token.py` & `edumfa-2.0.2/tests/test_api_token.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_api_tokengroup.py` & `edumfa-2.0.2/tests/test_api_tokengroup.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_api_ttype.py` & `edumfa-2.0.2/tests/test_api_ttype.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_api_u2f.py` & `edumfa-2.0.2/tests/test_api_u2f.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_api_users.py` & `edumfa-2.0.2/tests/test_api_users.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_api_validate.py` & `edumfa-2.0.2/tests/test_api_validate.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_app.py` & `edumfa-2.0.2/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_db_model.py` & `edumfa-2.0.2/tests/test_db_model.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_applications.py` & `edumfa-2.0.2/tests/test_lib_applications.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_apps.py` & `edumfa-2.0.2/tests/test_lib_apps.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_audit.py` & `edumfa-2.0.2/tests/test_lib_audit.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_auth.py` & `edumfa-2.0.2/tests/test_lib_auth.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_authcache.py` & `edumfa-2.0.2/tests/test_lib_authcache.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_caconnector.py` & `edumfa-2.0.2/tests/test_lib_caconnector.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_challenges.py` & `edumfa-2.0.2/tests/test_lib_challenges.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_clientapplication.py` & `edumfa-2.0.2/tests/test_lib_clientapplication.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_config.py` & `edumfa-2.0.2/tests/test_lib_config.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_counter.py` & `edumfa-2.0.2/tests/test_lib_counter.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_crypto.py` & `edumfa-2.0.2/tests/test_lib_crypto.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_edumfaserver.py` & `edumfa-2.0.2/tests/test_lib_edumfaserver.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_eventhandler_logging.py` & `edumfa-2.0.2/tests/test_lib_eventhandler_logging.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_eventhandler_usernotification.py` & `edumfa-2.0.2/tests/test_lib_eventhandler_usernotification.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_events.py` & `edumfa-2.0.2/tests/test_lib_events.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_framework.py` & `edumfa-2.0.2/tests/test_lib_framework.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_importotp.py` & `edumfa-2.0.2/tests/test_lib_importotp.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_lifecycle.py` & `edumfa-2.0.2/tests/test_lib_lifecycle.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_machine_resolver_ldap.py` & `edumfa-2.0.2/tests/test_lib_machine_resolver_ldap.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_machines.py` & `edumfa-2.0.2/tests/test_lib_machines.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_machinetokens.py` & `edumfa-2.0.2/tests/test_lib_machinetokens.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_monitoringstats.py` & `edumfa-2.0.2/tests/test_lib_monitoringstats.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_periodictask.py` & `edumfa-2.0.2/tests/test_lib_periodictask.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_policy.py` & `edumfa-2.0.2/tests/test_lib_policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1201,15 +1201,15 @@
         set_policy("verysecure", scope=SCOPE.AUTH, action="{0!s}=userstore".format(ACTION.OTPPIN),
                    conditions=[("userinfo", "type", "equals", "verysecure", True)])
         set_policy("notverysecure", scope=SCOPE.AUTH, action="{0!s}=userstore".format(ACTION.OTPPIN),
                    conditions=[("userinfo", "type", "equals", "notverysecure", True),
                                ("userinfo", "groups", "contains", "b", True)])
         P = PolicyClass()
 
-        class MockUser(object):
+        class MockUser:
             login = 'login'
             realm = 'realm'
             resolver = 'resolver'
 
         empty_user = User()
 
         user1 = MockUser()
@@ -1264,15 +1264,15 @@
                          set())
 
         delete_policy("extremelysecure")
 
     def test_30_filter_by_conditions_errors(self):
         P = PolicyClass()
 
-        class MockUser(object):
+        class MockUser:
             login = 'login'
             realm = 'realm'
             resolver = 'resolver'
 
         user1 = MockUser()
         user1.info = {"type": "verysecure", "groups": ["a", "b", "c"]}
 
@@ -1379,15 +1379,15 @@
         db_token = Token(serial, tokentype="spass")
         db_token.save()
         token = TokenClass(db_token)
         token.set_tokeninfo({"fixedpin": "true", "otherinfo": "true"})
 
         P = PolicyClass()
 
-        class MockUser(object):
+        class MockUser:
             login = 'login'
             realm = 'realm'
             resolver = 'resolver'
 
         user1 = MockUser()
         user1.info = {"email": "foo@bar.com"}
 
@@ -1422,15 +1422,15 @@
         from edumfa.models import Token
         serial = "filter_by_conditions_token"
         db_token = Token(serial, tokentype="spass")
         db_token.save()
 
         P = PolicyClass()
 
-        class MockUser(object):
+        class MockUser:
             login = 'login'
             realm = 'realm'
             resolver = 'resolver'
 
         user1 = MockUser()
         user1.info = {"email": "foo@bar.com"}
 
@@ -1474,15 +1474,15 @@
         self.assertRaises(PolicyError, P.match_policies, user_object=user1, serial=serial)
 
         delete_policy("setpin_pol")
         db_token.delete()
 
     def test_33_get_allowed_attributes(self):
 
-        class MockUser(object):
+        class MockUser:
             login = 'login'
             realm = 'realm'
             resolver = 'resolver'
 
         user = MockUser()
         g = FakeFlaskG()
         g.policy_object = PolicyClass()
```

### Comparing `edumfa-2.0.1/tests/test_lib_policydecorator.py` & `edumfa-2.0.2/tests/test_lib_policydecorator.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_pooling.py` & `edumfa-2.0.2/tests/test_lib_pooling.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_queue.py` & `edumfa-2.0.2/tests/test_lib_queue.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from edumfa.lib.error import ServerError
 from edumfa.lib.queue import job, JOB_COLLECTOR, JobCollector, get_job_queue, wrap_job, has_job_queue
 from edumfa.lib.queues.huey_queue import HueyQueue
 from edumfa.lib.queues.base import QueueError
 from .base import OverrideConfigTestCase, MyTestCase
 
 
-class TestSender(object):
+class TestSender:
     """ defined in order to be able to mock the ``send_mail`` function in tests """
     def send_mail(*args, **kwargs):
         pass
 
 
 SENDER = TestSender()
```

### Comparing `edumfa-2.0.1/tests/test_lib_radiusserver.py` & `edumfa-2.0.2/tests/test_lib_radiusserver.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_realm.py` & `edumfa-2.0.2/tests/test_lib_realm.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_recovery.py` & `edumfa-2.0.2/tests/test_lib_recovery.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_resolver.py` & `edumfa-2.0.2/tests/test_lib_resolver.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_serviceid.py` & `edumfa-2.0.2/tests/test_lib_serviceid.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_smsprovider.py` & `edumfa-2.0.2/tests/test_lib_smsprovider.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,23 +3,25 @@
 __doc__ = """
 This test file tests the modules:
  lib.smsprovider.httpsmsprovider
  lib.smsprovider.sipgateprovider
  lib.smsprovider.smtpsmsprovider
  lib.smsprovider.smppsmsprovider
  lib.smsprovider.scriptsmsprovider
+ lib.smsprovider.httpmessagetouidprovider
 """
 
 from .base import MyTestCase
 from edumfa.lib.smsprovider.HttpSMSProvider import HttpSMSProvider
 from edumfa.lib.smsprovider.SipgateSMSProvider import SipgateSMSProvider
 from edumfa.lib.smsprovider.SipgateSMSProvider import URL
 from edumfa.lib.smsprovider.SmtpSMSProvider import SmtpSMSProvider
 from edumfa.lib.smsprovider.SmppSMSProvider import SmppSMSProvider
 from edumfa.lib.smsprovider.ScriptSMSProvider import ScriptSMSProvider, SCRIPT_WAIT
+from edumfa.lib.smsprovider.HttpMessageToUidProvider import HttpMessageToUidProvider
 from edumfa.lib.smsprovider.SMSProvider import (SMSError,
                                                      get_sms_provider_class,
                                                      set_smsgateway,
                                                      get_smsgateway,
                                                      delete_smsgateway,
                                                      delete_smsgateway_option,
                                                      delete_smsgateway_header,
@@ -59,14 +61,18 @@
             "edumfa.lib.smsprovider.SmtpSMSProvider",
             "SmtpSMSProvider")
         
         _provider =get_sms_provider_class(
             "edumfa.lib.smsprovider.SmppSMSProvider",
             "SmppSMSProvider")
 
+        _provider =get_sms_provider_class(
+            "edumfa.lib.smsprovider.HttpMessageToUidProvider",
+            "HttpMessageToUidProvider")
+
         # A non-existing module will raise an error
         self.assertRaises(Exception,
                           get_sms_provider_class,
                           "DoesNotExist",
                           "DoesNotExist")
 
         # Any other arbitrary class will raise an error, since it has not
@@ -94,32 +100,36 @@
         gw = get_smsgateway(id=id)
         self.assertEqual(gw[0].description, "This is a sensible description")
 
         # update some options
         set_smsgateway(identifier, provider_module,
                        options={"HTTP_METHOD": "POST",
                                 "URL": "example.com",
-                                "IDENTICAL_KEY": "new option"},
+                                "IDENTICAL_KEY": "new option",
+                                "HTTP_PROXY": "myhttpproxy.example",
+                                "HTTPS_PROXY": "myhttpsproxy.example"},
                        headers={"Authorization": "ValueChanged",
                                 "IDENTICAL_KEY": "new header",
                                 "URL": "URL_in_headers"})
         gw = get_smsgateway(id=id)
-        self.assertEqual(len(gw[0].option_dict), 3)
+        self.assertEqual(len(gw[0].option_dict), 5)
         self.assertEqual(gw[0].option_dict.get("HTTP_METHOD"), "POST")
         self.assertEqual(gw[0].option_dict.get("URL"), "example.com")
         self.assertEqual(gw[0].option_dict.get("IDENTICAL_KEY"), "new option")
+        self.assertEqual(gw[0].option_dict.get("HTTP_PROXY"), "myhttpproxy.example")
+        self.assertEqual(gw[0].option_dict.get("HTTPS_PROXY"), "myhttpsproxy.example")
         self.assertEqual(gw[0].header_dict.get("Authorization"), "ValueChanged")
         self.assertEqual(gw[0].header_dict.get("BANANA"), None)
         self.assertEqual(gw[0].header_dict.get("IDENTICAL_KEY"), "new header")
         self.assertEqual(gw[0].header_dict.get("URL"), "URL_in_headers")
 
         # delete a single option
         r = delete_smsgateway_option(id, "URL")
         gw = get_smsgateway(id=id)
-        self.assertEqual(len(gw[0].option_dict), 2)
+        self.assertEqual(len(gw[0].option_dict), 4)
         self.assertEqual(gw[0].option_dict.get("HTTP_METHOD"), "POST")
         self.assertEqual(gw[0].option_dict.get("URL"), None)
         self.assertEqual(gw[0].option_dict.get("IDENTICAL_KEY"), "new option")
 
         # delete a single header
         r = delete_smsgateway_header(id, "IDENTICAL_KEY")
         gw = get_smsgateway(id=id)
@@ -220,14 +230,17 @@
 
     def test_01_missing_config(self):
         self.assertRaises(SMSError, self.missing_provider.submit_message,
                           "1234356", "Hello")
 
     @smtpmock.activate
     def test_02_simple_config_success(self):
+        params = self.simple_provider.parameters()
+        self.assertFalse(params.get("options_allowed"))
+        self.assertIn("MAILTO", params.get("parameters"))
         smtpmock.setdata(response={"recp@example.com": (200, "OK")})
         r = self.simple_provider.submit_message("123456", "Hello")
         self.assertTrue(r)
 
     @smtpmock.activate
     def test_03_simple_config_fail(self):
         smtpmock.setdata(response={"recp@example.com": (550,
@@ -309,14 +322,19 @@
               'PASSWORD': "password",
               'PROXY': "https://user:pw@1.2.3.4:8089"}
 
     def setUp(self):
         self.provider = SipgateSMSProvider()
         self.provider.load_config(self.config)
 
+    def test_00_config(self):
+        params = self.provider.parameters()
+        self.assertFalse(params.get("options_allowed"))
+        self.assertIn("REGEXP", params.get("parameters"))
+
     @responses.activate
     def test_01_success(self):
         responses.add(responses.POST,
                       self.url)
         # Here we need to send the SMS
         r = self.provider.submit_message("123456", "Hello")
         self.assertTrue(r)
@@ -431,27 +449,29 @@
                    "PARAMETER": {"from": "0170111111",
                                  "password": "yoursecret",
                                  "sender": "name",
                                  "account": "company_ltd"},
                    "SMS_TEXT_KEY": "text",
                    "SMS_PHONENUMBER_KEY": "destination",
                    "HTTP_Method": "POST",
-                   "PROXY": "http://username:password@your-proxy:8080",
+                   "HTTP_PROXY": "http://username:password@your-proxy:8080",
+                   "HTTPS_PROXY": "https://username:password@your-proxy:8080",
                    "RETURN_SUCCESS": "ID"
     }
 
     config_regexp = {"URL": post_url,
                      "PARAMETER": {"from": "0170111111",
                                    "password": "yoursecret",
                                    "sender": "name",
                                    "account": "company_ltd"},
                      "SMS_TEXT_KEY": "text",
                      "SMS_PHONENUMBER_KEY": "destination",
                      "HTTP_Method": "POST",
-                     "PROXY": "http://username:password@your-proxy:8080",
+                     "HTTP_PROXY": "http://username:password@your-proxy:8080",
+                     "HTTPS_PROXY": "https://username:password@your-proxy:8080",
                      "RETURN_SUCCESS": "ID",
                      "REGEXP": "/[+-/. ]//"
                      }
 
     get_url = "http://api.clickatell.com/http/sendmsg"
     config_get = {"URL": get_url,
                   "PARAMETER": {"user": "username",
@@ -763,7 +783,205 @@
         # Here we need to send the SMS
         with mock.patch("logging.Logger.debug") as log:
             r = regexp_provider.submit_message("+49 123/456-78", "Hello")
             self.assertTrue(r)
             log.assert_any_call("submitting message {0!r} to {1!s}".format("Hello", "4912345678"))
 
         delete_smsgateway(identifier_regexp)
+
+class HttpMessageToUidTestCase(MyTestCase):
+
+    url = "http://somegateway.com/send_api.cgi"
+    config = {"URL": url,
+               "PARAMETER": {"from": "0170111111",
+                             "password": "yoursecret",
+                             "sender": "name",
+                             "account": "company_ltd"},
+               "SMS_TEXT_KEY": "text",
+               "SMS_PHONENUMBER_KEY": "destination",
+               "HTTP_Method": "POST",
+               "HTTP_PROXY": "http://username:password@your-proxy:8080",
+               "HTTPS_PROXY": "https://username:password@your-proxy:8080",
+               "RETURN_SUCCESS": "ID",
+               "UID_TOKENINFO_ATTRIBUTE": "recipient_uid",
+               "POST_CHECK_URL": url
+               }
+
+    get_url = "http://api.clickatell.com/http/sendmsg"
+    config_get = {"URL": get_url,
+              "PARAMETER": {"user": "username",
+                            "password": "askme",
+                            "api_id": "12980436"},
+              "SMS_TEXT_KEY": "text",
+              "SMS_PHONENUMBER_KEY": "to",
+              "HTTP_Method": "GET",
+              "PROXY": "http://user:pass@1.2.3.4:8080",
+              "RETURN_FAIL": "Failed"
+              }
+
+    missing_url = "http://some.missing.url"
+    config_missing = {"PARAMETER": {"user": "username",
+                                    "password": "askme",
+                                    "api_id": "12980436"}
+                      }
+
+    basic_url = "https://fitz:sosecret@secret.gateway/some/path"
+    config_basicauth = {"URL": basic_url,
+                    "PARAMETER": {"user": "username",
+                                  "password": "askme",
+                                  "api_id": "12980436"}
+                    }
+
+    success_body = "ID 12345"
+    fail_body = "Failed"
+
+    def setUp(self):
+        self.provider = HttpMessageToUidProvider()
+        self.provider.load_config(self.config)
+
+        self.get_provider = HttpMessageToUidProvider()
+        self.get_provider.load_config(self.config_get)
+
+        self.missing_provider = HttpMessageToUidProvider()
+        self.missing_provider.load_config(self.config_missing)
+
+        self.auth_provider = HttpMessageToUidProvider()
+        self.auth_provider.load_config(self.config_basicauth)
+
+    def test_00_config(self):
+        self.assertTrue(self.provider.send_to_uid())
+        params = self.provider.parameters()
+        self.assertTrue(params.get("options_allowed"))
+        self.assertIn("UID_TOKENINFO_ATTRIBUTE", params.get("parameters"))
+
+    @responses.activate
+    def test_01_success(self):
+        responses.add(responses.POST,
+                      self.url,
+                      body=self.success_body)
+        # Here we need to send the SMS
+        r = self.provider.submit_message("testuser", "Hello")
+        self.assertTrue(r)
+
+    @responses.activate
+    def test_02_fail(self):
+        responses.add(responses.POST,
+                      self.url,
+                      body=self.fail_body)
+        # Here we need to send the SMS
+        self.assertRaises(SMSError, self.provider.submit_message,
+                          "testuser", "Hello")
+
+    @responses.activate
+    def test_03_code_fail(self):
+        responses.add(responses.POST,
+                      self.url,
+                      status=401)
+        # Here we need to send the SMS
+        self.assertRaises(SMSError, self.provider.submit_message,
+                          "testuser", "Hello")
+
+    @responses.activate
+    def test_04_postcheck_success(self):
+        responses.add(responses.POST,
+                      self.url,
+                      body=self.success_body)
+        # Here we need to send the SMS
+        r = self.provider.submit_post_check("testuser", "Hello")
+        self.assertTrue(r)
+
+    @responses.activate
+    def test_05_send_sms_get_success(self):
+        responses.add(responses.GET,
+                      self.get_url,
+                      body=self.success_body)
+        # Here we need to send the SMS
+        r = self.get_provider.submit_message("testuser", "Hello")
+        self.assertTrue(r)
+
+    @responses.activate
+    def test_06_send_sms_get_fail(self):
+        responses.add(responses.GET,
+                      self.get_url,
+                      body=self.fail_body)
+        # Here we need to send the SMS
+        self.assertRaises(SMSError, self.get_provider.submit_message,
+                          "testuser", "Hello")
+
+    @responses.activate
+    def test_07_missing_fail(self):
+        responses.add(responses.GET,
+                      self.missing_url)
+        self.assertRaises(SMSError, self.missing_provider.submit_message,
+                          "testuser", "Hello")
+
+    @responses.activate
+    def test_08_auth_success(self):
+        responses.add(responses.GET,
+                      self.basic_url)
+        r = self.auth_provider.submit_message("testuser", "Hello")
+        self.assertTrue(r)
+
+    @responses.activate
+    def test_08_auth_fail(self):
+        responses.add(responses.GET,
+                      self.basic_url,
+                      status=401)
+        self.assertRaises(SMSError, self.missing_provider.submit_message,
+                          "testuser", "Hello")
+
+    @responses.activate
+    def test_10_new_smsgateway(self):
+        identifier = "myGW"
+        provider_module = "edumfa.lib.smsprovider.HttpMessageToUidProvider" \
+                          ".HttpMessageToUidProvider"
+        id = set_smsgateway(identifier, provider_module, description="test",
+                            options={"HTTP_METHOD": "POST",
+                                     "URL": "http://example.com",
+                                     "SEND_DATA_AS_JSON": "no",
+                                     "RETURN_SUCCESS": "ID",
+                                     "text": "{otp}"},
+                            headers={"Authorization": "QWERTZ"})
+        self.assertTrue(id > 0)
+
+        sms = create_sms_instance(identifier)
+
+        responses.add(responses.POST,
+                      "http://example.com",
+                      body=self.success_body)
+        # Here we need to send the SMS
+        r = sms.submit_message("testuser", "Hello")
+        self.assertTrue(r)
+
+        delete_smsgateway(identifier)
+
+
+    @responses.activate
+    def test_11_send_sms_post_success_as_json(self):
+        identifier = "myGWJSON"
+        provider_module = "edumfa.lib.smsprovider.HttpMessageToUidProvider" \
+                          ".HttpMessageToUidProvider"
+        id = set_smsgateway(identifier, provider_module, description="test",
+                            options={"HTTP_METHOD": "POST",
+                                     "URL": "http://some.other.service",
+                                     "RETURN_SUCCESS": "ID",
+                                     "SEND_DATA_AS_JSON": "yes",
+                                     "text": "{otp}"},
+                            headers={"Authorization": "QWERTZ"})
+        self.assertTrue(id > 0)
+        provider = create_sms_instance(identifier=identifier)
+
+        # also check that the parameters are sent as json
+        responses.add(responses.POST,
+                      "http://some.other.service",
+                      body=self.success_body,
+                      match=[
+                          json_params_matcher({"text": 'Hello: 7'})
+                      ],)
+        # Here we need to send the SMS
+        with mock.patch("logging.Logger.debug") as mock_log:
+            r = provider.submit_message("testuser", 'Hello: 7')
+            self.assertTrue(r)
+            call = [x[0][0] for x in mock_log.call_args_list if x[0][0].startswith('passing')][0]
+            self.assertRegex(call, r'passing JSON data: {.*Hello: 7.*}', call)
+            r = provider.submit_post_check("testuser", 'Hello: 7')
+        delete_smsgateway(identifier)
```

### Comparing `edumfa-2.0.1/tests/test_lib_smtpserver.py` & `edumfa-2.0.2/tests/test_lib_smtpserver.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_sqlutils.py` & `edumfa-2.0.2/tests/test_lib_sqlutils.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_subscriptions.py` & `edumfa-2.0.2/tests/test_lib_subscriptions.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_task_eventcounter.py` & `edumfa-2.0.2/tests/test_lib_task_eventcounter.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_task_simplestats.py` & `edumfa-2.0.2/tests/test_lib_task_simplestats.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_tasks.py` & `edumfa-2.0.2/tests/test_lib_tasks.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_token.py` & `edumfa-2.0.2/tests/test_lib_token.py`

 * *Files 0% similar despite different names*

```diff
@@ -1602,15 +1602,15 @@
         tokenobject.token.save()
         r = tokenobject.token.check_pin("1234")
         self.assertTrue(r)
         remove_token(serial)
 
     def test_59_weigh_token_types(self):
 
-        class dummy_token(object):
+        class dummy_token:
             def __init__(self, type):
                 self.type = type
         self.assertEqual(1000, weigh_token_type(dummy_token("push")))
         self.assertTrue(weigh_token_type(dummy_token("push")) > weigh_token_type(dummy_token("hotp")))
         self.assertTrue(weigh_token_type(dummy_token("push")) > weigh_token_type(dummy_token("HOTP")))
         self.assertTrue(weigh_token_type(dummy_token("PUSH")) > weigh_token_type(dummy_token("hotp")))
```

### Comparing `edumfa-2.0.1/tests/test_lib_tokenclass.py` & `edumfa-2.0.2/tests/test_lib_tokenclass.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_tokengroup.py` & `edumfa-2.0.2/tests/test_lib_tokengroup.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_tokens_certificate.py` & `edumfa-2.0.2/tests/test_lib_tokens_certificate.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_tokens_daplug.py` & `edumfa-2.0.2/tests/test_lib_tokens_daplug.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_tokens_daypassword.py` & `edumfa-2.0.2/tests/test_lib_tokens_daypassword.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_tokens_email.py` & `edumfa-2.0.2/tests/test_lib_tokens_email.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_tokens_foureyes.py` & `edumfa-2.0.2/tests/test_lib_tokens_foureyes.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_tokens_hotp.py` & `edumfa-2.0.2/tests/test_lib_tokens_hotp.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_tokens_indexedsecret.py` & `edumfa-2.0.2/tests/test_lib_tokens_indexedsecret.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_tokens_motp.py` & `edumfa-2.0.2/tests/test_lib_tokens_motp.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_tokens_paper.py` & `edumfa-2.0.2/tests/test_lib_tokens_paper.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_tokens_passwordtoken.py` & `edumfa-2.0.2/tests/test_lib_tokens_passwordtoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_tokens_push.py` & `edumfa-2.0.2/tests/test_lib_tokens_push.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_tokens_questionnaire.py` & `edumfa-2.0.2/tests/test_lib_tokens_questionnaire.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_tokens_radius.py` & `edumfa-2.0.2/tests/test_lib_tokens_radius.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_tokens_registration.py` & `edumfa-2.0.2/tests/test_lib_tokens_registration.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_tokens_remote.py` & `edumfa-2.0.2/tests/test_lib_tokens_remote.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_tokens_sms.py` & `edumfa-2.0.2/tests/test_lib_tokens_sms.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_tokens_spass.py` & `edumfa-2.0.2/tests/test_lib_tokens_spass.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_tokens_ssh.py` & `edumfa-2.0.2/tests/test_lib_tokens_ssh.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_tokens_tan.py` & `edumfa-2.0.2/tests/test_lib_tokens_tan.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_tokens_tiqr.py` & `edumfa-2.0.2/tests/test_lib_tokens_tiqr.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_tokens_totp.py` & `edumfa-2.0.2/tests/test_lib_tokens_totp.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_tokens_u2f.py` & `edumfa-2.0.2/tests/test_lib_tokens_u2f.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_tokens_vasco.py` & `edumfa-2.0.2/tests/test_lib_tokens_vasco.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_tokens_webauthn.py` & `edumfa-2.0.2/tests/test_lib_tokens_webauthn.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_tokens_yubico.py` & `edumfa-2.0.2/tests/test_lib_tokens_yubico.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_tokens_yubikey.py` & `edumfa-2.0.2/tests/test_lib_tokens_yubikey.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_user.py` & `edumfa-2.0.2/tests/test_lib_user.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_usercache.py` & `edumfa-2.0.2/tests/test_lib_usercache.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_utils.py` & `edumfa-2.0.2/tests/test_lib_utils.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_lib_utils_compare.py` & `edumfa-2.0.2/tests/test_lib_utils_compare.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_mock_ldap3.py` & `edumfa-2.0.2/tests/test_mock_ldap3.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_resolver_realm.py` & `edumfa-2.0.2/tests/test_resolver_realm.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_scripts.py` & `edumfa-2.0.2/tests/test_scripts.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_ui_certificate.py` & `edumfa-2.0.2/tests/test_ui_certificate.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/test_ui_login.py` & `edumfa-2.0.2/tests/test_ui_login.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/testdata/FIDO-U2F-Security-Key-444x444.png` & `edumfa-2.0.2/tests/testdata/FIDO-U2F-Security-Key-444x444.png`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/testdata/attestation/yubico.pem` & `edumfa-2.0.2/tests/testdata/attestation/yubico.pem`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/testdata/audit.sqlite` & `edumfa-2.0.2/tests/testdata/audit.sqlite`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/testdata/ca/cacert.pem` & `edumfa-2.0.2/tests/testdata/ca/cacert.pem`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/testdata/ca/cakey.pem` & `edumfa-2.0.2/tests/testdata/ca/cakey.pem`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/testdata/ca/index.txt` & `edumfa-2.0.2/tests/testdata/ca/index.txt`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/testdata/ca/openssl.cnf` & `edumfa-2.0.2/tests/testdata/ca/openssl.cnf`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/testdata/dictionary` & `edumfa-2.0.2/tests/testdata/dictionary`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/testdata/event.conf` & `edumfa-2.0.2/tests/testdata/event.conf`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/testdata/firebase-test.json` & `edumfa-2.0.2/tests/testdata/firebase-test.json`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/testdata/google-services.json` & `edumfa-2.0.2/tests/testdata/google-services.json`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/testdata/gpg/pubring.gpg` & `edumfa-2.0.2/tests/testdata/gpg/pubring.gpg`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/testdata/gpg/random_seed` & `edumfa-2.0.2/tests/testdata/gpg/random_seed`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/testdata/gpg/secring.gpg` & `edumfa-2.0.2/tests/testdata/gpg/secring.gpg`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/testdata/gpg/trustdb.gpg` & `edumfa-2.0.2/tests/testdata/gpg/trustdb.gpg`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/testdata/import.oath.asc` & `edumfa-2.0.2/tests/testdata/import.oath.asc`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/testdata/jwt_sign.key` & `edumfa-2.0.2/tests/testdata/jwt_sign.key`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/testdata/logging.cfg` & `edumfa-2.0.2/tests/testdata/logging.cfg`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/testdata/logging.yml` & `edumfa-2.0.2/tests/testdata/logging.yml`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/testdata/msca-connector/ca.pem` & `edumfa-2.0.2/tests/testdata/msca-connector/ca.pem`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/testdata/msca-connector/privacyidea-encrypted.key` & `edumfa-2.0.2/tests/testdata/msca-connector/privacyidea-encrypted.key`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/testdata/msca-connector/privacyidea.key` & `edumfa-2.0.2/tests/testdata/msca-connector/privacyidea.key`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/testdata/msca-connector/privacyidea.pem` & `edumfa-2.0.2/tests/testdata/msca-connector/privacyidea.pem`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/testdata/passwd` & `edumfa-2.0.2/tests/testdata/passwd`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/testdata/passwords` & `edumfa-2.0.2/tests/testdata/passwords`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/testdata/policy.conf` & `edumfa-2.0.2/tests/testdata/policy.conf`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/testdata/private.pem` & `edumfa-2.0.2/tests/testdata/private.pem`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/testdata/pskc-aes.xml` & `edumfa-2.0.2/tests/testdata/pskc-aes.xml`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/testdata/pskc-password.xml` & `edumfa-2.0.2/tests/testdata/pskc-password.xml`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/testdata/test.sub` & `edumfa-2.0.2/tests/testdata/test.sub`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/testdata/test2.sub` & `edumfa-2.0.2/tests/testdata/test2.sub`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/testdata/testuser-api.sqlite` & `edumfa-2.0.2/tests/testdata/testuser-api.sqlite`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/testdata/testuser.sqlite` & `edumfa-2.0.2/tests/testdata/testuser.sqlite`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/testdata/testusercache.sqlite` & `edumfa-2.0.2/tests/testdata/testusercache.sqlite`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/testdata/trusted_attestation_roots/solokeys_device_attestation_ca.pem` & `edumfa-2.0.2/tests/testdata/trusted_attestation_roots/solokeys_device_attestation_ca.pem`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/testdata/trusted_attestation_roots/yubico_u2f_device_attestation_ca.pem` & `edumfa-2.0.2/tests/testdata/trusted_attestation_roots/yubico_u2f_device_attestation_ca.pem`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/testdata/yubico-oath-long.csv` & `edumfa-2.0.2/tests/testdata/yubico-oath-long.csv`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tests/testdata/yubico.csv` & `edumfa-2.0.2/tests/testdata/yubico.csv`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tools/creategoogleauthenticator-file` & `edumfa-2.0.2/tools/creategoogleauthenticator-file`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tools/edumfa-authorizedkeys` & `edumfa-2.0.2/tools/edumfa-authorizedkeys`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tools/edumfa-convert-base32.py` & `edumfa-2.0.2/tools/edumfa-convert-base32.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tools/edumfa-convert-token` & `edumfa-2.0.2/tools/edumfa-convert-token`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tools/edumfa-convert-token.1` & `edumfa-2.0.2/tools/edumfa-convert-token.1`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tools/edumfa-convert-xml-to-csv` & `edumfa-2.0.2/tools/edumfa-convert-xml-to-csv`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tools/edumfa-create-ad-users` & `edumfa-2.0.2/tools/edumfa-create-ad-users`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tools/edumfa-create-ad-users.1` & `edumfa-2.0.2/tools/edumfa-create-ad-users.1`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tools/edumfa-create-certificate` & `edumfa-2.0.2/tools/edumfa-create-certificate`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tools/edumfa-create-certificate.1` & `edumfa-2.0.2/tools/edumfa-create-certificate.1`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tools/edumfa-create-pwidresolver-user` & `edumfa-2.0.2/tools/edumfa-create-pwidresolver-user`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tools/edumfa-create-pwidresolver-user.1` & `edumfa-2.0.2/tools/edumfa-create-pwidresolver-user.1`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tools/edumfa-create-sqlidresolver-user` & `edumfa-2.0.2/tools/edumfa-create-sqlidresolver-user`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tools/edumfa-create-sqlidresolver-user.1` & `edumfa-2.0.2/tools/edumfa-create-sqlidresolver-user.1`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tools/edumfa-create-userdb` & `edumfa-2.0.2/tools/edumfa-create-userdb`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tools/edumfa-create-userdb.1` & `edumfa-2.0.2/tools/edumfa-create-userdb.1`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tools/edumfa-cron` & `edumfa-2.0.2/tools/edumfa-cron`

 * *Files 1% similar despite different names*

```diff
@@ -143,21 +143,21 @@
     print_stdout("=" * 120)
     for ptask in get_periodic_tasks():
         print_stdout(line_format.format(node_list=', '.join(ptask["nodes"]),
                                         options_json=json.dumps(ptask["options"]),
                                         **ptask))
 
 
-@cli.command()
+@cli.command("run_scheduled")
 @click.option("-d", "--dryrun",
               is_flag=True,
               help="Do not run any tasks, only show what would be done")
 @click.option("-n", "--node", "node_string",
               help="Override the node name (read from eduMFA config by default)")
-@click.option("-c", "--cron",
+@click.option("-c", "--cron", "cron_mode",
               is_flag=True,
               help="Run in 'cron mode', i.e. do not write to stdout, but write errors to stderr")
 def run_scheduled(node_string=None, dryrun=False, cron_mode=False):
     """
     Execute all periodic tasks that are scheduled to run.
     """
     app.config['cron_mode'] = cron_mode
```

### Comparing `edumfa-2.0.1/tools/edumfa-diag` & `edumfa-2.0.2/tools/edumfa-diag`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tools/edumfa-expired-users` & `edumfa-2.0.2/tools/edumfa-expired-users`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tools/edumfa-export-edumfa-counter.py` & `edumfa-2.0.2/tools/edumfa-export-edumfa-counter.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tools/edumfa-export-linotp-counter.py` & `edumfa-2.0.2/tools/edumfa-export-linotp-counter.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tools/edumfa-fetchssh` & `edumfa-2.0.2/tools/edumfa-fetchssh`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tools/edumfa-fetchssh.1` & `edumfa-2.0.2/tools/edumfa-fetchssh.1`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tools/edumfa-fix-access-rights` & `edumfa-2.0.2/tools/edumfa-fix-access-rights`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tools/edumfa-fix-access-rights.1` & `edumfa-2.0.2/tools/edumfa-fix-access-rights.1`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tools/edumfa-get-serial` & `edumfa-2.0.2/tools/edumfa-get-serial`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tools/edumfa-get-unused-tokens` & `edumfa-2.0.2/tools/edumfa-get-unused-tokens`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tools/edumfa-migrate-linotp.py` & `edumfa-2.0.2/tools/edumfa-migrate-linotp.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
                      "([0-9a-fA-F]{2})([0-9a-fA-F]{2})([0-9a-fA-F]{2})([0-9a-fA-F]{2})" \
                      "([0-9a-fA-F]{2})([0-9a-fA-F]{2})([0-9a-fA-F]{2})([0-9a-fA-F]{2})" \
                      "([0-9a-fA-F]{2})([0-9a-fA-F]{2})([0-9a-fA-F]{2})([0-9a-fA-F]{2})$"
 
 UUID_REPLACE_PATTERN = "\\4\\3\\2\\1-\\6\\5-\\8\\7-\\9\\10-\\11\\12\\13\\14\\15\\16"
 
 
-class Config(object):
+class Config:
 
     def __init__(self, config_file):
         with open(config_file, "r") as f:
             contents = f.read()
         config = json.loads(contents)
         self.ASSIGNMENTS = config.get("ASSIGNMENTS")
         self.LINOTP_URI = config.get("SQL").get("LINOTP_URI")
```

### Comparing `edumfa-2.0.1/tools/edumfa-pip-update` & `edumfa-2.0.2/tools/edumfa-pip-update`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tools/edumfa-pip-update.1` & `edumfa-2.0.2/tools/edumfa-pip-update.1`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tools/edumfa-queue-huey` & `edumfa-2.0.2/tools/edumfa-queue-huey`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tools/edumfa-schema-upgrade` & `edumfa-2.0.2/tools/edumfa-schema-upgrade`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tools/edumfa-standalone` & `edumfa-2.0.2/tools/edumfa-standalone`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tools/edumfa-sync-owncloud.py` & `edumfa-2.0.2/tools/edumfa-sync-owncloud.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         "EDUMFA_URI": "mysql+pymysql://pi:password@localhost/pi?charset=utf8mb4",
         "LOCAL_TABLE": "edumfa_oc_users",
         "INSERT_CHUNK_SIZE": 10000
     }
 }"""
 
 
-class Config(object):
+class Config:
 
     def __init__(self, config_file):
         with open(config_file, "r") as f:
             contents = f.read()
         config = json.loads(contents)
         self.OWNCLOUD_URI = config.get("SQL").get("OWNCLOUD_URI")
         self.EDUMFA_URI = config.get("SQL").get("EDUMFA_URI")
```

### Comparing `edumfa-2.0.1/tools/edumfa-token-janitor` & `edumfa-2.0.2/tools/edumfa-token-janitor`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tools/edumfa-update-counter.py` & `edumfa-2.0.2/tools/edumfa-update-counter.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tools/edumfa-update-linotp-counter.py` & `edumfa-2.0.2/tools/edumfa-update-linotp-counter.py`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tools/edumfa-user-action` & `edumfa-2.0.2/tools/edumfa-user-action`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tools/edumfa-usercache-cleanup` & `edumfa-2.0.2/tools/edumfa-usercache-cleanup`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tools/getgooglecodes` & `edumfa-2.0.2/tools/getgooglecodes`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tools/reset-edumfa` & `edumfa-2.0.2/tools/reset-edumfa`

 * *Files identical despite different names*

### Comparing `edumfa-2.0.1/tools/ssha.py` & `edumfa-2.0.2/tools/ssha.py`

 * *Files identical despite different names*

