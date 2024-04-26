# Comparing `tmp/databricks_labs_pylint-0.3.0.tar.gz` & `tmp/databricks_labs_pylint-0.4.0.tar.gz`

## Comparing `databricks_labs_pylint-0.3.0.tar` & `databricks_labs_pylint-0.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.3.0/databricks/__init__.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.3.0/databricks/labs/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.3.0/databricks/labs/pylint/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.3.0/databricks/labs/pylint/__init__.py
--rw-r--r--   0        0        0     4533 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.3.0/databricks/labs/pylint/airflow.py
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.3.0/databricks/labs/pylint/all.py
--rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.3.0/databricks/labs/pylint/cli.py
--rw-r--r--   0        0        0     6254 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.3.0/databricks/labs/pylint/dbutils.py
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.3.0/databricks/labs/pylint/eradicate.py
--rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.3.0/databricks/labs/pylint/legacy.py
--rw-r--r--   0        0        0     4483 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.3.0/databricks/labs/pylint/mocking.py
--rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.3.0/databricks/labs/pylint/notebooks.py
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.3.0/databricks/labs/pylint/spark.py
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.3.0/.gitignore
--rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.3.0/LICENSE
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.3.0/NOTICE
--rw-r--r--   0        0        0    19654 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.3.0/README.md
--rw-r--r--   0        0        0    26455 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.3.0/pyproject.toml
--rw-r--r--   0        0        0    20712 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.4.0/databricks/__init__.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.4.0/databricks/labs/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.4.0/databricks/labs/pylint/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.4.0/databricks/labs/pylint/__init__.py
+-rw-r--r--   0        0        0     4533 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.4.0/databricks/labs/pylint/airflow.py
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.4.0/databricks/labs/pylint/all.py
+-rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.4.0/databricks/labs/pylint/cli.py
+-rw-r--r--   0        0        0     6254 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.4.0/databricks/labs/pylint/dbutils.py
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.4.0/databricks/labs/pylint/eradicate.py
+-rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.4.0/databricks/labs/pylint/legacy.py
+-rw-r--r--   0        0        0     6450 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.4.0/databricks/labs/pylint/mocking.py
+-rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.4.0/databricks/labs/pylint/notebooks.py
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.4.0/databricks/labs/pylint/spark.py
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.4.0/.gitignore
+-rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.4.0/NOTICE
+-rw-r--r--   0        0        0    20495 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.4.0/README.md
+-rw-r--r--   0        0        0    26455 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0    21553 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.4.0/PKG-INFO
```

### Comparing `databricks_labs_pylint-0.3.0/databricks/labs/pylint/airflow.py` & `databricks_labs_pylint-0.4.0/databricks/labs/pylint/airflow.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_pylint-0.3.0/databricks/labs/pylint/all.py` & `databricks_labs_pylint-0.4.0/databricks/labs/pylint/all.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_pylint-0.3.0/databricks/labs/pylint/cli.py` & `databricks_labs_pylint-0.4.0/databricks/labs/pylint/cli.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_pylint-0.3.0/databricks/labs/pylint/dbutils.py` & `databricks_labs_pylint-0.4.0/databricks/labs/pylint/dbutils.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_pylint-0.3.0/databricks/labs/pylint/eradicate.py` & `databricks_labs_pylint-0.4.0/databricks/labs/pylint/eradicate.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_pylint-0.3.0/databricks/labs/pylint/legacy.py` & `databricks_labs_pylint-0.4.0/databricks/labs/pylint/legacy.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_pylint-0.3.0/databricks/labs/pylint/mocking.py` & `databricks_labs_pylint-0.4.0/databricks/labs/pylint/mocking.py`

 * *Files 26% similar despite different names*

```diff
@@ -38,14 +38,25 @@
             DOC_EXPLICIT_DEPENDENCY_REQUIRED,
         ),
         "R8919": (
             "Obscure implicit test dependency with MagicMock(). Rewrite with create_autospec(ConcreteType).",
             "obscure-mock",
             DOC_OBSCURE_MOCK,
         ),
+        "R8921": (
+            "Mock not assigned to a variable: %s",
+            "mock-no-assign",
+            "Every mocked object should be assigned to a variable to allow for assertions.",
+        ),
+        "R8922": (
+            "Missing usage of mock for %s",
+            "mock-no-usage",
+            "Usually this check means a hidden bug, where object is mocked, but we don't check if it was used "
+            "correctly. Every mock should have at least one assertion, return value, or side effect specified.",
+        ),
     }
 
     options = (
         (
             "require-explicit-dependency",
             {
                 "default": ("databricks",),
@@ -61,20 +72,53 @@
 
     def visit_call(self, node: nodes.Call) -> None:
         # this also means that rare cases, like MagicMock(side_effect=...) are fine
         if node.as_string() == "MagicMock()":
             # here we can go and figure out the expected type of the object being mocked based on the arguments
             # where it is being assigned to, but that is a bit too much for this check. Other people can add this later.
             self.add_message("obscure-mock", node=node)
+        if node.func.as_string() == "create_autospec" and self._no_mock_usage(node):
+            return
         if not node.args:
             return
         if self._require_explicit_dependency and node.func.as_string() in {"mocker.patch", "patch"}:
             argument_value = node.args[0].as_string()
             no_quotes = argument_value.strip("'\"")
             for module in self._require_explicit_dependency:
                 if not no_quotes.startswith(module):
                     continue
                 self.add_message("explicit-dependency-required", node=node, args=argument_value)
 
+    def _no_mock_usage(self, node: nodes.Call) -> bool:
+        assignment = node.parent
+        if not isinstance(assignment, nodes.Assign):
+            self.add_message("mock-no-assign", node=node, args=node.as_string())
+            return True
+        if not assignment.targets:
+            self.add_message("mock-no-assign", node=node, args=assignment.as_string())
+            return True
+        mocked_type = node.args[0].as_string()
+        variable = assignment.targets[0].as_string()
+        has_assertion = False
+        has_return_value = False
+        for statement in assignment.parent.get_children():
+            statement_str = statement.as_string()
+            if not statement_str.startswith(f"{variable}."):
+                # this is not a method call on the variable we are interested in
+                continue
+            if ".assert" in statement_str:
+                has_assertion = True
+                break
+            if ".return_value" in statement_str:
+                has_return_value = True
+                break
+            if ".side_effect" in statement_str:
+                has_return_value = True
+                break
+        if not has_assertion and not has_return_value:
+            self.add_message("mock-no-usage", node=node, args=mocked_type)
+            return True
+        return False
+
 
 def register(linter):
     linter.register_checker(MockingChecker(linter))
```

### Comparing `databricks_labs_pylint-0.3.0/databricks/labs/pylint/notebooks.py` & `databricks_labs_pylint-0.4.0/databricks/labs/pylint/notebooks.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_pylint-0.3.0/databricks/labs/pylint/spark.py` & `databricks_labs_pylint-0.4.0/databricks/labs/pylint/spark.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_pylint-0.3.0/.gitignore` & `databricks_labs_pylint-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `databricks_labs_pylint-0.3.0/LICENSE` & `databricks_labs_pylint-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `databricks_labs_pylint-0.3.0/NOTICE` & `databricks_labs_pylint-0.4.0/NOTICE`

 * *Files identical despite different names*

### Comparing `databricks_labs_pylint-0.3.0/README.md` & `databricks_labs_pylint-0.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,16 @@
   * [`spark` checker](#spark-checker)
     * [`C8915`: `spark-outside-function`](#c8915-spark-outside-function)
     * [`C8917`: `use-display-instead-of-show`](#c8917-use-display-instead-of-show)
     * [`W8916`: `no-spark-argument-in-function`](#w8916-no-spark-argument-in-function)
   * [`mocking` checker](#mocking-checker)
     * [`R8918`: `explicit-dependency-required`](#r8918-explicit-dependency-required)
     * [`R8919`: `obscure-mock`](#r8919-obscure-mock)
+    * [`R8921`: `mock-no-assign`](#r8921-mock-no-assign)
+    * [`R8922`: `mock-no-usage`](#r8922-mock-no-usage)
   * [`eradicate` checker](#eradicate-checker)
     * [`C8920`: `dead-code`](#c8920-dead-code)
   * [Testing in isolation](#testing-in-isolation)
 * [Project Support](#project-support)
 <!-- TOC -->
 
 # Installation as PyLint plugin
@@ -333,14 +335,30 @@
 maintainable unit tests. Moreover, reliance on `MagicMock` for testing leads to issues during refactoring,
 as updates to underlying implementations would necessitate changes across multiple unrelated unit tests.
 
 To disable this check on a specific line, add `# pylint: disable=obscure-mock` at the end of it.
 
 [[back to top](#pylint-plugin-for-databricks)]
 
+### `R8921`: `mock-no-assign`
+
+Mock not assigned to a variable: XXX. Every mocked object should be assigned to a variable to allow for assertions.
+
+To disable this check on a specific line, add `# pylint: disable=mock-no-assign` at the end of it.
+
+[[back to top](#pylint-plugin-for-databricks)]
+
+### `R8922`: `mock-no-usage`
+
+Missing usage of mock for XXX. Usually this check means a hidden bug, where object is mocked, but we don't check if it was used correctly. Every mock should have at least one assertion, return value, or side effect specified.
+
+To disable this check on a specific line, add `# pylint: disable=mock-no-usage` at the end of it.
+
+[[back to top](#pylint-plugin-for-databricks)]
+
 ## `eradicate` checker
 To use this checker, add `databricks.labs.pylint.eradicate` to `load-plugins` configuration in your `pylintrc` or `pyproject.toml` file.
 
 [[back to top](#pylint-plugin-for-databricks)]
 
 ### `C8920`: `dead-code`
 
@@ -350,15 +368,15 @@
 
 [[back to top](#pylint-plugin-for-databricks)]
 
 ## Testing in isolation
 To test this plugin in isolation, you can use the following command:
 
 ```bash
-pylint --load-plugins=databricks.labs.pylint.all --disable=all --enable=missing-data-security-mode,unsupported-runtime,dbutils-fs-cp,dbutils-fs-head,dbutils-fs-ls,dbutils-fs-mount,dbutils-credentials,dbutils-notebook-run,pat-token-leaked,internal-api,legacy-cli,incompatible-with-uc,notebooks-too-many-cells,notebooks-percent-run,spark-outside-function,use-display-instead-of-show,no-spark-argument-in-function,explicit-dependency-required,obscure-mock,dead-code .
+pylint --load-plugins=databricks.labs.pylint.all --disable=all --enable=missing-data-security-mode,unsupported-runtime,dbutils-fs-cp,dbutils-fs-head,dbutils-fs-ls,dbutils-fs-mount,dbutils-credentials,dbutils-notebook-run,pat-token-leaked,internal-api,legacy-cli,incompatible-with-uc,notebooks-too-many-cells,notebooks-percent-run,spark-outside-function,use-display-instead-of-show,no-spark-argument-in-function,explicit-dependency-required,obscure-mock,mock-no-assign,mock-no-usage,dead-code .
 ```
 
 [[back to top](#pylint-plugin-for-databricks)]
 
 <!-- END CHECKS -->
 
 # Project Support
```

### Comparing `databricks_labs_pylint-0.3.0/pyproject.toml` & `databricks_labs_pylint-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `databricks_labs_pylint-0.3.0/PKG-INFO` & `databricks_labs_pylint-0.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: databricks-labs-pylint
-Version: 0.3.0
+Version: 0.4.0
 Summary: Plugin for PyLint to support Databricks specific code patterns and best practices.
 Project-URL: Issues, https://github.com/databrickslabs/pylint-plugin/issues
 Project-URL: Source, https://github.com/databrickslabs/pylint-plugin
 Author-email: Serge Smertin <serge.smertin@databricks.com>
 License-File: LICENSE
 License-File: NOTICE
 Keywords: Databricks
@@ -65,14 +65,16 @@
   * [`spark` checker](#spark-checker)
     * [`C8915`: `spark-outside-function`](#c8915-spark-outside-function)
     * [`C8917`: `use-display-instead-of-show`](#c8917-use-display-instead-of-show)
     * [`W8916`: `no-spark-argument-in-function`](#w8916-no-spark-argument-in-function)
   * [`mocking` checker](#mocking-checker)
     * [`R8918`: `explicit-dependency-required`](#r8918-explicit-dependency-required)
     * [`R8919`: `obscure-mock`](#r8919-obscure-mock)
+    * [`R8921`: `mock-no-assign`](#r8921-mock-no-assign)
+    * [`R8922`: `mock-no-usage`](#r8922-mock-no-usage)
   * [`eradicate` checker](#eradicate-checker)
     * [`C8920`: `dead-code`](#c8920-dead-code)
   * [Testing in isolation](#testing-in-isolation)
 * [Project Support](#project-support)
 <!-- TOC -->
 
 # Installation as PyLint plugin
@@ -359,14 +361,30 @@
 maintainable unit tests. Moreover, reliance on `MagicMock` for testing leads to issues during refactoring,
 as updates to underlying implementations would necessitate changes across multiple unrelated unit tests.
 
 To disable this check on a specific line, add `# pylint: disable=obscure-mock` at the end of it.
 
 [[back to top](#pylint-plugin-for-databricks)]
 
+### `R8921`: `mock-no-assign`
+
+Mock not assigned to a variable: XXX. Every mocked object should be assigned to a variable to allow for assertions.
+
+To disable this check on a specific line, add `# pylint: disable=mock-no-assign` at the end of it.
+
+[[back to top](#pylint-plugin-for-databricks)]
+
+### `R8922`: `mock-no-usage`
+
+Missing usage of mock for XXX. Usually this check means a hidden bug, where object is mocked, but we don't check if it was used correctly. Every mock should have at least one assertion, return value, or side effect specified.
+
+To disable this check on a specific line, add `# pylint: disable=mock-no-usage` at the end of it.
+
+[[back to top](#pylint-plugin-for-databricks)]
+
 ## `eradicate` checker
 To use this checker, add `databricks.labs.pylint.eradicate` to `load-plugins` configuration in your `pylintrc` or `pyproject.toml` file.
 
 [[back to top](#pylint-plugin-for-databricks)]
 
 ### `C8920`: `dead-code`
 
@@ -376,15 +394,15 @@
 
 [[back to top](#pylint-plugin-for-databricks)]
 
 ## Testing in isolation
 To test this plugin in isolation, you can use the following command:
 
 ```bash
-pylint --load-plugins=databricks.labs.pylint.all --disable=all --enable=missing-data-security-mode,unsupported-runtime,dbutils-fs-cp,dbutils-fs-head,dbutils-fs-ls,dbutils-fs-mount,dbutils-credentials,dbutils-notebook-run,pat-token-leaked,internal-api,legacy-cli,incompatible-with-uc,notebooks-too-many-cells,notebooks-percent-run,spark-outside-function,use-display-instead-of-show,no-spark-argument-in-function,explicit-dependency-required,obscure-mock,dead-code .
+pylint --load-plugins=databricks.labs.pylint.all --disable=all --enable=missing-data-security-mode,unsupported-runtime,dbutils-fs-cp,dbutils-fs-head,dbutils-fs-ls,dbutils-fs-mount,dbutils-credentials,dbutils-notebook-run,pat-token-leaked,internal-api,legacy-cli,incompatible-with-uc,notebooks-too-many-cells,notebooks-percent-run,spark-outside-function,use-display-instead-of-show,no-spark-argument-in-function,explicit-dependency-required,obscure-mock,mock-no-assign,mock-no-usage,dead-code .
 ```
 
 [[back to top](#pylint-plugin-for-databricks)]
 
 <!-- END CHECKS -->
 
 # Project Support
```

