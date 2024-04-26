# Comparing `tmp/prefect_gitlab-0.2.3.tar.gz` & `tmp/prefect_gitlab-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefect_gitlab-0.2.3.tar", last modified: Thu Apr 25 19:20:17 2024, max compression
+gzip compressed data, was "prefect_gitlab-0.2.4.tar", last modified: Fri Apr 26 15:03:59 2024, max compression
```

## Comparing `prefect_gitlab-0.2.3.tar` & `prefect_gitlab-0.2.4.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:17.937241 prefect_gitlab-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-04-25 19:20:17.937241 prefect_gitlab-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-25 19:20:05.000000 prefect_gitlab-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:17.933241 prefect_gitlab-0.2.3/prefect_gitlab/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-25 19:20:05.000000 prefect_gitlab-0.2.3/prefect_gitlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-25 19:20:17.000000 prefect_gitlab-0.2.3/prefect_gitlab/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-25 19:20:05.000000 prefect_gitlab-0.2.3/prefect_gitlab/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     7759 2024-04-25 19:20:05.000000 prefect_gitlab-0.2.3/prefect_gitlab/repositories.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:17.937241 prefect_gitlab-0.2.3/prefect_gitlab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-04-25 19:20:17.000000 prefect_gitlab-0.2.3/prefect_gitlab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-25 19:20:17.000000 prefect_gitlab-0.2.3/prefect_gitlab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:20:17.000000 prefect_gitlab-0.2.3/prefect_gitlab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-25 19:20:17.000000 prefect_gitlab-0.2.3/prefect_gitlab.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-25 19:20:17.000000 prefect_gitlab-0.2.3/prefect_gitlab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-25 19:20:17.000000 prefect_gitlab-0.2.3/prefect_gitlab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-25 19:20:05.000000 prefect_gitlab-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 19:20:17.937241 prefect_gitlab-0.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:17.937241 prefect_gitlab-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-25 19:20:05.000000 prefect_gitlab-0.2.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-25 19:20:05.000000 prefect_gitlab-0.2.3/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    10310 2024-04-25 19:20:05.000000 prefect_gitlab-0.2.3/tests/test_repositories.py
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-25 19:20:05.000000 prefect_gitlab-0.2.3/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:59.843779 prefect_gitlab-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-26 15:03:46.000000 prefect_gitlab-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-26 15:03:46.000000 prefect_gitlab-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4103 2024-04-26 15:03:59.843779 prefect_gitlab-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-26 15:03:46.000000 prefect_gitlab-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:59.839779 prefect_gitlab-0.2.4/prefect_gitlab/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-26 15:03:46.000000 prefect_gitlab-0.2.4/prefect_gitlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-26 15:03:59.000000 prefect_gitlab-0.2.4/prefect_gitlab/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-26 15:03:46.000000 prefect_gitlab-0.2.4/prefect_gitlab/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7759 2024-04-26 15:03:46.000000 prefect_gitlab-0.2.4/prefect_gitlab/repositories.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:59.843779 prefect_gitlab-0.2.4/prefect_gitlab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4103 2024-04-26 15:03:59.000000 prefect_gitlab-0.2.4/prefect_gitlab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-26 15:03:59.000000 prefect_gitlab-0.2.4/prefect_gitlab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 15:03:59.000000 prefect_gitlab-0.2.4/prefect_gitlab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-26 15:03:59.000000 prefect_gitlab-0.2.4/prefect_gitlab.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-26 15:03:59.000000 prefect_gitlab-0.2.4/prefect_gitlab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-26 15:03:59.000000 prefect_gitlab-0.2.4/prefect_gitlab.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-26 15:03:46.000000 prefect_gitlab-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 15:03:59.843779 prefect_gitlab-0.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:59.843779 prefect_gitlab-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-26 15:03:46.000000 prefect_gitlab-0.2.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-26 15:03:46.000000 prefect_gitlab-0.2.4/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10310 2024-04-26 15:03:46.000000 prefect_gitlab-0.2.4/tests/test_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-26 15:03:46.000000 prefect_gitlab-0.2.4/tests/test_version.py
```

### Comparing `prefect_gitlab-0.2.3/PKG-INFO` & `prefect_gitlab-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-gitlab
-Version: 0.2.3
+Version: 0.2.4
 Summary: A Prefect collection for working with GitLab repositories.
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-gitlab
 Keywords: prefect
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: prefect>=2.13.5
 Requires-Dist: python-gitlab>=3.12.0
 Requires-Dist: tenacity>=8.2.3
 Provides-Extra: dev
 Requires-Dist: aiohttp; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: interrogate; extra == "dev"
```

#### html2text {}

```diff
@@ -1,31 +1,31 @@
-Metadata-Version: 2.1 Name: prefect-gitlab Version: 0.2.3 Summary: A Prefect
+Metadata-Version: 2.1 Name: prefect-gitlab Version: 0.2.4 Summary: A Prefect
 collection for working with GitLab repositories. Author-email: "Prefect
 Technologies, Inc."
 prefect.io> License: Apache License 2.0 Project-URL: Homepage, https://
 github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-gitlab
 Keywords: prefect Classifier: Natural Language :: English Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Topic :: Software Development :: Libraries Requires-Python: >=3.8 Description-
-Content-Type: text/markdown Requires-Dist: prefect>=2.13.5 Requires-Dist:
-python-gitlab>=3.12.0 Requires-Dist: tenacity>=8.2.3 Provides-Extra: dev
-Requires-Dist: aiohttp; extra == "dev" Requires-Dist: coverage; extra == "dev"
-Requires-Dist: interrogate; extra == "dev" Requires-Dist: mkdocs-gen-files;
-extra == "dev" Requires-Dist: mkdocs-material; extra == "dev" Requires-Dist:
-mkdocs; extra == "dev" Requires-Dist: mkdocstrings[python]; extra == "dev"
-Requires-Dist: mock; python_version < "3.8" and extra == "dev" Requires-Dist:
-mypy; extra == "dev" Requires-Dist: pillow; extra == "dev" Requires-Dist: pre-
-commit; extra == "dev" Requires-Dist: pytest-asyncio; extra == "dev" Requires-
-Dist: pytest; extra == "dev" Requires-Dist: pytest-xdist; extra == "dev" #
-prefect-gitlab
+Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+prefect>=2.13.5 Requires-Dist: python-gitlab>=3.12.0 Requires-Dist:
+tenacity>=8.2.3 Provides-Extra: dev Requires-Dist: aiohttp; extra == "dev"
+Requires-Dist: coverage; extra == "dev" Requires-Dist: interrogate; extra ==
+"dev" Requires-Dist: mkdocs-gen-files; extra == "dev" Requires-Dist: mkdocs-
+material; extra == "dev" Requires-Dist: mkdocs; extra == "dev" Requires-Dist:
+mkdocstrings[python]; extra == "dev" Requires-Dist: mock; python_version <
+"3.8" and extra == "dev" Requires-Dist: mypy; extra == "dev" Requires-Dist:
+pillow; extra == "dev" Requires-Dist: pre-commit; extra == "dev" Requires-Dist:
+pytest-asyncio; extra == "dev" Requires-Dist: pytest; extra == "dev" Requires-
+Dist: pytest-xdist; extra == "dev" # prefect-gitlab
                 _[_P_y_P_I_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_d_m_/_p_r_e_f_e_c_t_-
                     _g_i_t_l_a_b_?_c_o_l_o_r_=_2_6_2_7_2_B_&_l_a_b_e_l_C_o_l_o_r_=_0_9_0_4_2_2_]
 ## Welcome! `prefect-gitlab` is a Prefect collection for working with GitLab
 repositories. ## Getting Started ### Python setup Requires an installation of
 Python 3.8 or higher. We recommend using a Python virtual environment manager
 such as pipenv, conda, or virtualenv. This integration is designed to work with
 Prefect 2.3.0 or higher. For more information about how to use Prefect, please
```

### Comparing `prefect_gitlab-0.2.3/README.md` & `prefect_gitlab-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `prefect_gitlab-0.2.3/prefect_gitlab/credentials.py` & `prefect_gitlab-0.2.4/prefect_gitlab/credentials.py`

 * *Files identical despite different names*

### Comparing `prefect_gitlab-0.2.3/prefect_gitlab/repositories.py` & `prefect_gitlab-0.2.4/prefect_gitlab/repositories.py`

 * *Files identical despite different names*

### Comparing `prefect_gitlab-0.2.3/prefect_gitlab.egg-info/PKG-INFO` & `prefect_gitlab-0.2.4/prefect_gitlab.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-gitlab
-Version: 0.2.3
+Version: 0.2.4
 Summary: A Prefect collection for working with GitLab repositories.
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-gitlab
 Keywords: prefect
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: prefect>=2.13.5
 Requires-Dist: python-gitlab>=3.12.0
 Requires-Dist: tenacity>=8.2.3
 Provides-Extra: dev
 Requires-Dist: aiohttp; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: interrogate; extra == "dev"
```

#### html2text {}

```diff
@@ -1,31 +1,31 @@
-Metadata-Version: 2.1 Name: prefect-gitlab Version: 0.2.3 Summary: A Prefect
+Metadata-Version: 2.1 Name: prefect-gitlab Version: 0.2.4 Summary: A Prefect
 collection for working with GitLab repositories. Author-email: "Prefect
 Technologies, Inc."
 prefect.io> License: Apache License 2.0 Project-URL: Homepage, https://
 github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-gitlab
 Keywords: prefect Classifier: Natural Language :: English Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Topic :: Software Development :: Libraries Requires-Python: >=3.8 Description-
-Content-Type: text/markdown Requires-Dist: prefect>=2.13.5 Requires-Dist:
-python-gitlab>=3.12.0 Requires-Dist: tenacity>=8.2.3 Provides-Extra: dev
-Requires-Dist: aiohttp; extra == "dev" Requires-Dist: coverage; extra == "dev"
-Requires-Dist: interrogate; extra == "dev" Requires-Dist: mkdocs-gen-files;
-extra == "dev" Requires-Dist: mkdocs-material; extra == "dev" Requires-Dist:
-mkdocs; extra == "dev" Requires-Dist: mkdocstrings[python]; extra == "dev"
-Requires-Dist: mock; python_version < "3.8" and extra == "dev" Requires-Dist:
-mypy; extra == "dev" Requires-Dist: pillow; extra == "dev" Requires-Dist: pre-
-commit; extra == "dev" Requires-Dist: pytest-asyncio; extra == "dev" Requires-
-Dist: pytest; extra == "dev" Requires-Dist: pytest-xdist; extra == "dev" #
-prefect-gitlab
+Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+prefect>=2.13.5 Requires-Dist: python-gitlab>=3.12.0 Requires-Dist:
+tenacity>=8.2.3 Provides-Extra: dev Requires-Dist: aiohttp; extra == "dev"
+Requires-Dist: coverage; extra == "dev" Requires-Dist: interrogate; extra ==
+"dev" Requires-Dist: mkdocs-gen-files; extra == "dev" Requires-Dist: mkdocs-
+material; extra == "dev" Requires-Dist: mkdocs; extra == "dev" Requires-Dist:
+mkdocstrings[python]; extra == "dev" Requires-Dist: mock; python_version <
+"3.8" and extra == "dev" Requires-Dist: mypy; extra == "dev" Requires-Dist:
+pillow; extra == "dev" Requires-Dist: pre-commit; extra == "dev" Requires-Dist:
+pytest-asyncio; extra == "dev" Requires-Dist: pytest; extra == "dev" Requires-
+Dist: pytest-xdist; extra == "dev" # prefect-gitlab
                 _[_P_y_P_I_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_d_m_/_p_r_e_f_e_c_t_-
                     _g_i_t_l_a_b_?_c_o_l_o_r_=_2_6_2_7_2_B_&_l_a_b_e_l_C_o_l_o_r_=_0_9_0_4_2_2_]
 ## Welcome! `prefect-gitlab` is a Prefect collection for working with GitLab
 repositories. ## Getting Started ### Python setup Requires an installation of
 Python 3.8 or higher. We recommend using a Python virtual environment manager
 such as pipenv, conda, or virtualenv. This integration is designed to work with
 Prefect 2.3.0 or higher. For more information about how to use Prefect, please
```

### Comparing `prefect_gitlab-0.2.3/pyproject.toml` & `prefect_gitlab-0.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `prefect_gitlab-0.2.3/tests/test_credentials.py` & `prefect_gitlab-0.2.4/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `prefect_gitlab-0.2.3/tests/test_repositories.py` & `prefect_gitlab-0.2.4/tests/test_repositories.py`

 * *Files identical despite different names*

