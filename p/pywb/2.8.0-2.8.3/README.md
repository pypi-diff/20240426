# Comparing `tmp/pywb-2.8.0.tar.gz` & `tmp/pywb-2.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywb-2.8.0.tar", last modified: Wed Apr 24 12:25:57 2024, max compression
+gzip compressed data, was "pywb-2.8.3.tar", last modified: Fri Apr 26 08:34:30 2024, max compression
```

## Comparing `pywb-2.8.0.tar` & `pywb-2.8.3.tar`

### file list

```diff
@@ -1,432 +1,432 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.310810 pywb-2.8.0/
--rwxr-xr-x   0 runner    (1001) docker     (127)      316 2024-04-24 12:25:48.000000 pywb-2.8.0/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-24 12:25:48.000000 pywb-2.8.0/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-24 12:25:48.000000 pywb-2.8.0/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (127)    81373 2024-04-24 12:25:48.000000 pywb-2.8.0/CHANGES.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)      619 2024-04-24 12:25:48.000000 pywb-2.8.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     6371 2024-04-24 12:25:48.000000 pywb-2.8.0/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (127)    35121 2024-04-24 12:25:48.000000 pywb-2.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-24 12:25:48.000000 pywb-2.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-24 12:25:48.000000 pywb-2.8.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     5645 2024-04-24 12:25:57.310810 pywb-2.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4247 2024-04-24 12:25:48.000000 pywb-2.8.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-04-24 12:25:48.000000 pywb-2.8.0/Vagrantfile
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-24 12:25:48.000000 pywb-2.8.0/appveyor.disabled.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)      126 2024-04-24 12:25:48.000000 pywb-2.8.0/build-vue-ui.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      192 2024-04-24 12:25:48.000000 pywb-2.8.0/build-wombat.sh
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-24 12:25:48.000000 pywb-2.8.0/config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-24 12:25:48.000000 pywb-2.8.0/docker-compose.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)     1115 2024-04-24 12:25:48.000000 pywb-2.8.0/docker-entrypoint.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.250810 pywb-2.8.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.254810 pywb-2.8.0/docs/code/
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/code/pywb.apps.rst
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/code/pywb.indexer.rst
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/code/pywb.manager.rst
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/code/pywb.recorder.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/code/pywb.rewrite.rst
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/code/pywb.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/code/pywb.utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/code/pywb.warcserver.index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/code/pywb.warcserver.resource.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/code/pywb.warcserver.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5479 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.258810 pywb-2.8.0/docs/manual/
--rw-r--r--   0 runner    (1001) docker     (127)    11121 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/manual/access-control.rst
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/manual/apis.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/manual/apps.rst
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/manual/architecture.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10951 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/manual/cdxserver_api.rst
--rw-r--r--   0 runner    (1001) docker     (127)    27156 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/manual/configuring.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4583 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/manual/indexing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5681 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/manual/localization.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/manual/memento.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/manual/migrating-cdx.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/manual/outbackcdx.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/manual/owb-pywb-terms.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10341 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/manual/owb-to-pywb-config.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/manual/owb-to-pywb-deploy.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/manual/owb-to-pywb-exclusions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/manual/owb-transition.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/manual/recorder.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6729 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/manual/rewriter.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12846 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/manual/template-guide.rst
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/manual/ui-customization.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/manual/ui-guide.rst
--rw-r--r--   0 runner    (1001) docker     (127)    16666 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/manual/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/manual/vue-ui.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12367 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/manual/warcserver.rst
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-24 12:25:48.000000 pywb-2.8.0/extra_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.258810 pywb-2.8.0/pywb/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.258810 pywb-2.8.0/pywb/apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/apps/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    35718 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/apps/frontendapp.py
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/apps/live.py
--rw-r--r--   0 runner    (1001) docker     (127)    36131 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/apps/rewriterapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/apps/static_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.262810 pywb-2.8.0/pywb/apps/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/apps/test/test_rewriter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/apps/test/test_wbrequestresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/apps/warcserverapp.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/apps/wayback.py
--rw-r--r--   0 runner    (1001) docker     (127)     8584 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/apps/wbrequestresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/default_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-24 12:25:56.000000 pywb-2.8.0/pywb/git_hash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.262810 pywb-2.8.0/pywb/indexer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/indexer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11456 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/indexer/archiveindexer.py
--rw-r--r--   0 runner    (1001) docker     (127)    14604 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/indexer/cdxindexer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.262810 pywb-2.8.0/pywb/indexer/test/
--rw-r--r--   0 runner    (1001) docker     (127)    26788 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/indexer/test/test_indexing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.262810 pywb-2.8.0/pywb/manager/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11183 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/manager/aclmanager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/manager/autoindex.py
--rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/manager/locmanager.py
--rw-r--r--   0 runner    (1001) docker     (127)    22199 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/manager/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/manager/migrate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.262810 pywb-2.8.0/pywb/recorder/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/recorder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/recorder/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     8246 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/recorder/multifilewarcwriter.py
--rw-r--r--   0 runner    (1001) docker     (127)    11083 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/recorder/recorderapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4345 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/recorder/redisindexer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.262810 pywb-2.8.0/pywb/recorder/test/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/recorder/test/rec.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/recorder/test/simplerec.py
--rw-r--r--   0 runner    (1001) docker     (127)    25051 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/recorder/test/test_recorder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.266810 pywb-2.8.0/pywb/rewrite/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/rewrite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17686 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/rewrite/content_rewriter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/rewrite/cookie_rewriter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5336 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/rewrite/cookies.py
--rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/rewrite/default_rewriter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/rewrite/header_rewriter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/rewrite/html_insert_rewriter.py
--rw-r--r--   0 runner    (1001) docker     (127)    22052 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/rewrite/html_rewriter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/rewrite/jsonp_rewriter.py
--rw-r--r--   0 runner    (1001) docker     (127)    13030 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/rewrite/regex_rewriters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/rewrite/rewrite_amf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/rewrite/rewrite_dash.py
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/rewrite/rewrite_hls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/rewrite/rewrite_js_workers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/rewrite/rewriteinputreq.py
--rw-r--r--   0 runner    (1001) docker     (127)    17726 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/rewrite/templateview.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.266810 pywb-2.8.0/pywb/rewrite/test/
--rw-r--r--   0 runner    (1001) docker     (127)    36556 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/rewrite/test/test_content_rewriter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5643 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/rewrite/test/test_cookie_rewriter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7809 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/rewrite/test/test_header_rewriter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/rewrite/test/test_html_insert_rewriter.py
--rw-r--r--   0 runner    (1001) docker     (127)    23601 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/rewrite/test/test_html_rewriter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/rewrite/test/test_jsonp_rewriter.py
--rw-r--r--   0 runner    (1001) docker     (127)    14291 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/rewrite/test/test_regex_rewriters.py
--rw-r--r--   0 runner    (1001) docker     (127)     8356 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/rewrite/test/test_url_rewriter.py
--rw-r--r--   0 runner    (1001) docker     (127)    11273 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/rewrite/test/test_wburl.py
--rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/rewrite/url_rewriter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9806 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/rewrite/wburl.py
--rw-r--r--   0 runner    (1001) docker     (127)    13671 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/rules.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.270810 pywb-2.8.0/pywb/static/
--rw-r--r--   0 runner    (1001) docker     (127)    11677 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/autoFetchWorker.js
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/calendar.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.270810 pywb-2.8.0/pywb/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/css/base.css
--rw-r--r--   0 runner    (1001) docker     (127)   153136 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    54636 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/css/font-awesome.min.css
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/css/query.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.270810 pywb-2.8.0/pywb/static/flowplayer/
--rw-r--r--   0 runner    (1001) docker     (127)   129773 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/flowplayer/flowplayer-3.2.18.swf
--rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/flowplayer/flowplayer.audio-3.2.11.swf
--rw-r--r--   0 runner    (1001) docker     (127)    38275 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/flowplayer/flowplayer.controls-3.2.16.swf
--rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/flowplayer/flowplayer.pseudostreaming-3.2.13.swf
--rw-r--r--   0 runner    (1001) docker     (127)     6773 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/flowplayer/toolbox.flashembed.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.270810 pywb-2.8.0/pywb/static/fonts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.278810 pywb-2.8.0/pywb/static/fonts/font-awesome/
--rw-r--r--   0 runner    (1001) docker     (127)   125320 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/fonts/font-awesome/fa-brands-400.eot
--rw-r--r--   0 runner    (1001) docker     (127)   660056 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/fonts/font-awesome/fa-brands-400.svg
--rw-r--r--   0 runner    (1001) docker     (127)   125016 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/fonts/font-awesome/fa-brands-400.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    84568 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/fonts/font-awesome/fa-brands-400.woff
--rw-r--r--   0 runner    (1001) docker     (127)    72148 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/fonts/font-awesome/fa-brands-400.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    34388 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/fonts/font-awesome/fa-regular-400.eot
--rw-r--r--   0 runner    (1001) docker     (127)   144523 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/fonts/font-awesome/fa-regular-400.svg
--rw-r--r--   0 runner    (1001) docker     (127)    34092 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/fonts/font-awesome/fa-regular-400.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    16812 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/fonts/font-awesome/fa-regular-400.woff
--rw-r--r--   0 runner    (1001) docker     (127)    13608 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/fonts/font-awesome/fa-regular-400.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   186512 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/fonts/font-awesome/fa-solid-900.eot
--rw-r--r--   0 runner    (1001) docker     (127)   816218 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/fonts/font-awesome/fa-solid-900.svg
--rw-r--r--   0 runner    (1001) docker     (127)   186228 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/fonts/font-awesome/fa-solid-900.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    96248 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/fonts/font-awesome/fa-solid-900.woff
--rw-r--r--   0 runner    (1001) docker     (127)    74320 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/fonts/font-awesome/fa-solid-900.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    20127 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 runner    (1001) docker     (127)   108738 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 runner    (1001) docker     (127)    45404 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    23424 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 runner    (1001) docker     (127)    18028 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.278810 pywb-2.8.0/pywb/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)    76308 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/js/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    86926 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/js/jquery-latest.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     6243 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/js/url-polyfill.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.278810 pywb-2.8.0/pywb/static/loading-spinner/
--rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/loading-spinner/loading-spinner.js
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/loading-spinner/test.html
--rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/pywb-logo-sm.png
--rw-r--r--   0 runner    (1001) docker     (127)    10492 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/pywb-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    37329 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/query.js
--rw-r--r--   0 runner    (1001) docker     (127)     5563 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/queryWorker.js
--rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/scroll-webkit.css
--rw-r--r--   0 runner    (1001) docker     (127)     6950 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/search.js
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/transclusions.js
--rw-r--r--   0 runner    (1001) docker     (127)    22029 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/vidrw.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.278810 pywb-2.8.0/pywb/static/vue/
--rw-r--r--   0 runner    (1001) docker     (127)  1577587 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/vue/vueui.js
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/vue_banner.css
--rw-r--r--   0 runner    (1001) docker     (127)     8654 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/wb_frame.js
--rw-r--r--   0 runner    (1001) docker     (127)   130193 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/wombat.js
--rw-r--r--   0 runner    (1001) docker     (127)    15514 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/wombatProxyMode.js
--rw-r--r--   0 runner    (1001) docker     (127)     8893 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/wombatWorkers.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.282810 pywb-2.8.0/pywb/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/templates/banner.html
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/templates/bootstrap_jquery.html
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/templates/collinfo.json
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/templates/custom_banner.html
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/templates/error.html
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/templates/footer.html
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/templates/frame_insert.html
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/templates/head.html
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/templates/head_insert.html
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/templates/header.html
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)    15304 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/templates/instructions.html
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/templates/not_found.html
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/templates/proxy_cert_download.html
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/templates/proxy_select.html
--rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/templates/query.html
--rw-r--r--   0 runner    (1001) docker     (127)    10372 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/templates/search.html
--rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/templates/vue_loc.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.286810 pywb-2.8.0/pywb/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/utils/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/utils/binsearch.py
--rw-r--r--   0 runner    (1001) docker     (127)     6272 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/utils/canonicalize.py
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/utils/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/utils/geventserver.py
--rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (127)    14378 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/utils/loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/utils/memento.py
--rw-r--r--   0 runner    (1001) docker     (127)     3910 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/utils/merge.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.286810 pywb-2.8.0/pywb/utils/test/
--rw-r--r--   0 runner    (1001) docker     (127)     6488 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/utils/test/test_binsearch.py
--rw-r--r--   0 runner    (1001) docker     (127)     6680 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/utils/test/test_loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/utils/wbexception.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.246810 pywb-2.8.0/pywb/vueui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.246810 pywb-2.8.0/pywb/vueui/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.286810 pywb-2.8.0/pywb/vueui/src/cdx-simulator/
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/vueui/src/cdx-simulator/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.286810 pywb-2.8.0/pywb/warcserver/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12158 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/access_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/amf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4884 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/basewarcserver.py
--rw-r--r--   0 runner    (1001) docker     (127)     6953 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/http.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.286810 pywb-2.8.0/pywb/warcserver/index/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12890 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/index/aggregator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9008 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/index/cdxobject.py
--rw-r--r--   0 runner    (1001) docker     (127)     9816 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/index/cdxops.py
--rw-r--r--   0 runner    (1001) docker     (127)     8361 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/index/fuzzymatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    24183 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/index/indexsource.py
--rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/index/query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.290810 pywb-2.8.0/pywb/warcserver/index/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/index/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/index/test/test_cdxobject.py
--rw-r--r--   0 runner    (1001) docker     (127)    20273 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/index/test/test_cdxops.py
--rw-r--r--   0 runner    (1001) docker     (127)     8987 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/index/test/test_dir_agg.py
--rw-r--r--   0 runner    (1001) docker     (127)    11325 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/index/test/test_fuzzymatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     8986 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/index/test/test_indexsource.py
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/index/test/test_lazy_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)    15181 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/index/test/test_memento_agg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/index/test/test_redis_agg.py
--rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/index/test/test_timeouts.py
--rw-r--r--   0 runner    (1001) docker     (127)     6859 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/index/test/test_xmlquery_indexsource.py
--rw-r--r--   0 runner    (1001) docker     (127)    13783 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/index/test/test_zipnum.py
--rw-r--r--   0 runner    (1001) docker     (127)    12327 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/index/zipnum.py
--rw-r--r--   0 runner    (1001) docker     (127)     9770 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/inputrequest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.290810 pywb-2.8.0/pywb/warcserver/resource/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/resource/blockrecordloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/resource/pathresolvers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9310 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/resource/resolvingloader.py
--rw-r--r--   0 runner    (1001) docker     (127)    20858 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/resource/responseloader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.290810 pywb-2.8.0/pywb/warcserver/resource/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/resource/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15994 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/resource/test/test_loading.py
--rw-r--r--   0 runner    (1001) docker     (127)     7582 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/resource/test/test_pathresolvers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.290810 pywb-2.8.0/pywb/warcserver/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/test/live.ini
--rw-r--r--   0 runner    (1001) docker     (127)     5595 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/test/test_access.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/test/test_amf.py
--rw-r--r--   0 runner    (1001) docker     (127)    22680 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/test/test_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7475 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/test/test_inputreq.py
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/test/test_upstream.py
--rw-r--r--   0 runner    (1001) docker     (127)     5341 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/test/test_warcserver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/test/test_warcserver_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6243 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/test/testutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/upstreamindexsource.py
--rw-r--r--   0 runner    (1001) docker     (127)    11691 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/warcserver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.258810 pywb-2.8.0/pywb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5645 2024-04-24 12:25:57.000000 pywb-2.8.0/pywb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12313 2024-04-24 12:25:57.000000 pywb-2.8.0/pywb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 12:25:57.000000 pywb-2.8.0/pywb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-24 12:25:57.000000 pywb-2.8.0/pywb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 12:25:57.000000 pywb-2.8.0/pywb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-24 12:25:57.000000 pywb-2.8.0/pywb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-24 12:25:57.000000 pywb-2.8.0/pywb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-24 12:25:48.000000 pywb-2.8.0/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      183 2024-04-24 12:25:48.000000 pywb-2.8.0/run-gunicorn.sh
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-24 12:25:48.000000 pywb-2.8.0/run-tests.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      283 2024-04-24 12:25:48.000000 pywb-2.8.0/run-uwsgi.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.246810 pywb-2.8.0/sample_archive/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.294810 pywb-2.8.0/sample_archive/access/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/access/allow_all.aclj
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/access/allows.aclj
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/access/blocks.aclj
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/access/list1.aclj
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/access/list2.aclj
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/access/pywb.aclj
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/access/single-line.aclj
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.294810 pywb-2.8.0/sample_archive/cdx/
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/cdx/bad.cdx
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/cdx/dupes.cdx
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/cdx/example-arc-test.cdx
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/cdx/example-extra.cdx
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/cdx/example.cdx
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/cdx/httpbin-resource.cdxj
--rw-r--r--   0 runner    (1001) docker     (127)    30399 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/cdx/iana.cdx
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/cdx/missing-status-text.cdxj
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/cdx/post-test.cdx
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/cdx/url-agnost-example.cdx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.294810 pywb-2.8.0/sample_archive/cdxj/
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/cdxj/dupes.cdxj
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/cdxj/example-no-digest.cdxj
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/cdxj/example.cdx.gz
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/cdxj/example.cdxj
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/cdxj/example2.cdxj
--rw-r--r--   0 runner    (1001) docker     (127)    43062 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/cdxj/iana.cdxj
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/cdxj/post-test.cdxj
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/cdxj/url-agnost-example.cdxj
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.294810 pywb-2.8.0/sample_archive/non-surt-cdx/
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/non-surt-cdx/example-non-surt.cdx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.298810 pywb-2.8.0/sample_archive/text_content/
--rw-r--r--   0 runner    (1001) docker     (127)    13676 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/text_content/link_headers.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/text_content/pathindex.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/text_content/quickfox_repeated.compressed
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/text_content/sample.html
--rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/text_content/sample_dash.mpd
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/text_content/sample_hls.m3u8
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/text_content/sample_no_head.html
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/text_content/sample_no_head_2.html
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/text_content/sample_unclosed_script.html
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/text_content/toptest.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.298810 pywb-2.8.0/sample_archive/warcs/
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/warcs/bad.arc
--rw-r--r--   0 runner    (1001) docker     (127)    12905 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/warcs/dupes.warc.gz
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/warcs/example-bad.warc.gz.bad
--rw-r--r--   0 runner    (1001) docker     (127)     6416 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/warcs/example-extra.warc
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/warcs/example-url-agnostic-orig.warc.gz
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/warcs/example-url-agnostic-revisit.warc.gz
--rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/warcs/example-wget-1-14.warc.gz
--rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/warcs/example-wpull.warc.gz
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/warcs/example.arc
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/warcs/example.arc.gz
--rw-r--r--   0 runner    (1001) docker     (127)     5629 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/warcs/example.warc
--rw-r--r--   0 runner    (1001) docker     (127)     3484 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/warcs/example.warc.gz
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/warcs/example2.warc.gz
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/warcs/httpbin-resource.warc.gz
--rw-r--r--   0 runner    (1001) docker     (127)   786828 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/warcs/iana.warc.gz
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/warcs/missing-status-text.warc
--rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/warcs/post-test.warc.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.302810 pywb-2.8.0/sample_archive/zipcdx/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/zipcdx/zipnum-bad.idx
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/zipcdx/zipnum-bad.loc
--rw-r--r--   0 runner    (1001) docker     (127)     9797 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/zipcdx/zipnum-sample.cdx.gz
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/zipcdx/zipnum-sample.idx
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/zipcdx/zipnum-sample.loc
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 12:25:57.310810 pywb-2.8.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     4729 2024-04-24 12:25:48.000000 pywb-2.8.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-24 12:25:48.000000 pywb-2.8.0/test_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.306810 pywb-2.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/base_config_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/config_test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/config_test_access.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/config_test_cert_req.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/config_test_loc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/config_test_record.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/config_test_record_dedup.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/config_test_redirect_classic.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/config_test_root_coll.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.246810 pywb-2.8.0/tests/i18n-data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.246810 pywb-2.8.0/tests/i18n-data/l337/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.306810 pywb-2.8.0/tests/i18n-data/l337/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/i18n-data/l337/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/memento_fixture.py
--rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/test_acl.py
--rw-r--r--   0 runner    (1001) docker     (127)     7013 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/test_acl_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    19956 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/test_auto_colls.py
--rw-r--r--   0 runner    (1001) docker     (127)    10828 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/test_cdx_server_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/test_cert_req.py
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/test_embargo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/test_force_https.py
--rw-r--r--   0 runner    (1001) docker     (127)    25129 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     8676 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/test_live_rewriter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/test_locales.py
--rw-r--r--   0 runner    (1001) docker     (127)     6590 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    12071 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/test_memento.py
--rw-r--r--   0 runner    (1001) docker     (127)    10613 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/test_prefer_header.py
--rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/test_prefixed_deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)    19147 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/test_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/test_range.py
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/test_record_dedup.py
--rw-r--r--   0 runner    (1001) docker     (127)     9150 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/test_record_replay.py
--rw-r--r--   0 runner    (1001) docker     (127)     3721 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/test_redirect_classic.py
--rw-r--r--   0 runner    (1001) docker     (127)     5439 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/test_redirect_revisits.py
--rw-r--r--   0 runner    (1001) docker     (127)     7380 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/test_redirects.py
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/test_root_coll.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/test_socks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/test_zipnum_auto_dir.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.310810 pywb-2.8.0/tests_disabled/
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-24 12:25:48.000000 pywb-2.8.0/tests_disabled/fixture.py
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-24 12:25:48.000000 pywb-2.8.0/tests_disabled/live.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-24 12:25:48.000000 pywb-2.8.0/tests_disabled/perms_fixture.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-24 12:25:48.000000 pywb-2.8.0/tests_disabled/server_mock.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-24 12:25:48.000000 pywb-2.8.0/tests_disabled/server_thread.py
--rw-r--r--   0 runner    (1001) docker     (127)     5713 2024-04-24 12:25:48.000000 pywb-2.8.0/tests_disabled/test_cdxserver.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-24 12:25:48.000000 pywb-2.8.0/tests_disabled/test_config_frames.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-24 12:25:48.000000 pywb-2.8.0/tests_disabled/test_config_memento.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-24 12:25:48.000000 pywb-2.8.0/tests_disabled/test_config_proxy_http_cookie.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-24 12:25:48.000000 pywb-2.8.0/tests_disabled/test_config_proxy_https_cookie.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-24 12:25:48.000000 pywb-2.8.0/tests_disabled/test_config_proxy_ip.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-24 12:25:48.000000 pywb-2.8.0/tests_disabled/test_config_proxy_ip_redis.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-24 12:25:48.000000 pywb-2.8.0/tests_disabled/test_config_proxy_no_banner.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-24 12:25:48.000000 pywb-2.8.0/tests_disabled/test_config_root_coll.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8144 2024-04-24 12:25:48.000000 pywb-2.8.0/tests_disabled/test_live_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)    17290 2024-04-24 12:25:48.000000 pywb-2.8.0/tests_disabled/test_memento.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-24 12:25:48.000000 pywb-2.8.0/tests_disabled/test_perms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-24 12:25:48.000000 pywb-2.8.0/tests_disabled/test_perms_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-04-24 12:25:48.000000 pywb-2.8.0/tests_disabled/test_proxy_http_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     6504 2024-04-24 12:25:48.000000 pywb-2.8.0/tests_disabled/test_proxy_http_cookie.py
--rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-04-24 12:25:48.000000 pywb-2.8.0/tests_disabled/test_proxy_http_ip.py
--rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-04-24 12:25:48.000000 pywb-2.8.0/tests_disabled/test_proxy_http_ip_redis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-04-24 12:25:48.000000 pywb-2.8.0/tests_disabled/test_proxy_http_no_banner.py
--rw-r--r--   0 runner    (1001) docker     (127)     6906 2024-04-24 12:25:48.000000 pywb-2.8.0/tests_disabled/test_proxy_https_cookie.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-24 12:25:48.000000 pywb-2.8.0/tests_disabled/test_rewrite_content.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      178 2024-04-24 12:25:48.000000 pywb-2.8.0/update-tag.sh
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-24 12:25:48.000000 pywb-2.8.0/uwsgi.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:34:30.320335 pywb-2.8.3/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      316 2024-04-26 08:34:21.000000 pywb-2.8.3/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-26 08:34:21.000000 pywb-2.8.3/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-26 08:34:21.000000 pywb-2.8.3/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    81373 2024-04-26 08:34:21.000000 pywb-2.8.3/CHANGES.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)      619 2024-04-26 08:34:21.000000 pywb-2.8.3/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     6371 2024-04-26 08:34:21.000000 pywb-2.8.3/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35121 2024-04-26 08:34:21.000000 pywb-2.8.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-26 08:34:21.000000 pywb-2.8.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-26 08:34:21.000000 pywb-2.8.3/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-04-26 08:34:30.320335 pywb-2.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-04-26 08:34:21.000000 pywb-2.8.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-04-26 08:34:21.000000 pywb-2.8.3/Vagrantfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-26 08:34:21.000000 pywb-2.8.3/appveyor.disabled.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      126 2024-04-26 08:34:21.000000 pywb-2.8.3/build-vue-ui.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      192 2024-04-26 08:34:21.000000 pywb-2.8.3/build-wombat.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-26 08:34:21.000000 pywb-2.8.3/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-26 08:34:21.000000 pywb-2.8.3/docker-compose.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1115 2024-04-26 08:34:21.000000 pywb-2.8.3/docker-entrypoint.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:34:30.260334 pywb-2.8.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-26 08:34:21.000000 pywb-2.8.3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:34:30.260334 pywb-2.8.3/docs/code/
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-26 08:34:21.000000 pywb-2.8.3/docs/code/pywb.apps.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-26 08:34:21.000000 pywb-2.8.3/docs/code/pywb.indexer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-26 08:34:21.000000 pywb-2.8.3/docs/code/pywb.manager.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-26 08:34:21.000000 pywb-2.8.3/docs/code/pywb.recorder.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-04-26 08:34:21.000000 pywb-2.8.3/docs/code/pywb.rewrite.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-26 08:34:21.000000 pywb-2.8.3/docs/code/pywb.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-26 08:34:21.000000 pywb-2.8.3/docs/code/pywb.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-26 08:34:21.000000 pywb-2.8.3/docs/code/pywb.warcserver.index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-26 08:34:21.000000 pywb-2.8.3/docs/code/pywb.warcserver.resource.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-26 08:34:21.000000 pywb-2.8.3/docs/code/pywb.warcserver.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5479 2024-04-26 08:34:21.000000 pywb-2.8.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-26 08:34:21.000000 pywb-2.8.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-26 08:34:21.000000 pywb-2.8.3/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:34:30.264334 pywb-2.8.3/docs/manual/
+-rw-r--r--   0 runner    (1001) docker     (127)    11121 2024-04-26 08:34:21.000000 pywb-2.8.3/docs/manual/access-control.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-26 08:34:21.000000 pywb-2.8.3/docs/manual/apis.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-04-26 08:34:21.000000 pywb-2.8.3/docs/manual/apps.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-26 08:34:21.000000 pywb-2.8.3/docs/manual/architecture.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10951 2024-04-26 08:34:21.000000 pywb-2.8.3/docs/manual/cdxserver_api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    27156 2024-04-26 08:34:21.000000 pywb-2.8.3/docs/manual/configuring.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4583 2024-04-26 08:34:21.000000 pywb-2.8.3/docs/manual/indexing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5681 2024-04-26 08:34:21.000000 pywb-2.8.3/docs/manual/localization.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-04-26 08:34:21.000000 pywb-2.8.3/docs/manual/memento.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-26 08:34:21.000000 pywb-2.8.3/docs/manual/migrating-cdx.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-04-26 08:34:21.000000 pywb-2.8.3/docs/manual/outbackcdx.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-26 08:34:21.000000 pywb-2.8.3/docs/manual/owb-pywb-terms.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10341 2024-04-26 08:34:21.000000 pywb-2.8.3/docs/manual/owb-to-pywb-config.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-04-26 08:34:21.000000 pywb-2.8.3/docs/manual/owb-to-pywb-deploy.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-26 08:34:21.000000 pywb-2.8.3/docs/manual/owb-to-pywb-exclusions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-26 08:34:21.000000 pywb-2.8.3/docs/manual/owb-transition.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-26 08:34:21.000000 pywb-2.8.3/docs/manual/recorder.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6729 2024-04-26 08:34:21.000000 pywb-2.8.3/docs/manual/rewriter.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12846 2024-04-26 08:34:21.000000 pywb-2.8.3/docs/manual/template-guide.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-26 08:34:21.000000 pywb-2.8.3/docs/manual/ui-customization.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-04-26 08:34:21.000000 pywb-2.8.3/docs/manual/ui-guide.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    16666 2024-04-26 08:34:21.000000 pywb-2.8.3/docs/manual/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-04-26 08:34:21.000000 pywb-2.8.3/docs/manual/vue-ui.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12367 2024-04-26 08:34:21.000000 pywb-2.8.3/docs/manual/warcserver.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-26 08:34:21.000000 pywb-2.8.3/extra_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:34:30.268334 pywb-2.8.3/pywb/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:34:30.268334 pywb-2.8.3/pywb/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/apps/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35718 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/apps/frontendapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/apps/live.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36131 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/apps/rewriterapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/apps/static_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:34:30.268334 pywb-2.8.3/pywb/apps/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/apps/test/test_rewriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/apps/test/test_wbrequestresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/apps/warcserverapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/apps/wayback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8584 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/apps/wbrequestresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/default_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-26 08:34:29.000000 pywb-2.8.3/pywb/git_hash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:34:30.268334 pywb-2.8.3/pywb/indexer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/indexer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11456 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/indexer/archiveindexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14604 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/indexer/cdxindexer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:34:30.272334 pywb-2.8.3/pywb/indexer/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    26788 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/indexer/test/test_indexing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:34:30.272334 pywb-2.8.3/pywb/manager/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11183 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/manager/aclmanager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/manager/autoindex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/manager/locmanager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22199 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/manager/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/manager/migrate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:34:30.272334 pywb-2.8.3/pywb/recorder/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/recorder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/recorder/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8246 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/recorder/multifilewarcwriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11083 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/recorder/recorderapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4345 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/recorder/redisindexer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:34:30.272334 pywb-2.8.3/pywb/recorder/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/recorder/test/rec.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/recorder/test/simplerec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25051 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/recorder/test/test_recorder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:34:30.276334 pywb-2.8.3/pywb/rewrite/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/rewrite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17686 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/rewrite/content_rewriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/rewrite/cookie_rewriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5336 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/rewrite/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/rewrite/default_rewriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/rewrite/header_rewriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/rewrite/html_insert_rewriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22052 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/rewrite/html_rewriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/rewrite/jsonp_rewriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13030 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/rewrite/regex_rewriters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/rewrite/rewrite_amf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/rewrite/rewrite_dash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/rewrite/rewrite_hls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/rewrite/rewrite_js_workers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/rewrite/rewriteinputreq.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17726 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/rewrite/templateview.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:34:30.276334 pywb-2.8.3/pywb/rewrite/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    36556 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/rewrite/test/test_content_rewriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5643 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/rewrite/test/test_cookie_rewriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7809 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/rewrite/test/test_header_rewriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/rewrite/test/test_html_insert_rewriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23601 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/rewrite/test/test_html_rewriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/rewrite/test/test_jsonp_rewriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14291 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/rewrite/test/test_regex_rewriters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8356 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/rewrite/test/test_url_rewriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11273 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/rewrite/test/test_wburl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/rewrite/url_rewriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9806 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/rewrite/wburl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13671 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/rules.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:34:30.280334 pywb-2.8.3/pywb/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    11677 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/static/autoFetchWorker.js
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/static/calendar.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:34:30.280334 pywb-2.8.3/pywb/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/static/css/base.css
+-rw-r--r--   0 runner    (1001) docker     (127)   153136 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/static/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    54636 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/static/css/font-awesome.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/static/css/query.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:34:30.280334 pywb-2.8.3/pywb/static/flowplayer/
+-rw-r--r--   0 runner    (1001) docker     (127)   129773 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/static/flowplayer/flowplayer-3.2.18.swf
+-rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/static/flowplayer/flowplayer.audio-3.2.11.swf
+-rw-r--r--   0 runner    (1001) docker     (127)    38275 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/static/flowplayer/flowplayer.controls-3.2.16.swf
+-rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/static/flowplayer/flowplayer.pseudostreaming-3.2.13.swf
+-rw-r--r--   0 runner    (1001) docker     (127)     6773 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/static/flowplayer/toolbox.flashembed.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:34:30.280334 pywb-2.8.3/pywb/static/fonts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:34:30.288334 pywb-2.8.3/pywb/static/fonts/font-awesome/
+-rw-r--r--   0 runner    (1001) docker     (127)   125320 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/static/fonts/font-awesome/fa-brands-400.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   660056 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/static/fonts/font-awesome/fa-brands-400.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   125016 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/static/fonts/font-awesome/fa-brands-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    84568 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/static/fonts/font-awesome/fa-brands-400.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    72148 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/static/fonts/font-awesome/fa-brands-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    34388 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/static/fonts/font-awesome/fa-regular-400.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   144523 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/static/fonts/font-awesome/fa-regular-400.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    34092 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/static/fonts/font-awesome/fa-regular-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    16812 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/static/fonts/font-awesome/fa-regular-400.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    13608 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/static/fonts/font-awesome/fa-regular-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   186512 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/static/fonts/font-awesome/fa-solid-900.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   816218 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/static/fonts/font-awesome/fa-solid-900.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   186228 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/static/fonts/font-awesome/fa-solid-900.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    96248 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/static/fonts/font-awesome/fa-solid-900.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    74320 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/static/fonts/font-awesome/fa-solid-900.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    20127 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/static/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   108738 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/static/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    45404 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/static/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    23424 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/static/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    18028 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/static/fonts/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:34:30.288334 pywb-2.8.3/pywb/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    76308 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/static/js/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    86926 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/static/js/jquery-latest.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6243 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/static/js/url-polyfill.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:34:30.288334 pywb-2.8.3/pywb/static/loading-spinner/
+-rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/static/loading-spinner/loading-spinner.js
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/static/loading-spinner/test.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/static/pywb-logo-sm.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10492 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/static/pywb-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    37329 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/static/query.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5563 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/static/queryWorker.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/static/scroll-webkit.css
+-rw-r--r--   0 runner    (1001) docker     (127)     6950 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/static/search.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/static/transclusions.js
+-rw-r--r--   0 runner    (1001) docker     (127)    22029 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/static/vidrw.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:34:30.288334 pywb-2.8.3/pywb/static/vue/
+-rw-r--r--   0 runner    (1001) docker     (127)  1577587 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/static/vue/vueui.js
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/static/vue_banner.css
+-rw-r--r--   0 runner    (1001) docker     (127)     8654 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/static/wb_frame.js
+-rw-r--r--   0 runner    (1001) docker     (127)   130193 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/static/wombat.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15514 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/static/wombatProxyMode.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8893 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/static/wombatWorkers.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:34:30.292334 pywb-2.8.3/pywb/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/templates/banner.html
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/templates/bootstrap_jquery.html
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/templates/collinfo.json
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/templates/custom_banner.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/templates/error.html
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/templates/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/templates/frame_insert.html
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/templates/head.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/templates/head_insert.html
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/templates/header.html
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)    15304 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/templates/instructions.html
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/templates/not_found.html
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/templates/proxy_cert_download.html
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/templates/proxy_select.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/templates/query.html
+-rw-r--r--   0 runner    (1001) docker     (127)    10372 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/templates/search.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/templates/vue_loc.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:34:30.292334 pywb-2.8.3/pywb/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/utils/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/utils/binsearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6272 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/utils/canonicalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/utils/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/utils/geventserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14378 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/utils/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/utils/memento.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3910 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/utils/merge.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:34:30.292334 pywb-2.8.3/pywb/utils/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     6488 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/utils/test/test_binsearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6680 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/utils/test/test_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/utils/wbexception.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:34:30.252334 pywb-2.8.3/pywb/vueui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:34:30.252334 pywb-2.8.3/pywb/vueui/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:34:30.292334 pywb-2.8.3/pywb/vueui/src/cdx-simulator/
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/vueui/src/cdx-simulator/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:34:30.296334 pywb-2.8.3/pywb/warcserver/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/warcserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12158 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/warcserver/access_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/warcserver/amf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4884 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/warcserver/basewarcserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6953 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/warcserver/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/warcserver/http.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:34:30.296334 pywb-2.8.3/pywb/warcserver/index/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/warcserver/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12890 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/warcserver/index/aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9008 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/warcserver/index/cdxobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9816 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/warcserver/index/cdxops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8361 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/warcserver/index/fuzzymatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24183 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/warcserver/index/indexsource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/warcserver/index/query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:34:30.300335 pywb-2.8.3/pywb/warcserver/index/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/warcserver/index/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/warcserver/index/test/test_cdxobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20273 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/warcserver/index/test/test_cdxops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8987 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/warcserver/index/test/test_dir_agg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11325 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/warcserver/index/test/test_fuzzymatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8986 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/warcserver/index/test/test_indexsource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/warcserver/index/test/test_lazy_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15181 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/warcserver/index/test/test_memento_agg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/warcserver/index/test/test_redis_agg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/warcserver/index/test/test_timeouts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6859 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/warcserver/index/test/test_xmlquery_indexsource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13783 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/warcserver/index/test/test_zipnum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12327 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/warcserver/index/zipnum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9770 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/warcserver/inputrequest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:34:30.300335 pywb-2.8.3/pywb/warcserver/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/warcserver/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/warcserver/resource/blockrecordloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/warcserver/resource/pathresolvers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9310 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/warcserver/resource/resolvingloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20858 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/warcserver/resource/responseloader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:34:30.300335 pywb-2.8.3/pywb/warcserver/resource/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/warcserver/resource/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15994 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/warcserver/resource/test/test_loading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7582 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/warcserver/resource/test/test_pathresolvers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:34:30.300335 pywb-2.8.3/pywb/warcserver/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/warcserver/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/warcserver/test/live.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     5595 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/warcserver/test/test_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/warcserver/test/test_amf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22680 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/warcserver/test/test_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7475 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/warcserver/test/test_inputreq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/warcserver/test/test_upstream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5341 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/warcserver/test/test_warcserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/warcserver/test/test_warcserver_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6243 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/warcserver/test/testutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/warcserver/upstreamindexsource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11691 2024-04-26 08:34:21.000000 pywb-2.8.3/pywb/warcserver/warcserver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:34:30.268334 pywb-2.8.3/pywb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-04-26 08:34:30.000000 pywb-2.8.3/pywb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12313 2024-04-26 08:34:30.000000 pywb-2.8.3/pywb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 08:34:30.000000 pywb-2.8.3/pywb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-26 08:34:30.000000 pywb-2.8.3/pywb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 08:34:30.000000 pywb-2.8.3/pywb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-26 08:34:30.000000 pywb-2.8.3/pywb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-26 08:34:30.000000 pywb-2.8.3/pywb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-26 08:34:21.000000 pywb-2.8.3/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      183 2024-04-26 08:34:21.000000 pywb-2.8.3/run-gunicorn.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-26 08:34:21.000000 pywb-2.8.3/run-tests.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      283 2024-04-26 08:34:21.000000 pywb-2.8.3/run-uwsgi.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:34:30.256334 pywb-2.8.3/sample_archive/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:34:30.300335 pywb-2.8.3/sample_archive/access/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-26 08:34:21.000000 pywb-2.8.3/sample_archive/access/allow_all.aclj
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-26 08:34:21.000000 pywb-2.8.3/sample_archive/access/allows.aclj
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-26 08:34:21.000000 pywb-2.8.3/sample_archive/access/blocks.aclj
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-26 08:34:21.000000 pywb-2.8.3/sample_archive/access/list1.aclj
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-26 08:34:21.000000 pywb-2.8.3/sample_archive/access/list2.aclj
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-26 08:34:21.000000 pywb-2.8.3/sample_archive/access/pywb.aclj
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-26 08:34:21.000000 pywb-2.8.3/sample_archive/access/single-line.aclj
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:34:30.304334 pywb-2.8.3/sample_archive/cdx/
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-26 08:34:21.000000 pywb-2.8.3/sample_archive/cdx/bad.cdx
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-26 08:34:21.000000 pywb-2.8.3/sample_archive/cdx/dupes.cdx
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-26 08:34:21.000000 pywb-2.8.3/sample_archive/cdx/example-arc-test.cdx
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-26 08:34:21.000000 pywb-2.8.3/sample_archive/cdx/example-extra.cdx
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-26 08:34:21.000000 pywb-2.8.3/sample_archive/cdx/example.cdx
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-26 08:34:21.000000 pywb-2.8.3/sample_archive/cdx/httpbin-resource.cdxj
+-rw-r--r--   0 runner    (1001) docker     (127)    30399 2024-04-26 08:34:21.000000 pywb-2.8.3/sample_archive/cdx/iana.cdx
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-26 08:34:21.000000 pywb-2.8.3/sample_archive/cdx/missing-status-text.cdxj
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-26 08:34:21.000000 pywb-2.8.3/sample_archive/cdx/post-test.cdx
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-26 08:34:21.000000 pywb-2.8.3/sample_archive/cdx/url-agnost-example.cdx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:34:30.304334 pywb-2.8.3/sample_archive/cdxj/
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-04-26 08:34:21.000000 pywb-2.8.3/sample_archive/cdxj/dupes.cdxj
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-26 08:34:21.000000 pywb-2.8.3/sample_archive/cdxj/example-no-digest.cdxj
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-26 08:34:21.000000 pywb-2.8.3/sample_archive/cdxj/example.cdx.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-26 08:34:21.000000 pywb-2.8.3/sample_archive/cdxj/example.cdxj
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-26 08:34:21.000000 pywb-2.8.3/sample_archive/cdxj/example2.cdxj
+-rw-r--r--   0 runner    (1001) docker     (127)    43062 2024-04-26 08:34:21.000000 pywb-2.8.3/sample_archive/cdxj/iana.cdxj
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-26 08:34:21.000000 pywb-2.8.3/sample_archive/cdxj/post-test.cdxj
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-26 08:34:21.000000 pywb-2.8.3/sample_archive/cdxj/url-agnost-example.cdxj
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:34:30.304334 pywb-2.8.3/sample_archive/non-surt-cdx/
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-26 08:34:21.000000 pywb-2.8.3/sample_archive/non-surt-cdx/example-non-surt.cdx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:34:30.308334 pywb-2.8.3/sample_archive/text_content/
+-rw-r--r--   0 runner    (1001) docker     (127)    13676 2024-04-26 08:34:21.000000 pywb-2.8.3/sample_archive/text_content/link_headers.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-26 08:34:21.000000 pywb-2.8.3/sample_archive/text_content/pathindex.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-26 08:34:21.000000 pywb-2.8.3/sample_archive/text_content/quickfox_repeated.compressed
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-26 08:34:21.000000 pywb-2.8.3/sample_archive/text_content/sample.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-04-26 08:34:21.000000 pywb-2.8.3/sample_archive/text_content/sample_dash.mpd
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-26 08:34:21.000000 pywb-2.8.3/sample_archive/text_content/sample_hls.m3u8
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-26 08:34:21.000000 pywb-2.8.3/sample_archive/text_content/sample_no_head.html
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-26 08:34:21.000000 pywb-2.8.3/sample_archive/text_content/sample_no_head_2.html
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-26 08:34:21.000000 pywb-2.8.3/sample_archive/text_content/sample_unclosed_script.html
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-26 08:34:21.000000 pywb-2.8.3/sample_archive/text_content/toptest.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:34:30.308334 pywb-2.8.3/sample_archive/warcs/
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-26 08:34:21.000000 pywb-2.8.3/sample_archive/warcs/bad.arc
+-rw-r--r--   0 runner    (1001) docker     (127)    12905 2024-04-26 08:34:21.000000 pywb-2.8.3/sample_archive/warcs/dupes.warc.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-04-26 08:34:21.000000 pywb-2.8.3/sample_archive/warcs/example-bad.warc.gz.bad
+-rw-r--r--   0 runner    (1001) docker     (127)     6416 2024-04-26 08:34:21.000000 pywb-2.8.3/sample_archive/warcs/example-extra.warc
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-26 08:34:21.000000 pywb-2.8.3/sample_archive/warcs/example-url-agnostic-orig.warc.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-26 08:34:21.000000 pywb-2.8.3/sample_archive/warcs/example-url-agnostic-revisit.warc.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-04-26 08:34:21.000000 pywb-2.8.3/sample_archive/warcs/example-wget-1-14.warc.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-04-26 08:34:21.000000 pywb-2.8.3/sample_archive/warcs/example-wpull.warc.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-26 08:34:21.000000 pywb-2.8.3/sample_archive/warcs/example.arc
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-26 08:34:21.000000 pywb-2.8.3/sample_archive/warcs/example.arc.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     5629 2024-04-26 08:34:21.000000 pywb-2.8.3/sample_archive/warcs/example.warc
+-rw-r--r--   0 runner    (1001) docker     (127)     3484 2024-04-26 08:34:21.000000 pywb-2.8.3/sample_archive/warcs/example.warc.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-26 08:34:21.000000 pywb-2.8.3/sample_archive/warcs/example2.warc.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-26 08:34:21.000000 pywb-2.8.3/sample_archive/warcs/httpbin-resource.warc.gz
+-rw-r--r--   0 runner    (1001) docker     (127)   786828 2024-04-26 08:34:21.000000 pywb-2.8.3/sample_archive/warcs/iana.warc.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-26 08:34:21.000000 pywb-2.8.3/sample_archive/warcs/missing-status-text.warc
+-rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-04-26 08:34:21.000000 pywb-2.8.3/sample_archive/warcs/post-test.warc.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:34:30.312335 pywb-2.8.3/sample_archive/zipcdx/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-26 08:34:21.000000 pywb-2.8.3/sample_archive/zipcdx/zipnum-bad.idx
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-26 08:34:21.000000 pywb-2.8.3/sample_archive/zipcdx/zipnum-bad.loc
+-rw-r--r--   0 runner    (1001) docker     (127)     9797 2024-04-26 08:34:21.000000 pywb-2.8.3/sample_archive/zipcdx/zipnum-sample.cdx.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-26 08:34:21.000000 pywb-2.8.3/sample_archive/zipcdx/zipnum-sample.idx
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-26 08:34:21.000000 pywb-2.8.3/sample_archive/zipcdx/zipnum-sample.loc
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 08:34:30.320335 pywb-2.8.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4729 2024-04-26 08:34:21.000000 pywb-2.8.3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-26 08:34:21.000000 pywb-2.8.3/test_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:34:30.316335 pywb-2.8.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:34:21.000000 pywb-2.8.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-04-26 08:34:21.000000 pywb-2.8.3/tests/base_config_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-26 08:34:21.000000 pywb-2.8.3/tests/config_test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-26 08:34:21.000000 pywb-2.8.3/tests/config_test_access.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-26 08:34:21.000000 pywb-2.8.3/tests/config_test_cert_req.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-26 08:34:21.000000 pywb-2.8.3/tests/config_test_loc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-26 08:34:21.000000 pywb-2.8.3/tests/config_test_record.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-26 08:34:21.000000 pywb-2.8.3/tests/config_test_record_dedup.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-26 08:34:21.000000 pywb-2.8.3/tests/config_test_redirect_classic.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-26 08:34:21.000000 pywb-2.8.3/tests/config_test_root_coll.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:34:30.256334 pywb-2.8.3/tests/i18n-data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:34:30.256334 pywb-2.8.3/tests/i18n-data/l337/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:34:30.316335 pywb-2.8.3/tests/i18n-data/l337/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-26 08:34:21.000000 pywb-2.8.3/tests/i18n-data/l337/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-26 08:34:21.000000 pywb-2.8.3/tests/memento_fixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-04-26 08:34:21.000000 pywb-2.8.3/tests/test_acl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7013 2024-04-26 08:34:21.000000 pywb-2.8.3/tests/test_acl_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19956 2024-04-26 08:34:21.000000 pywb-2.8.3/tests/test_auto_colls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10828 2024-04-26 08:34:21.000000 pywb-2.8.3/tests/test_cdx_server_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-26 08:34:21.000000 pywb-2.8.3/tests/test_cert_req.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-26 08:34:21.000000 pywb-2.8.3/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-04-26 08:34:21.000000 pywb-2.8.3/tests/test_embargo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-04-26 08:34:21.000000 pywb-2.8.3/tests/test_force_https.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25129 2024-04-26 08:34:21.000000 pywb-2.8.3/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8676 2024-04-26 08:34:21.000000 pywb-2.8.3/tests/test_live_rewriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-26 08:34:21.000000 pywb-2.8.3/tests/test_locales.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6590 2024-04-26 08:34:21.000000 pywb-2.8.3/tests/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12071 2024-04-26 08:34:21.000000 pywb-2.8.3/tests/test_memento.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10613 2024-04-26 08:34:21.000000 pywb-2.8.3/tests/test_prefer_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-04-26 08:34:21.000000 pywb-2.8.3/tests/test_prefixed_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19147 2024-04-26 08:34:21.000000 pywb-2.8.3/tests/test_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-26 08:34:21.000000 pywb-2.8.3/tests/test_range.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-04-26 08:34:21.000000 pywb-2.8.3/tests/test_record_dedup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9150 2024-04-26 08:34:21.000000 pywb-2.8.3/tests/test_record_replay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3721 2024-04-26 08:34:21.000000 pywb-2.8.3/tests/test_redirect_classic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5439 2024-04-26 08:34:21.000000 pywb-2.8.3/tests/test_redirect_revisits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7380 2024-04-26 08:34:21.000000 pywb-2.8.3/tests/test_redirects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-26 08:34:21.000000 pywb-2.8.3/tests/test_root_coll.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-26 08:34:21.000000 pywb-2.8.3/tests/test_socks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-04-26 08:34:21.000000 pywb-2.8.3/tests/test_zipnum_auto_dir.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:34:30.320335 pywb-2.8.3/tests_disabled/
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-26 08:34:21.000000 pywb-2.8.3/tests_disabled/fixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-26 08:34:21.000000 pywb-2.8.3/tests_disabled/live.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-26 08:34:21.000000 pywb-2.8.3/tests_disabled/perms_fixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-26 08:34:21.000000 pywb-2.8.3/tests_disabled/server_mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-26 08:34:21.000000 pywb-2.8.3/tests_disabled/server_thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5713 2024-04-26 08:34:21.000000 pywb-2.8.3/tests_disabled/test_cdxserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-26 08:34:21.000000 pywb-2.8.3/tests_disabled/test_config_frames.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-26 08:34:21.000000 pywb-2.8.3/tests_disabled/test_config_memento.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-26 08:34:21.000000 pywb-2.8.3/tests_disabled/test_config_proxy_http_cookie.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-26 08:34:21.000000 pywb-2.8.3/tests_disabled/test_config_proxy_https_cookie.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-26 08:34:21.000000 pywb-2.8.3/tests_disabled/test_config_proxy_ip.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-26 08:34:21.000000 pywb-2.8.3/tests_disabled/test_config_proxy_ip_redis.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-26 08:34:21.000000 pywb-2.8.3/tests_disabled/test_config_proxy_no_banner.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-26 08:34:21.000000 pywb-2.8.3/tests_disabled/test_config_root_coll.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8144 2024-04-26 08:34:21.000000 pywb-2.8.3/tests_disabled/test_live_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17290 2024-04-26 08:34:21.000000 pywb-2.8.3/tests_disabled/test_memento.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-26 08:34:21.000000 pywb-2.8.3/tests_disabled/test_perms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-26 08:34:21.000000 pywb-2.8.3/tests_disabled/test_perms_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-04-26 08:34:21.000000 pywb-2.8.3/tests_disabled/test_proxy_http_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6504 2024-04-26 08:34:21.000000 pywb-2.8.3/tests_disabled/test_proxy_http_cookie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-04-26 08:34:21.000000 pywb-2.8.3/tests_disabled/test_proxy_http_ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-04-26 08:34:21.000000 pywb-2.8.3/tests_disabled/test_proxy_http_ip_redis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-04-26 08:34:21.000000 pywb-2.8.3/tests_disabled/test_proxy_http_no_banner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6906 2024-04-26 08:34:21.000000 pywb-2.8.3/tests_disabled/test_proxy_https_cookie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-26 08:34:21.000000 pywb-2.8.3/tests_disabled/test_rewrite_content.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      178 2024-04-26 08:34:21.000000 pywb-2.8.3/update-tag.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-26 08:34:21.000000 pywb-2.8.3/uwsgi.ini
```

### Comparing `pywb-2.8.0/.travis.yml` & `pywb-2.8.3/.travis.yml`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/CHANGES.rst` & `pywb-2.8.3/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/Dockerfile` & `pywb-2.8.3/Dockerfile`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/INSTALL.rst` & `pywb-2.8.3/INSTALL.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/LICENSE` & `pywb-2.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/MANIFEST.in` & `pywb-2.8.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/PKG-INFO` & `pywb-2.8.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywb
-Version: 2.8.0
+Version: 2.8.3
 Summary: Pywb Webrecorder web archive replay and capture tools
 Home-page: https://github.com/webrecorder/pywb
 Author: Ilya Kreymer
 Author-email: ikreymer@gmail.com
 License: GPL
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -43,15 +43,15 @@
       :target: https://codecov.io/gh/webrecorder/pywb
 
 Web Archiving Tools for All
 ---------------------------
 
 `View the full pywb documentation <https://pywb.readthedocs.org>`_
 
-**pywb** is a Python (2 and 3) web archiving toolkit for replaying web archives large and small as accurately as possible.
+**pywb** is a Python 3 web archiving toolkit for replaying web archives large and small as accurately as possible.
 The toolkit now also includes new features for creating high-fidelity web archives.
 
 This toolset forms the foundation of Webrecorder project, but also provides a generic web archiving toolkit
 that is used by other web archives, including the traditional "Wayback Machine" functionality.
 
 
 New Features
```

### Comparing `pywb-2.8.0/README.rst` & `pywb-2.8.3/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
       :target: https://codecov.io/gh/webrecorder/pywb
 
 Web Archiving Tools for All
 ---------------------------
 
 `View the full pywb documentation <https://pywb.readthedocs.org>`_
 
-**pywb** is a Python (2 and 3) web archiving toolkit for replaying web archives large and small as accurately as possible.
+**pywb** is a Python 3 web archiving toolkit for replaying web archives large and small as accurately as possible.
 The toolkit now also includes new features for creating high-fidelity web archives.
 
 This toolset forms the foundation of Webrecorder project, but also provides a generic web archiving toolkit
 that is used by other web archives, including the traditional "Wayback Machine" functionality.
 
 
 New Features
```

### Comparing `pywb-2.8.0/Vagrantfile` & `pywb-2.8.3/Vagrantfile`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/appveyor.disabled.yml` & `pywb-2.8.3/appveyor.disabled.yml`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/config.yaml` & `pywb-2.8.3/config.yaml`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/docker-entrypoint.sh` & `pywb-2.8.3/docker-entrypoint.sh`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/docs/Makefile` & `pywb-2.8.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/docs/code/pywb.apps.rst` & `pywb-2.8.3/docs/code/pywb.apps.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/docs/code/pywb.manager.rst` & `pywb-2.8.3/docs/code/pywb.manager.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/docs/code/pywb.recorder.rst` & `pywb-2.8.3/docs/code/pywb.recorder.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/docs/code/pywb.rewrite.rst` & `pywb-2.8.3/docs/code/pywb.rewrite.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/docs/code/pywb.utils.rst` & `pywb-2.8.3/docs/code/pywb.utils.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/docs/code/pywb.warcserver.index.rst` & `pywb-2.8.3/docs/code/pywb.warcserver.index.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/docs/code/pywb.warcserver.resource.rst` & `pywb-2.8.3/docs/code/pywb.warcserver.resource.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/docs/code/pywb.warcserver.rst` & `pywb-2.8.3/docs/code/pywb.warcserver.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/docs/conf.py` & `pywb-2.8.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/docs/index.rst` & `pywb-2.8.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/docs/make.bat` & `pywb-2.8.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/docs/manual/access-control.rst` & `pywb-2.8.3/docs/manual/access-control.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/docs/manual/apps.rst` & `pywb-2.8.3/docs/manual/apps.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/docs/manual/cdxserver_api.rst` & `pywb-2.8.3/docs/manual/cdxserver_api.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/docs/manual/configuring.rst` & `pywb-2.8.3/docs/manual/configuring.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/docs/manual/indexing.rst` & `pywb-2.8.3/docs/manual/indexing.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/docs/manual/localization.rst` & `pywb-2.8.3/docs/manual/localization.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/docs/manual/memento.rst` & `pywb-2.8.3/docs/manual/memento.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/docs/manual/migrating-cdx.rst` & `pywb-2.8.3/docs/manual/migrating-cdx.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/docs/manual/outbackcdx.rst` & `pywb-2.8.3/docs/manual/outbackcdx.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/docs/manual/owb-pywb-terms.rst` & `pywb-2.8.3/docs/manual/owb-pywb-terms.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/docs/manual/owb-to-pywb-config.rst` & `pywb-2.8.3/docs/manual/owb-to-pywb-config.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/docs/manual/owb-to-pywb-deploy.rst` & `pywb-2.8.3/docs/manual/owb-to-pywb-deploy.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/docs/manual/owb-to-pywb-exclusions.rst` & `pywb-2.8.3/docs/manual/owb-to-pywb-exclusions.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/docs/manual/recorder.rst` & `pywb-2.8.3/docs/manual/recorder.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/docs/manual/rewriter.rst` & `pywb-2.8.3/docs/manual/rewriter.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/docs/manual/template-guide.rst` & `pywb-2.8.3/docs/manual/template-guide.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/docs/manual/ui-guide.rst` & `pywb-2.8.3/docs/manual/ui-guide.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/docs/manual/usage.rst` & `pywb-2.8.3/docs/manual/usage.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/docs/manual/vue-ui.rst` & `pywb-2.8.3/docs/manual/vue-ui.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/docs/manual/warcserver.rst` & `pywb-2.8.3/docs/manual/warcserver.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/apps/cli.py` & `pywb-2.8.3/pywb/apps/cli.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/apps/frontendapp.py` & `pywb-2.8.3/pywb/apps/frontendapp.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/apps/rewriterapp.py` & `pywb-2.8.3/pywb/apps/rewriterapp.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/apps/static_handler.py` & `pywb-2.8.3/pywb/apps/static_handler.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/apps/test/test_rewriter.py` & `pywb-2.8.3/pywb/apps/test/test_rewriter.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/apps/test/test_wbrequestresponse.py` & `pywb-2.8.3/pywb/apps/test/test_wbrequestresponse.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/apps/wbrequestresponse.py` & `pywb-2.8.3/pywb/apps/wbrequestresponse.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/default_config.yaml` & `pywb-2.8.3/pywb/default_config.yaml`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/indexer/archiveindexer.py` & `pywb-2.8.3/pywb/indexer/archiveindexer.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/indexer/cdxindexer.py` & `pywb-2.8.3/pywb/indexer/cdxindexer.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/indexer/test/test_indexing.py` & `pywb-2.8.3/pywb/indexer/test/test_indexing.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/manager/aclmanager.py` & `pywb-2.8.3/pywb/manager/aclmanager.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/manager/autoindex.py` & `pywb-2.8.3/pywb/manager/autoindex.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/manager/locmanager.py` & `pywb-2.8.3/pywb/manager/locmanager.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/manager/manager.py` & `pywb-2.8.3/pywb/manager/manager.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/manager/migrate.py` & `pywb-2.8.3/pywb/manager/migrate.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/recorder/filters.py` & `pywb-2.8.3/pywb/recorder/filters.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/recorder/multifilewarcwriter.py` & `pywb-2.8.3/pywb/recorder/multifilewarcwriter.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/recorder/recorderapp.py` & `pywb-2.8.3/pywb/recorder/recorderapp.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/recorder/redisindexer.py` & `pywb-2.8.3/pywb/recorder/redisindexer.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/recorder/test/simplerec.py` & `pywb-2.8.3/pywb/recorder/test/simplerec.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/recorder/test/test_recorder.py` & `pywb-2.8.3/pywb/recorder/test/test_recorder.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/rewrite/content_rewriter.py` & `pywb-2.8.3/pywb/rewrite/content_rewriter.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/rewrite/cookie_rewriter.py` & `pywb-2.8.3/pywb/rewrite/cookie_rewriter.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/rewrite/cookies.py` & `pywb-2.8.3/pywb/rewrite/cookies.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/rewrite/default_rewriter.py` & `pywb-2.8.3/pywb/rewrite/default_rewriter.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/rewrite/header_rewriter.py` & `pywb-2.8.3/pywb/rewrite/header_rewriter.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/rewrite/html_insert_rewriter.py` & `pywb-2.8.3/pywb/rewrite/html_insert_rewriter.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/rewrite/html_rewriter.py` & `pywb-2.8.3/pywb/rewrite/html_rewriter.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/rewrite/jsonp_rewriter.py` & `pywb-2.8.3/pywb/rewrite/jsonp_rewriter.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/rewrite/regex_rewriters.py` & `pywb-2.8.3/pywb/rewrite/regex_rewriters.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/rewrite/rewrite_amf.py` & `pywb-2.8.3/pywb/rewrite/rewrite_amf.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/rewrite/rewrite_dash.py` & `pywb-2.8.3/pywb/rewrite/rewrite_dash.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/rewrite/rewrite_hls.py` & `pywb-2.8.3/pywb/rewrite/rewrite_hls.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/rewrite/rewrite_js_workers.py` & `pywb-2.8.3/pywb/rewrite/rewrite_js_workers.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/rewrite/rewriteinputreq.py` & `pywb-2.8.3/pywb/rewrite/rewriteinputreq.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/rewrite/templateview.py` & `pywb-2.8.3/pywb/rewrite/templateview.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/rewrite/test/test_content_rewriter.py` & `pywb-2.8.3/pywb/rewrite/test/test_content_rewriter.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/rewrite/test/test_cookie_rewriter.py` & `pywb-2.8.3/pywb/rewrite/test/test_cookie_rewriter.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/rewrite/test/test_header_rewriter.py` & `pywb-2.8.3/pywb/rewrite/test/test_header_rewriter.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/rewrite/test/test_html_insert_rewriter.py` & `pywb-2.8.3/pywb/rewrite/test/test_html_insert_rewriter.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/rewrite/test/test_html_rewriter.py` & `pywb-2.8.3/pywb/rewrite/test/test_html_rewriter.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/rewrite/test/test_jsonp_rewriter.py` & `pywb-2.8.3/pywb/rewrite/test/test_jsonp_rewriter.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/rewrite/test/test_regex_rewriters.py` & `pywb-2.8.3/pywb/rewrite/test/test_regex_rewriters.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/rewrite/test/test_url_rewriter.py` & `pywb-2.8.3/pywb/rewrite/test/test_url_rewriter.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/rewrite/test/test_wburl.py` & `pywb-2.8.3/pywb/rewrite/test/test_wburl.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/rewrite/url_rewriter.py` & `pywb-2.8.3/pywb/rewrite/url_rewriter.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/rewrite/wburl.py` & `pywb-2.8.3/pywb/rewrite/wburl.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/rules.yaml` & `pywb-2.8.3/pywb/rules.yaml`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/static/autoFetchWorker.js` & `pywb-2.8.3/pywb/static/autoFetchWorker.js`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/static/css/base.css` & `pywb-2.8.3/pywb/static/css/base.css`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/static/css/bootstrap.min.css` & `pywb-2.8.3/pywb/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/static/css/font-awesome.min.css` & `pywb-2.8.3/pywb/static/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/static/flowplayer/flowplayer-3.2.18.swf` & `pywb-2.8.3/pywb/static/flowplayer/flowplayer-3.2.18.swf`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/static/flowplayer/flowplayer.audio-3.2.11.swf` & `pywb-2.8.3/pywb/static/flowplayer/flowplayer.audio-3.2.11.swf`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/static/flowplayer/flowplayer.controls-3.2.16.swf` & `pywb-2.8.3/pywb/static/flowplayer/flowplayer.controls-3.2.16.swf`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/static/flowplayer/flowplayer.pseudostreaming-3.2.13.swf` & `pywb-2.8.3/pywb/static/flowplayer/flowplayer.pseudostreaming-3.2.13.swf`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/static/flowplayer/toolbox.flashembed.js` & `pywb-2.8.3/pywb/static/flowplayer/toolbox.flashembed.js`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/static/fonts/font-awesome/fa-brands-400.eot` & `pywb-2.8.3/pywb/static/fonts/font-awesome/fa-brands-400.eot`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/static/fonts/font-awesome/fa-brands-400.svg` & `pywb-2.8.3/pywb/static/fonts/font-awesome/fa-brands-400.svg`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/static/fonts/font-awesome/fa-brands-400.ttf` & `pywb-2.8.3/pywb/static/fonts/font-awesome/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/static/fonts/font-awesome/fa-brands-400.woff` & `pywb-2.8.3/pywb/static/fonts/font-awesome/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/static/fonts/font-awesome/fa-brands-400.woff2` & `pywb-2.8.3/pywb/static/fonts/font-awesome/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/static/fonts/font-awesome/fa-regular-400.eot` & `pywb-2.8.3/pywb/static/fonts/font-awesome/fa-regular-400.eot`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/static/fonts/font-awesome/fa-regular-400.svg` & `pywb-2.8.3/pywb/static/fonts/font-awesome/fa-regular-400.svg`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/static/fonts/font-awesome/fa-regular-400.ttf` & `pywb-2.8.3/pywb/static/fonts/font-awesome/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/static/fonts/font-awesome/fa-regular-400.woff` & `pywb-2.8.3/pywb/static/fonts/font-awesome/fa-regular-400.woff`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/static/fonts/font-awesome/fa-regular-400.woff2` & `pywb-2.8.3/pywb/static/fonts/font-awesome/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/static/fonts/font-awesome/fa-solid-900.eot` & `pywb-2.8.3/pywb/static/fonts/font-awesome/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/static/fonts/font-awesome/fa-solid-900.svg` & `pywb-2.8.3/pywb/static/fonts/font-awesome/fa-solid-900.svg`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/static/fonts/font-awesome/fa-solid-900.ttf` & `pywb-2.8.3/pywb/static/fonts/font-awesome/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/static/fonts/font-awesome/fa-solid-900.woff` & `pywb-2.8.3/pywb/static/fonts/font-awesome/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/static/fonts/font-awesome/fa-solid-900.woff2` & `pywb-2.8.3/pywb/static/fonts/font-awesome/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/static/fonts/glyphicons-halflings-regular.eot` & `pywb-2.8.3/pywb/static/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/static/fonts/glyphicons-halflings-regular.svg` & `pywb-2.8.3/pywb/static/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/static/fonts/glyphicons-halflings-regular.ttf` & `pywb-2.8.3/pywb/static/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/static/fonts/glyphicons-halflings-regular.woff` & `pywb-2.8.3/pywb/static/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/static/fonts/glyphicons-halflings-regular.woff2` & `pywb-2.8.3/pywb/static/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/static/js/bootstrap.min.js` & `pywb-2.8.3/pywb/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/static/js/jquery-latest.min.js` & `pywb-2.8.3/pywb/static/js/jquery-latest.min.js`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/static/js/url-polyfill.min.js` & `pywb-2.8.3/pywb/static/js/url-polyfill.min.js`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/static/loading-spinner/loading-spinner.js` & `pywb-2.8.3/pywb/static/loading-spinner/loading-spinner.js`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/static/pywb-logo-sm.png` & `pywb-2.8.3/pywb/static/pywb-logo-sm.png`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/static/pywb-logo.png` & `pywb-2.8.3/pywb/static/pywb-logo.png`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/static/query.js` & `pywb-2.8.3/pywb/static/query.js`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/static/queryWorker.js` & `pywb-2.8.3/pywb/static/queryWorker.js`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/static/scroll-webkit.css` & `pywb-2.8.3/pywb/static/scroll-webkit.css`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/static/search.js` & `pywb-2.8.3/pywb/static/search.js`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/static/transclusions.js` & `pywb-2.8.3/pywb/static/transclusions.js`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/static/vidrw.js` & `pywb-2.8.3/pywb/static/vidrw.js`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/static/vue/vueui.js` & `pywb-2.8.3/pywb/static/vue/vueui.js`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/static/wb_frame.js` & `pywb-2.8.3/pywb/static/wb_frame.js`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/static/wombat.js` & `pywb-2.8.3/pywb/static/wombat.js`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/static/wombatProxyMode.js` & `pywb-2.8.3/pywb/static/wombatProxyMode.js`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/static/wombatWorkers.js` & `pywb-2.8.3/pywb/static/wombatWorkers.js`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/templates/banner.html` & `pywb-2.8.3/pywb/templates/banner.html`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/templates/base.html` & `pywb-2.8.3/pywb/templates/base.html`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/templates/error.html` & `pywb-2.8.3/pywb/templates/error.html`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/templates/frame_insert.html` & `pywb-2.8.3/pywb/templates/frame_insert.html`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/templates/head_insert.html` & `pywb-2.8.3/pywb/templates/head_insert.html`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/templates/header.html` & `pywb-2.8.3/pywb/templates/header.html`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/templates/index.html` & `pywb-2.8.3/pywb/templates/index.html`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/templates/instructions.html` & `pywb-2.8.3/pywb/templates/instructions.html`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/templates/not_found.html` & `pywb-2.8.3/pywb/templates/not_found.html`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/templates/proxy_cert_download.html` & `pywb-2.8.3/pywb/templates/proxy_cert_download.html`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/templates/proxy_select.html` & `pywb-2.8.3/pywb/templates/proxy_select.html`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/templates/query.html` & `pywb-2.8.3/pywb/templates/query.html`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/templates/search.html` & `pywb-2.8.3/pywb/templates/search.html`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/templates/vue_loc.html` & `pywb-2.8.3/pywb/templates/vue_loc.html`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/utils/README.md` & `pywb-2.8.3/pywb/utils/README.md`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/utils/binsearch.py` & `pywb-2.8.3/pywb/utils/binsearch.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/utils/canonicalize.py` & `pywb-2.8.3/pywb/utils/canonicalize.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/utils/format.py` & `pywb-2.8.3/pywb/utils/format.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/utils/geventserver.py` & `pywb-2.8.3/pywb/utils/geventserver.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/utils/io.py` & `pywb-2.8.3/pywb/utils/io.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/utils/loaders.py` & `pywb-2.8.3/pywb/utils/loaders.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/utils/memento.py` & `pywb-2.8.3/pywb/utils/memento.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/utils/merge.py` & `pywb-2.8.3/pywb/utils/merge.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/utils/test/test_binsearch.py` & `pywb-2.8.3/pywb/utils/test/test_binsearch.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/utils/test/test_loaders.py` & `pywb-2.8.3/pywb/utils/test/test_loaders.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/utils/wbexception.py` & `pywb-2.8.3/pywb/utils/wbexception.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/vueui/src/cdx-simulator/README.md` & `pywb-2.8.3/pywb/vueui/src/cdx-simulator/README.md`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/warcserver/access_checker.py` & `pywb-2.8.3/pywb/warcserver/access_checker.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/warcserver/amf.py` & `pywb-2.8.3/pywb/warcserver/amf.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/warcserver/basewarcserver.py` & `pywb-2.8.3/pywb/warcserver/basewarcserver.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/warcserver/handlers.py` & `pywb-2.8.3/pywb/warcserver/handlers.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/warcserver/http.py` & `pywb-2.8.3/pywb/warcserver/http.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/warcserver/index/aggregator.py` & `pywb-2.8.3/pywb/warcserver/index/aggregator.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/warcserver/index/cdxobject.py` & `pywb-2.8.3/pywb/warcserver/index/cdxobject.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/warcserver/index/cdxops.py` & `pywb-2.8.3/pywb/warcserver/index/cdxops.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/warcserver/index/fuzzymatcher.py` & `pywb-2.8.3/pywb/warcserver/index/fuzzymatcher.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/warcserver/index/indexsource.py` & `pywb-2.8.3/pywb/warcserver/index/indexsource.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/warcserver/index/query.py` & `pywb-2.8.3/pywb/warcserver/index/query.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/warcserver/index/test/test_cdxobject.py` & `pywb-2.8.3/pywb/warcserver/index/test/test_cdxobject.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/warcserver/index/test/test_cdxops.py` & `pywb-2.8.3/pywb/warcserver/index/test/test_cdxops.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/warcserver/index/test/test_dir_agg.py` & `pywb-2.8.3/pywb/warcserver/index/test/test_dir_agg.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/warcserver/index/test/test_fuzzymatcher.py` & `pywb-2.8.3/pywb/warcserver/index/test/test_fuzzymatcher.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/warcserver/index/test/test_indexsource.py` & `pywb-2.8.3/pywb/warcserver/index/test/test_indexsource.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/warcserver/index/test/test_lazy_ops.py` & `pywb-2.8.3/pywb/warcserver/index/test/test_lazy_ops.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/warcserver/index/test/test_memento_agg.py` & `pywb-2.8.3/pywb/warcserver/index/test/test_memento_agg.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/warcserver/index/test/test_redis_agg.py` & `pywb-2.8.3/pywb/warcserver/index/test/test_redis_agg.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/warcserver/index/test/test_timeouts.py` & `pywb-2.8.3/pywb/warcserver/index/test/test_timeouts.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/warcserver/index/test/test_xmlquery_indexsource.py` & `pywb-2.8.3/pywb/warcserver/index/test/test_xmlquery_indexsource.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/warcserver/index/test/test_zipnum.py` & `pywb-2.8.3/pywb/warcserver/index/test/test_zipnum.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/warcserver/index/zipnum.py` & `pywb-2.8.3/pywb/warcserver/index/zipnum.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/warcserver/inputrequest.py` & `pywb-2.8.3/pywb/warcserver/inputrequest.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/warcserver/resource/blockrecordloader.py` & `pywb-2.8.3/pywb/warcserver/resource/blockrecordloader.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/warcserver/resource/pathresolvers.py` & `pywb-2.8.3/pywb/warcserver/resource/pathresolvers.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/warcserver/resource/resolvingloader.py` & `pywb-2.8.3/pywb/warcserver/resource/resolvingloader.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/warcserver/resource/responseloader.py` & `pywb-2.8.3/pywb/warcserver/resource/responseloader.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/warcserver/resource/test/test_loading.py` & `pywb-2.8.3/pywb/warcserver/resource/test/test_loading.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/warcserver/resource/test/test_pathresolvers.py` & `pywb-2.8.3/pywb/warcserver/resource/test/test_pathresolvers.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/warcserver/test/test_access.py` & `pywb-2.8.3/pywb/warcserver/test/test_access.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/warcserver/test/test_amf.py` & `pywb-2.8.3/pywb/warcserver/test/test_amf.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/warcserver/test/test_handlers.py` & `pywb-2.8.3/pywb/warcserver/test/test_handlers.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/warcserver/test/test_inputreq.py` & `pywb-2.8.3/pywb/warcserver/test/test_inputreq.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/warcserver/test/test_upstream.py` & `pywb-2.8.3/pywb/warcserver/test/test_upstream.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/warcserver/test/test_warcserver.py` & `pywb-2.8.3/pywb/warcserver/test/test_warcserver.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/warcserver/test/test_warcserver_config.yaml` & `pywb-2.8.3/pywb/warcserver/test/test_warcserver_config.yaml`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/warcserver/test/testutils.py` & `pywb-2.8.3/pywb/warcserver/test/testutils.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/warcserver/upstreamindexsource.py` & `pywb-2.8.3/pywb/warcserver/upstreamindexsource.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb/warcserver/warcserver.py` & `pywb-2.8.3/pywb/warcserver/warcserver.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/pywb.egg-info/PKG-INFO` & `pywb-2.8.3/pywb.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywb
-Version: 2.8.0
+Version: 2.8.3
 Summary: Pywb Webrecorder web archive replay and capture tools
 Home-page: https://github.com/webrecorder/pywb
 Author: Ilya Kreymer
 Author-email: ikreymer@gmail.com
 License: GPL
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -43,15 +43,15 @@
       :target: https://codecov.io/gh/webrecorder/pywb
 
 Web Archiving Tools for All
 ---------------------------
 
 `View the full pywb documentation <https://pywb.readthedocs.org>`_
 
-**pywb** is a Python (2 and 3) web archiving toolkit for replaying web archives large and small as accurately as possible.
+**pywb** is a Python 3 web archiving toolkit for replaying web archives large and small as accurately as possible.
 The toolkit now also includes new features for creating high-fidelity web archives.
 
 This toolset forms the foundation of Webrecorder project, but also provides a generic web archiving toolkit
 that is used by other web archives, including the traditional "Wayback Machine" functionality.
 
 
 New Features
```

### Comparing `pywb-2.8.0/pywb.egg-info/SOURCES.txt` & `pywb-2.8.3/pywb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/sample_archive/access/pywb.aclj` & `pywb-2.8.3/sample_archive/access/pywb.aclj`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/sample_archive/cdx/bad.cdx` & `pywb-2.8.3/sample_archive/cdx/bad.cdx`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/sample_archive/cdx/dupes.cdx` & `pywb-2.8.3/sample_archive/cdx/dupes.cdx`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/sample_archive/cdx/iana.cdx` & `pywb-2.8.3/sample_archive/cdx/iana.cdx`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/sample_archive/cdx/post-test.cdx` & `pywb-2.8.3/sample_archive/cdx/post-test.cdx`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/sample_archive/cdxj/dupes.cdxj` & `pywb-2.8.3/sample_archive/cdxj/dupes.cdxj`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/sample_archive/cdxj/example.cdxj` & `pywb-2.8.3/sample_archive/cdxj/example.cdxj`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/sample_archive/cdxj/iana.cdxj` & `pywb-2.8.3/sample_archive/cdxj/iana.cdxj`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/sample_archive/cdxj/post-test.cdxj` & `pywb-2.8.3/sample_archive/cdxj/post-test.cdxj`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/sample_archive/text_content/link_headers.yaml` & `pywb-2.8.3/sample_archive/text_content/link_headers.yaml`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/sample_archive/text_content/sample_dash.mpd` & `pywb-2.8.3/sample_archive/text_content/sample_dash.mpd`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/sample_archive/text_content/sample_hls.m3u8` & `pywb-2.8.3/sample_archive/text_content/sample_hls.m3u8`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/sample_archive/warcs/dupes.warc.gz` & `pywb-2.8.3/sample_archive/warcs/dupes.warc.gz`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/sample_archive/warcs/example-bad.warc.gz.bad` & `pywb-2.8.3/sample_archive/warcs/example-bad.warc.gz.bad`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/sample_archive/warcs/example-extra.warc` & `pywb-2.8.3/sample_archive/warcs/example-extra.warc`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/sample_archive/warcs/example-url-agnostic-orig.warc.gz` & `pywb-2.8.3/sample_archive/warcs/example-url-agnostic-orig.warc.gz`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/sample_archive/warcs/example-url-agnostic-revisit.warc.gz` & `pywb-2.8.3/sample_archive/warcs/example-url-agnostic-revisit.warc.gz`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/sample_archive/warcs/example-wget-1-14.warc.gz` & `pywb-2.8.3/sample_archive/warcs/example-wget-1-14.warc.gz`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/sample_archive/warcs/example-wpull.warc.gz` & `pywb-2.8.3/sample_archive/warcs/example-wpull.warc.gz`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/sample_archive/warcs/example.arc` & `pywb-2.8.3/sample_archive/warcs/example.arc`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/sample_archive/warcs/example.arc.gz` & `pywb-2.8.3/sample_archive/warcs/example.arc.gz`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/sample_archive/warcs/example.warc` & `pywb-2.8.3/sample_archive/warcs/example.warc`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/sample_archive/warcs/example.warc.gz` & `pywb-2.8.3/sample_archive/warcs/example.warc.gz`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/sample_archive/warcs/example2.warc.gz` & `pywb-2.8.3/sample_archive/warcs/example2.warc.gz`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/sample_archive/warcs/iana.warc.gz` & `pywb-2.8.3/sample_archive/warcs/iana.warc.gz`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/sample_archive/warcs/post-test.warc.gz` & `pywb-2.8.3/sample_archive/warcs/post-test.warc.gz`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/sample_archive/zipcdx/zipnum-sample.cdx.gz` & `pywb-2.8.3/sample_archive/zipcdx/zipnum-sample.cdx.gz`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/sample_archive/zipcdx/zipnum-sample.idx` & `pywb-2.8.3/sample_archive/zipcdx/zipnum-sample.idx`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/setup.py` & `pywb-2.8.3/setup.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/tests/base_config_test.py` & `pywb-2.8.3/tests/base_config_test.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/tests/config_test.yaml` & `pywb-2.8.3/tests/config_test.yaml`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/tests/config_test_access.yaml` & `pywb-2.8.3/tests/config_test_access.yaml`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/tests/i18n-data/l337/LC_MESSAGES/messages.po` & `pywb-2.8.3/tests/i18n-data/l337/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/tests/memento_fixture.py` & `pywb-2.8.3/tests/memento_fixture.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/tests/test_acl.py` & `pywb-2.8.3/tests/test_acl.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/tests/test_acl_manager.py` & `pywb-2.8.3/tests/test_acl_manager.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/tests/test_auto_colls.py` & `pywb-2.8.3/tests/test_auto_colls.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/tests/test_cdx_server_app.py` & `pywb-2.8.3/tests/test_cdx_server_app.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/tests/test_cert_req.py` & `pywb-2.8.3/tests/test_cert_req.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/tests/test_cli.py` & `pywb-2.8.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/tests/test_embargo.py` & `pywb-2.8.3/tests/test_embargo.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/tests/test_force_https.py` & `pywb-2.8.3/tests/test_force_https.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/tests/test_integration.py` & `pywb-2.8.3/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/tests/test_live_rewriter.py` & `pywb-2.8.3/tests/test_live_rewriter.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/tests/test_locales.py` & `pywb-2.8.3/tests/test_locales.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/tests/test_manager.py` & `pywb-2.8.3/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/tests/test_memento.py` & `pywb-2.8.3/tests/test_memento.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/tests/test_prefer_header.py` & `pywb-2.8.3/tests/test_prefer_header.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/tests/test_prefixed_deploy.py` & `pywb-2.8.3/tests/test_prefixed_deploy.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/tests/test_proxy.py` & `pywb-2.8.3/tests/test_proxy.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/tests/test_range.py` & `pywb-2.8.3/tests/test_range.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/tests/test_record_dedup.py` & `pywb-2.8.3/tests/test_record_dedup.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/tests/test_record_replay.py` & `pywb-2.8.3/tests/test_record_replay.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/tests/test_redirect_classic.py` & `pywb-2.8.3/tests/test_redirect_classic.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/tests/test_redirect_revisits.py` & `pywb-2.8.3/tests/test_redirect_revisits.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/tests/test_redirects.py` & `pywb-2.8.3/tests/test_redirects.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/tests/test_root_coll.py` & `pywb-2.8.3/tests/test_root_coll.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/tests/test_socks.py` & `pywb-2.8.3/tests/test_socks.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/tests/test_zipnum_auto_dir.py` & `pywb-2.8.3/tests/test_zipnum_auto_dir.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/tests_disabled/fixture.py` & `pywb-2.8.3/tests_disabled/fixture.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/tests_disabled/live.py` & `pywb-2.8.3/tests_disabled/live.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/tests_disabled/perms_fixture.py` & `pywb-2.8.3/tests_disabled/perms_fixture.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/tests_disabled/server_mock.py` & `pywb-2.8.3/tests_disabled/server_mock.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/tests_disabled/server_thread.py` & `pywb-2.8.3/tests_disabled/server_thread.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/tests_disabled/test_cdxserver.py` & `pywb-2.8.3/tests_disabled/test_cdxserver.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/tests_disabled/test_config_memento.yaml` & `pywb-2.8.3/tests_disabled/test_config_memento.yaml`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/tests_disabled/test_config_proxy_https_cookie.yaml` & `pywb-2.8.3/tests_disabled/test_config_proxy_https_cookie.yaml`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/tests_disabled/test_live_proxy.py` & `pywb-2.8.3/tests_disabled/test_live_proxy.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/tests_disabled/test_memento.py` & `pywb-2.8.3/tests_disabled/test_memento.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/tests_disabled/test_perms.py` & `pywb-2.8.3/tests_disabled/test_perms.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/tests_disabled/test_perms_app.py` & `pywb-2.8.3/tests_disabled/test_perms_app.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/tests_disabled/test_proxy_http_auth.py` & `pywb-2.8.3/tests_disabled/test_proxy_http_auth.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/tests_disabled/test_proxy_http_cookie.py` & `pywb-2.8.3/tests_disabled/test_proxy_http_cookie.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/tests_disabled/test_proxy_http_ip.py` & `pywb-2.8.3/tests_disabled/test_proxy_http_ip.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/tests_disabled/test_proxy_http_ip_redis.py` & `pywb-2.8.3/tests_disabled/test_proxy_http_ip_redis.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/tests_disabled/test_proxy_http_no_banner.py` & `pywb-2.8.3/tests_disabled/test_proxy_http_no_banner.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/tests_disabled/test_proxy_https_cookie.py` & `pywb-2.8.3/tests_disabled/test_proxy_https_cookie.py`

 * *Files identical despite different names*

### Comparing `pywb-2.8.0/tests_disabled/test_rewrite_content.py` & `pywb-2.8.3/tests_disabled/test_rewrite_content.py`

 * *Files identical despite different names*

