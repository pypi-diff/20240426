# Comparing `tmp/svtter_template_creator-0.5.0.tar.gz` & `tmp/svtter_template_creator-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "svtter_template_creator-0.5.0.tar", max compression
+gzip compressed data, was "svtter_template_creator-0.6.0.tar", max compression
```

## Comparing `svtter_template_creator-0.5.0.tar` & `svtter_template_creator-0.6.0.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0     1067 2024-04-16 08:26:32.251785 svtter_template_creator-0.5.0/LICENSE
--rw-r--r--   0        0        0      579 2024-04-16 08:46:58.609471 svtter_template_creator-0.5.0/README.md
--rw-r--r--   0        0        0     1015 2024-04-16 08:41:08.095185 svtter_template_creator-0.5.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-16 08:32:06.941521 svtter_template_creator-0.5.0/src/__init__.py
--rw-r--r--   0        0        0       22 2024-04-16 08:46:16.612727 svtter_template_creator-0.5.0/src/svtter_template_creator/__init__.py
--rw-r--r--   0        0        0     1029 2024-04-16 08:42:48.311329 svtter_template_creator-0.5.0/src/svtter_template_creator/__main__.py
--rw-r--r--   0        0        0     1042 2024-04-16 08:45:06.742666 svtter_template_creator-0.5.0/src/svtter_template_creator/lib.py
--rw-r--r--   0        0        0        0 2024-04-16 08:20:55.369974 svtter_template_creator-0.5.0/src/svtter_template_creator/tests/__init__.py
--rw-r--r--   0        0        0     1069 1970-01-01 00:00:00.000000 svtter_template_creator-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-16 08:26:32.251785 svtter_template_creator-0.6.0/LICENSE
+-rw-r--r--   0        0        0      579 2024-04-16 08:47:34.010358 svtter_template_creator-0.6.0/README.md
+-rw-r--r--   0        0        0     1042 2024-04-26 01:47:03.790434 svtter_template_creator-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-16 08:47:34.010890 svtter_template_creator-0.6.0/src/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-16 08:47:34.011171 svtter_template_creator-0.6.0/src/svtter_template_creator/__init__.py
+-rw-r--r--   0        0        0     1612 2024-04-26 01:46:50.589328 svtter_template_creator-0.6.0/src/svtter_template_creator/__main__.py
+-rw-r--r--   0        0        0     1166 2024-04-26 01:46:50.589723 svtter_template_creator-0.6.0/src/svtter_template_creator/lib.py
+-rw-r--r--   0        0        0     1333 2024-04-26 01:46:50.589979 svtter_template_creator-0.6.0/src/svtter_template_creator/repl.py
+-rw-r--r--   0        0        0        0 2024-04-16 08:47:34.011838 svtter_template_creator-0.6.0/src/svtter_template_creator/tests/__init__.py
+-rw-r--r--   0        0        0      823 2024-04-26 01:46:50.590344 svtter_template_creator-0.6.0/src/svtter_template_creator/utils.py
+-rw-r--r--   0        0        0     1117 1970-01-01 00:00:00.000000 svtter_template_creator-0.6.0/PKG-INFO
```

### Comparing `svtter_template_creator-0.5.0/LICENSE` & `svtter_template_creator-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `svtter_template_creator-0.5.0/README.md` & `svtter_template_creator-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `svtter_template_creator-0.5.0/pyproject.toml` & `svtter_template_creator-0.6.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 # poetry version == 1.6
 name = "svtter_template_creator"
-version = "0.5.0"
+version = "0.6.0"
 readme = "README.md"
 description = ""
 authors = [ "svtter <svtter@163.com>",]
 keywords = ["template", "django"]
 include = ["src/*",]
 
 
@@ -28,14 +28,15 @@
 priority = "supplemental"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 click = "^8.1.3"
 cookiecutter = "^2.1.1"
 toml = "^0.10.2"
+prompt-toolkit = "^3.0.43"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2.0"
 pytest-xdist = "^3.0.2"
 pre-commit = "^2.20.0"
 
 [tool.poetry.scripts]
```

### Comparing `svtter_template_creator-0.5.0/src/svtter_template_creator/lib.py` & `svtter_template_creator-0.6.0/src/svtter_template_creator/lib.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,31 +14,33 @@
         "django": "{prefix}/cookiecutter-django.git".format(prefix=prefix),
         "package": "{prefix}/cookiecutter-pypackage.git".format(prefix=prefix),
         "compose": "{prefix}/cookiecutter-compose.git".format(prefix=prefix),
     }
     return template_dict
 
 
-def create(name):
+def create(name) -> None:
     """
     create template via name
     """
     # repo: dict[name, url]
     template_dict = read_repo()
 
-    template = template_dict[name]
+    template = template_dict.get(name, None)
+    if template is None:
+        raise ValueError(f"template {name} not found")
     os.system(f"cookiecutter {template}")
 
 
 def get_choice() -> t.List[str]:
     """get the choice from toml file"""
     repos = read_repo()
-    return repos.keys()
+    return list(repos.keys())
 
 
-def read_repo():
+def read_repo() -> t.Dict[str, str]:
     """get the repos from toml file"""
     c_path = pathlib.Path.home() / ".config" / "tt.toml"
     with open(c_path, "rb") as fp:
         config = tomli.load(fp)
 
     return config["repos"]
```

### Comparing `svtter_template_creator-0.5.0/PKG-INFO` & `svtter_template_creator-0.6.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: svtter_template_creator
-Version: 0.5.0
+Version: 0.6.0
 Summary: 
 Keywords: template,django
 Author: svtter
 Author-email: svtter@163.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: cookiecutter (>=2.1.1,<3.0.0)
+Requires-Dist: prompt-toolkit (>=3.0.43,<4.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Description-Content-Type: text/markdown
 
 # TT (Template Creator)
 
 This commandline application is built for create new project with specify code template.
```

