# Comparing `tmp/coveralls-3.3.1.tar.gz` & `tmp/coveralls-3.3.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/coveralls-3.3.1.tar", last modified: Thu Nov 11 20:59:40 2021, max compression
+gzip compressed data, was "coveralls-3.3.2a0.tar", max compression
```

## Comparing `coveralls-3.3.1.tar` & `coveralls-3.3.2a0.tar`

### file list

```diff
@@ -1,24 +1,11 @@
-drwxr-xr-x   0 kevin      (503) staff       (20)        0 2021-11-11 20:59:40.000000 coveralls-3.3.1/
--rw-r--r--   0 kevin      (503) staff       (20)    11396 2021-11-11 20:59:26.000000 coveralls-3.3.1/CHANGELOG.md
--rw-r--r--   0 kevin      (503) staff       (20)     1058 2021-01-13 07:52:06.000000 coveralls-3.3.1/LICENSE.txt
--rw-r--r--   0 kevin      (503) staff       (20)       44 2019-08-22 22:45:43.000000 coveralls-3.3.1/MANIFEST.in
--rw-r--r--   0 kevin      (503) staff       (20)     4861 2021-11-11 20:59:40.000000 coveralls-3.3.1/PKG-INFO
--rw-r--r--   0 kevin      (503) staff       (20)     3686 2021-01-13 20:03:46.000000 coveralls-3.3.1/README.rst
-drwxr-xr-x   0 kevin      (503) staff       (20)        0 2021-11-11 20:59:40.000000 coveralls-3.3.1/coveralls/
--rw-r--r--   0 kevin      (503) staff       (20)      101 2020-11-19 23:06:05.000000 coveralls-3.3.1/coveralls/__init__.py
--rw-r--r--   0 kevin      (503) staff       (20)       62 2020-04-03 04:38:38.000000 coveralls-3.3.1/coveralls/__main__.py
--rw-r--r--   0 kevin      (503) staff       (20)    16112 2021-11-11 20:54:57.000000 coveralls-3.3.1/coveralls/api.py
--rw-r--r--   0 kevin      (503) staff       (20)     3426 2021-11-03 22:27:21.000000 coveralls-3.3.1/coveralls/cli.py
--rw-r--r--   0 kevin      (503) staff       (20)      300 2020-11-19 23:06:05.000000 coveralls-3.3.1/coveralls/exception.py
--rw-r--r--   0 kevin      (503) staff       (20)     4061 2021-11-04 00:22:05.000000 coveralls-3.3.1/coveralls/git.py
--rw-r--r--   0 kevin      (503) staff       (20)     8573 2021-11-03 21:53:22.000000 coveralls-3.3.1/coveralls/reporter.py
--rw-r--r--   0 kevin      (503) staff       (20)       22 2021-11-11 20:58:18.000000 coveralls-3.3.1/coveralls/version.py
-drwxr-xr-x   0 kevin      (503) staff       (20)        0 2021-11-11 20:59:40.000000 coveralls-3.3.1/coveralls.egg-info/
--rw-r--r--   0 kevin      (503) staff       (20)     4861 2021-11-11 20:59:40.000000 coveralls-3.3.1/coveralls.egg-info/PKG-INFO
--rw-r--r--   0 kevin      (503) staff       (20)      427 2021-11-11 20:59:40.000000 coveralls-3.3.1/coveralls.egg-info/SOURCES.txt
--rw-r--r--   0 kevin      (503) staff       (20)        1 2021-11-11 20:59:40.000000 coveralls-3.3.1/coveralls.egg-info/dependency_links.txt
--rw-r--r--   0 kevin      (503) staff       (20)       50 2021-11-11 20:59:40.000000 coveralls-3.3.1/coveralls.egg-info/entry_points.txt
--rw-r--r--   0 kevin      (503) staff       (20)       92 2021-11-11 20:59:40.000000 coveralls-3.3.1/coveralls.egg-info/requires.txt
--rw-r--r--   0 kevin      (503) staff       (20)       10 2021-11-11 20:59:40.000000 coveralls-3.3.1/coveralls.egg-info/top_level.txt
--rw-r--r--   0 kevin      (503) staff       (20)      100 2021-11-11 20:59:40.000000 coveralls-3.3.1/setup.cfg
--rw-r--r--   0 kevin      (503) staff       (20)     1919 2021-11-11 20:54:05.000000 coveralls-3.3.1/setup.py
+-rw-r--r--   0        0        0     1080 2024-04-26 13:41:01.159193 coveralls-3.3.2a0/LICENSE.rst
+-rw-r--r--   0        0        0     3694 2024-04-26 13:41:01.159193 coveralls-3.3.2a0/README.rst
+-rw-r--r--   0        0        0      134 2024-04-26 13:41:01.159193 coveralls-3.3.2a0/coveralls/__init__.py
+-rw-r--r--   0        0        0       62 2024-04-26 13:41:01.159193 coveralls-3.3.2a0/coveralls/__main__.py
+-rw-r--r--   0        0        0    16232 2024-04-26 13:41:01.159193 coveralls-3.3.2a0/coveralls/api.py
+-rw-r--r--   0        0        0     3485 2024-04-26 13:41:01.159193 coveralls-3.3.2a0/coveralls/cli.py
+-rw-r--r--   0        0        0      336 2024-04-26 13:41:01.159193 coveralls-3.3.2a0/coveralls/exception.py
+-rw-r--r--   0        0        0     4040 2024-04-26 13:41:01.159193 coveralls-3.3.2a0/coveralls/git.py
+-rw-r--r--   0        0        0     7174 2024-04-26 13:41:01.159193 coveralls-3.3.2a0/coveralls/reporter.py
+-rw-r--r--   0        0        0     1359 2024-04-26 13:41:01.163193 coveralls-3.3.2a0/pyproject.toml
+-rw-r--r--   0        0        0     5029 1970-01-01 00:00:00.000000 coveralls-3.3.2a0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `coveralls-3.3.1/LICENSE.txt` & `coveralls-3.3.2a0/LICENSE.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,22 @@
-Copyright (c) 2013 by TheKevJames
+MIT License
+===========
+
+Copyright (c) 2023 Kevin James
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
 
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
-THE SOFTWARE.
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `coveralls-3.3.1/PKG-INFO` & `coveralls-3.3.2a0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,46 +1,48 @@
 Metadata-Version: 2.1
 Name: coveralls
-Version: 3.3.1
+Version: 3.3.2a0
 Summary: Show coverage stats online via coveralls.io
 Home-page: http://github.com/TheKevJames/coveralls-python
-Author: TheKevJames
 License: MIT
-Project-URL: Changelog, https://github.com/TheKevJames/coveralls-python/blob/master/CHANGELOG.md
-Project-URL: Docs, https://coveralls-python.rtfd.io/
-Platform: UNKNOWN
+Author: Kevin James
+Author-email: coveralls-python@thekev.in
+Requires-Python: >=3.8,<3.11
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Topic :: Software Development :: Testing
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >= 3.5
+Classifier: Topic :: Software Development :: Testing
 Provides-Extra: yaml
-License-File: LICENSE.txt
+Requires-Dist: coverage (>=5.0,<7.0,!=6.0.*,!=6.1,!=6.1.1)
+Requires-Dist: docopt (>=0.6.1,<0.7.0)
+Requires-Dist: pyyaml (>=3.10,<7.0) ; extra == "yaml"
+Requires-Dist: requests (>=1.0.0,<3.0.0)
+Project-URL: Changelog, https://github.com/TheKevJames/coveralls-python/blob/master/CHANGELOG.md
+Project-URL: Docs, https://coveralls-python.rtfd.io/
+Project-URL: Repository, http://github.com/TheKevJames/coveralls-python
+Description-Content-Type: text/x-rst
 
 Coveralls for Python
 ====================
 
 :Test Status:
     .. image:: https://img.shields.io/circleci/project/github/TheKevJames/coveralls-python/master.svg?style=flat-square&label=CircleCI
         :target: https://circleci.com/gh/TheKevJames/coveralls-python
 
     .. image:: https://img.shields.io/travis/TheKevJames/coveralls-python/master.svg?style=flat-square&label=TravisCI
         :target: https://travis-ci.org/TheKevJames/coveralls-python
 
-    .. image:: https://img.shields.io/github/workflow/status/TheKevJames/coveralls-python/coveralls/master?style=flat-square&label=Github%20Actions
+    .. image:: https://img.shields.io/github/actions/workflow/status/TheKevJames/coveralls-python/coveralls/master?style=flat-square&label=Github%20Actions
         :target: https://github.com/TheKevJames/coveralls-python/actions
 
     .. image:: https://img.shields.io/coveralls/TheKevJames/coveralls-python/master.svg?style=flat-square&label=Coverage
         :target: https://coveralls.io/r/TheKevJames/coveralls-python
 
 :Version Info:
     .. image:: https://img.shields.io/conda/v/conda-forge/coveralls?style=flat-square&label=Conda
@@ -98,8 +100,7 @@
 
 .. _Docs: http://coveralls-python.readthedocs.io/en/latest/
 .. _coverage.py: https://coverage.readthedocs.io/en/latest/
 .. _coveralls.io: https://coveralls.io/
 .. _documentation: http://coveralls-python.readthedocs.io/en/latest/
 .. _the PyPA docs: https://packaging.python.org/guides/distributing-packages-using-setuptools/#python-requires
 
-
```

### Comparing `coveralls-3.3.1/README.rst` & `coveralls-3.3.2a0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 :Test Status:
     .. image:: https://img.shields.io/circleci/project/github/TheKevJames/coveralls-python/master.svg?style=flat-square&label=CircleCI
         :target: https://circleci.com/gh/TheKevJames/coveralls-python
 
     .. image:: https://img.shields.io/travis/TheKevJames/coveralls-python/master.svg?style=flat-square&label=TravisCI
         :target: https://travis-ci.org/TheKevJames/coveralls-python
 
-    .. image:: https://img.shields.io/github/workflow/status/TheKevJames/coveralls-python/coveralls/master?style=flat-square&label=Github%20Actions
+    .. image:: https://img.shields.io/github/actions/workflow/status/TheKevJames/coveralls-python/coveralls/master?style=flat-square&label=Github%20Actions
         :target: https://github.com/TheKevJames/coveralls-python/actions
 
     .. image:: https://img.shields.io/coveralls/TheKevJames/coveralls-python/master.svg?style=flat-square&label=Coverage
         :target: https://coveralls.io/r/TheKevJames/coveralls-python
 
 :Version Info:
     .. image:: https://img.shields.io/conda/v/conda-forge/coveralls?style=flat-square&label=Conda
```

### Comparing `coveralls-3.3.1/coveralls/api.py` & `coveralls-3.3.2a0/coveralls/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,20 +52,21 @@
         if self.config.get('repo_token') or not self._token_required:
             return
 
         if os.environ.get('GITHUB_ACTIONS'):
             raise CoverallsException(
                 'Running on Github Actions but GITHUB_TOKEN is not set. '
                 'Add "env: GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}" to '
-                'your step config.')
+                'your step config.',
+            )
 
         raise CoverallsException(
-            'Not on TravisCI. You have to provide either repo_token in {} or '
-            'set the COVERALLS_REPO_TOKEN env var.'.format(
-                self.config_filename))
+            'Not on TravisCI. You have to provide either repo_token in '
+            f'{self.config_filename} or set the COVERALLS_REPO_TOKEN env var.',
+        )
 
     def load_config(self, kwargs, service_name):
         """
         Loads all coveralls configuration in the following precedence order.
 
             1. automatic CI configuration
             2. COVERALLS_* env vars
@@ -93,16 +94,18 @@
         pr = os.environ.get('BUILDKITE_PULL_REQUEST')
         if pr == 'false':
             pr = None
         return 'buildkite', os.environ.get('BUILDKITE_JOB_ID'), None, pr
 
     @staticmethod
     def load_config_from_circle():
-        number = (os.environ.get('CIRCLE_WORKFLOW_ID')
-                  or os.environ.get('CIRCLE_BUILD_NUM'))
+        number = (
+            os.environ.get('CIRCLE_WORKFLOW_ID')
+            or os.environ.get('CIRCLE_BUILD_NUM')
+        )
         pr = (os.environ.get('CI_PULL_REQUEST') or '').split('/')[-1] or None
         job = os.environ.get('CIRCLE_NODE_INDEX')
         return 'circleci', job, number, pr
 
     def load_config_from_github(self):
         # Github tokens and standard Coveralls tokens are almost but not quite
         # the same -- forceibly using Github's flow seems to be more stable
@@ -168,14 +171,15 @@
         if pr_match:
             config['service_pull_request'] = pr_match[-1]
 
         non_empty = {key: value for key, value in config.items() if value}
         self.config.update(non_empty)
 
     def load_config_from_ci_environment(self):
+        # pylint: disable=too-complex
         # As defined at the bottom of
         # https://docs.coveralls.io/supported-ci-services
         # there are a few env vars that should support any arbitrary CI.
         # We load them first and allow more specific vars to overwrite
         self.load_config_from_generic_ci_environment()
 
         if os.environ.get('APPVEYOR'):
@@ -234,68 +238,79 @@
             fname = os.path.join(os.getcwd(), self.config_filename)
 
             with open(fname) as config:
                 try:
                     import yaml  # pylint: disable=import-outside-toplevel
                     self.config.update(yaml.safe_load(config))
                 except ImportError:
-                    log.warning('PyYAML is not installed, skipping %s.',
-                                self.config_filename)
+                    log.warning(
+                        'PyYAML is not installed, skipping %s.',
+                        self.config_filename,
+                    )
         except OSError:
-            log.debug('Missing %s file. Using only env variables.',
-                      self.config_filename)
+            log.debug(
+                'Missing %s file. Using only env variables.',
+                self.config_filename,
+            )
 
     def merge(self, path):
         reader = codecs.getreader('utf-8')
         with open(path, 'rb') as fh:
             extra = json.load(reader(fh))
             self.create_data(extra)
 
     def wear(self, dry_run=False):
         json_string = self.create_report()
         if dry_run:
             return {}
         return self.submit_report(json_string)
 
     def submit_report(self, json_string):
-        endpoint = '{}/api/v1/jobs'.format(self._coveralls_host.rstrip('/'))
+        endpoint = f'{self._coveralls_host.rstrip("/")}/api/v1/jobs'
         verify = not bool(os.environ.get('COVERALLS_SKIP_SSL_VERIFY'))
-        response = requests.post(endpoint, files={'json_file': json_string},
-                                 verify=verify)
+        response = requests.post(
+            endpoint, files={'json_file': json_string}, verify=verify,
+        )
 
         # check and adjust/resubmit if submission looks like it failed due to
         # resubmission (non-unique)
         if response.status_code == 422:
             # attach a random value to ensure uniqueness
             # TODO: an auto-incrementing integer might be easier to reason
             # about if we could fetch the previous value
             # N.B. Github Actions fails if this is not set to null.
             # Other services fail if this is set to null. Sigh x2.
             if os.environ.get('GITHUB_REPOSITORY'):
                 new_id = None
             else:
-                new_id = '{}-{}'.format(
-                    self.config.get('service_job_id', 42),
-                    random.randint(0, sys.maxsize))
-            print('resubmitting with id {}'.format(new_id))
+                new_id = '-'.join((
+                    self.config.get('service_job_id', '42'),
+                    str(random.randint(0, sys.maxsize)),
+                ))
+            print(f'resubmitting with id {new_id}')
 
             self.config['service_job_id'] = new_id
             self._data = None  # force create_report to use updated data
             json_string = self.create_report()
 
-            response = requests.post(endpoint,
-                                     files={'json_file': json_string},
-                                     verify=verify)
+            response = requests.post(
+                endpoint,
+                files={'json_file': json_string},
+                verify=verify,
+            )
 
         try:
             response.raise_for_status()
-            return response.json()
+            data = response.json()
         except Exception as e:
             raise CoverallsException(
-                'Could not submit coverage: {}'.format(e)) from e
+                f'Could not submit coverage: {e}',
+            ) from e
+
+        return data
 
     # https://docs.coveralls.io/parallel-build-webhook
     def parallel_finish(self):
         payload = {'payload': {'status': 'done'}}
 
         # required args
         if self.config.get('repo_token'):
@@ -304,59 +319,65 @@
             payload['payload']['build_num'] = self.config['service_number']
 
         # service-specific parameters
         if os.environ.get('GITHUB_REPOSITORY'):
             # Github Actions only
             payload['repo_name'] = os.environ.get('GITHUB_REPOSITORY')
 
-        endpoint = '{}/webhook'.format(self._coveralls_host.rstrip('/'))
+        endpoint = f'{self._coveralls_host.rstrip("/")}/webhook'
         verify = not bool(os.environ.get('COVERALLS_SKIP_SSL_VERIFY'))
         response = requests.post(endpoint, json=payload, verify=verify)
         try:
             response.raise_for_status()
             response = response.json()
         except Exception as e:
             raise CoverallsException(
-                'Parallel finish failed: {}'.format(e)) from e
+                f'Parallel finish failed: {e}',
+            ) from e
 
         if 'error' in response:
             e = response['error']
-            raise CoverallsException('Parallel finish failed: {}'.format(e))
+            raise CoverallsException(f'Parallel finish failed: {e}')
 
         if 'done' not in response or not response['done']:
             raise CoverallsException('Parallel finish failed')
 
         return response
 
     def create_report(self):
         """Generate json dumped report for coveralls api."""
         data = self.create_data()
         try:
             json_string = json.dumps(data)
-        except UnicodeDecodeError as e:
-            log.error('ERROR: While preparing JSON:', exc_info=e)
+        except UnicodeDecodeError:
+            log.exception('ERROR: While preparing JSON:')
             self.debug_bad_encoding(data)
             raise
 
-        log_string = re.sub(r'"repo_token": "(.+?)"',
-                            '"repo_token": "[secure]"', json_string)
+        log_string = re.sub(
+            r'"repo_token": "(.+?)"',
+            '"repo_token": "[secure]"',
+            json_string,
+        )
         log.debug(log_string)
         log.debug('==\nReporting %s files\n==\n', len(data['source_files']))
         for source_file in data['source_files']:
-            log.debug('%s - %s/%s', source_file['name'],
-                      sum(filter(None, source_file['coverage'])),
-                      len(source_file['coverage']))
+            log.debug(
+                '%s - %d/%d', source_file['name'],
+                sum(filter(None, source_file['coverage'])),
+                len(source_file['coverage']),
+            )
         return json_string
 
     def save_report(self, file_path):
         """Write coveralls report to file."""
         try:
             report = self.create_report()
-        except coverage.CoverageException as e:
-            log.error('Failure to gather coverage:', exc_info=e)
+        except coverage.CoverageException:
+            log.exception('Failure to gather coverage:')
         else:
             with open(file_path, 'w') as report_file:
                 report_file.write(report)
 
     def create_data(self, extra=None):
         r"""
         Generate object for api.
@@ -386,38 +407,41 @@
         self._data = {'source_files': self.get_coverage()}
         self._data.update(git_info())
         self._data.update(self.config)
         if extra:
             if 'source_files' in extra:
                 self._data['source_files'].extend(extra['source_files'])
             else:
-                log.warning('No data to be merged; does the json file contain '
-                            '"source_files" data?')
+                log.warning(
+                    'No data to be merged; does the json file contain '
+                    '"source_files" data?',
+                )
 
         return self._data
 
     def get_coverage(self):
         config_file = self.config.get('config_file', True)
-        workman = coverage.coverage(config_file=config_file)
-        workman.load()
-        workman.get_data()
+        work = coverage.coverage(config_file=config_file)
+        work.load()
+        work.get_data()
 
         base_dir = self.config.get('base_dir') or ''
         src_dir = self.config.get('src_dir') or ''
-        return CoverallReporter(workman, workman.config, base_dir,
-                                src_dir).coverage
+        return CoverallReporter(work, base_dir, src_dir).coverage
 
     @staticmethod
     def debug_bad_encoding(data):
         """Let's try to help user figure out what is at fault."""
         at_fault_files = set()
         for source_file_data in data['source_files']:
             for value in source_file_data.values():
                 try:
                     json.dumps(value)
                 except UnicodeDecodeError:
                     at_fault_files.add(source_file_data['name'])
 
         if at_fault_files:
-            log.error('HINT: Following files cannot be decoded properly into '
-                      'unicode. Check their content: %s',
-                      ', '.join(at_fault_files))
+            log.error(
+                'HINT: Following files cannot be decoded properly into '
+                'unicode. Check their content: %s',
+                ', '.join(at_fault_files),
+            )
```

### Comparing `coveralls-3.3.1/coveralls/cli.py` & `coveralls-3.3.2a0/coveralls/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,44 +32,48 @@
 -------
     $ coveralls
     Submitting coverage to coveralls.io...
     Coverage submitted!
     Job #38.1
     https://coveralls.io/jobs/92059
 """
+import importlib.metadata
 import logging
 import sys
 
 import docopt
 
 from .api import Coveralls
 from .exception import CoverallsException
-from .version import __version__
 
 
 log = logging.getLogger('coveralls')
 
 
 def main(argv=None):
-    options = docopt.docopt(__doc__, argv=argv, version=__version__)
+    # pylint: disable=too-complex
+    version = importlib.metadata.version('coveralls')
+    options = docopt.docopt(__doc__, argv=argv, version=version)
     if options['debug']:
         options['--verbose'] = True
 
     level = logging.DEBUG if options['--verbose'] else logging.INFO
     log.addHandler(logging.StreamHandler())
     log.setLevel(level)
 
     token_required = not options['debug'] and not options['--output']
 
     try:
-        coverallz = Coveralls(token_required,
-                              config_file=options['--rcfile'],
-                              service_name=options['--service'],
-                              base_dir=options.get('--basedir') or '',
-                              src_dir=options.get('--srcdir') or '')
+        coverallz = Coveralls(
+            token_required,
+            config_file=options['--rcfile'],
+            service_name=options['--service'],
+            base_dir=options.get('--basedir') or '',
+            src_dir=options.get('--srcdir') or '',
+        )
 
         if options['--merge']:
             coverallz.merge(options['--merge'])
 
         if options['debug']:
             log.info('Testing coveralls-python...')
             coverallz.wear(dry_run=True)
@@ -98,9 +102,9 @@
         log.debug(result)
         if result:
             log.info(result.get('message'))
             log.info(result.get('url'))
     except KeyboardInterrupt:  # pragma: no cover
         log.info('Aborted')
     except CoverallsException as e:
-        log.exception(e)
+        log.exception('Error running coveralls: %s', e)
         sys.exit(1)
```

### Comparing `coveralls-3.3.1/coveralls/git.py` & `coveralls-3.3.2a0/coveralls/git.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,29 +5,32 @@
 from .exception import CoverallsException
 
 
 log = logging.getLogger('coveralls.git')
 
 
 def run_command(*args):
-    with subprocess.Popen(list(args), stdout=subprocess.PIPE,
-                          stderr=subprocess.PIPE) as cmd:
+    with subprocess.Popen(
+        list(args), stdout=subprocess.PIPE, stderr=subprocess.PIPE,
+    ) as cmd:
         stdout, stderr = cmd.communicate()
 
         if cmd.returncode != 0:
             raise CoverallsException(
-                'command return code {}, STDOUT: "{}"\nSTDERR: "{}"'.format(
-                    cmd.returncode, stdout, stderr))
+                f'command returned code {cmd.returncode}, STDOUT: "{stdout}"\n'
+                f'STDERR: "{stderr}"',
+            )
 
         return stdout.decode().strip()
 
 
 def gitlog(fmt):
-    glog = run_command('git', '--no-pager', 'log', '-1',
-                       '--pretty=format:{}'.format(fmt))
+    glog = run_command(
+        'git', '--no-pager', 'log', '-1', f'--pretty=format:{fmt}',
+    )
 
     return str(glog)
 
 
 def git_branch():
     branch = None
     if os.environ.get('GITHUB_ACTIONS'):
@@ -38,22 +41,24 @@
         ):
             # E.g. in push events.
             branch = github_ref.split('/', 2)[-1]
         else:
             # E.g. in pull_request events.
             branch = os.environ.get('GITHUB_HEAD_REF')
     else:
-        branch = (os.environ.get('APPVEYOR_REPO_BRANCH')
-                  or os.environ.get('BUILDKITE_BRANCH')
-                  or os.environ.get('CI_BRANCH')
-                  or os.environ.get('CIRCLE_BRANCH')
-                  or os.environ.get('GIT_BRANCH')
-                  or os.environ.get('TRAVIS_BRANCH')
-                  or os.environ.get('BRANCH_NAME')
-                  or run_command('git', 'rev-parse', '--abbrev-ref', 'HEAD'))
+        branch = (
+            os.environ.get('APPVEYOR_REPO_BRANCH')
+            or os.environ.get('BUILDKITE_BRANCH')
+            or os.environ.get('CI_BRANCH')
+            or os.environ.get('CIRCLE_BRANCH')
+            or os.environ.get('GIT_BRANCH')
+            or os.environ.get('TRAVIS_BRANCH')
+            or os.environ.get('BRANCH_NAME')
+            or run_command('git', 'rev-parse', '--abbrev-ref', 'HEAD')
+        )
 
     return branch
 
 
 def git_info():
     """
     A hash of Git data that can be used to display more information to users.
@@ -82,17 +87,19 @@
             'id': gitlog('%H'),
             'author_name': gitlog('%aN'),
             'author_email': gitlog('%ae'),
             'committer_name': gitlog('%cN'),
             'committer_email': gitlog('%ce'),
             'message': gitlog('%s'),
         }
-        remotes = [{'name': line.split()[0], 'url': line.split()[1]}
-                   for line in run_command('git', 'remote', '-v').splitlines()
-                   if '(fetch)' in line]
+        remotes = [
+            {'name': line.split()[0], 'url': line.split()[1]}
+            for line in run_command('git', 'remote', '-v').splitlines()
+            if '(fetch)' in line
+        ]
     except (CoverallsException, OSError) as ex:
         # When git is not available, try env vars as per Coveralls docs:
         # https://docs.coveralls.io/mercurial-support
         # Additionally, these variables have been extended by GIT_URL and
         # GIT_REMOTE
         branch = os.environ.get('GIT_BRANCH')
         head = {
@@ -104,17 +111,19 @@
             'message': os.environ.get('GIT_MESSAGE'),
         }
         remotes = [{
             'name': os.environ.get('GIT_REMOTE'),
             'url': os.environ.get('GIT_URL'),
         }]
         if not all(head.values()):
-            log.warning('Failed collecting git data. Are you running '
-                        'coveralls inside a git repository? Is git installed?',
-                        exc_info=ex)
+            log.warning(
+                'Failed collecting git data. Are you running '
+                'coveralls inside a git repository? Is git installed?',
+                exc_info=ex,
+            )
             return {}
 
     return {
         'git': {
             'branch': branch,
             'head': head,
             'remotes': remotes,
```

### Comparing `coveralls-3.3.1/coveralls/reporter.py` & `coveralls-3.3.2a0/coveralls/reporter.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 import logging
 import os
 
-from coverage import __version__
+from coverage.files import FnmatchMatcher
+from coverage.files import prep_patterns
 
 try:
+    # coverage v6.x
     from coverage.exceptions import NoSource
     from coverage.exceptions import NotPython
 except ImportError:
+    # coverage v5.x
     from coverage.misc import NoSource
     from coverage.misc import NotPython
 
 log = logging.getLogger('coveralls.reporter')
 
 
 class CoverallReporter:
     """Custom coverage.py reporter for coveralls.io."""
 
-    def __init__(self, cov, conf, base_dir='', src_dir=''):
+    def __init__(self, cov, base_dir='', src_dir=''):
         self.coverage = []
         self.base_dir = self.sanitize_dir(base_dir)
         self.src_dir = self.sanitize_dir(src_dir)
-        self.report(cov, conf)
+        self.report(cov)
 
     @staticmethod
     def sanitize_dir(directory):
         if directory:
             directory = directory.replace(os.path.sep, '/')
             if directory[-1] != '/':
                 directory += '/'
         return directory
 
-    def report5(self, cov):
+    def report(self, cov):
         # N.B. this method is 99% copied from the coverage source code;
         # unfortunately, the coverage v5 style of `get_analysis_to_report`
         # errors out entirely if any source file has issues -- which would be a
         # breaking change for us. In the interest of backwards compatibility,
         # I've copied their code here so we can maintain the same `coveralls`
         # API regardless of which `coverage` version is being used.
         #
@@ -57,29 +60,31 @@
         #     # with get_analysis_to_report (a single exception breaks the
         #     # whole loop)
         #     log.warning('A source file is not python')
         # except CoverageException as e:
         #     if str(e) != 'No data to report.':
         #         raise
 
-        from coverage.files import FnmatchMatcher, prep_patterns  # pylint: disable=import-outside-toplevel
-
         # get_analysis_to_report starts here; changes marked with TODOs
         file_reporters = cov._get_file_reporters(None)  # pylint: disable=W0212
         config = cov.config
 
         if config.report_include:
             matcher = FnmatchMatcher(prep_patterns(config.report_include))
-            file_reporters = [fr for fr in file_reporters
-                              if matcher.match(fr.filename)]
+            file_reporters = [
+                fr for fr in file_reporters
+                if matcher.match(fr.filename)
+            ]
 
         if config.report_omit:
             matcher = FnmatchMatcher(prep_patterns(config.report_omit))
-            file_reporters = [fr for fr in file_reporters
-                              if not matcher.match(fr.filename)]
+            file_reporters = [
+                fr for fr in file_reporters
+                if not matcher.match(fr.filename)
+            ]
 
         # TODO: deprecate changes
         # if not file_reporters:
         #     raise CoverageException("No data to report.")
 
         for fr in sorted(file_reporters):
             try:
@@ -92,59 +97,29 @@
             except NotPython:
                 # Only report errors for .py files, and only if we didn't
                 # explicitly suppress those errors.
                 # NotPython is only raised by PythonFileReporter, which has a
                 # should_be_python() method.
                 if fr.should_be_python():
                     if config.ignore_errors:
-                        msg = "Couldn't parse Python file '{}'".format(
-                            fr.filename)
-                        cov._warn(msg,  # pylint: disable=W0212
-                                  slug='couldnt-parse')
+                        msg = f"Couldn't parse Python file '{fr.filename}'"
+                        cov._warn(  # pylint: disable=W0212
+                            msg, slug='couldnt-parse',
+                        )
                     else:
                         # TODO: deprecate changes
                         # raise
-                        log.warning('Source file is not python %s',
-                                    fr.filename)
+                        log.warning(
+                            'Source file is not python %s', fr.filename,
+                        )
             else:
                 # TODO: deprecate changes (well, this one is fine /shrug)
                 # yield (fr, analysis)
                 self.parse_file(fr, analysis)
 
-    def report(self, cov, conf, morfs=None):
-        """
-        Generate a part of json report for coveralls.
-
-        `morfs` is a list of modules or filenames.
-        `outfile` is a file object to write the json to.
-        """
-        # pylint: disable=too-many-branches
-        try:
-            from coverage.report import Reporter  # pylint: disable=import-outside-toplevel
-            self.reporter = Reporter(cov, conf)
-        except ImportError:  # coverage >= 5.0
-            return self.report5(cov)
-
-        for cu in self.reporter.find_file_reporters(morfs):
-            try:
-                _fn = self.reporter.coverage._analyze  # pylint: disable=W0212
-                analyzed = _fn(cu)
-                self.parse_file(cu, analyzed)
-            except NoSource:
-                if not self.reporter.config.ignore_errors:
-                    log.warning('No source for %s', cu.filename)
-            except NotPython:
-                # Only report errors for .py files, and only if we didn't
-                # explicitly suppress those errors.
-                if (cu.should_be_python()
-                        and not self.reporter.config.ignore_errors):
-                    log.warning('Source file is not python %s', cu.filename)
-
-        return self.coverage
-
     @staticmethod
     def get_hits(line_num, analysis):
         """
         Source file stats for each line.
 
         * A positive integer if the line is covered, representing the number
           of times the line is hit during the test suite.
@@ -170,21 +145,18 @@
         2. block-number (not used)
         3. branch-number
         4. hits (we only get 1/0 from coverage.py)
         """
         if not analysis.has_arcs():
             return None
 
-        if not hasattr(analysis, 'branch_lines'):
-            # N.B. switching to the public method analysis.missing_branch_arcs
-            # would work for half of what we need, but there doesn't seem to be
-            # an equivalent analysis.executed_branch_arcs
-            branch_lines = analysis._branch_lines()  # pylint: disable=W0212
-        else:
-            branch_lines = analysis.branch_lines()
+        # N.B. switching to the public method analysis.missing_branch_arcs
+        # would work for half of what we need, but there doesn't seem to be an
+        # equivalent analysis.executed_branch_arcs
+        branch_lines = analysis._branch_lines()  # pylint: disable=W0212
 
         branches = []
 
         for l1, l2 in analysis.arcs_executed():
             if l1 in branch_lines:
                 branches.extend((l1, 0, abs(l2), 1))
 
@@ -204,16 +176,18 @@
         if self.base_dir and posix_filename.startswith(self.base_dir):
             posix_filename = posix_filename[len(self.base_dir):]
         posix_filename = self.src_dir + posix_filename
 
         source = analysis.file_reporter.source()
 
         token_lines = analysis.file_reporter.source_token_lines()
-        coverage_lines = [self.get_hits(i, analysis)
-                          for i, _ in enumerate(token_lines, 1)]
+        coverage_lines = [
+            self.get_hits(i, analysis)
+            for i, _ in enumerate(token_lines, 1)
+        ]
 
         results = {
             'name': posix_filename,
             'source': source,
             'coverage': coverage_lines,
         }
```

