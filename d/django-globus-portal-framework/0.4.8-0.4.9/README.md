# Comparing `tmp/django-globus-portal-framework-0.4.8.tar.gz` & `tmp/django-globus-portal-framework-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-globus-portal-framework-0.4.8.tar", last modified: Wed Mar 29 22:09:21 2023, max compression
+gzip compressed data, was "django-globus-portal-framework-0.4.9.tar", last modified: Tue Dec 19 16:40:54 2023, max compression
```

## Comparing `django-globus-portal-framework-0.4.8.tar` & `django-globus-portal-framework-0.4.9.tar`

### file list

```diff
@@ -1,135 +1,135 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 22:09:21.918273 django-globus-portal-framework-0.4.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-03-29 22:09:21.918273 django-globus-portal-framework-0.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 22:09:21.902273 django-globus-portal-framework-0.4.8/django_globus_portal_framework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-03-29 22:09:21.000000 django-globus-portal-framework-0.4.8/django_globus_portal_framework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-03-29 22:09:21.000000 django-globus-portal-framework-0.4.8/django_globus_portal_framework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 22:09:21.000000 django-globus-portal-framework-0.4.8/django_globus_portal_framework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-03-29 22:09:21.000000 django-globus-portal-framework-0.4.8/django_globus_portal_framework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-29 22:09:21.000000 django-globus-portal-framework-0.4.8/django_globus_portal_framework.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 22:09:21.902273 django-globus-portal-framework-0.4.8/globus_portal_framework/
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/context_processors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 22:09:21.902273 django-globus-portal-framework-0.4.8/globus_portal_framework/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/data/datacite.json
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/exc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9911 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/gclients.py
--rw-r--r--   0 runner    (1001) docker     (123)    37836 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/gsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/gtransfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 22:09:21.906273 django-globus-portal-framework-0.4.8/globus_portal_framework/modifiers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/modifiers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/modifiers/facets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 22:09:21.906273 django-globus-portal-framework-0.4.8/globus_portal_framework/search/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/search/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     8863 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 22:09:21.902273 django-globus-portal-framework-0.4.8/globus_portal_framework/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 22:09:21.898273 django-globus-portal-framework-0.4.8/globus_portal_framework/static/bootstrap/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 22:09:21.906273 django-globus-portal-framework-0.4.8/globus_portal_framework/static/bootstrap/css/
--rw-r--r--   0 runner    (1001) docker     (123)    43852 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/static/bootstrap/css/bootstrap-grid.css
--rw-r--r--   0 runner    (1001) docker     (123)    95910 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/static/bootstrap/css/bootstrap-grid.css.map
--rw-r--r--   0 runner    (1001) docker     (123)    34243 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/static/bootstrap/css/bootstrap-grid.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    76209 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/static/bootstrap/css/bootstrap-grid.min.css.map
--rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/static/bootstrap/css/bootstrap-reboot.css
--rw-r--r--   0 runner    (1001) docker     (123)    57721 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/static/bootstrap/css/bootstrap-reboot.css.map
--rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/static/bootstrap/css/bootstrap-reboot.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    25881 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/static/bootstrap/css/bootstrap-reboot.min.css.map
--rw-r--r--   0 runner    (1001) docker     (123)   178152 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/static/bootstrap/css/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (123)   411645 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/static/bootstrap/css/bootstrap.css.map
--rw-r--r--   0 runner    (1001) docker     (123)   144877 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/static/bootstrap/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   551641 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/static/bootstrap/css/bootstrap.min.css.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 22:09:21.910273 django-globus-portal-framework-0.4.8/globus_portal_framework/static/bootstrap/js/
--rw-r--r--   0 runner    (1001) docker     (123)   195855 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/static/bootstrap/js/bootstrap.bundle.js
--rw-r--r--   0 runner    (1001) docker     (123)   326634 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/static/bootstrap/js/bootstrap.bundle.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    67742 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/static/bootstrap/js/bootstrap.bundle.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   273872 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/static/bootstrap/js/bootstrap.bundle.min.js.map
--rw-r--r--   0 runner    (1001) docker     (123)   115048 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/static/bootstrap/js/bootstrap.js
--rw-r--r--   0 runner    (1001) docker     (123)   195373 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/static/bootstrap/js/bootstrap.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    48944 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/static/bootstrap/js/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   161998 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/static/bootstrap/js/bootstrap.min.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 22:09:21.910273 django-globus-portal-framework-0.4.8/globus_portal_framework/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/static/css/detail-base.css
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/static/css/detail-overview.css
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/static/css/search.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 22:09:21.902273 django-globus-portal-framework-0.4.8/globus_portal_framework/static/globus-portal-framework/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 22:09:21.910273 django-globus-portal-framework-0.4.8/globus_portal_framework/static/globus-portal-framework/images/
--rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/static/globus-portal-framework/images/globus.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 22:09:21.914273 django-globus-portal-framework-0.4.8/globus_portal_framework/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)   672449 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/static/js/fontawesome-all.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    86927 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/static/js/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    19188 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/static/js/popper.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   112587 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/static/js/popper.min.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 22:09:21.914273 django-globus-portal-framework-0.4.8/globus_portal_framework/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/templates/404.html
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/templates/500.html
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/templates/allowed-groups.html
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/templates/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 22:09:21.914273 django-globus-portal-framework-0.4.8/globus_portal_framework/templates/components/
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/templates/components/detail-error.html
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/templates/components/detail-nav.html
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/templates/components/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/templates/components/message.html
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/templates/components/messages.html
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/templates/components/permission-error.html
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/templates/components/search-facets.html
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/templates/components/search-results.html
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/templates/detail-base.html
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/templates/detail-overview.html
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/templates/detail-preview.html
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/templates/detail-transfer.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 22:09:21.902273 django-globus-portal-framework-0.4.8/globus_portal_framework/templates/globus-portal-framework/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 22:09:21.918273 django-globus-portal-framework-0.4.8/globus_portal_framework/templates/globus-portal-framework/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/templates/globus-portal-framework/v2/allowed-groups.html
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/templates/globus-portal-framework/v2/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 22:09:21.918273 django-globus-portal-framework-0.4.8/globus_portal_framework/templates/globus-portal-framework/v2/components/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/templates/globus-portal-framework/v2/components/base-head-extras.html
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/templates/globus-portal-framework/v2/components/base-nav.html
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/templates/globus-portal-framework/v2/components/copy-to-clipboard.html
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/templates/globus-portal-framework/v2/components/detail-dc-metadata.html
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/templates/globus-portal-framework/v2/components/detail-general-metadata.html
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/templates/globus-portal-framework/v2/components/detail-nav.html
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/templates/globus-portal-framework/v2/components/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/templates/globus-portal-framework/v2/components/message.html
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/templates/globus-portal-framework/v2/components/messages.html
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/templates/globus-portal-framework/v2/components/search-facets.html
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/templates/globus-portal-framework/v2/components/search-nav.html
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/templates/globus-portal-framework/v2/components/search-results.html
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/templates/globus-portal-framework/v2/detail-base.html
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/templates/globus-portal-framework/v2/detail-overview.html
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/templates/globus-portal-framework/v2/detail-preview.html
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/templates/globus-portal-framework/v2/detail-transfer.html
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/templates/globus-portal-framework/v2/index-selection.html
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/templates/globus-portal-framework/v2/landing-page.html
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/templates/globus-portal-framework/v2/search-about.html
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/templates/globus-portal-framework/v2/search-base.html
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/templates/globus-portal-framework/v2/search-debug-detail.html
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/templates/globus-portal-framework/v2/search-debug.html
--rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/templates/globus-portal-framework/v2/search.html
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/templates/index-selection.html
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/templates/search-debug-detail.html
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/templates/search-debug.html
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/templates/search.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 22:09:21.918273 django-globus-portal-framework-0.4.8/globus_portal_framework/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/templatetags/index_template.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/templatetags/is_active.py
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/urls_debugging.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 22:09:21.918273 django-globus-portal-framework-0.4.8/globus_portal_framework/views/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12921 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/views/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/views/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/globus_portal_framework/views/mixins.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      555 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/manage.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-03-29 22:09:21.918273 django-globus-portal-framework-0.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-03-29 22:09:13.000000 django-globus-portal-framework-0.4.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 16:40:54.726224 django-globus-portal-framework-0.4.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2023-12-19 16:40:54.726224 django-globus-portal-framework-0.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 16:40:54.726224 django-globus-portal-framework-0.4.9/django_globus_portal_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2023-12-19 16:40:54.000000 django-globus-portal-framework-0.4.9/django_globus_portal_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6417 2023-12-19 16:40:54.000000 django-globus-portal-framework-0.4.9/django_globus_portal_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-19 16:40:54.000000 django-globus-portal-framework-0.4.9/django_globus_portal_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2023-12-19 16:40:54.000000 django-globus-portal-framework-0.4.9/django_globus_portal_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2023-12-19 16:40:54.000000 django-globus-portal-framework-0.4.9/django_globus_portal_framework.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 16:40:54.706224 django-globus-portal-framework-0.4.9/globus_portal_framework/
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6593 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4228 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/context_processors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 16:40:54.706224 django-globus-portal-framework-0.4.9/globus_portal_framework/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/data/datacite.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4636 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/exc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9911 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/gclients.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37166 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/gsearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8624 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/gtransfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3431 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 16:40:54.706224 django-globus-portal-framework-0.4.9/globus_portal_framework/modifiers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/modifiers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/modifiers/facets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 16:40:54.706224 django-globus-portal-framework-0.4.9/globus_portal_framework/search/
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/search/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8863 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 16:40:54.698224 django-globus-portal-framework-0.4.9/globus_portal_framework/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 16:40:54.698224 django-globus-portal-framework-0.4.9/globus_portal_framework/static/bootstrap/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 16:40:54.710224 django-globus-portal-framework-0.4.9/globus_portal_framework/static/bootstrap/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    43852 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/static/bootstrap/css/bootstrap-grid.css
+-rw-r--r--   0 runner    (1001) docker     (127)    95910 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/static/bootstrap/css/bootstrap-grid.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    34243 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/static/bootstrap/css/bootstrap-grid.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    76209 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/static/bootstrap/css/bootstrap-grid.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)     4798 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/static/bootstrap/css/bootstrap-reboot.css
+-rw-r--r--   0 runner    (1001) docker     (127)    57721 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/static/bootstrap/css/bootstrap-reboot.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)     3936 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/static/bootstrap/css/bootstrap-reboot.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    25881 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/static/bootstrap/css/bootstrap-reboot.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)   178152 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/static/bootstrap/css/bootstrap.css
+-rw-r--r--   0 runner    (1001) docker     (127)   411645 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/static/bootstrap/css/bootstrap.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)   144877 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/static/bootstrap/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   551641 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/static/bootstrap/css/bootstrap.min.css.map
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 16:40:54.714224 django-globus-portal-framework-0.4.9/globus_portal_framework/static/bootstrap/js/
+-rw-r--r--   0 runner    (1001) docker     (127)   195855 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/static/bootstrap/js/bootstrap.bundle.js
+-rw-r--r--   0 runner    (1001) docker     (127)   326634 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/static/bootstrap/js/bootstrap.bundle.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)    67742 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/static/bootstrap/js/bootstrap.bundle.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   273872 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/static/bootstrap/js/bootstrap.bundle.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)   115048 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/static/bootstrap/js/bootstrap.js
+-rw-r--r--   0 runner    (1001) docker     (127)   195373 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/static/bootstrap/js/bootstrap.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)    48944 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/static/bootstrap/js/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   161998 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/static/bootstrap/js/bootstrap.min.js.map
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 16:40:54.714224 django-globus-portal-framework-0.4.9/globus_portal_framework/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/static/css/detail-base.css
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/static/css/detail-overview.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/static/css/search.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 16:40:54.698224 django-globus-portal-framework-0.4.9/globus_portal_framework/static/globus-portal-framework/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 16:40:54.714224 django-globus-portal-framework-0.4.9/globus_portal_framework/static/globus-portal-framework/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     6177 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/static/globus-portal-framework/images/globus.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 16:40:54.718224 django-globus-portal-framework-0.4.9/globus_portal_framework/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)   672449 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/static/js/fontawesome-all.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    86927 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/static/js/jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    19188 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/static/js/popper.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   112587 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/static/js/popper.min.js.map
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 16:40:54.718224 django-globus-portal-framework-0.4.9/globus_portal_framework/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/templates/404.html
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/templates/500.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/templates/allowed-groups.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2387 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/templates/base.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 16:40:54.722224 django-globus-portal-framework-0.4.9/globus_portal_framework/templates/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/templates/components/detail-error.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/templates/components/detail-nav.html
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/templates/components/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/templates/components/message.html
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/templates/components/messages.html
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/templates/components/permission-error.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/templates/components/search-facets.html
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/templates/components/search-results.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/templates/detail-base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/templates/detail-overview.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/templates/detail-preview.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/templates/detail-transfer.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 16:40:54.698224 django-globus-portal-framework-0.4.9/globus_portal_framework/templates/globus-portal-framework/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 16:40:54.722224 django-globus-portal-framework-0.4.9/globus_portal_framework/templates/globus-portal-framework/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/templates/globus-portal-framework/v2/allowed-groups.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/templates/globus-portal-framework/v2/base.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 16:40:54.726224 django-globus-portal-framework-0.4.9/globus_portal_framework/templates/globus-portal-framework/v2/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/templates/globus-portal-framework/v2/components/base-head-extras.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/templates/globus-portal-framework/v2/components/base-nav.html
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/templates/globus-portal-framework/v2/components/copy-to-clipboard.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/templates/globus-portal-framework/v2/components/detail-dc-metadata.html
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/templates/globus-portal-framework/v2/components/detail-general-metadata.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/templates/globus-portal-framework/v2/components/detail-nav.html
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/templates/globus-portal-framework/v2/components/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/templates/globus-portal-framework/v2/components/message.html
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/templates/globus-portal-framework/v2/components/messages.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/templates/globus-portal-framework/v2/components/search-facets.html
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/templates/globus-portal-framework/v2/components/search-nav.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/templates/globus-portal-framework/v2/components/search-results.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/templates/globus-portal-framework/v2/detail-base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/templates/globus-portal-framework/v2/detail-overview.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/templates/globus-portal-framework/v2/detail-preview.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/templates/globus-portal-framework/v2/detail-transfer.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/templates/globus-portal-framework/v2/index-selection.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/templates/globus-portal-framework/v2/landing-page.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/templates/globus-portal-framework/v2/search-about.html
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/templates/globus-portal-framework/v2/search-base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/templates/globus-portal-framework/v2/search-debug-detail.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/templates/globus-portal-framework/v2/search-debug.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/templates/globus-portal-framework/v2/search.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/templates/index-selection.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/templates/search-debug-detail.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/templates/search-debug.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3261 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/templates/search.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 16:40:54.726224 django-globus-portal-framework-0.4.9/globus_portal_framework/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/templatetags/index_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/templatetags/is_active.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/urls_debugging.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 16:40:54.726224 django-globus-portal-framework-0.4.9/globus_portal_framework/views/
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12921 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/views/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6585 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/views/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/globus_portal_framework/views/mixins.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      555 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/manage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2023-12-19 16:40:54.726224 django-globus-portal-framework-0.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2023-12-19 16:40:47.000000 django-globus-portal-framework-0.4.9/setup.py
```

### Comparing `django-globus-portal-framework-0.4.8/LICENSE` & `django-globus-portal-framework-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/MANIFEST.in` & `django-globus-portal-framework-0.4.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/PKG-INFO` & `django-globus-portal-framework-0.4.9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-globus-portal-framework
-Version: 0.4.8
+Version: 0.4.9
 Summary: A framework for collating Globus Search data for use with various Globus services. 
 Home-page: https://github.com/globus/django-globus-portal-framework
 Author: Globus Team
 Author-email: support@globus.org
 License: apache 2.0
 Keywords: globus,django
 Classifier: Intended Audience :: Developers
@@ -15,14 +15,19 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Communications :: File Sharing
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: django<5
+Requires-Dist: globus_sdk<4.0.0
+Requires-Dist: social-auth-app-django<6.0.0,>=3.0.0
+Requires-Dist: python-jose[cryptography]>=3.0.1
+Requires-Dist: packaging>=21.0
 
 Django Globus Portal Framework
 ==============================
 
 .. image:: https://zenodo.org/badge/118486682.svg
    :target: https://zenodo.org/badge/latestdoi/118486682
```

### Comparing `django-globus-portal-framework-0.4.8/README.rst` & `django-globus-portal-framework-0.4.9/README.rst`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/django_globus_portal_framework.egg-info/PKG-INFO` & `django-globus-portal-framework-0.4.9/django_globus_portal_framework.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-globus-portal-framework
-Version: 0.4.8
+Version: 0.4.9
 Summary: A framework for collating Globus Search data for use with various Globus services. 
 Home-page: https://github.com/globus/django-globus-portal-framework
 Author: Globus Team
 Author-email: support@globus.org
 License: apache 2.0
 Keywords: globus,django
 Classifier: Intended Audience :: Developers
@@ -15,14 +15,19 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Communications :: File Sharing
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: django<5
+Requires-Dist: globus_sdk<4.0.0
+Requires-Dist: social-auth-app-django<6.0.0,>=3.0.0
+Requires-Dist: python-jose[cryptography]>=3.0.1
+Requires-Dist: packaging>=21.0
 
 Django Globus Portal Framework
 ==============================
 
 .. image:: https://zenodo.org/badge/118486682.svg
    :target: https://zenodo.org/badge/latestdoi/118486682
```

### Comparing `django-globus-portal-framework-0.4.8/django_globus_portal_framework.egg-info/SOURCES.txt` & `django-globus-portal-framework-0.4.9/django_globus_portal_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/__init__.py` & `django-globus-portal-framework-0.4.9/globus_portal_framework/__init__.py`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/api.py` & `django-globus-portal-framework-0.4.9/globus_portal_framework/api.py`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/auth.py` & `django-globus-portal-framework-0.4.9/globus_portal_framework/auth.py`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/checks.py` & `django-globus-portal-framework-0.4.9/globus_portal_framework/checks.py`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/constants.py` & `django-globus-portal-framework-0.4.9/globus_portal_framework/constants.py`

 * *Files 12% similar despite different names*

```diff
@@ -50,23 +50,21 @@
     'month': '%Y-%m',
     'day': '%Y-%m-%d',
     'time': '%Y-%m-%d %H:%M:%S'
 }
 
 VALID_SEARCH_KEYS = [
     'q', 'limit', 'offset', 'facets', 'filters', 'boosts', 'sort',
-    'query_template', 'advanced', 'bypass_visible_to', 'result_format_version',
+    'query_template', 'advanced', 'bypass_visible_to',
 ]
 
 VALID_SEARCH_FACET_KEYS = [
     'name', 'type', 'field_name', 'size', 'histogram_range', 'date_interval',
     'missing'
 ]
-# https://docs.globus.org/api/search/search/#request_documents
-DEFAULT_RESULT_FORMAT_VERSION = '2019-08-27'
 
 BASE_TEMPLATES = 'globus-portal-framework/v2/'
 
 # drop_empty enforces backwards compatible facet handling for 0.3.x
 DEFAULT_FACET_MODIFIERS = [
     'globus_portal_framework.modifiers.facets.drop_empty',
 ]
```

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/context_processors.py` & `django-globus-portal-framework-0.4.9/globus_portal_framework/context_processors.py`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/data/datacite.json` & `django-globus-portal-framework-0.4.9/globus_portal_framework/data/datacite.json`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/exc.py` & `django-globus-portal-framework-0.4.9/globus_portal_framework/exc.py`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/gclients.py` & `django-globus-portal-framework-0.4.9/globus_portal_framework/gclients.py`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/gsearch.py` & `django-globus-portal-framework-0.4.9/globus_portal_framework/gsearch.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,16 +23,14 @@
     FACET_NAME_PATTERN,
 
     FILTER_YEAR, FILTER_MONTH, FILTER_DAY, FILTER_HOUR, FILTER_MINUTE,
     FILTER_SECOND,
 
     VALID_SEARCH_FACET_KEYS, VALID_SEARCH_KEYS,
 
-    DEFAULT_RESULT_FORMAT_VERSION,
-
     DEFAULT_FACET_MODIFIERS,
 )
 FILTER_RANGE_SEPARATOR = getattr(settings, 'FILTER_RANGE_SEPARATOR',
                                  FILTER_DEFAULT_RANGE_SEPARATOR)
 
 
 log = logging.getLogger(__name__)
@@ -92,16 +90,14 @@
         'q': query,
         'facets': prepare_search_facets(index_data.get('facets', [])),
         'filters': filters,
         'offset': (int(page) - 1) * get_setting('SEARCH_RESULTS_PER_PAGE'),
         'limit': get_setting('SEARCH_RESULTS_PER_PAGE')
     })
     search_data.update(search_kwargs or {})
-    search_data['result_format_version'] = search_data.get(
-        'result_format_version', DEFAULT_RESULT_FORMAT_VERSION)
     try:
         result = client.post_search(index_data['uuid'], search_data)
         return {
             'search_results': process_search_data(index_data.get('fields', []),
                                                   result.data['gmeta']),
             'facets': get_facets(result, index_data.get('facets', []),
                                  filters, index_data.get('filter_match'),
@@ -439,20 +435,15 @@
 def get_subject(index, subject, user=None):
     """Get a subject and run the result through the SEARCH_MAPPER defined
     in settings.py. If no subject exists, return context with the 'subject'
     and an 'error' message."""
     client = load_search_client(user)
     try:
         idata = get_index(index)
-        if version.parse(globus_sdk.version.__version__).major < 3:
-            params = dict(result_format_version=DEFAULT_RESULT_FORMAT_VERSION)
-        else:
-            rfv = dict(result_format_version=DEFAULT_RESULT_FORMAT_VERSION)
-            params = dict(query_params=rfv)
-        result = client.get_subject(idata['uuid'], unquote(subject), **params)
+        result = client.get_subject(idata['uuid'], unquote(subject))
         return process_search_data(idata.get('fields', {}), [result.data])[0]
     except globus_sdk.SearchAPIError:
         return {'subject': subject, 'error': 'No data was found for subject'}
 
 
 def process_search_data(field_mappers, results):
     """
@@ -462,18 +453,14 @@
     :param results: List of GMeta results, which would be the r.data['gmeta']
     in from a simple query to Globus Search. See here:
     https://docs.globus.org/api/search/schemas/GMetaResult/
     :return: A list of search results:
     """
     structured_results = []
     for gmeta_result in results:
-        if gmeta_result.get('@version') != DEFAULT_RESULT_FORMAT_VERSION:
-            log.warning('Unsupported result format version '
-                        '{}'.format(gmeta_result['@version']))
-            continue
 
         entries = gmeta_result['entries']
         content = [e['content'] for e in entries]
         result = {
             'subject': quote_plus(gmeta_result['subject']),
             'all': content
         }
```

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/gtransfer.py` & `django-globus-portal-framework-0.4.9/globus_portal_framework/gtransfer.py`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/middleware.py` & `django-globus-portal-framework-0.4.9/globus_portal_framework/middleware.py`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/modifiers/facets.py` & `django-globus-portal-framework-0.4.9/globus_portal_framework/modifiers/facets.py`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/settings.py` & `django-globus-portal-framework-0.4.9/globus_portal_framework/settings.py`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/static/bootstrap/css/bootstrap-grid.css` & `django-globus-portal-framework-0.4.9/globus_portal_framework/static/bootstrap/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/static/bootstrap/css/bootstrap-grid.css.map` & `django-globus-portal-framework-0.4.9/globus_portal_framework/static/bootstrap/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/static/bootstrap/css/bootstrap-grid.min.css` & `django-globus-portal-framework-0.4.9/globus_portal_framework/static/bootstrap/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/static/bootstrap/css/bootstrap-grid.min.css.map` & `django-globus-portal-framework-0.4.9/globus_portal_framework/static/bootstrap/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/static/bootstrap/css/bootstrap-reboot.css` & `django-globus-portal-framework-0.4.9/globus_portal_framework/static/bootstrap/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/static/bootstrap/css/bootstrap-reboot.css.map` & `django-globus-portal-framework-0.4.9/globus_portal_framework/static/bootstrap/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/static/bootstrap/css/bootstrap-reboot.min.css` & `django-globus-portal-framework-0.4.9/globus_portal_framework/static/bootstrap/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/static/bootstrap/css/bootstrap-reboot.min.css.map` & `django-globus-portal-framework-0.4.9/globus_portal_framework/static/bootstrap/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/static/bootstrap/css/bootstrap.css` & `django-globus-portal-framework-0.4.9/globus_portal_framework/static/bootstrap/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/static/bootstrap/css/bootstrap.css.map` & `django-globus-portal-framework-0.4.9/globus_portal_framework/static/bootstrap/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/static/bootstrap/css/bootstrap.min.css` & `django-globus-portal-framework-0.4.9/globus_portal_framework/static/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/static/bootstrap/css/bootstrap.min.css.map` & `django-globus-portal-framework-0.4.9/globus_portal_framework/static/bootstrap/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/static/bootstrap/js/bootstrap.bundle.js` & `django-globus-portal-framework-0.4.9/globus_portal_framework/static/bootstrap/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/static/bootstrap/js/bootstrap.bundle.js.map` & `django-globus-portal-framework-0.4.9/globus_portal_framework/static/bootstrap/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/static/bootstrap/js/bootstrap.bundle.min.js` & `django-globus-portal-framework-0.4.9/globus_portal_framework/static/bootstrap/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/static/bootstrap/js/bootstrap.bundle.min.js.map` & `django-globus-portal-framework-0.4.9/globus_portal_framework/static/bootstrap/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/static/bootstrap/js/bootstrap.js` & `django-globus-portal-framework-0.4.9/globus_portal_framework/static/bootstrap/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/static/bootstrap/js/bootstrap.js.map` & `django-globus-portal-framework-0.4.9/globus_portal_framework/static/bootstrap/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/static/bootstrap/js/bootstrap.min.js` & `django-globus-portal-framework-0.4.9/globus_portal_framework/static/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/static/bootstrap/js/bootstrap.min.js.map` & `django-globus-portal-framework-0.4.9/globus_portal_framework/static/bootstrap/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/static/css/search.css` & `django-globus-portal-framework-0.4.9/globus_portal_framework/static/css/search.css`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/static/globus-portal-framework/images/globus.png` & `django-globus-portal-framework-0.4.9/globus_portal_framework/static/globus-portal-framework/images/globus.png`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/static/js/fontawesome-all.min.js` & `django-globus-portal-framework-0.4.9/globus_portal_framework/static/js/fontawesome-all.min.js`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/static/js/jquery.min.js` & `django-globus-portal-framework-0.4.9/globus_portal_framework/static/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/static/js/popper.min.js` & `django-globus-portal-framework-0.4.9/globus_portal_framework/static/js/popper.min.js`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/static/js/popper.min.js.map` & `django-globus-portal-framework-0.4.9/globus_portal_framework/static/js/popper.min.js.map`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/templates/allowed-groups.html` & `django-globus-portal-framework-0.4.9/globus_portal_framework/templates/allowed-groups.html`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/templates/base.html` & `django-globus-portal-framework-0.4.9/globus_portal_framework/templates/base.html`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/templates/components/detail-error.html` & `django-globus-portal-framework-0.4.9/globus_portal_framework/templates/components/detail-error.html`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/templates/components/detail-nav.html` & `django-globus-portal-framework-0.4.9/globus_portal_framework/templates/components/detail-nav.html`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/templates/components/message.html` & `django-globus-portal-framework-0.4.9/globus_portal_framework/templates/components/message.html`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/templates/components/search-facets.html` & `django-globus-portal-framework-0.4.9/globus_portal_framework/templates/components/search-facets.html`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/templates/components/search-results.html` & `django-globus-portal-framework-0.4.9/globus_portal_framework/templates/components/search-results.html`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/templates/detail-base.html` & `django-globus-portal-framework-0.4.9/globus_portal_framework/templates/detail-base.html`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/templates/detail-overview.html` & `django-globus-portal-framework-0.4.9/globus_portal_framework/templates/detail-overview.html`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/templates/detail-preview.html` & `django-globus-portal-framework-0.4.9/globus_portal_framework/templates/detail-preview.html`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/templates/detail-transfer.html` & `django-globus-portal-framework-0.4.9/globus_portal_framework/templates/detail-transfer.html`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/templates/globus-portal-framework/v2/allowed-groups.html` & `django-globus-portal-framework-0.4.9/globus_portal_framework/templates/globus-portal-framework/v2/allowed-groups.html`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/templates/globus-portal-framework/v2/base.html` & `django-globus-portal-framework-0.4.9/globus_portal_framework/templates/globus-portal-framework/v2/base.html`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/templates/globus-portal-framework/v2/components/base-nav.html` & `django-globus-portal-framework-0.4.9/globus_portal_framework/templates/globus-portal-framework/v2/components/base-nav.html`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/templates/globus-portal-framework/v2/components/copy-to-clipboard.html` & `django-globus-portal-framework-0.4.9/globus_portal_framework/templates/globus-portal-framework/v2/components/copy-to-clipboard.html`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/templates/globus-portal-framework/v2/components/detail-dc-metadata.html` & `django-globus-portal-framework-0.4.9/globus_portal_framework/templates/globus-portal-framework/v2/components/detail-dc-metadata.html`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/templates/globus-portal-framework/v2/components/detail-nav.html` & `django-globus-portal-framework-0.4.9/globus_portal_framework/templates/globus-portal-framework/v2/components/detail-nav.html`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/templates/globus-portal-framework/v2/components/message.html` & `django-globus-portal-framework-0.4.9/globus_portal_framework/templates/globus-portal-framework/v2/components/message.html`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/templates/globus-portal-framework/v2/components/search-facets.html` & `django-globus-portal-framework-0.4.9/globus_portal_framework/templates/globus-portal-framework/v2/components/search-facets.html`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/templates/globus-portal-framework/v2/components/search-results.html` & `django-globus-portal-framework-0.4.9/globus_portal_framework/templates/globus-portal-framework/v2/components/search-results.html`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/templates/globus-portal-framework/v2/detail-base.html` & `django-globus-portal-framework-0.4.9/globus_portal_framework/templates/globus-portal-framework/v2/detail-base.html`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/templates/globus-portal-framework/v2/detail-overview.html` & `django-globus-portal-framework-0.4.9/globus_portal_framework/templates/globus-portal-framework/v2/detail-overview.html`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/templates/globus-portal-framework/v2/detail-preview.html` & `django-globus-portal-framework-0.4.9/globus_portal_framework/templates/globus-portal-framework/v2/detail-preview.html`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/templates/globus-portal-framework/v2/detail-transfer.html` & `django-globus-portal-framework-0.4.9/globus_portal_framework/templates/globus-portal-framework/v2/detail-transfer.html`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/templates/globus-portal-framework/v2/index-selection.html` & `django-globus-portal-framework-0.4.9/globus_portal_framework/templates/globus-portal-framework/v2/index-selection.html`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/templates/globus-portal-framework/v2/landing-page.html` & `django-globus-portal-framework-0.4.9/globus_portal_framework/templates/globus-portal-framework/v2/landing-page.html`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/templates/globus-portal-framework/v2/search-about.html` & `django-globus-portal-framework-0.4.9/globus_portal_framework/templates/globus-portal-framework/v2/search-about.html`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/templates/globus-portal-framework/v2/search-base.html` & `django-globus-portal-framework-0.4.9/globus_portal_framework/templates/globus-portal-framework/v2/search-base.html`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/templates/globus-portal-framework/v2/search-debug-detail.html` & `django-globus-portal-framework-0.4.9/globus_portal_framework/templates/globus-portal-framework/v2/search-debug-detail.html`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/templates/globus-portal-framework/v2/search-debug.html` & `django-globus-portal-framework-0.4.9/globus_portal_framework/templates/globus-portal-framework/v2/search-debug.html`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/templates/globus-portal-framework/v2/search.html` & `django-globus-portal-framework-0.4.9/globus_portal_framework/templates/globus-portal-framework/v2/search.html`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/templates/index-selection.html` & `django-globus-portal-framework-0.4.9/globus_portal_framework/templates/index-selection.html`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/templates/search-debug-detail.html` & `django-globus-portal-framework-0.4.9/globus_portal_framework/templates/search-debug-detail.html`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/templates/search-debug.html` & `django-globus-portal-framework-0.4.9/globus_portal_framework/templates/search-debug.html`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/templates/search.html` & `django-globus-portal-framework-0.4.9/globus_portal_framework/templates/search.html`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/templatetags/index_template.py` & `django-globus-portal-framework-0.4.9/globus_portal_framework/templatetags/index_template.py`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/templatetags/is_active.py` & `django-globus-portal-framework-0.4.9/globus_portal_framework/templatetags/is_active.py`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/urls.py` & `django-globus-portal-framework-0.4.9/globus_portal_framework/urls.py`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/views/base.py` & `django-globus-portal-framework-0.4.9/globus_portal_framework/views/base.py`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/globus_portal_framework/views/generic.py` & `django-globus-portal-framework-0.4.9/globus_portal_framework/views/generic.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,14 @@
     get_search_query, process_search_data, get_index, prepare_search_facets,
     get_pagination, get_subject,
     )
 from globus_portal_framework.gclients import (
     load_search_client
 )
 import globus_portal_framework.exc
-from globus_portal_framework.constants import DEFAULT_RESULT_FORMAT_VERSION
 
 
 log = logging.getLogger(__name__)
 
 
 class SearchView(View):
     """
@@ -122,15 +121,14 @@
         data = {
             'q': self.query,
             'filters': self.filters,
             'facets': self.facets,
             'offset': self.offset,
             'sort': self.sort,
             'limit': self.results_per_page,
-            'result_format_version': DEFAULT_RESULT_FORMAT_VERSION,
         }
         try:
             index_info = self.get_index_info(index)
             result = self.post_search(self.get_search_client(),
                                       index_info['uuid'], data)
             return self.process_result(index_info, result)
         except globus_portal_framework.exc.ExpiredGlobusToken:
```

### Comparing `django-globus-portal-framework-0.4.8/manage.py` & `django-globus-portal-framework-0.4.9/manage.py`

 * *Files identical despite different names*

### Comparing `django-globus-portal-framework-0.4.8/setup.py` & `django-globus-portal-framework-0.4.9/setup.py`

 * *Files identical despite different names*

