# Comparing `tmp/pydeequ-1.2.0.tar.gz` & `tmp/pydeequ-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydeequ-1.2.0.tar", max compression
+gzip compressed data, was "pydeequ-1.3.0.tar", max compression
```

## Comparing `pydeequ-1.2.0.tar` & `pydeequ-1.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11357 2023-06-08 15:55:16.576797 pydeequ-1.2.0/LICENSE
--rw-r--r--   0        0        0     7951 2023-07-08 04:26:32.485192 pydeequ-1.2.0/README.md
--rw-r--r--   0        0        0     1595 2023-12-13 03:22:35.584082 pydeequ-1.2.0/pydeequ/__init__.py
--rw-r--r--   0        0        0    27263 2023-09-21 00:49:32.499642 pydeequ-1.2.0/pydeequ/analyzers.py
--rw-r--r--   0        0        0    10670 2023-06-08 15:55:16.581996 pydeequ-1.2.0/pydeequ/anomaly_detection.py
--rw-r--r--   0        0        0       37 2023-10-25 20:38:06.741917 pydeequ-1.2.0/pydeequ/check_functions.py
--rw-r--r--   0        0        0    42999 2023-12-13 03:09:43.271425 pydeequ-1.2.0/pydeequ/checks.py
--rw-r--r--   0        0        0     1434 2023-12-05 02:22:44.033094 pydeequ-1.2.0/pydeequ/configs.py
--rw-r--r--   0        0        0     2061 2023-06-08 15:55:16.582423 pydeequ-1.2.0/pydeequ/metrics.py
--rw-r--r--   0        0        0     2475 2023-06-08 15:55:16.582525 pydeequ-1.2.0/pydeequ/pandas_utils.py
--rw-r--r--   0        0        0    17640 2023-06-08 15:55:16.582681 pydeequ-1.2.0/pydeequ/profiles.py
--rw-r--r--   0        0        0     6704 2023-06-08 15:55:16.582819 pydeequ-1.2.0/pydeequ/repository.py
--rw-r--r--   0        0        0     3774 2023-10-26 02:16:48.743769 pydeequ-1.2.0/pydeequ/scala_utils.py
--rw-r--r--   0        0        0     8740 2023-06-08 15:55:16.583035 pydeequ-1.2.0/pydeequ/suggestions.py
--rw-r--r--   0        0        0    10216 2023-06-08 15:55:16.583154 pydeequ-1.2.0/pydeequ/verification.py
--rw-r--r--   0        0        0     2778 2023-12-13 03:22:35.584746 pydeequ-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     9092 1970-01-01 00:00:00.000000 pydeequ-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-12 21:10:03.605191 pydeequ-1.3.0/LICENSE
+-rw-r--r--   0        0        0     8304 2024-04-12 21:10:03.605620 pydeequ-1.3.0/README.md
+-rw-r--r--   0        0        0     1595 2024-04-12 21:10:03.613679 pydeequ-1.3.0/pydeequ/__init__.py
+-rw-r--r--   0        0        0    28158 2024-04-26 20:33:57.732979 pydeequ-1.3.0/pydeequ/analyzers.py
+-rw-r--r--   0        0        0    10670 2024-04-12 21:10:03.614580 pydeequ-1.3.0/pydeequ/anomaly_detection.py
+-rw-r--r--   0        0        0       37 2024-04-12 21:10:03.614745 pydeequ-1.3.0/pydeequ/check_functions.py
+-rw-r--r--   0        0        0    43544 2024-04-26 20:33:57.733851 pydeequ-1.3.0/pydeequ/checks.py
+-rw-r--r--   0        0        0     1353 2024-04-26 20:33:57.734639 pydeequ-1.3.0/pydeequ/configs.py
+-rw-r--r--   0        0        0     2061 2024-04-12 21:10:03.615497 pydeequ-1.3.0/pydeequ/metrics.py
+-rw-r--r--   0        0        0     2475 2024-04-12 21:10:03.615672 pydeequ-1.3.0/pydeequ/pandas_utils.py
+-rw-r--r--   0        0        0    17699 2024-04-12 21:10:03.615941 pydeequ-1.3.0/pydeequ/profiles.py
+-rw-r--r--   0        0        0     6704 2024-04-12 21:10:03.616186 pydeequ-1.3.0/pydeequ/repository.py
+-rw-r--r--   0        0        0     3774 2024-04-12 21:10:03.616457 pydeequ-1.3.0/pydeequ/scala_utils.py
+-rw-r--r--   0        0        0     8740 2024-04-12 21:10:03.616737 pydeequ-1.3.0/pydeequ/suggestions.py
+-rw-r--r--   0        0        0    10216 2024-04-12 21:10:03.616955 pydeequ-1.3.0/pydeequ/verification.py
+-rw-r--r--   0        0        0     2779 2024-04-26 20:33:57.735359 pydeequ-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     9494 1970-01-01 00:00:00.000000 pydeequ-1.3.0/PKG-INFO
```

### Comparing `pydeequ-1.2.0/LICENSE` & `pydeequ-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydeequ-1.2.0/README.md` & `pydeequ-1.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -240,8 +240,18 @@
 
 ## Running Tests Locally
 
 Take a look at tests in `tests/dataquality` and `tests/jobs`
 
 ```bash
 $ poetry run pytest
-```
+```
+
+## Running Tests Locally (Docker)
+
+If you have issues installing the dependencies listed above, another way to run the tests and verify your changes is through Docker. There is a Dockerfile that will install the required dependencies and run the tests in a container.
+
+```
+docker build . -t spark-3.3-docker-test
+docker run spark-3.3-docker-test
+```
+
```

### Comparing `pydeequ-1.2.0/pydeequ/__init__.py` & `pydeequ-1.3.0/pydeequ/__init__.py`

 * *Files identical despite different names*

### Comparing `pydeequ-1.2.0/pydeequ/analyzers.py` & `pydeequ-1.3.0/pydeequ/analyzers.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from pyspark.sql import DataFrame, SparkSession, SQLContext
 
 from pydeequ.pandas_utils import ensure_pyspark_df
 from pydeequ.repository import MetricsRepository, ResultKey
 from enum import Enum
 from pydeequ.scala_utils import to_scala_seq
-
+from pydeequ.configs import SPARK_VERSION
 
 class _AnalyzerObject:
     """
     Analyzer base object to pass and accumulate the analyzers of the run with respect to the JVM
     """
 
     def _set_jvm(self, jvm):
@@ -267,15 +267,19 @@
 
     @property
     def _analyzer_jvm(self):
         """Returns the value of the computed completeness
 
         :return self: access the value of the Completeness analyzer.
         """
-        return self._deequAnalyzers.Completeness(self.column, self._jvm.scala.Option.apply(self.where))
+        return self._deequAnalyzers.Completeness(
+            self.column,
+            self._jvm.scala.Option.apply(self.where),
+            self._jvm.scala.Option.apply(None)
+        )
 
 
 class Compliance(_AnalyzerObject):
     """
     Compliance measures the fraction of rows that complies with the given
     column constraint. E.g if the constraint is "att1>3" and data frame
     has 5 rows with att1 column value greater than 3 and 10 rows under
@@ -299,15 +303,21 @@
 
     @property
     def _analyzer_jvm(self):
         """Returns the value of the computed compliance
 
         :return self
         """
-        return self._deequAnalyzers.Compliance(self.instance, self.predicate, self._jvm.scala.Option.apply(self.where))
+        return self._deequAnalyzers.Compliance(
+            self.instance,
+            self.predicate,
+            self._jvm.scala.Option.apply(self.where),
+            self._jvm.scala.collection.Seq.empty(),
+            self._jvm.scala.Option.apply(None)
+        )
 
 
 class Correlation(_AnalyzerObject):
     """
     Computes the pearson correlation coefficient between the two given columns.
 
     :param str column1: First column in the DataFrame for which the Correlation is analyzed.
@@ -458,14 +468,16 @@
         if not self.maxDetailBins:
             self.maxDetailBins = getattr(self._jvm.com.amazon.deequ.analyzers.Histogram, "apply$default$3")()
         return self._deequAnalyzers.Histogram(
             self.column,
             self._jvm.scala.Option.apply(self.binningUdf),
             self.maxDetailBins,
             self._jvm.scala.Option.apply(self.where),
+            getattr(self._jvm.com.amazon.deequ.analyzers.Histogram, "apply$default$5")(),
+            getattr(self._jvm.com.amazon.deequ.analyzers.Histogram, "apply$default$6")()
         )
 
 
 class KLLParameters:
     """
     Parameter definition for KLL Sketches.
 
@@ -527,15 +539,17 @@
 
     @property
     def _analyzer_jvm(self):
         """Returns the maximum value in a column.
 
         :return self
         """
-        return self._deequAnalyzers.Maximum(self.column, self._jvm.scala.Option.apply(self.where))
+        return self._deequAnalyzers.Maximum(
+            self.column, self._jvm.scala.Option.apply(self.where), self._jvm.scala.Option.apply(None)
+        )
 
 
 class MaxLength(_AnalyzerObject):
     """MaxLength Analyzer. Get Max length of a str type column.
 
     :param str column: column in DataFrame to find the maximum length.
             Column is expected to be a str type.
@@ -549,15 +563,19 @@
 
     @property
     def _analyzer_jvm(self):
         """Returns the maximum length in a column.
 
         :return self
         """
-        return self._deequAnalyzers.MaxLength(self.column, self._jvm.scala.Option.apply(self.where))
+        return self._deequAnalyzers.MaxLength(
+            self.column,
+            self._jvm.scala.Option.apply(self.where),
+            self._jvm.scala.Option.apply(None)
+        )
 
 
 class Mean(_AnalyzerObject):
     """
     Mean Analyzer. Get mean of a column
 
     :param str column: Column in DataFrame to find the mean.
@@ -592,15 +610,17 @@
 
     @property
     def _analyzer_jvm(self):
         """Returns the minimum of a column.
 
         :return self
         """
-        return self._deequAnalyzers.Minimum(self.column, self._jvm.scala.Option.apply(self.where))
+        return self._deequAnalyzers.Minimum(
+            self.column, self._jvm.scala.Option.apply(self.where), self._jvm.scala.Option.apply(None)
+        )
 
 
 class MinLength(_AnalyzerObject):
     """
     Get the minimum length of a column
 
     :param str column: Column in DataFrame to find the minimum Length.
@@ -615,15 +635,19 @@
     @property
     def _analyzer_jvm(self):
         """
         Returns the minimum length of column.
 
         :return self
         """
-        return self._deequAnalyzers.MinLength(self.column, self._jvm.scala.Option.apply(self.where))
+        return self._deequAnalyzers.MinLength(
+            self.column,
+            self._jvm.scala.Option.apply(self.where),
+            self._jvm.scala.Option.apply(None)
+        )
 
 
 class MutualInformation(_AnalyzerObject):
     """
     Describes how much information about one column can be inferred from another column.
 
     :param list[str] columns: Columns in DataFrame for mutual information analysis.
@@ -679,14 +703,15 @@
         """
         return self._deequAnalyzers.PatternMatch(
             self.column,
             self._jvm.scala.util.matching.Regex(self.pattern_regex, None),
             # TODO: revisit bc scala constructor does some weird implicit type casting from python str -> java list
             #  if we don't cast it to str()
             self._jvm.scala.Option.apply(self.where),
+            self._jvm.scala.Option.apply(None)
         )
 
 
 class Size(_AnalyzerObject):
     """
     Size is the number of rows in a DataFrame.
 
@@ -768,15 +793,17 @@
     def _analyzer_jvm(self):
         """
         Returns the uniqueness in columns.
 
         :return self
         """
         return self._deequAnalyzers.Uniqueness(
-            to_scala_seq(self._jvm, self.columns), self._jvm.scala.Option.apply(self.where)
+            to_scala_seq(self._jvm, self.columns),
+            self._jvm.scala.Option.apply(self.where),
+            self._jvm.scala.Option.apply(None)
         )
 
 
 class UniqueValueRatio(_AnalyzerObject):
     """
     Calculates the ratio of uniqueness.
 
@@ -793,15 +820,17 @@
     def _analyzer_jvm(self):
         """
         Returns the unique value ratio in columns.
 
         :return self
         """
         return self._deequAnalyzers.UniqueValueRatio(
-            to_scala_seq(self._jvm, self.columns), self._jvm.scala.Option.apply(self.where)
+            to_scala_seq(self._jvm, self.columns),
+            self._jvm.scala.Option.apply(self.where),
+            self._jvm.scala.Option.apply(None)
         )
 
 class DataTypeInstances(Enum):
     """
     An enum class that types columns to scala datatypes
     """
     Boolean = "Boolean"
```

### Comparing `pydeequ-1.2.0/pydeequ/anomaly_detection.py` & `pydeequ-1.3.0/pydeequ/anomaly_detection.py`

 * *Files identical despite different names*

### Comparing `pydeequ-1.2.0/pydeequ/checks.py` & `pydeequ-1.3.0/pydeequ/checks.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from enum import Enum
 
 from py4j.protocol import Py4JError
 from pyspark.sql import SparkSession
 
 from pydeequ.check_functions import is_one
 from pydeequ.scala_utils import ScalaFunction1, to_scala_seq
-
+from pydeequ.configs import SPARK_VERSION
 
 # TODO implement custom assertions
 # TODO implement all methods without outside class dependencies
 # TODO Integration with Constraints
 
 
 class CheckLevel(Enum):
@@ -150,15 +150,15 @@
         """Creates a constraint that asserts on a column completion.
 
         :param str column: Column in Data Frame to run the assertion on.
         :param str hint: A hint that discerns why a constraint could have failed.
         :return: isComplete self:A Check.scala object that asserts on a column completion.
         """
         hint = self._jvm.scala.Option.apply(hint)
-        self._Check = self._Check.isComplete(column, hint)
+        self._Check = self._Check.isComplete(column, hint, self._jvm.scala.Option.apply(None))
         return self
 
     def hasCompleteness(self, column, assertion, hint=None):
         """
         Creates a constraint that asserts column completion.
         Uses the given history selection strategy to retrieve historical completeness values on this
         column from the history provider.
@@ -166,15 +166,15 @@
         :param str column: Column in Data Frame to run the assertion on.
         :param lambda assertion: A function that accepts an int or float parameter.
         :param str hint: A hint that states why a constraint could have failed.
         :return: hasCompleteness self: A Check object that implements the assertion.
         """
         assertion_func = ScalaFunction1(self._spark_session.sparkContext._gateway, assertion)
         hint = self._jvm.scala.Option.apply(hint)
-        self._Check = self._Check.hasCompleteness(column, assertion_func, hint)
+        self._Check = self._Check.hasCompleteness(column, assertion_func, hint, self._jvm.scala.Option.apply(None))
         return self
 
     def areComplete(self, columns, hint=None):
         """Creates a constraint that asserts completion in combined set of columns.
 
         :param list[str] columns: Columns in Data Frame to run the assertion on.
         :param str hint: A hint that states why a constraint could have failed.
@@ -230,15 +230,15 @@
         Creates a constraint that asserts on a column uniqueness
 
         :param list[str] columns: Columns in Data Frame to run the assertion on.
         :param str hint: A hint that states why a constraint could have failed.
         :return: isUnique self: A Check.scala object that asserts uniqueness in the column.
         """
         hint = self._jvm.scala.Option.apply(hint)
-        self._Check = self._Check.isUnique(column, hint)
+        self._Check = self._Check.isUnique(column, hint, self._jvm.scala.Option.apply(None))
         return self
 
     def isPrimaryKey(self, column, *columns, hint=None):
         """
         Creates a constraint that asserts on a column(s) primary key characteristics.
         Currently only checks uniqueness, but reserved for primary key checks if there is another
         assertion to run on primary key columns.
@@ -293,15 +293,15 @@
         :param lambda assertion: A function that accepts an int or float parameter.
         :param str hint: A hint that states why a constraint could have failed.
         :return: hasUniqueValueRatio self: A Check object that asserts the unique value ratio in the columns.
         """
         assertion_func = ScalaFunction1(self._spark_session.sparkContext._gateway, assertion)
         hint = self._jvm.scala.Option.apply(hint)
         columns_seq = to_scala_seq(self._jvm, columns)
-        self._Check = self._Check.hasUniqueValueRatio(columns_seq, assertion_func, hint)
+        self._Check = self._Check.hasUniqueValueRatio(columns_seq, assertion_func, hint, self._jvm.scala.Option.apply(None))
         return self
 
     def hasNumberOfDistinctValues(self, column, assertion, binningUdf, maxBins, hint=None):
         """Creates a constraint that asserts on the number of distinct values a column has.
 
         :param str column: Column in Data Frame to run the assertion on.
         :param lambda assertion: A function that accepts an int or float parameter.
@@ -414,30 +414,30 @@
         :param lambda assertion: A function which accepts the int or float parameter
                 that discerns the minimum length of the string.
         :param str hint: A hint that states why a constraint could have failed.
         :return: hasMinLength self: A Check object that asserts minLength of the column.
         """
         assertion_func = ScalaFunction1(self._spark_session.sparkContext._gateway, assertion)
         hint = self._jvm.scala.Option.apply(hint)
-        self._Check = self._Check.hasMinLength(column, assertion_func, hint)
+        self._Check = self._Check.hasMinLength(column, assertion_func, hint, self._jvm.scala.Option.apply(None))
         return self
 
     def hasMaxLength(self, column, assertion, hint=None):
         """
         Creates a constraint that asserts on the maximum length of a string datatype column
 
         :param str column: Column in Data Frame to run the assertion on. The column is expected to be a string type.
         :param lanmbda assertion: A function which accepts an int or float parameter
                 that discerns the maximum length of the string.
         :param str hint: A hint that states why a constraint could have failed.
         :return: hasMaxLength self : A Check object that asserts maxLength of the column.
         """
         assertion_func = ScalaFunction1(self._spark_session.sparkContext._gateway, assertion)
         hint = self._jvm.scala.Option.apply(hint)
-        self._Check = self._Check.hasMaxLength(column, assertion_func, hint)
+        self._Check = self._Check.hasMaxLength(column, assertion_func, hint, self._jvm.scala.Option.apply(None))
         return self
 
     def hasMin(self, column, assertion, hint=None):
         """
         Creates a constraint that asserts on the minimum of a column. The column is contains either a long,
         int or float datatype.
 
@@ -445,15 +445,15 @@
         :param lambda assertion: A function which accepts an int or float parameter
                 that discerns the minumum value of the column.
         :param str hint: A hint that states why a constraint could have failed.
         :return: hasMaxLength self: A Check object that asserts the minumum of the column.
         """
         assertion_func = ScalaFunction1(self._spark_session.sparkContext._gateway, assertion)
         hint = self._jvm.scala.Option.apply(hint)
-        self._Check = self._Check.hasMin(column, assertion_func, hint)
+        self._Check = self._Check.hasMin(column, assertion_func, hint, self._jvm.scala.Option.apply(None))
         return self
 
     def hasMax(self, column, assertion, hint=None):
         """
         Creates a constraint that asserts on the maximum of the column. The column contains either a long,
         int or float datatype.
 
@@ -461,15 +461,15 @@
         :param lambda assertion: A function which accepts an int or float parameter
                 that discerns the maximum value of the column.
         :param str hint: A hint that states why a constraint could have failed.
         :return: hasMax self: A Check object that asserts maximum of the column.
         """
         assertion_func = ScalaFunction1(self._spark_session.sparkContext._gateway, assertion)
         hint = self._jvm.scala.Option.apply(hint)
-        self._Check = self._Check.hasMax(column, assertion_func, hint)
+        self._Check = self._Check.hasMax(column, assertion_func, hint, self._jvm.scala.Option.apply(None))
         return self
 
     def hasMean(self, column, assertion, hint=None):
         """
         Creates a constraint that asserts on the mean of the column
 
         :param str column: Column in Data Frame to run the assertion on.
@@ -551,18 +551,25 @@
         :param lambda assertion: A function with an int or float parameter.
         :param str hint: A hint that states why a constraint could have failed.
         :return: satisfies self: A Check object that runs the condition on the data frame.
         """
         assertion_func = (
             ScalaFunction1(self._spark_session.sparkContext._gateway, assertion)
             if assertion
-            else getattr(self._Check, "satisfies$default$2")()
+            else getattr(self._Check, "satisfies$default$3")()
         )
         hint = self._jvm.scala.Option.apply(hint)
-        self._Check = self._Check.satisfies(columnCondition, constraintName, assertion_func, hint)
+        self._Check = self._Check.satisfies(
+            columnCondition,
+            constraintName,
+            assertion_func,
+            hint,
+            self._jvm.scala.collection.Seq.empty(),
+            self._jvm.scala.Option.apply(None)
+        )
         return self
 
     def hasPattern(self, column, pattern, assertion=None, name=None, hint=None):
         """
         Checks for pattern compliance. Given a column name and a regular expression, defines a
         Check on the average compliance of the column's values to the regular expression.
 
@@ -577,15 +584,17 @@
         if not assertion:
             assertion = is_one
 
         assertion_func = ScalaFunction1(self._spark_session.sparkContext._gateway, assertion)
         name = self._jvm.scala.Option.apply(name)
         hint = self._jvm.scala.Option.apply(hint)
         pattern_regex = self._jvm.scala.util.matching.Regex(pattern, None)
-        self._Check = self._Check.hasPattern(column, pattern_regex, assertion_func, name, hint)
+        self._Check = self._Check.hasPattern(
+            column, pattern_regex, assertion_func, name, hint, self._jvm.scala.Option.apply(None)
+        )
         return self
 
     def containsCreditCardNumber(self, column, assertion=None, hint=None):
         """
         Check to run against the compliance of a column against a Credit Card pattern.
 
         :param str column: Column in DataFrame to be checked. The column is expected to be a string type.
```

### Comparing `pydeequ-1.2.0/pydeequ/configs.py` & `pydeequ-1.3.0/pydeequ/configs.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 # -*- coding: utf-8 -*-
 from functools import lru_cache
 import os
 import re
 
 
 SPARK_TO_DEEQU_COORD_MAPPING = {
-    "3.3": "com.amazon.deequ:deequ:2.0.3-spark-3.3",
-    "3.2": "com.amazon.deequ:deequ:2.0.1-spark-3.2",
-    "3.1": "com.amazon.deequ:deequ:2.0.0-spark-3.1",
-    "3.0": "com.amazon.deequ:deequ:1.2.2-spark-3.0",
-    "2.4": "com.amazon.deequ:deequ:1.1.0_spark-2.4-scala-2.11",
+    "3.3": "com.amazon.deequ:deequ:2.0.7-spark-3.3",
+    "3.2": "com.amazon.deequ:deequ:2.0.7-spark-3.2",
+    "3.1": "com.amazon.deequ:deequ:2.0.7-spark-3.1"
 }
 
 
 def _extract_major_minor_versions(full_version: str):
     major_minor_pattern = re.compile(r"(\d+\.\d+)\.*")
     match = re.match(major_minor_pattern, full_version)
     if match:
@@ -36,9 +34,10 @@
         return SPARK_TO_DEEQU_COORD_MAPPING[spark_version[:3]]
     except KeyError:
         raise RuntimeError(
             f"Found incompatible Spark version {spark_version}; Use one of the Supported Spark versions for Deequ: {SPARK_TO_DEEQU_COORD_MAPPING.keys()}"
         )
 
 
+SPARK_VERSION = _get_spark_version()
 DEEQU_MAVEN_COORD = _get_deequ_maven_config()
 IS_DEEQU_V1 = re.search("com\.amazon\.deequ\:deequ\:1.*", DEEQU_MAVEN_COORD) is not None
```

### Comparing `pydeequ-1.2.0/pydeequ/metrics.py` & `pydeequ-1.3.0/pydeequ/metrics.py`

 * *Files identical despite different names*

### Comparing `pydeequ-1.2.0/pydeequ/pandas_utils.py` & `pydeequ-1.3.0/pydeequ/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `pydeequ-1.2.0/pydeequ/profiles.py` & `pydeequ-1.3.0/pydeequ/profiles.py`

 * *Files 1% similar despite different names*

```diff
@@ -237,15 +237,17 @@
 
         self._spark_session = spark_session
         self._sc = spark_session.sparkContext
         self._jvm = spark_session._jvm
         self._profiles = []
         self.columnProfileClasses = {
             "StandardColumnProfile": StandardColumnProfile,
+            "StringColumnProfile": StandardColumnProfile,
             "NumericColumnProfile": NumericColumnProfile,
+
         }
 
     def _columnProfilesFromColumnRunBuilderRun(self, run):
         """
         Produces a Java profile based on the designated column
 
         :param run: columnProfilerRunner result
```

### Comparing `pydeequ-1.2.0/pydeequ/repository.py` & `pydeequ-1.3.0/pydeequ/repository.py`

 * *Files identical despite different names*

### Comparing `pydeequ-1.2.0/pydeequ/scala_utils.py` & `pydeequ-1.3.0/pydeequ/scala_utils.py`

 * *Files identical despite different names*

### Comparing `pydeequ-1.2.0/pydeequ/suggestions.py` & `pydeequ-1.3.0/pydeequ/suggestions.py`

 * *Files identical despite different names*

### Comparing `pydeequ-1.2.0/pydeequ/verification.py` & `pydeequ-1.3.0/pydeequ/verification.py`

 * *Files identical despite different names*

### Comparing `pydeequ-1.2.0/pyproject.toml` & `pydeequ-1.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "pydeequ"
-version = "1.2.0"
+version = "1.3.0"
 description = "PyDeequ - Unit Tests for Data"
-authors = ["Calvin Wang <calviwan@amazon.com>", "Chenyang Liu <peterl@amazon.com>"]
-maintainers = ["Calvin Wang <calviwan@amazon.com>", "Chenyang Liu <peterl@amazon.com>"]
+authors = ["Chenyang Liu <peterl@amazon.com>", "Rahul Sharma <rdsharma@amazon.com>"]
+maintainers = ["Chenyang Liu <peterl@amazon.com>","Rahul Sharma <rdsharma@amazon.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://pydeequ.readthedocs.io"
 repository = "https://github.com/awslabs/python-deequ"
 documentation = "https://pydeequ.readthedocs.io"
 keywords = [
     "deequ",
```

### Comparing `pydeequ-1.2.0/PKG-INFO` & `pydeequ-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: pydeequ
-Version: 1.2.0
+Version: 1.3.0
 Summary: PyDeequ - Unit Tests for Data
 Home-page: https://pydeequ.readthedocs.io
 License: Apache-2.0
 Keywords: deequ,pydeequ,data-engineering,data-quality,data-profiling,dataquality,dataunittest,data-unit-tests,data-profilers
-Author: Calvin Wang
-Author-email: calviwan@amazon.com
-Maintainer: Calvin Wang
-Maintainer-email: calviwan@amazon.com
+Author: Chenyang Liu
+Author-email: peterl@amazon.com
+Maintainer: Chenyang Liu
+Maintainer-email: peterl@amazon.com
 Requires-Python: >=3.7,<4
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: pyspark
 Requires-Dist: numpy (>=1.14.1)
 Requires-Dist: pandas (>=0.23.0)
 Requires-Dist: pyspark (>=2.4.7,<3.3.0) ; extra == "pyspark"
 Project-URL: Documentation, https://pydeequ.readthedocs.io
 Project-URL: Repository, https://github.com/awslabs/python-deequ
 Description-Content-Type: text/markdown
@@ -269,7 +270,18 @@
 ## Running Tests Locally
 
 Take a look at tests in `tests/dataquality` and `tests/jobs`
 
 ```bash
 $ poetry run pytest
 ```
+
+## Running Tests Locally (Docker)
+
+If you have issues installing the dependencies listed above, another way to run the tests and verify your changes is through Docker. There is a Dockerfile that will install the required dependencies and run the tests in a container.
+
+```
+docker build . -t spark-3.3-docker-test
+docker run spark-3.3-docker-test
+```
+
+
```

