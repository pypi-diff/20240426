# Comparing `tmp/matricula_online_scraper-0.1.0.tar.gz` & `tmp/matricula_online_scraper-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matricula_online_scraper-0.1.0.tar", max compression
+gzip compressed data, was "matricula_online_scraper-0.2.2.tar", max compression
```

## Comparing `matricula_online_scraper-0.1.0.tar` & `matricula_online_scraper-0.2.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1069 2024-03-27 11:36:20.656439 matricula_online_scraper-0.1.0/LICENSE
--rw-r--r--   0        0        0     2337 2024-04-20 12:29:46.885391 matricula_online_scraper-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-04-14 16:06:16.035412 matricula_online_scraper-0.1.0/matricula_online_scraper/__init__.py
--rw-r--r--   0        0        0       65 2024-04-14 16:27:07.451976 matricula_online_scraper-0.1.0/matricula_online_scraper/__main__.py
--rw-r--r--   0        0        0        0 2024-04-14 09:44:43.603006 matricula_online_scraper-0.1.0/matricula_online_scraper/cli/__init__.py
--rw-r--r--   0        0        0     5801 2024-04-20 11:46:40.048266 matricula_online_scraper-0.1.0/matricula_online_scraper/cli/fetch.py
--rw-r--r--   0        0        0      707 2024-04-20 11:04:38.829286 matricula_online_scraper-0.1.0/matricula_online_scraper/cli/utils.py
--rwxr-xr-x   0        0        0      397 2024-04-18 11:28:02.591738 matricula_online_scraper-0.1.0/matricula_online_scraper/main.py
--rw-r--r--   0        0        0        0 2024-04-14 09:44:39.143678 matricula_online_scraper-0.1.0/matricula_online_scraper/spiders/__init__.py
--rw-r--r--   0        0        0     3191 2024-04-18 12:09:27.574662 matricula_online_scraper-0.1.0/matricula_online_scraper/spiders/locations_spider.py
--rw-r--r--   0        0        0     2852 2024-04-14 16:08:08.463555 matricula_online_scraper-0.1.0/matricula_online_scraper/spiders/parish_registers_spider.py
--rw-r--r--   0        0        0      600 2024-04-20 12:38:21.814623 matricula_online_scraper-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2846 1970-01-01 00:00:00.000000 matricula_online_scraper-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-26 09:00:25.992085 matricula_online_scraper-0.2.2/LICENSE
+-rw-r--r--   0        0        0     2337 2024-04-26 09:00:25.992085 matricula_online_scraper-0.2.2/README.md
+-rw-r--r--   0        0        0        0 2024-04-26 09:00:25.992085 matricula_online_scraper-0.2.2/matricula_online_scraper/__init__.py
+-rw-r--r--   0        0        0       65 2024-04-26 09:00:25.992085 matricula_online_scraper-0.2.2/matricula_online_scraper/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-26 09:00:25.992085 matricula_online_scraper-0.2.2/matricula_online_scraper/cli/__init__.py
+-rw-r--r--   0        0        0     5816 2024-04-26 09:00:25.992085 matricula_online_scraper-0.2.2/matricula_online_scraper/cli/fetch.py
+-rw-r--r--   0        0        0      707 2024-04-26 09:00:25.992085 matricula_online_scraper-0.2.2/matricula_online_scraper/cli/utils.py
+-rwxr-xr-x   0        0        0     1123 2024-04-26 09:00:25.992085 matricula_online_scraper-0.2.2/matricula_online_scraper/main.py
+-rw-r--r--   0        0        0        0 2024-04-26 09:00:25.992085 matricula_online_scraper-0.2.2/matricula_online_scraper/spiders/__init__.py
+-rw-r--r--   0        0        0     3191 2024-04-26 09:00:25.992085 matricula_online_scraper-0.2.2/matricula_online_scraper/spiders/locations_spider.py
+-rw-r--r--   0        0        0     4000 2024-04-26 09:00:25.992085 matricula_online_scraper-0.2.2/matricula_online_scraper/spiders/parish_registers_spider.py
+-rw-r--r--   0        0        0      856 2024-04-26 09:00:25.992085 matricula_online_scraper-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3157 1970-01-01 00:00:00.000000 matricula_online_scraper-0.2.2/PKG-INFO
```

### Comparing `matricula_online_scraper-0.1.0/LICENSE` & `matricula_online_scraper-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `matricula_online_scraper-0.1.0/README.md` & `matricula_online_scraper-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `matricula_online_scraper-0.1.0/matricula_online_scraper/cli/fetch.py` & `matricula_online_scraper-0.2.2/matricula_online_scraper/cli/fetch.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
 
 
 @app.command()
 def parish(
     output_file: Annotated[Path, typer.Argument()],
     urls: Annotated[
         List[URL],
-        typer.Option(parser=URL, help="One ore more URLs to scrape."),
+        typer.Option("--url", "-u", parser=URL, help="One ore more URLs to scrape."),
     ],
     log_level: LogLevelOption = DEFAULT_SCRAPER_LOG_LEVEL,
     silent: SilentOption = DEFAULT_SCRAPER_SILENT,
 ):
     """
     Scrape a parish register
     """
```

### Comparing `matricula_online_scraper-0.1.0/matricula_online_scraper/cli/utils.py` & `matricula_online_scraper-0.2.2/matricula_online_scraper/cli/utils.py`

 * *Files identical despite different names*

### Comparing `matricula_online_scraper-0.1.0/matricula_online_scraper/spiders/locations_spider.py` & `matricula_online_scraper-0.2.2/matricula_online_scraper/spiders/locations_spider.py`

 * *Files identical despite different names*

### Comparing `matricula_online_scraper-0.1.0/pyproject.toml` & `matricula_online_scraper-0.2.2/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 [tool.poetry]
 name = "matricula-online-scraper"
-version = "0.1.0"
+version = "0.2.2"
 description = "Command Line Interface tool for scraping Matricula Online https://data.matricula-online.eu."
+repository = "https://github.com/lsg551/matricula-online-scraper"
 authors = ["Luis Schulte"]
 license = "MIT"
 readme = "README.md"
+keywords = ["matricula-online", "matricula", "scraper", "parish-registers"]
+classifiers = [
+    "Environment :: Console",
+    "Development Status :: 3 - Alpha",
+    "Framework :: Scrapy",
+]
 
 [tool.poetry.scripts]
 matricula-online-scraper = "matricula_online_scraper.main:app"
 
 [tool.poetry.dependencies]
 python = "^3.12"
 scrapy = "^2.11.1"
```

### Comparing `matricula_online_scraper-0.1.0/PKG-INFO` & `matricula_online_scraper-0.2.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 Metadata-Version: 2.1
 Name: matricula-online-scraper
-Version: 0.1.0
+Version: 0.2.2
 Summary: Command Line Interface tool for scraping Matricula Online https://data.matricula-online.eu.
+Home-page: https://github.com/lsg551/matricula-online-scraper
 License: MIT
+Keywords: matricula-online,matricula,scraper,parish-registers
 Author: Luis Schulte
 Requires-Python: >=3.12,<4.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Console
+Classifier: Framework :: Scrapy
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: scrapy (>=2.11.1,<3.0.0)
 Requires-Dist: typer[all] (>=0.12.3,<0.13.0)
+Project-URL: Repository, https://github.com/lsg551/matricula-online-scraper
 Description-Content-Type: text/markdown
 
 # Matricula Online Scraper
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/matricula-online-scraper?logo=python)
 ![GitHub License](https://img.shields.io/github/license/lsg551/matricula-online-scraper?logo=pypi)
 ![PyPI - Version](https://img.shields.io/pypi/v/matricula-online-scraper?logo=pypi)
```

