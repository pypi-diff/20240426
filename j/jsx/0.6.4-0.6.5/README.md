# Comparing `tmp/jsx-0.6.4.tar.gz` & `tmp/jsx-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsx-0.6.4.tar", last modified: Wed Apr 24 00:28:11 2024, max compression
+gzip compressed data, was "jsx-0.6.5.tar", last modified: Fri Apr 26 13:50:01 2024, max compression
```

## Comparing `jsx-0.6.4.tar` & `jsx-0.6.5.tar`

### file list

```diff
@@ -1,117 +1,117 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:28:11.052363 jsx-0.6.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-24 00:28:04.000000 jsx-0.6.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-04-24 00:28:11.052363 jsx-0.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-04-24 00:28:04.000000 jsx-0.6.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:28:11.036363 jsx-0.6.4/jsx/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:28:11.036363 jsx-0.6.4/jsx/components/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/components/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/components/page.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/element.py
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:28:11.048363 jsx-0.6.4/jsx/html/
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/_auto_html.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/a.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/abbr.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/address.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/area.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/article.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/aside.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/b.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/base.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/blockquote.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/body.py
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/br.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/button.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/canvas.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/cite.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/code.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/col.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/div.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/em.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/embed.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/footer.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/form.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/fragment.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/h1.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/h2.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/h3.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/h4.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/h5.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/h6.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/head.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/header.py
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/hr.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/html.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/i.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/img.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/input.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/label.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/li.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/link.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/main.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/meta.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/nav.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/ol.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/option.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/p.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/param.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/pre.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/script.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/section.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/select.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/small.py
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/source.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/span.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/strong.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/sub.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/sup.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/table.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/tbody.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/td.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/textarea.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/th.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/thead.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/time.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/title.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/tr.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/track.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/u.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/ul.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/wbr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/internal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:28:11.048363 jsx-0.6.4/jsx/middlewares/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/middlewares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/middlewares/asgi.py
--rw-r--r--   0 runner    (1001) docker     (127)     5589 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/middlewares/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:28:11.048363 jsx-0.6.4/jsx/server/
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/server/components.py
--rw-r--r--   0 runner    (1001) docker     (127)     5150 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/server/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/server/request.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/server/ws_router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:28:11.052363 jsx-0.6.4/jsx/styling/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/styling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5031 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/styling/color.py
--rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/styling/css_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/styling/style.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:28:11.052363 jsx-0.6.4/jsx/types/
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/types/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/types/events.py
--rw-r--r--   0 runner    (1001) docker     (127)    10941 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/types/html.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:28:11.052363 jsx-0.6.4/jsx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-04-24 00:28:11.000000 jsx-0.6.4/jsx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-24 00:28:11.000000 jsx-0.6.4/jsx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 00:28:11.000000 jsx-0.6.4/jsx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-24 00:28:11.000000 jsx-0.6.4/jsx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-24 00:28:11.000000 jsx-0.6.4/jsx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-24 00:28:04.000000 jsx-0.6.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-24 00:28:04.000000 jsx-0.6.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 00:28:11.052363 jsx-0.6.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:28:11.052363 jsx-0.6.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-24 00:28:04.000000 jsx-0.6.4/tests/test_asgi_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-24 00:28:04.000000 jsx-0.6.4/tests/test_nested.py
--rw-r--r--   0 runner    (1001) docker     (127)     4608 2024-04-24 00:28:04.000000 jsx-0.6.4/tests/test_rendering.py
+drwxrwxrwx   0        0        0        0 2024-04-26 13:50:01.147458 jsx-0.6.5/
+-rw-rw-rw-   0        0        0     1062 2024-03-15 12:41:45.000000 jsx-0.6.5/LICENSE
+-rw-rw-rw-   0        0        0      737 2024-04-26 13:50:01.146451 jsx-0.6.5/PKG-INFO
+-rw-rw-rw-   0        0        0      115 2024-04-26 13:49:31.000000 jsx-0.6.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-26 13:50:01.032663 jsx-0.6.5/jsx/
+-rw-rw-rw-   0        0        0      159 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 13:50:01.043920 jsx-0.6.5/jsx/components/
+-rw-rw-rw-   0        0        0       70 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/components/__init__.py
+-rw-rw-rw-   0        0        0     1278 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/components/base.py
+-rw-rw-rw-   0        0        0     1244 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/components/page.py
+-rw-rw-rw-   0        0        0     1938 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/element.py
+-rw-rw-rw-   0        0        0       67 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/errors.py
+drwxrwxrwx   0        0        0        0 2024-04-26 13:50:01.125951 jsx-0.6.5/jsx/html/
+-rw-rw-rw-   0        0        0     2230 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/__init__.py
+-rw-rw-rw-   0        0        0      483 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/_auto_html.py
+-rw-rw-rw-   0        0        0       69 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/a.py
+-rw-rw-rw-   0        0        0       75 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/abbr.py
+-rw-rw-rw-   0        0        0       81 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/address.py
+-rw-rw-rw-   0        0        0       93 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/area.py
+-rw-rw-rw-   0        0        0       81 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/article.py
+-rw-rw-rw-   0        0        0       77 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/aside.py
+-rw-rw-rw-   0        0        0       69 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/b.py
+-rw-rw-rw-   0        0        0       75 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/base.py
+-rw-rw-rw-   0        0        0       87 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/blockquote.py
+-rw-rw-rw-   0        0        0       75 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/body.py
+-rw-rw-rw-   0        0        0       89 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/br.py
+-rw-rw-rw-   0        0        0       79 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/button.py
+-rw-rw-rw-   0        0        0       79 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/canvas.py
+-rw-rw-rw-   0        0        0       75 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/cite.py
+-rw-rw-rw-   0        0        0       75 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/code.py
+-rw-rw-rw-   0        0        0       91 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/col.py
+-rw-rw-rw-   0        0        0      347 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/div.py
+-rw-rw-rw-   0        0        0       71 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/em.py
+-rw-rw-rw-   0        0        0       95 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/embed.py
+-rw-rw-rw-   0        0        0       79 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/footer.py
+-rw-rw-rw-   0        0        0       75 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/form.py
+-rw-rw-rw-   0        0        0       65 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/fragment.py
+-rw-rw-rw-   0        0        0       71 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/h1.py
+-rw-rw-rw-   0        0        0       71 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/h2.py
+-rw-rw-rw-   0        0        0       71 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/h3.py
+-rw-rw-rw-   0        0        0       71 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/h4.py
+-rw-rw-rw-   0        0        0       71 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/h5.py
+-rw-rw-rw-   0        0        0       71 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/h6.py
+-rw-rw-rw-   0        0        0       75 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/head.py
+-rw-rw-rw-   0        0        0       79 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/header.py
+-rw-rw-rw-   0        0        0       89 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/hr.py
+-rw-rw-rw-   0        0        0       75 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/html.py
+-rw-rw-rw-   0        0        0       69 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/i.py
+-rw-rw-rw-   0        0        0       91 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/img.py
+-rw-rw-rw-   0        0        0       95 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/input.py
+-rw-rw-rw-   0        0        0       77 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/label.py
+-rw-rw-rw-   0        0        0       71 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/li.py
+-rw-rw-rw-   0        0        0       93 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/link.py
+-rw-rw-rw-   0        0        0       75 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/main.py
+-rw-rw-rw-   0        0        0       93 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/meta.py
+-rw-rw-rw-   0        0        0       73 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/nav.py
+-rw-rw-rw-   0        0        0       71 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/ol.py
+-rw-rw-rw-   0        0        0       79 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/option.py
+-rw-rw-rw-   0        0        0       69 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/p.py
+-rw-rw-rw-   0        0        0       77 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/param.py
+-rw-rw-rw-   0        0        0       73 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/pre.py
+-rw-rw-rw-   0        0        0       79 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/script.py
+-rw-rw-rw-   0        0        0       81 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/section.py
+-rw-rw-rw-   0        0        0       79 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/select.py
+-rw-rw-rw-   0        0        0       77 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/small.py
+-rw-rw-rw-   0        0        0       97 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/source.py
+-rw-rw-rw-   0        0        0       75 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/span.py
+-rw-rw-rw-   0        0        0       79 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/strong.py
+-rw-rw-rw-   0        0        0       73 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/sub.py
+-rw-rw-rw-   0        0        0       73 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/sup.py
+-rw-rw-rw-   0        0        0       77 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/table.py
+-rw-rw-rw-   0        0        0       77 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/tbody.py
+-rw-rw-rw-   0        0        0       71 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/td.py
+-rw-rw-rw-   0        0        0       83 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/textarea.py
+-rw-rw-rw-   0        0        0       71 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/th.py
+-rw-rw-rw-   0        0        0       77 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/thead.py
+-rw-rw-rw-   0        0        0       75 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/time.py
+-rw-rw-rw-   0        0        0       77 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/title.py
+-rw-rw-rw-   0        0        0       71 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/tr.py
+-rw-rw-rw-   0        0        0       95 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/track.py
+-rw-rw-rw-   0        0        0       69 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/u.py
+-rw-rw-rw-   0        0        0       71 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/ul.py
+-rw-rw-rw-   0        0        0       91 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/html/wbr.py
+-rw-rw-rw-   0        0        0     2214 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/internal.py
+drwxrwxrwx   0        0        0        0 2024-04-26 13:50:01.130211 jsx-0.6.5/jsx/middlewares/
+-rw-rw-rw-   0        0        0       63 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/middlewares/__init__.py
+-rw-rw-rw-   0        0        0     1466 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/middlewares/asgi.py
+-rw-rw-rw-   0        0        0     5589 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/middlewares/base.py
+-rw-rw-rw-   0        0        0     2429 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/renderer.py
+drwxrwxrwx   0        0        0        0 2024-04-26 13:50:01.133937 jsx-0.6.5/jsx/server/
+-rw-rw-rw-   0        0        0      437 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/server/components.py
+-rw-rw-rw-   0        0        0     5150 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/server/database.py
+-rw-rw-rw-   0        0        0     1680 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/server/request.py
+-rw-rw-rw-   0        0        0      739 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/server/ws_router.py
+drwxrwxrwx   0        0        0        0 2024-04-26 13:50:01.138216 jsx-0.6.5/jsx/styling/
+-rw-rw-rw-   0        0        0       70 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/styling/__init__.py
+-rw-rw-rw-   0        0        0     5031 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/styling/color.py
+-rw-rw-rw-   0        0        0     4159 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/styling/css_modules.py
+-rw-rw-rw-   0        0        0     1063 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/styling/style.py
+drwxrwxrwx   0        0        0        0 2024-04-26 13:50:01.140537 jsx-0.6.5/jsx/types/
+-rw-rw-rw-   0        0        0      331 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/types/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/types/base.py
+-rw-rw-rw-   0        0        0      488 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/types/events.py
+-rw-rw-rw-   0        0        0    10941 2024-04-26 13:49:31.000000 jsx-0.6.5/jsx/types/html.py
+drwxrwxrwx   0        0        0        0 2024-04-26 13:50:01.145440 jsx-0.6.5/jsx.egg-info/
+-rw-rw-rw-   0        0        0      737 2024-04-26 13:50:00.000000 jsx-0.6.5/jsx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1944 2024-04-26 13:50:01.000000 jsx-0.6.5/jsx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 13:50:00.000000 jsx-0.6.5/jsx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-04-26 13:50:00.000000 jsx-0.6.5/jsx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-04-26 13:50:00.000000 jsx-0.6.5/jsx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      687 2024-04-26 13:49:31.000000 jsx-0.6.5/pyproject.toml
+-rw-rw-rw-   0        0        0       39 2024-04-23 22:59:15.000000 jsx-0.6.5/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-04-26 13:50:01.147458 jsx-0.6.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-26 13:50:01.143996 jsx-0.6.5/tests/
+-rw-rw-rw-   0        0        0      404 2024-04-23 22:59:15.000000 jsx-0.6.5/tests/test_asgi_server.py
+-rw-rw-rw-   0        0        0      778 2024-04-26 13:49:31.000000 jsx-0.6.5/tests/test_nested.py
+-rw-rw-rw-   0        0        0     4608 2024-04-26 13:49:31.000000 jsx-0.6.5/tests/test_rendering.py
```

### Comparing `jsx-0.6.4/LICENSE` & `jsx-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jsx-0.6.4/jsx/components/base.py` & `jsx-0.6.5/jsx/components/base.py`

 * *Files identical despite different names*

### Comparing `jsx-0.6.4/jsx/components/page.py` & `jsx-0.6.5/jsx/components/page.py`

 * *Files identical despite different names*

### Comparing `jsx-0.6.4/jsx/element.py` & `jsx-0.6.5/jsx/element.py`

 * *Files identical despite different names*

### Comparing `jsx-0.6.4/jsx/html/__init__.py` & `jsx-0.6.5/jsx/html/__init__.py`

 * *Files identical despite different names*

### Comparing `jsx-0.6.4/jsx/internal.py` & `jsx-0.6.5/jsx/internal.py`

 * *Files identical despite different names*

### Comparing `jsx-0.6.4/jsx/middlewares/asgi.py` & `jsx-0.6.5/jsx/middlewares/asgi.py`

 * *Files identical despite different names*

### Comparing `jsx-0.6.4/jsx/middlewares/base.py` & `jsx-0.6.5/jsx/middlewares/base.py`

 * *Files identical despite different names*

### Comparing `jsx-0.6.4/jsx/renderer.py` & `jsx-0.6.5/jsx/renderer.py`

 * *Files identical despite different names*

### Comparing `jsx-0.6.4/jsx/server/database.py` & `jsx-0.6.5/jsx/server/database.py`

 * *Files identical despite different names*

### Comparing `jsx-0.6.4/jsx/server/request.py` & `jsx-0.6.5/jsx/server/request.py`

 * *Files identical despite different names*

### Comparing `jsx-0.6.4/jsx/server/ws_router.py` & `jsx-0.6.5/jsx/server/ws_router.py`

 * *Files identical despite different names*

### Comparing `jsx-0.6.4/jsx/styling/color.py` & `jsx-0.6.5/jsx/styling/color.py`

 * *Files identical despite different names*

### Comparing `jsx-0.6.4/jsx/styling/css_modules.py` & `jsx-0.6.5/jsx/styling/css_modules.py`

 * *Files identical despite different names*

### Comparing `jsx-0.6.4/jsx/styling/style.py` & `jsx-0.6.5/jsx/styling/style.py`

 * *Files identical despite different names*

### Comparing `jsx-0.6.4/jsx/types/html.py` & `jsx-0.6.5/jsx/types/html.py`

 * *Files identical despite different names*

### Comparing `jsx-0.6.4/jsx.egg-info/SOURCES.txt` & `jsx-0.6.5/jsx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jsx-0.6.4/pyproject.toml` & `jsx-0.6.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [project]
 name = "jsx"
-version = "0.6.4"
+version = "0.6.5"
 authors = [
   { name="Xpo Development", email="dev@xpo.dev" },
 ]
-description = "A Python package for creating and manipulating HTML components. It is working similar to React.js, but in Python"
+description = "This package is deprecated. Please use the `python-seamless` package instead."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dynamic = ["dependencies"]
 
 [project.urls]
-Homepage = "https://github.com/xpodev/jsx"
-Issues = "https://github.com/xpodev/jsx/issues"
+Homepage = "https://github.com/xpodev/seamless"
+Issues = "https://github.com/xpodev/seamless/issues"
 
 [tool.setuptools.packages.find]
 include = ["jsx*"]
 exclude = ["tests*"]
 
 
 [tool.setuptools.dynamic]
```

### Comparing `jsx-0.6.4/tests/test_nested.py` & `jsx-0.6.5/tests/test_nested.py`

 * *Files identical despite different names*

### Comparing `jsx-0.6.4/tests/test_rendering.py` & `jsx-0.6.5/tests/test_rendering.py`

 * *Files identical despite different names*

