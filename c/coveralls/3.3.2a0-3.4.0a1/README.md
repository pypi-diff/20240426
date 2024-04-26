# Comparing `tmp/coveralls-3.3.2a0.tar.gz` & `tmp/coveralls-3.4.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coveralls-3.3.2a0.tar", max compression
+gzip compressed data, was "coveralls-3.4.0a1.tar", max compression
```

## Comparing `coveralls-3.3.2a0.tar` & `coveralls-3.4.0a1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1080 2024-04-26 13:41:01.159193 coveralls-3.3.2a0/LICENSE.rst
--rw-r--r--   0        0        0     3694 2024-04-26 13:41:01.159193 coveralls-3.3.2a0/README.rst
--rw-r--r--   0        0        0      134 2024-04-26 13:41:01.159193 coveralls-3.3.2a0/coveralls/__init__.py
--rw-r--r--   0        0        0       62 2024-04-26 13:41:01.159193 coveralls-3.3.2a0/coveralls/__main__.py
--rw-r--r--   0        0        0    16232 2024-04-26 13:41:01.159193 coveralls-3.3.2a0/coveralls/api.py
--rw-r--r--   0        0        0     3485 2024-04-26 13:41:01.159193 coveralls-3.3.2a0/coveralls/cli.py
--rw-r--r--   0        0        0      336 2024-04-26 13:41:01.159193 coveralls-3.3.2a0/coveralls/exception.py
--rw-r--r--   0        0        0     4040 2024-04-26 13:41:01.159193 coveralls-3.3.2a0/coveralls/git.py
--rw-r--r--   0        0        0     7174 2024-04-26 13:41:01.159193 coveralls-3.3.2a0/coveralls/reporter.py
--rw-r--r--   0        0        0     1359 2024-04-26 13:41:01.163193 coveralls-3.3.2a0/pyproject.toml
--rw-r--r--   0        0        0     5029 1970-01-01 00:00:00.000000 coveralls-3.3.2a0/PKG-INFO
+-rw-r--r--   0        0        0     1080 2024-04-26 16:43:14.938078 coveralls-3.4.0a1/LICENSE.rst
+-rw-r--r--   0        0        0     3880 2024-04-26 16:43:14.938078 coveralls-3.4.0a1/README.rst
+-rw-r--r--   0        0        0      134 2024-04-26 16:43:14.938078 coveralls-3.4.0a1/coveralls/__init__.py
+-rw-r--r--   0        0        0       62 2024-04-26 16:43:14.938078 coveralls-3.4.0a1/coveralls/__main__.py
+-rw-r--r--   0        0        0    16232 2024-04-26 16:43:14.938078 coveralls-3.4.0a1/coveralls/api.py
+-rw-r--r--   0        0        0     3434 2024-04-26 16:43:14.938078 coveralls-3.4.0a1/coveralls/cli.py
+-rw-r--r--   0        0        0      336 2024-04-26 16:43:14.938078 coveralls-3.4.0a1/coveralls/exception.py
+-rw-r--r--   0        0        0     4086 2024-04-26 16:43:14.938078 coveralls-3.4.0a1/coveralls/git.py
+-rw-r--r--   0        0        0     7466 2024-04-26 16:43:14.938078 coveralls-3.4.0a1/coveralls/reporter.py
+-rw-r--r--   0        0        0     1689 2024-04-26 16:43:14.942078 coveralls-3.4.0a1/pyproject.toml
+-rw-r--r--   0        0        0     5317 1970-01-01 00:00:00.000000 coveralls-3.4.0a1/PKG-INFO
```

### Comparing `coveralls-3.3.2a0/LICENSE.rst` & `coveralls-3.4.0a1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `coveralls-3.3.2a0/README.rst` & `coveralls-3.4.0a1/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,49 +1,47 @@
 Coveralls for Python
 ====================
 
 :Test Status:
+
     .. image:: https://img.shields.io/circleci/project/github/TheKevJames/coveralls-python/master.svg?style=flat-square&label=CircleCI
         :target: https://circleci.com/gh/TheKevJames/coveralls-python
-
-    .. image:: https://img.shields.io/travis/TheKevJames/coveralls-python/master.svg?style=flat-square&label=TravisCI
-        :target: https://travis-ci.org/TheKevJames/coveralls-python
-
-    .. image:: https://img.shields.io/github/actions/workflow/status/TheKevJames/coveralls-python/coveralls/master?style=flat-square&label=Github%20Actions
+    .. image:: https://img.shields.io/github/actions/workflow/status/TheKevJames/coveralls-python/test.yml?branch=master&style=flat-square&label=Github%20Actions
         :target: https://github.com/TheKevJames/coveralls-python/actions
-
     .. image:: https://img.shields.io/coveralls/TheKevJames/coveralls-python/master.svg?style=flat-square&label=Coverage
         :target: https://coveralls.io/r/TheKevJames/coveralls-python
+    .. image:: https://img.shields.io/readthedocs/coveralls-python?style=flat-square&label=Docs
+        :target: http://coveralls-python.readthedocs.io/en/latest/
 
 :Version Info:
-    .. image:: https://img.shields.io/conda/v/conda-forge/coveralls?style=flat-square&label=Conda
-        :target: https://anaconda.org/conda-forge/coveralls
 
     .. image:: https://img.shields.io/pypi/v/coveralls.svg?style=flat-square&label=PyPI
         :target: https://pypi.org/project/coveralls/
-
-    .. image:: https://img.shields.io/conda/dn/conda-forge/coveralls?label=Conda%20Downloads&style=flat-square
+    .. image:: https://img.shields.io/conda/v/conda-forge/coveralls?style=flat-square&label=Conda
         :target: https://anaconda.org/conda-forge/coveralls
-
-    .. image:: https://img.shields.io/pypi/dm/coveralls.svg?style=flat-square&label=PyPI%20Downloads
-        :target: https://pypi.org/project/coveralls/
+    .. image:: https://img.shields.io/docker/v/thekevjames/coveralls?sort=semver&style=flat-square&label=Dockerhub
+        :target: https://hub.docker.com/r/thekevjames/coveralls
+    .. image:: https://img.shields.io/docker/v/thekevjames/coveralls?sort=semver&style=flat-square&label=Quay
+        :target: https://quay.io/repository/thekevjames/coveralls
 
 :Compatibility:
+
     .. image:: https://img.shields.io/pypi/pyversions/coveralls.svg?style=flat-square&label=Python%20Versions
         :target: https://pypi.org/project/coveralls/
-
     .. image:: https://img.shields.io/pypi/implementation/coveralls.svg?style=flat-square&label=Python%20Implementations
         :target: https://pypi.org/project/coveralls/
 
-:Misc:
-    .. image:: https://img.shields.io/docker/cloud/build/thekevjames/coveralls?style=flat-square&label=Docker
-        :target: https://hub.docker.com/r/thekevjames/coveralls
+:Downloads:
 
-    .. image:: https://img.shields.io/readthedocs/coveralls-python?style=flat-square&label=Docs
-        :target: http://coveralls-python.readthedocs.io/en/latest/
+    .. image:: https://img.shields.io/pypi/dm/coveralls.svg?style=flat-square&label=PyPI
+        :target: https://pypi.org/project/coveralls/
+    .. image:: https://img.shields.io/conda/dn/conda-forge/coveralls?style=flat-square&label=Conda
+        :target: https://anaconda.org/conda-forge/coveralls
+    .. image:: https://img.shields.io/docker/pulls/thekevjames/coveralls?style=flat-square&label=Dockerhub
+        :target: https://hub.docker.com/r/thekevjames/coveralls
 
 `coveralls.io`_ is a service for publishing your coverage stats online. This
 package provides seamless integration with `coverage.py`_ (and thus ``pytest``,
 ``nosetests``, etc...) in your Python projects::
 
     pip install coveralls
     coverage run --source=mypkg -m pytest tests/
@@ -51,25 +49,25 @@
 
 For more information and usage instructions, see our `documentation`_.
 
 Version Compatibility
 ---------------------
 
 As of version 2.0, we have dropped support for end-of-life'd versions of Python
-and particularly old version of coverage. Support for non-EOL'd environments is
-provided on a best-effort basis and will generally be removed once they make
+and particularly old versions of coverage. Support for non-EOL'd environments
+is provided on a best-effort basis and will generally be removed once they make
 maintenance too difficult.
 
 If you're running on an outdated environment with a new enough package manager
 to support version checks (see `the PyPA docs`_), then installing the latest
-compatible version should do the trick. If you're even more outdated than that,
-please pin to ``coveralls<2``.
+compatible version should do the trick automatically! If you're even more
+outdated than that, please pin to ``coveralls<2``.
 
-If you're in an outdated environment and experiencing an issue, feel free to
-open a ticket -- but please mention your environment! I'm willing to backport
-fixes to the 1.x branch if need be.
+If you're in an outdated environment and experiencing an issue, you're welcome
+to open a ticket -- but please mention your environment! I'm willing to
+backport fixes to the 1.x branch if the need is great enough.
 
 .. _Docs: http://coveralls-python.readthedocs.io/en/latest/
 .. _coverage.py: https://coverage.readthedocs.io/en/latest/
 .. _coveralls.io: https://coveralls.io/
 .. _documentation: http://coveralls-python.readthedocs.io/en/latest/
 .. _the PyPA docs: https://packaging.python.org/guides/distributing-packages-using-setuptools/#python-requires
```

### Comparing `coveralls-3.3.2a0/coveralls/api.py` & `coveralls-3.4.0a1/coveralls/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,17 +50,17 @@
 
     def ensure_token(self):
         if self.config.get('repo_token') or not self._token_required:
             return
 
         if os.environ.get('GITHUB_ACTIONS'):
             raise CoverallsException(
-                'Running on Github Actions but GITHUB_TOKEN is not set. '
-                'Add "env: GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}" to '
-                'your step config.',
+                'Running on Github Actions but GITHUB_TOKEN is not set. Add '
+                '"env: GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}" to your '
+                'step config.',
             )
 
         raise CoverallsException(
             'Not on TravisCI. You have to provide either repo_token in '
             f'{self.config_filename} or set the COVERALLS_REPO_TOKEN env var.',
         )
```

### Comparing `coveralls-3.3.2a0/coveralls/cli.py` & `coveralls-3.4.0a1/coveralls/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 import importlib.metadata
 import logging
 import sys
 
 import docopt
 
 from .api import Coveralls
-from .exception import CoverallsException
 
 
 log = logging.getLogger('coveralls')
 
 
 def main(argv=None):
     # pylint: disable=too-complex
@@ -101,10 +100,10 @@
         log.info('Coverage submitted!')
         log.debug(result)
         if result:
             log.info(result.get('message'))
             log.info(result.get('url'))
     except KeyboardInterrupt:  # pragma: no cover
         log.info('Aborted')
-    except CoverallsException as e:
+    except Exception as e:
         log.exception('Error running coveralls: %s', e)
         sys.exit(1)
```

### Comparing `coveralls-3.3.2a0/coveralls/git.py` & `coveralls-3.4.0a1/coveralls/git.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 import logging
 import os
 import subprocess
+from typing import Any
+from typing import Dict
+from typing import Optional
 
 from .exception import CoverallsException
 
 
 log = logging.getLogger('coveralls.git')
 
 
-def run_command(*args):
-    with subprocess.Popen(
-        list(args), stdout=subprocess.PIPE, stderr=subprocess.PIPE,
-    ) as cmd:
-        stdout, stderr = cmd.communicate()
-
-        if cmd.returncode != 0:
-            raise CoverallsException(
-                f'command returned code {cmd.returncode}, STDOUT: "{stdout}"\n'
-                f'STDERR: "{stderr}"',
-            )
+def run_command(*args: str) -> str:
+    try:
+        cmd = subprocess.run(
+            list(args),
+            check=True,
+            capture_output=True,
+        )
+    except subprocess.CalledProcessError as e:
+        raise CoverallsException(
+            f'{e}\nSTDOUT: {e.stdout}\nSTDERR: {e.stderr}',
+        ) from e
 
-        return stdout.decode().strip()
+    return cmd.stdout.decode('utf-8').strip()
 
 
-def gitlog(fmt):
-    glog = run_command(
+def gitlog(fmt: str) -> str:
+    return run_command(
         'git', '--no-pager', 'log', '-1', f'--pretty=format:{fmt}',
     )
 
-    return str(glog)
-
 
-def git_branch():
+def git_branch() -> Optional[str]:
     branch = None
     if os.environ.get('GITHUB_ACTIONS'):
         github_ref = os.environ.get('GITHUB_REF')
         if (
             github_ref.startswith('refs/heads/')
             or github_ref.startswith('refs/tags/')
         ):
@@ -55,15 +56,15 @@
             or os.environ.get('BRANCH_NAME')
             or run_command('git', 'rev-parse', '--abbrev-ref', 'HEAD')
         )
 
     return branch
 
 
-def git_info():
+def git_info() -> Dict[str, Dict[str, Any]]:
     """
     A hash of Git data that can be used to display more information to users.
 
     Example:
     -------
         "git": {
             "head": {
@@ -112,17 +113,16 @@
         }
         remotes = [{
             'name': os.environ.get('GIT_REMOTE'),
             'url': os.environ.get('GIT_URL'),
         }]
         if not all(head.values()):
             log.warning(
-                'Failed collecting git data. Are you running '
-                'coveralls inside a git repository? Is git installed?',
-                exc_info=ex,
+                'Failed collecting git data. Are you running coveralls inside '
+                'a git repository? Is git installed?', exc_info=ex,
             )
             return {}
 
     return {
         'git': {
             'branch': branch,
             'head': head,
```

### Comparing `coveralls-3.3.2a0/coveralls/reporter.py` & `coveralls-3.4.0a1/coveralls/reporter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 import logging
 import os
 
-from coverage.files import FnmatchMatcher
 from coverage.files import prep_patterns
 
+
+try:
+    # coverage v7.x
+    from coverage.files import GlobMatcher
+except ImportError:
+    # coverage v5.x and v6.x
+    from coverage.files import FnmatchMatcher as GlobMatcher
+
 try:
     # coverage v6.x
     from coverage.exceptions import NoSource
     from coverage.exceptions import NotPython
 except ImportError:
     # coverage v5.x
     from coverage.misc import NoSource
@@ -31,15 +38,15 @@
             directory = directory.replace(os.path.sep, '/')
             if directory[-1] != '/':
                 directory += '/'
         return directory
 
     def report(self, cov):
         # N.B. this method is 99% copied from the coverage source code;
-        # unfortunately, the coverage v5 style of `get_analysis_to_report`
+        # unfortunately, the coverage v5+ style of `get_analysis_to_report`
         # errors out entirely if any source file has issues -- which would be a
         # breaking change for us. In the interest of backwards compatibility,
         # I've copied their code here so we can maintain the same `coveralls`
         # API regardless of which `coverage` version is being used.
         #
         # TODO: deprecate the relevant APIs so we can just use the coverage
         # public API directly.
@@ -61,26 +68,28 @@
         #     # whole loop)
         #     log.warning('A source file is not python')
         # except CoverageException as e:
         #     if str(e) != 'No data to report.':
         #         raise
 
         # get_analysis_to_report starts here; changes marked with TODOs
+        # TODO: in v7.5, this returns list of tuples (fr->morf)
+        # https://github.com/nedbat/coveragepy/commit/4e5027338b93fc893c5e6e82c8a234c48f0b95e7
         file_reporters = cov._get_file_reporters(None)  # pylint: disable=W0212
         config = cov.config
 
         if config.report_include:
-            matcher = FnmatchMatcher(prep_patterns(config.report_include))
+            matcher = GlobMatcher(prep_patterns(config.report_include))
             file_reporters = [
                 fr for fr in file_reporters
                 if matcher.match(fr.filename)
             ]
 
         if config.report_omit:
-            matcher = FnmatchMatcher(prep_patterns(config.report_omit))
+            matcher = GlobMatcher(prep_patterns(config.report_omit))
             file_reporters = [
                 fr for fr in file_reporters
                 if not matcher.match(fr.filename)
             ]
 
         # TODO: deprecate changes
         # if not file_reporters:
```

### Comparing `coveralls-3.3.2a0/pyproject.toml` & `coveralls-3.4.0a1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "coveralls"
-version = "3.3.2a0"
+version = "3.4.0a1"
 description = "Show coverage stats online via coveralls.io"
 readme = "README.rst"
 
 repository = "http://github.com/TheKevJames/coveralls-python"
 authors = ["Kevin James <coveralls-python@thekev.in>"]
 license = "MIT"
 
@@ -24,29 +24,40 @@
 
 [tool.poetry.urls]
 Changelog = "https://github.com/TheKevJames/coveralls-python/blob/master/CHANGELOG.md"
 Docs = "https://coveralls-python.rtfd.io/"
 
 [tool.poetry.scripts]
 coveralls = "coveralls.cli:main"
+python-coveralls = "coveralls.cli:main"
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.11"
-coverage = ">=5.0,<7.0,!=6.0.*,!=6.1,!=6.1.1"
+python = ">=3.8,<3.13"
+coverage = ">=5.0,<7.5,!=6.0.*,!=6.1,!=6.1.1"
 docopt = ">=0.6.1,<0.7.0"
 requests = ">=1.0.0,<3.0.0"
 
 pyyaml = { version = ">=3.10,<7.0", optional = true }
 
 [tool.poetry.group.dev.dependencies]
 pytest = "8.1.1"
 responses = "0.25.0"
 
+[tool.poetry.group.docs]
+optional = true
+[tool.poetry.group.docs.dependencies]
+sphinx = { version = "7.3.7", python = ">=3.9" }
+
 [tool.poetry.extras]
 yaml = ["pyyaml"]
 
 [tool.pytest.ini_options]
-addopts = "-Werror"
+# addopts = "-Werror"
+filterwarnings = [
+    "error",
+    # cov5 and cov6 are deprecated on py3.12+
+    "ignore:co_lnotab is deprecated, use co_lines instead:DeprecationWarning",
+]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `coveralls-3.3.2a0/PKG-INFO` & `coveralls-3.4.0a1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,79 +1,79 @@
 Metadata-Version: 2.1
 Name: coveralls
-Version: 3.3.2a0
+Version: 3.4.0a1
 Summary: Show coverage stats online via coveralls.io
 Home-page: http://github.com/TheKevJames/coveralls-python
 License: MIT
 Author: Kevin James
 Author-email: coveralls-python@thekev.in
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.8,<3.13
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Testing
 Provides-Extra: yaml
-Requires-Dist: coverage (>=5.0,<7.0,!=6.0.*,!=6.1,!=6.1.1)
+Requires-Dist: coverage (>=5.0,<7.5,!=6.0.*,!=6.1,!=6.1.1)
 Requires-Dist: docopt (>=0.6.1,<0.7.0)
 Requires-Dist: pyyaml (>=3.10,<7.0) ; extra == "yaml"
 Requires-Dist: requests (>=1.0.0,<3.0.0)
 Project-URL: Changelog, https://github.com/TheKevJames/coveralls-python/blob/master/CHANGELOG.md
 Project-URL: Docs, https://coveralls-python.rtfd.io/
 Project-URL: Repository, http://github.com/TheKevJames/coveralls-python
 Description-Content-Type: text/x-rst
 
 Coveralls for Python
 ====================
 
 :Test Status:
+
     .. image:: https://img.shields.io/circleci/project/github/TheKevJames/coveralls-python/master.svg?style=flat-square&label=CircleCI
         :target: https://circleci.com/gh/TheKevJames/coveralls-python
-
-    .. image:: https://img.shields.io/travis/TheKevJames/coveralls-python/master.svg?style=flat-square&label=TravisCI
-        :target: https://travis-ci.org/TheKevJames/coveralls-python
-
-    .. image:: https://img.shields.io/github/actions/workflow/status/TheKevJames/coveralls-python/coveralls/master?style=flat-square&label=Github%20Actions
+    .. image:: https://img.shields.io/github/actions/workflow/status/TheKevJames/coveralls-python/test.yml?branch=master&style=flat-square&label=Github%20Actions
         :target: https://github.com/TheKevJames/coveralls-python/actions
-
     .. image:: https://img.shields.io/coveralls/TheKevJames/coveralls-python/master.svg?style=flat-square&label=Coverage
         :target: https://coveralls.io/r/TheKevJames/coveralls-python
+    .. image:: https://img.shields.io/readthedocs/coveralls-python?style=flat-square&label=Docs
+        :target: http://coveralls-python.readthedocs.io/en/latest/
 
 :Version Info:
-    .. image:: https://img.shields.io/conda/v/conda-forge/coveralls?style=flat-square&label=Conda
-        :target: https://anaconda.org/conda-forge/coveralls
 
     .. image:: https://img.shields.io/pypi/v/coveralls.svg?style=flat-square&label=PyPI
         :target: https://pypi.org/project/coveralls/
-
-    .. image:: https://img.shields.io/conda/dn/conda-forge/coveralls?label=Conda%20Downloads&style=flat-square
+    .. image:: https://img.shields.io/conda/v/conda-forge/coveralls?style=flat-square&label=Conda
         :target: https://anaconda.org/conda-forge/coveralls
-
-    .. image:: https://img.shields.io/pypi/dm/coveralls.svg?style=flat-square&label=PyPI%20Downloads
-        :target: https://pypi.org/project/coveralls/
+    .. image:: https://img.shields.io/docker/v/thekevjames/coveralls?sort=semver&style=flat-square&label=Dockerhub
+        :target: https://hub.docker.com/r/thekevjames/coveralls
+    .. image:: https://img.shields.io/docker/v/thekevjames/coveralls?sort=semver&style=flat-square&label=Quay
+        :target: https://quay.io/repository/thekevjames/coveralls
 
 :Compatibility:
+
     .. image:: https://img.shields.io/pypi/pyversions/coveralls.svg?style=flat-square&label=Python%20Versions
         :target: https://pypi.org/project/coveralls/
-
     .. image:: https://img.shields.io/pypi/implementation/coveralls.svg?style=flat-square&label=Python%20Implementations
         :target: https://pypi.org/project/coveralls/
 
-:Misc:
-    .. image:: https://img.shields.io/docker/cloud/build/thekevjames/coveralls?style=flat-square&label=Docker
-        :target: https://hub.docker.com/r/thekevjames/coveralls
+:Downloads:
 
-    .. image:: https://img.shields.io/readthedocs/coveralls-python?style=flat-square&label=Docs
-        :target: http://coveralls-python.readthedocs.io/en/latest/
+    .. image:: https://img.shields.io/pypi/dm/coveralls.svg?style=flat-square&label=PyPI
+        :target: https://pypi.org/project/coveralls/
+    .. image:: https://img.shields.io/conda/dn/conda-forge/coveralls?style=flat-square&label=Conda
+        :target: https://anaconda.org/conda-forge/coveralls
+    .. image:: https://img.shields.io/docker/pulls/thekevjames/coveralls?style=flat-square&label=Dockerhub
+        :target: https://hub.docker.com/r/thekevjames/coveralls
 
 `coveralls.io`_ is a service for publishing your coverage stats online. This
 package provides seamless integration with `coverage.py`_ (and thus ``pytest``,
 ``nosetests``, etc...) in your Python projects::
 
     pip install coveralls
     coverage run --source=mypkg -m pytest tests/
@@ -81,26 +81,26 @@
 
 For more information and usage instructions, see our `documentation`_.
 
 Version Compatibility
 ---------------------
 
 As of version 2.0, we have dropped support for end-of-life'd versions of Python
-and particularly old version of coverage. Support for non-EOL'd environments is
-provided on a best-effort basis and will generally be removed once they make
+and particularly old versions of coverage. Support for non-EOL'd environments
+is provided on a best-effort basis and will generally be removed once they make
 maintenance too difficult.
 
 If you're running on an outdated environment with a new enough package manager
 to support version checks (see `the PyPA docs`_), then installing the latest
-compatible version should do the trick. If you're even more outdated than that,
-please pin to ``coveralls<2``.
+compatible version should do the trick automatically! If you're even more
+outdated than that, please pin to ``coveralls<2``.
 
-If you're in an outdated environment and experiencing an issue, feel free to
-open a ticket -- but please mention your environment! I'm willing to backport
-fixes to the 1.x branch if need be.
+If you're in an outdated environment and experiencing an issue, you're welcome
+to open a ticket -- but please mention your environment! I'm willing to
+backport fixes to the 1.x branch if the need is great enough.
 
 .. _Docs: http://coveralls-python.readthedocs.io/en/latest/
 .. _coverage.py: https://coverage.readthedocs.io/en/latest/
 .. _coveralls.io: https://coveralls.io/
 .. _documentation: http://coveralls-python.readthedocs.io/en/latest/
 .. _the PyPA docs: https://packaging.python.org/guides/distributing-packages-using-setuptools/#python-requires
```

