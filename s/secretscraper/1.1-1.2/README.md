# Comparing `tmp/secretscraper-1.1.tar.gz` & `tmp/secretscraper-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secretscraper-1.1.tar", max compression
+gzip compressed data, was "secretscraper-1.2.tar", max compression
```

## Comparing `secretscraper-1.1.tar` & `secretscraper-1.2.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0     1065 2024-04-08 13:21:30.604636 secretscraper-1.1/LICENSE
--rw-r--r--   0        0        0     6151 2024-04-16 12:13:13.795094 secretscraper-1.1/README.md
--rw-r--r--   0        0        0     1436 2024-04-16 12:27:38.251795 secretscraper-1.1/pyproject.toml
--rw-r--r--   0        0        0       41 2024-04-08 13:21:34.793928 secretscraper-1.1/src/secretscraper/__init__.py
--rw-r--r--   0        0        0     3993 2024-04-16 11:33:57.828364 secretscraper-1.1/src/secretscraper/cmdline.py
--rw-r--r--   0        0        0     1061 2024-04-16 09:41:18.245730 secretscraper-1.1/src/secretscraper/config/__init__.py
--rw-r--r--   0        0        0     1574 2024-04-16 11:30:07.208957 secretscraper-1.1/src/secretscraper/config/settings.yml
--rw-r--r--   0        0        0     7291 2024-04-15 07:08:57.009196 secretscraper-1.1/src/secretscraper/coroutinue.py
--rw-r--r--   0        0        0    12962 2024-04-16 12:29:17.184270 secretscraper-1.1/src/secretscraper/crawler.py
--rw-r--r--   0        0        0     1364 2024-04-15 07:17:15.401289 secretscraper-1.1/src/secretscraper/entity.py
--rw-r--r--   0        0        0      570 2024-04-16 10:31:30.720928 secretscraper-1.1/src/secretscraper/exception.py
--rw-r--r--   0        0        0     8868 2024-04-16 12:29:17.175298 secretscraper-1.1/src/secretscraper/facade.py
--rw-r--r--   0        0        0     2093 2024-04-15 07:08:56.960583 secretscraper-1.1/src/secretscraper/filter.py
--rw-r--r--   0        0        0     4817 2024-04-15 07:08:56.998319 secretscraper-1.1/src/secretscraper/handler.py
--rw-r--r--   0        0        0     1863 2024-04-16 09:41:19.559435 secretscraper-1.1/src/secretscraper/log.py
--rw-r--r--   0        0        0     6018 2024-04-16 10:31:30.770214 secretscraper-1.1/src/secretscraper/output_formatter.py
--rw-r--r--   0        0        0     2645 2024-04-15 07:08:56.999973 secretscraper-1.1/src/secretscraper/urlparser.py
--rw-r--r--   0        0        0      873 2024-04-16 10:31:30.742064 secretscraper-1.1/src/secretscraper/util.py
--rw-r--r--   0        0        0     7123 1970-01-01 00:00:00.000000 secretscraper-1.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-08 13:21:30.604636 secretscraper-1.2/LICENSE
+-rw-r--r--   0        0        0     6489 2024-04-26 08:06:31.965119 secretscraper-1.2/README.md
+-rw-r--r--   0        0        0     1436 2024-04-26 08:13:08.726579 secretscraper-1.2/pyproject.toml
+-rw-r--r--   0        0        0       41 2024-04-08 13:21:34.793928 secretscraper-1.2/src/secretscraper/__init__.py
+-rw-r--r--   0        0        0     4348 2024-04-26 07:57:48.575721 secretscraper-1.2/src/secretscraper/cmdline.py
+-rw-r--r--   0        0        0     1061 2024-04-16 09:41:18.245730 secretscraper-1.2/src/secretscraper/config/__init__.py
+-rw-r--r--   0        0        0     1574 2024-04-16 11:30:07.208957 secretscraper-1.2/src/secretscraper/config/settings.yml
+-rw-r--r--   0        0        0     7291 2024-04-15 07:08:57.009196 secretscraper-1.2/src/secretscraper/coroutinue.py
+-rw-r--r--   0        0        0    12962 2024-04-16 12:29:17.184270 secretscraper-1.2/src/secretscraper/crawler.py
+-rw-r--r--   0        0        0     1364 2024-04-15 07:17:15.401289 secretscraper-1.2/src/secretscraper/entity.py
+-rw-r--r--   0        0        0      675 2024-04-26 06:48:33.569989 secretscraper-1.2/src/secretscraper/exception.py
+-rw-r--r--   0        0        0    11771 2024-04-26 08:03:45.874327 secretscraper-1.2/src/secretscraper/facade.py
+-rw-r--r--   0        0        0     2093 2024-04-15 07:08:56.960583 secretscraper-1.2/src/secretscraper/filter.py
+-rw-r--r--   0        0        0     4817 2024-04-15 07:08:56.998319 secretscraper-1.2/src/secretscraper/handler.py
+-rw-r--r--   0        0        0     1863 2024-04-16 09:41:19.559435 secretscraper-1.2/src/secretscraper/log.py
+-rw-r--r--   0        0        0     6802 2024-04-26 08:02:37.301072 secretscraper-1.2/src/secretscraper/output_formatter.py
+-rw-r--r--   0        0        0     1396 2024-04-26 08:09:43.131988 secretscraper-1.2/src/secretscraper/scanner.py
+-rw-r--r--   0        0        0     2645 2024-04-15 07:08:56.999973 secretscraper-1.2/src/secretscraper/urlparser.py
+-rw-r--r--   0        0        0      873 2024-04-16 10:31:30.742064 secretscraper-1.2/src/secretscraper/util.py
+-rw-r--r--   0        0        0     7461 1970-01-01 00:00:00.000000 secretscraper-1.2/PKG-INFO
```

### Comparing `secretscraper-1.1/LICENSE` & `secretscraper-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `secretscraper-1.1/README.md` & `secretscraper-1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -114,14 +114,16 @@
   -s, --status TEXT            Filter response status to display, seperated by
                                commas, e.g. 200,300-400
   -x, --proxy TEXT             Set proxy, e.g. http://127.0.0.1:8080,
                                http://127.0.0.1:7890
   -H, --hide-regex             Hide regex search result
   -F, --follow-redirects       Follow redirects
   -u, --url TEXT               Target url
+  -l, --local PATH             Local file or directory, scan local
+                               file/directory recursively
   --help                       Show this message and exit.
 ```
 
 ### Advanced Usage
 
 #### Thorough Crawl
 
@@ -138,14 +140,20 @@
 ```
 
 #### Hide Regex Result
 Use `-H` option to hide regex-matching results. Only found links will be displayed.
 ```bash
 secretscraper -u https://scrapeme.live/shop/ -H
 ```
+
+#### Extract secrets from local file
+```bash
+secretscraper -l <dir or file>
+```
+
 #### Customize Configuration
 The built-in config is shown as below. You can assign custom configuration via `-i settings.yml`.
 ```yaml
 verbose: false
 debug: false
 loglevel: warning
 logpath: log
@@ -190,7 +198,15 @@
     regex: (=deleteMe|rememberMe=)
     loaded: true
   - name: Suspicious API Key
     regex: "[\"'][0-9a-zA-Z]{32}['\"]"
     loaded: true
 
 ```
+
+---
+
+# TODO
+- [x] Scan local file
+- [ ] Support windows
+- [ ] Support headless browser
+- [ ] Extract links additionally via regex
```

### Comparing `secretscraper-1.1/pyproject.toml` & `secretscraper-1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "secretscraper"
-version = "1.1"
+version = "1.2"
 description = "SecretScraper is a web scraper tool that can scrape the content through target websites and extract secret information via regular expression."
 readme = "README.md"
 authors = ["Padishah <straystrayer@gmail.com>"]
 license = "MIT"
 classifiers = [
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.11",
```

### Comparing `secretscraper-1.1/src/secretscraper/cmdline.py` & `secretscraper-1.2/src/secretscraper/cmdline.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import click
 from click import Context
 from dynaconf.base import Settings
 
 from secretscraper import __version__
 from secretscraper.config import settings
 from secretscraper.exception import FacadeException
-from secretscraper.facade import CrawlerFacade
+from secretscraper.facade import CrawlerFacade, FileScannerFacade
 from secretscraper.handler import HyperscanRegexHandler
 from secretscraper.log import init_log
 
 facade_settings = settings  # for unit test
 facade_obj = None
 
 
@@ -96,14 +96,16 @@
     "--proxy",
     help="Set proxy, e.g. http://127.0.0.1:8080, http://127.0.0.1:7890",
     type=click.STRING,
 )
 @click.option("-H", "--hide-regex", help="Hide regex search result", is_flag=True)
 @click.option("-F", "--follow-redirects", help="Follow redirects", is_flag=True, default=False)
 @click.option("-u", "--url", help="Target url", type=click.STRING)
+@click.option("-l", "--local", help="Local file or directory, scan local file/directory recursively ",
+              type=click.Path(exists=True, file_okay=True, dir_okay=True, path_type=pathlib.Path))
 def main(**options):
     """Main commands"""
     if options["version"]:
         click.echo(__version__)
         exit(1)
     if options["debug"]:
         settings.DEBUG = True
@@ -118,15 +120,18 @@
         if value is not None:
             options_dict[key] = value
     # settings.update(options_dict)
     try:
         global facade_settings, facade_obj
         print_func = functools.partial(click.echo, color=True)
         init_log()
-        facade = CrawlerFacade(settings, options_dict, print_func=print_func)
+        if options['local'] is not None:
+            facade = FileScannerFacade(settings, options_dict, print_func)
+        else:
+            facade = CrawlerFacade(settings, options_dict, print_func=print_func)
         facade_obj = facade
         facade_settings = facade.settings
     except FacadeException as e:
         click.echo(f"Error: {e}")
         exit(1)
     else:
         facade.start()
```

### Comparing `secretscraper-1.1/src/secretscraper/config/__init__.py` & `secretscraper-1.2/src/secretscraper/config/__init__.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.1/src/secretscraper/config/settings.yml` & `secretscraper-1.2/src/secretscraper/config/settings.yml`

 * *Files identical despite different names*

### Comparing `secretscraper-1.1/src/secretscraper/coroutinue.py` & `secretscraper-1.2/src/secretscraper/coroutinue.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.1/src/secretscraper/crawler.py` & `secretscraper-1.2/src/secretscraper/crawler.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.1/src/secretscraper/entity.py` & `secretscraper-1.2/src/secretscraper/entity.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.1/src/secretscraper/exception.py` & `secretscraper-1.2/src/secretscraper/exception.py`

 * *Files 15% similar despite different names*

```diff
@@ -25,7 +25,11 @@
     pass
 
 
 class FacadeException(SecretScraperException):
     """Exception raised by facade classes"""
 
     pass
+
+class FileScannerException(SecretScraperException):
+    """Exception raised by file scanner"""
+    pass
```

### Comparing `secretscraper-1.1/src/secretscraper/facade.py` & `secretscraper-1.2/src/secretscraper/facade.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,59 @@
 """Facade classes"""
 
 import copy
 import functools
 import logging
 import pathlib
+import traceback
 import typing
 import warnings
 from collections import namedtuple
 
 import click
 import dynaconf
 
 from .crawler import Crawler
-from .exception import FacadeException
+from .exception import FacadeException, FileScannerException
 from .filter import (ChainedURLFilter, DomainBlackListURLFilter,
                      DomainWhiteListURLFilter)
 from .handler import HyperscanRegexHandler
 from .output_formatter import Formatter
+from .scanner import FileScanner
 from .urlparser import URLParser
 from .util import Range, read_rules_from_setting
 
 logger = logging.getLogger(__name__)
 
 warnings.filterwarnings("ignore")  # ignore all warnings
 
 
+def print_func(f: typing.IO, func: typing.Callable, content: str, **kwargs) -> None:
+    func(content, **kwargs)
+    func(content, file=f, **kwargs)
+
+
+def print_func_colorful(
+    f: typing.IO,
+    func: typing.Callable,
+    content: str,
+    fg: str = None,
+    bg: str = None,
+    blink=False,
+    bold=False,
+):
+    print_func(f,
+               func,
+               click.style(content, fg=fg, bg=bg, blink=blink, bold=bold)
+               )
+
+
+print_config = functools.partial(click.secho, fg="bright_black", bold=True)
+
+
 class CrawlerFacade:
     """Crawler facade"""
 
     def __init__(
         self,
         full_settings: dynaconf.Dynaconf,
         custom_settings: dict,
@@ -51,58 +76,43 @@
         self.crawler: Crawler = self.create_crawler()
 
     def start(self):
         """Start the crawler and output"""
         with self.outfile.open("w") as f:
             try:
 
-                def print_func(content: str, **kwargs) -> None:
-                    self.print_func(content, **kwargs)
-                    self.print_func(content, file=f, **kwargs)
-
-                def print_func_colorful(
-                    content: str,
-                    fg: str = None,
-                    bg: str = None,
-                    blink=False,
-                    bold=False,
-                ):
-                    print_func(
-                        click.style(content, fg=fg, bg=bg, blink=blink, bold=bold)
-                    )
-
                 # print_func(f"Starting crawler...")
-                print_func_colorful(
-                    f"Target URLs: {', '.join(self.crawler.start_urls)}",
-                    bold=True,
-                    blink=True,
-                )
+                print_func_colorful(f,
+                                    self.print_func,
+                                    f"Target URLs: {', '.join(self.crawler.start_urls)}",
+                                    bold=True,
+                                    blink=True,
+                                    )
                 self.crawler.start()
 
-                # print_func_colorful(f"Total page: {self.crawler.total_page}")
+                # print_func_colorful(self.print_func,f"Total page: {self.crawler.total_page}")
                 self.formatter.output_url_hierarchy(self.crawler.url_dict, True)
 
                 self.formatter.output_found_domains(list(self.crawler.found_urls), True)
 
                 if not self.hide_regex:
-                    print_func_colorful(
-                        f"{self.formatter.output_secrets(self.crawler.url_secrets)}"
-                    )
-                print_func_colorful(f"{self.formatter.output_js(self.crawler.js_dict)}")
+                    print_func_colorful(self.print_func,
+                                        f"{self.formatter.output_secrets(self.crawler.url_secrets)}"
+                                        )
+                print_func_colorful(self.print_func, f"{self.formatter.output_js(self.crawler.js_dict)}")
             except KeyboardInterrupt:
                 self.print_func("\nExiting...")
                 self.crawler.close_all()
             except Exception as e:
                 self.print_func(f"Unexpected error: {e}.\nExiting...")
                 self.crawler.close_all()
                 # raise FacadeException from e
 
     def create_crawler(self) -> Crawler:
         """Create a Crawler"""
-        print_config = functools.partial(click.secho, fg="bright_black", bold=True)
         # Follow redirects
         if self.custom_settings.get("follow_redirects", False) is True:
             self.settings["follow_redirects"] = True
         # Hide regex output
         if self.custom_settings.get("hide_regex", False) is True:
             self.hide_regex = True
         # Get url filter
@@ -231,7 +241,83 @@
             headers=headers,
             verbose=self.settings.get("verbose"),
             timeout=self.settings.get("timeout"),
             debug=self.debug,
             follow_redirects=self.settings["follow_redirects"],
         )
         return crawler
+
+
+class FileScannerFacade:
+    """Facade for local file scanner"""
+
+    def __init__(
+        self,
+        full_settings: dynaconf.Dynaconf,
+        custom_settings: dict,
+        print_func: typing.Callable[[str], ...] = print,
+    ):
+        self.settings = full_settings
+        self.custom_settings = custom_settings
+        self.print_func = print_func
+        self.outfile = pathlib.Path(__file__).parent / "scanner.log"
+
+        self.formatter = Formatter()
+        self.scanner = self.init()
+
+    def start(self):
+        """Start file scanner"""
+        with open(self.outfile, "w") as f:
+            try:
+                print_func_colorful(f, self.print_func, f"Targets: {len(self.scanner.targets)}", bold=True)
+                self.scanner.start()
+
+                result = self.formatter.output_local_scan_secrets(self.scanner.secrets)
+                f.write(result)
+
+            except FileScannerException as e:
+                print_func_colorful(f, self.print_func,
+                                    f"Exception while scanning file: {e}\nTraceback: {traceback.format_exc()}",
+                                    fg="red")
+            except KeyboardInterrupt:
+                print_func_colorful(f, self.print_func, f"\nExiting")
+            except Exception as e:
+                print_func_colorful(f, self.print_func,
+                                    f"Unexpected error: {e}.\nTraceback: {traceback.format_exc()}\n Exiting...")
+
+    def init(self) -> FileScanner:
+        """Initialize options"""
+        # Verbose
+        verbose: typing.Optional[bool] = self.custom_settings.get("verbose", None)
+        if verbose is not None:
+            self.settings["verbose"] = verbose
+
+        # Outfile
+        outfile: typing.Optional[pathlib.Path] = self.custom_settings.get(
+            "outfile", None
+        )
+        if outfile is not None:
+            self.outfile = outfile
+        print_config(f"Output file: {self.outfile}")
+
+        # Read rules from config file
+        rules: dict[str, str] = read_rules_from_setting(self.settings)
+        handler = HyperscanRegexHandler(rules)
+
+        # Get all files from directory
+        base: typing.Optional[pathlib.Path] = self.custom_settings.get('local', None)
+        if base is None:
+            raise FacadeException(f"Internal error: No base directory")
+        targets: list[pathlib.Path] = list()
+        if base.is_file():
+            targets.append(base)
+        else:
+            for path in base.rglob("*"):
+                if path.is_file():
+                    targets.append(path)
+
+        # Create file scanner
+        file_scanner = FileScanner(
+            targets=targets,
+            handler=handler
+        )
+        return file_scanner
```

### Comparing `secretscraper-1.1/src/secretscraper/filter.py` & `secretscraper-1.2/src/secretscraper/filter.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.1/src/secretscraper/handler.py` & `secretscraper-1.2/src/secretscraper/handler.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.1/src/secretscraper/log.py` & `secretscraper-1.2/src/secretscraper/log.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.1/src/secretscraper/output_formatter.py` & `secretscraper-1.2/src/secretscraper/output_formatter.py`

 * *Files 10% similar despite different names*

```diff
@@ -158,7 +158,24 @@
             if secrets is not None and len(list(secrets)) > 0:
                 secret_set = {
                     f"{str(secret.type)}: {str(secret.data)}" for secret in secrets
                 }
                 secrets_str = "\n".join(secret_set)
                 url_secrets_str += f"\n{len(secret_set)} Secrets found in {url.url} {str(url.response_status)}:\n{secrets_str}\n"
         return url_secrets_str
+
+    def output_local_scan_secrets(self, path_secrets: dict[pathlib.Path, typing.Iterable[Secret]]) -> str:
+        """Display all secrets found in local file"""
+        if len(path_secrets) == 0:
+            click.echo("No secrets found.\n")
+        result = ""
+        for path, secrets in path_secrets.items():
+            if secrets is not None and len(list(secrets)) > 0:
+                secret_set = {
+                    f"{str(secret.type)}: {str(secret.data)}" for secret in secrets
+                }
+                secrets_str = "\n".join(secret_set)
+                s = click.style(f"\n{len(secret_set)} Secrets found in {str(path)}:", fg="cyan") + \
+                    f"\n{secrets_str}\n"
+                result += s
+                click.echo(s)
+        return result
```

### Comparing `secretscraper-1.1/src/secretscraper/urlparser.py` & `secretscraper-1.2/src/secretscraper/urlparser.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.1/src/secretscraper/util.py` & `secretscraper-1.2/src/secretscraper/util.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.1/PKG-INFO` & `secretscraper-1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secretscraper
-Version: 1.1
+Version: 1.2
 Summary: SecretScraper is a web scraper tool that can scrape the content through target websites and extract secret information via regular expression.
 License: MIT
 Author: Padishah
 Author-email: straystrayer@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -138,14 +138,16 @@
   -s, --status TEXT            Filter response status to display, seperated by
                                commas, e.g. 200,300-400
   -x, --proxy TEXT             Set proxy, e.g. http://127.0.0.1:8080,
                                http://127.0.0.1:7890
   -H, --hide-regex             Hide regex search result
   -F, --follow-redirects       Follow redirects
   -u, --url TEXT               Target url
+  -l, --local PATH             Local file or directory, scan local
+                               file/directory recursively
   --help                       Show this message and exit.
 ```
 
 ### Advanced Usage
 
 #### Thorough Crawl
 
@@ -162,14 +164,20 @@
 ```
 
 #### Hide Regex Result
 Use `-H` option to hide regex-matching results. Only found links will be displayed.
 ```bash
 secretscraper -u https://scrapeme.live/shop/ -H
 ```
+
+#### Extract secrets from local file
+```bash
+secretscraper -l <dir or file>
+```
+
 #### Customize Configuration
 The built-in config is shown as below. You can assign custom configuration via `-i settings.yml`.
 ```yaml
 verbose: false
 debug: false
 loglevel: warning
 logpath: log
@@ -215,7 +223,15 @@
     loaded: true
   - name: Suspicious API Key
     regex: "[\"'][0-9a-zA-Z]{32}['\"]"
     loaded: true
 
 ```
 
+---
+
+# TODO
+- [x] Scan local file
+- [ ] Support windows
+- [ ] Support headless browser
+- [ ] Extract links additionally via regex
+
```

