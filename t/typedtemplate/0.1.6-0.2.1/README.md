# Comparing `tmp/typedtemplate-0.1.6.tar.gz` & `tmp/typedtemplate-0.2.1.tar.gz`

## Comparing `typedtemplate-0.1.6.tar` & `typedtemplate-0.2.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 typedtemplate-0.1.6/tests/__init__.py
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 typedtemplate-0.1.6/tests/conftest.py
--rw-r--r--   0        0        0     2670 2020-02-02 00:00:00.000000 typedtemplate-0.1.6/tests/test_engine.py
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 typedtemplate-0.1.6/tests/test_template.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 typedtemplate-0.1.6/tests/test_data/test_template.txt
--rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 typedtemplate-0.1.6/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 typedtemplate-0.1.6/LICENSE
--rw-r--r--   0        0        0     7860 2020-02-02 00:00:00.000000 typedtemplate-0.1.6/README.md
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 typedtemplate-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     8218 2020-02-02 00:00:00.000000 typedtemplate-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 typedtemplate-0.2.1/tests/__init__.py
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 typedtemplate-0.2.1/tests/conftest.py
+-rw-r--r--   0        0        0     2670 2020-02-02 00:00:00.000000 typedtemplate-0.2.1/tests/test_engine.py
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 typedtemplate-0.2.1/tests/test_template.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 typedtemplate-0.2.1/tests/test_data/test_template.txt
+-rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 typedtemplate-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 typedtemplate-0.2.1/LICENSE
+-rw-r--r--   0        0        0     7860 2020-02-02 00:00:00.000000 typedtemplate-0.2.1/README.md
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 typedtemplate-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     8218 2020-02-02 00:00:00.000000 typedtemplate-0.2.1/PKG-INFO
```

### Comparing `typedtemplate-0.1.6/tests/conftest.py` & `typedtemplate-0.2.1/tests/conftest.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 from typing import ClassVar, Type
 
 import pytest
-from typedtemplate import TypedTemplate, DjangoTemplateEngine, JinjaTemplateEngine
+from typedtemplate import TypedTemplate, DjangoTemplateEngine, JinjaTemplateEngine, BaseTemplateEngine
 from pydantic import Field
 
 
 def pytest_sessionstart(session):
     """
     Initialize the Django settings for testing.
     :param session:
@@ -33,25 +33,28 @@
 
 @pytest.fixture(name="jinja_engine")
 def get_jinja_engine():
     dirs = get_dirs()
     return JinjaTemplateEngine(dirs=dirs, debug=True)
 
 
+@pytest.fixture(name="template_engine", params=("jinja_engine", "django_engine"))
+def get_template_engine(request):
+    return request.getfixturevalue(request.param)
+
+
 @pytest.fixture(name="string_template")
-def get_string_template(django_engine: DjangoTemplateEngine) -> Type[TypedTemplate]:
+def get_string_template(template_engine) -> Type[TypedTemplate]:
     class StringTemplate(TypedTemplate):
-        template_engine = django_engine
         template_string: ClassVar[str] = "Hello, {{ name }}!"
         name: str = Field(description="Person's name.")
-
+    StringTemplate.template_engine = template_engine
     return StringTemplate
 
 
 @pytest.fixture(name="file_template")
-def get_file_template(django_engine: DjangoTemplateEngine) -> Type[TypedTemplate]:
+def get_file_template(template_engine) -> Type[TypedTemplate]:
     class FileTemplate(TypedTemplate):
-        template_engine = django_engine
         template_file: ClassVar[str] = "test_template.txt"
         name: str = Field(description="Person's name.")
-
+    FileTemplate.template_engine = template_engine
     return FileTemplate
```

### Comparing `typedtemplate-0.1.6/tests/test_engine.py` & `typedtemplate-0.2.1/tests/test_engine.py`

 * *Files identical despite different names*

### Comparing `typedtemplate-0.1.6/.gitignore` & `typedtemplate-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `typedtemplate-0.1.6/LICENSE` & `typedtemplate-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `typedtemplate-0.1.6/README.md` & `typedtemplate-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `typedtemplate-0.1.6/pyproject.toml` & `typedtemplate-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `typedtemplate-0.1.6/PKG-INFO` & `typedtemplate-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: typedtemplate
-Version: 0.1.6
+Version: 0.2.1
 Summary: A typed string templating library using Pydantic
 Author-email: Todd Cullen <todd@100-x.ai>
 License: MIT
 License-File: LICENSE
 Requires-Python: >=3.9
 Requires-Dist: pydantic>=2.6.3
 Provides-Extra: jinja2
```

