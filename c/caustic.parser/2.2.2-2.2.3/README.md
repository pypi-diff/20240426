# Comparing `tmp/caustic.parser-2.2.2.tar.gz` & `tmp/caustic.parser-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caustic.parser-2.2.2.tar", last modified: Thu Apr 25 17:27:39 2024, max compression
+gzip compressed data, was "caustic.parser-2.2.3.tar", last modified: Thu Apr 25 20:20:27 2024, max compression
```

## Comparing `caustic.parser-2.2.2.tar` & `caustic.parser-2.2.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-25 17:27:39.970394 caustic.parser-2.2.2/
--rw-r--r--   0 shae      (1000) shae      (1000)    11337 2024-04-08 15:09:28.000000 caustic.parser-2.2.2/LICENSE
--rw-r--r--   0 shae      (1000) shae      (1000)     1860 2024-04-25 17:27:39.970394 caustic.parser-2.2.2/PKG-INFO
--rw-r--r--   0 shae      (1000) shae      (1000)      985 2024-04-24 20:59:46.000000 caustic.parser-2.2.2/README.md
--rw-r--r--   0 shae      (1000) shae      (1000)     1001 2024-04-25 16:57:24.000000 caustic.parser-2.2.2/pyproject.toml
--rw-r--r--   0 shae      (1000) shae      (1000)       38 2024-04-25 17:27:39.970394 caustic.parser-2.2.2/setup.cfg
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-25 17:27:39.963727 caustic.parser-2.2.2/src/
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-25 17:27:39.963727 caustic.parser-2.2.2/src/caustic/
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-25 17:27:39.970394 caustic.parser-2.2.2/src/caustic/parser/
--rw-r--r--   0 shae      (1000) shae      (1000)     2157 2024-04-24 21:00:34.000000 caustic.parser-2.2.2/src/caustic/parser/__init__.py
--rw-r--r--   0 shae      (1000) shae      (1000)     5307 2024-04-25 16:58:16.000000 caustic.parser-2.2.2/src/caustic/parser/cli.py
--rw-r--r--   0 shae      (1000) shae      (1000)     3305 2024-04-25 04:27:15.000000 caustic.parser-2.2.2/src/caustic/parser/error.py
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-25 17:27:39.970394 caustic.parser-2.2.2/src/caustic.parser.egg-info/
--rw-r--r--   0 shae      (1000) shae      (1000)     1860 2024-04-25 17:27:39.000000 caustic.parser-2.2.2/src/caustic.parser.egg-info/PKG-INFO
--rw-r--r--   0 shae      (1000) shae      (1000)      371 2024-04-25 17:27:39.000000 caustic.parser-2.2.2/src/caustic.parser.egg-info/SOURCES.txt
--rw-r--r--   0 shae      (1000) shae      (1000)        1 2024-04-25 17:27:39.000000 caustic.parser-2.2.2/src/caustic.parser.egg-info/dependency_links.txt
--rw-r--r--   0 shae      (1000) shae      (1000)       47 2024-04-25 17:27:39.000000 caustic.parser-2.2.2/src/caustic.parser.egg-info/entry_points.txt
--rw-r--r--   0 shae      (1000) shae      (1000)       13 2024-04-25 17:27:39.000000 caustic.parser-2.2.2/src/caustic.parser.egg-info/requires.txt
--rw-r--r--   0 shae      (1000) shae      (1000)        8 2024-04-25 17:27:39.000000 caustic.parser-2.2.2/src/caustic.parser.egg-info/top_level.txt
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-25 20:20:27.563827 caustic.parser-2.2.3/
+-rw-r--r--   0 shae      (1000) shae      (1000)    11337 2024-04-08 15:09:28.000000 caustic.parser-2.2.3/LICENSE
+-rw-r--r--   0 shae      (1000) shae      (1000)     1860 2024-04-25 20:20:27.563827 caustic.parser-2.2.3/PKG-INFO
+-rw-r--r--   0 shae      (1000) shae      (1000)      985 2024-04-24 20:59:46.000000 caustic.parser-2.2.3/README.md
+-rw-r--r--   0 shae      (1000) shae      (1000)     1001 2024-04-25 20:17:59.000000 caustic.parser-2.2.3/pyproject.toml
+-rw-r--r--   0 shae      (1000) shae      (1000)       38 2024-04-25 20:20:27.563827 caustic.parser-2.2.3/setup.cfg
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-25 20:20:27.557160 caustic.parser-2.2.3/src/
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-25 20:20:27.557160 caustic.parser-2.2.3/src/caustic/
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-25 20:20:27.563827 caustic.parser-2.2.3/src/caustic/parser/
+-rw-r--r--   0 shae      (1000) shae      (1000)     2157 2024-04-24 21:00:34.000000 caustic.parser-2.2.3/src/caustic/parser/__init__.py
+-rw-r--r--   0 shae      (1000) shae      (1000)     5458 2024-04-25 20:19:44.000000 caustic.parser-2.2.3/src/caustic/parser/cli.py
+-rw-r--r--   0 shae      (1000) shae      (1000)     3305 2024-04-25 04:27:15.000000 caustic.parser-2.2.3/src/caustic/parser/error.py
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-25 20:20:27.563827 caustic.parser-2.2.3/src/caustic.parser.egg-info/
+-rw-r--r--   0 shae      (1000) shae      (1000)     1860 2024-04-25 20:20:27.000000 caustic.parser-2.2.3/src/caustic.parser.egg-info/PKG-INFO
+-rw-r--r--   0 shae      (1000) shae      (1000)      371 2024-04-25 20:20:27.000000 caustic.parser-2.2.3/src/caustic.parser.egg-info/SOURCES.txt
+-rw-r--r--   0 shae      (1000) shae      (1000)        1 2024-04-25 20:20:27.000000 caustic.parser-2.2.3/src/caustic.parser.egg-info/dependency_links.txt
+-rw-r--r--   0 shae      (1000) shae      (1000)       47 2024-04-25 20:20:27.000000 caustic.parser-2.2.3/src/caustic.parser.egg-info/entry_points.txt
+-rw-r--r--   0 shae      (1000) shae      (1000)       13 2024-04-25 20:20:27.000000 caustic.parser-2.2.3/src/caustic.parser.egg-info/requires.txt
+-rw-r--r--   0 shae      (1000) shae      (1000)        8 2024-04-25 20:20:27.000000 caustic.parser-2.2.3/src/caustic.parser.egg-info/top_level.txt
```

### Comparing `caustic.parser-2.2.2/LICENSE` & `caustic.parser-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `caustic.parser-2.2.2/PKG-INFO` & `caustic.parser-2.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caustic.parser
-Version: 2.2.2
+Version: 2.2.3
 Summary: Caustic's parsing framework
 Author: Shae.c32
 Project-URL: Homepage, https://codeberg.org/Caustic/CausticParser
 Project-URL: Issues, https://codeberg.org/Caustic/CausticParser/issues
 Keywords: caustic,language,parser,syntax,grammar
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `caustic.parser-2.2.2/README.md` & `caustic.parser-2.2.3/README.md`

 * *Files identical despite different names*

### Comparing `caustic.parser-2.2.2/pyproject.toml` & `caustic.parser-2.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "caustic.parser"
-version = "2.2.2"
+version = "2.2.3"
 dependencies = []
 requires-python = ">=3.9"
 authors = [{name="Shae.c32"}]
 maintainers = []
 description = "Caustic's parsing framework"
 readme = "README.md"
 keywords = ['caustic', 'language', 'parser', 'syntax', 'grammar']
```

### Comparing `caustic.parser-2.2.2/src/caustic/parser/__init__.py` & `caustic.parser-2.2.3/src/caustic/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `caustic.parser-2.2.2/src/caustic/parser/cli.py` & `caustic.parser-2.2.3/src/caustic/parser/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,34 +54,36 @@
 @click.command('Caustic Parser')
 @click.argument('source', type=click.Path('r', dir_okay=False, allow_dash=True, path_type=Path), default='-')
 @click.option('-g', '--grammar', type=click.Path(exists=True, dir_okay=False, path_type=Path), help='Alternative grammar file', default=None)
 @click.option('--glr', help='Use a GLR parser instead', is_flag=True, default=False)
 @click.option('-o', '--output', type=click.File('wb'), help='Where to write the output (defaults to a filename depending on the SOURCE and format, use "-" for STDOUT)', default=None)
 @click.option('-f', '--format', type=click.Choice(('pickle', 'json', 'json-pretty', 'pretty', 'tree')), help='What format to write as', default='pickle')
 @click.option('-q', '--quiet', help='Don\'t output status messages unless a failure occurs', is_flag=True, default=False)
-def cli(*, source: Path, grammar: Path | None, output: typing.BinaryIO | None, format: typing.Literal['pickle', 'json', 'json-pretty'], quiet: bool, glr: bool) -> None:
+@click.option('--debug', help='Put the parser in "debug" mode (see ParGlare docs)', is_flag=True, default=False)
+def cli(*, source: Path, grammar: Path | None, output: typing.BinaryIO | None, format: typing.Literal['pickle', 'json', 'json-pretty'],
+        quiet: bool, glr: bool, debug: bool) -> None:
     '''
         Parses a Caustic source file into a CST for compiling
 
         SOURCE is the file to compile (defaults to STDIN)
 
         Note that the "pickle" format is the only format that can be used by the (default) compiler
             "pretty" is recommended for viewing (without post-processing)
         Note that the "tree" format will force the LR (the default parser if --glr is not set) parser to generate a tree
     '''
     error = lambda *a,**kw: click.echo(click.style(*a, (255, 63, 63)), color=True, file=sys.stderr, **kw)
-    debug = (lambda *a,**kw: None) if quiet else (lambda *a,**kw: click.echo(*a, file=sys.stderr, **kw))
+    debug_ = (lambda *a,**kw: None) if quiet else (lambda *a,**kw: click.echo(*a, file=sys.stderr, **kw))
     real_source = str(source) != '-'
     tree_fmt = format == 'tree'
     # Load grammar
     if grammar is None:
         grammar = default_grammar()
-        debug(f'Default grammar discovered at {grammar}')
-    debug(f'Loading grammar and constructing parser from {grammar}')
-    parser = CausticParser.from_file(grammar, parser_type=(GLRParser if glr else Parser), build_tree=(tree_fmt or glr))
+        debug_(f'Default grammar discovered at {grammar}')
+    debug_(f'Loading grammar and constructing parser from {grammar}')
+    parser = CausticParser.from_file(grammar, parser_type=(GLRParser if glr else Parser), build_tree=(tree_fmt or glr), debug=debug)
     # Parse data
     try:
         parsed = (parser.parser.parse_file(source) if real_source
                   else parser.parse(sys.stdin.read(), file_name=None))
     except ParseError as e:
         error(format_exc(e))
         sys.exit(1)
@@ -113,12 +115,12 @@
         case 'tree':
             data = parsed.to_str().encode() + b'\n'
             suff = 'tree.txt'
         case _: raise ValueError(f'Unknown format: {format!r}')
     # Output
     if output is None:
         output = click.open_file((source.with_suffix(f'.cst.{suff}') if real_source else '-'), 'wb')
-    debug(f'Wrote {output.write(data)} byte(s) to {output.name}')
+    debug_(f'Wrote {output.write(data)} byte(s) to {output.name}')
 #</Header
 
 #> Main >/
 if __name__ == '__main__': cli()
```

### Comparing `caustic.parser-2.2.2/src/caustic/parser/error.py` & `caustic.parser-2.2.3/src/caustic/parser/error.py`

 * *Files identical despite different names*

### Comparing `caustic.parser-2.2.2/src/caustic.parser.egg-info/PKG-INFO` & `caustic.parser-2.2.3/src/caustic.parser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caustic.parser
-Version: 2.2.2
+Version: 2.2.3
 Summary: Caustic's parsing framework
 Author: Shae.c32
 Project-URL: Homepage, https://codeberg.org/Caustic/CausticParser
 Project-URL: Issues, https://codeberg.org/Caustic/CausticParser/issues
 Keywords: caustic,language,parser,syntax,grammar
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

